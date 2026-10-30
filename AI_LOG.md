## Nhật ký hỗ trợ AI: Ảnh không hiển thị trên GitHub Pages

### Hiện tượng và dữ kiện ban đầu

- Người dùng báo ảnh không hiển thị, nghi ngờ sai đường dẫn; Network được báo trả `304`.
- Trong `index.html`, ảnh đại diện và ảnh dự án dùng đường dẫn tương đối `assets/...`.
- Đã đối chiếu tên các ảnh được tham chiếu với tệp trong thư mục `assets`; tên khớp ở bản làm việc. Công cụ đọc trang công khai cũng nhận diện các URL ảnh dưới `/K20_Portfolio_CNTT20-04/assets/`.
- Status `304` là thông tin người dùng cung cấp; chưa tự ghi nhận request/response của từng ảnh trong DevTools. Việc công cụ đọc được URL ảnh không xác nhận ảnh đã hiển thị trong trình duyệt.

### Nhận định trước AI

Ghi chú ban đầu trong log là “Không hiện ảnh / Không đúng đường dẫn”. Đây là nhận định ban đầu, chưa có bằng chứng `404` để xác nhận đường dẫn sai.

### Công cụ, yêu cầu và phản hồi AI

- **Công cụ đã dùng:** đọc `index.html` và README, liệt kê thư mục `assets`, và tải nội dung trang GitHub Pages để kiểm tra các URL ảnh trong HTML.
- **Yêu cầu người dùng:** nêu giả thuyết, dữ kiện cần kiểm tra và bản sửa tối thiểu; chỉ tư vấn, không sửa tệp.
- **Phản hồi mẫu (tóm tắt):** đường dẫn cục bộ khớp với tên asset; `304 Not Modified` thường cho phép trình duyệt dùng nội dung cache và không tự chứng minh ảnh lỗi. Chưa kết luận nguyên nhân.

### Gợi ý được đưa ra

Trong DevTools → Network, bật `Disable cache`, tải lại trang và lọc `Img`; kiểm tra URL đầy đủ, status, `Content-Type` và Preview. Nếu ảnh trả `404`, đối chiếu chữ hoa/thường, đường dẫn và việc tệp có trong nhánh/thư mục GitHub Pages đang xuất bản hay không. Nếu trả `200`/`304` nhưng không thấy ảnh, kiểm tra Preview, kích thước hiển thị và Console.

### Quyết định và lý do

Không đổi đường dẫn `src` khi chưa có phản hồi `404`, vì các đường dẫn hiện tại khớp với tên asset trong bản làm việc và `304` riêng lẻ không xác nhận lỗi. Chờ dữ liệu Network trước khi chọn sửa mã nguồn hay cấu hình xuất bản.

### Phần sửa

Không sửa HTML, CSS hoặc asset để xử lý ảnh trong lần chẩn đoán này. Chỉ cập nhật tài liệu nhật ký để ghi lại giả thuyết và cách kiểm tra; chưa có bản sửa chức năng.

### Cách thử lại và kết quả

- **Cách thử:** thực hiện các bước Network nêu trên, lưu URL và status cho từng ảnh; kiểm tra Preview. Nếu thấy `404`, sửa đúng URL/tên tệp hoặc bổ sung tệp vào nguồn xuất bản, sau đó tải lại với cache tắt.
- **Kết quả hiện tại:** chưa thực hiện bước thử lại trong DevTools; chưa xác định nguyên nhân cuối cùng và chưa xác nhận sửa thành công.
- **Sử dụng AI:** Có. AI hỗ trợ đối chiếu mã nguồn/tài nguyên và đề xuất kiểm tra; không thay thế bước xác minh Network trên trình duyệt.
