# Portfolio CV cá nhân

## Snapshot `1030936`

- **Mã phiên bản:** snapshot commit `1030936fa46a510751a44d3055cd8f5d61b0e841` (dùng SHA để nhận diện chính xác mã; không khẳng định đây là tag phát hành).
- **Ngày cập nhật ghi chú:** 2026-10-30.
- **Commit liên quan:** [1030936fa46a510751a44d3055cd8f5d61b0e841](https://github.com/daoduythuong/K20_Portfolio_CNTT20-04/commit/1030936fa46a510751a44d3055cd8f5d61b0e841).
- **Mã nguồn đúng snapshot:** [Toàn bộ mã tại commit này](https://github.com/daoduythuong/K20_Portfolio_CNTT20-04/tree/1030936fa46a510751a44d3055cd8f5d61b0e841). Snapshot đang ở local; tại lần kiểm tra gần nhất, nhánh `main` ahead 2 commit so với `origin/main`, nên các liên kết SHA chỉ dùng được công khai sau khi push.
- **Bản Pages:** [K20 Portfolio](https://daoduythuong.github.io/K20_Portfolio_CNTT20-04/). Chưa xác nhận Pages đang chạy đúng snapshot SHA nêu trên; cần kiểm tra sau khi push và deploy hoàn tất.

### Thay đổi chính trong snapshot

- Website portfolio tĩnh có các mục giới thiệu, kỹ năng, dự án, học tập và liên hệ.
- Có ảnh đại diện và hình minh họa dự án trong `assets/`, định dạng bằng `css/style.css`.
- Form liên hệ dùng kiểm tra dữ liệu HTML5 và gửi bằng GET tới `ket-qua.html`.

### Lỗi đã sửa

- Chưa có lỗi chức năng nào được xác nhận là đã sửa trong snapshot này.
- Báo cáo ảnh không hiển thị vẫn đang điều tra: đường dẫn trong HTML khớp tên tệp cục bộ; `304` là thông tin được báo nhưng chưa được đối chiếu trực tiếp trong DevTools. Không ghi nhận đây là lỗi đã sửa.

### Hạn chế còn lại

- Form chỉ là bài thực hành: không gửi email và không lưu dữ liệu; dữ liệu gửi bằng GET có thể xuất hiện trên URL.
- `ket-qua.html` hiện hiển thị tên Việt Anh/Trần Việt Anh, không đồng nhất với tên Đào Duy Thương ở trang chính.
- Chưa kiểm tra trực tiếp status/Preview của từng ảnh trên trình duyệt và chưa xác nhận cấu hình Pages đang phục vụ đúng commit.
- Tại lần kiểm tra Git gần nhất, README có chỉnh sửa chưa commit, `AI_LOG.md` và `RELEASE_NOTES.md` là tệp chưa được theo dõi, còn `AI log.md` bị xóa. Các thay đổi tài liệu này không nằm trong snapshot commit `1030936`.

### Tiếp tục kiểm tra và bàn giao

1. Rà soát các thay đổi tài liệu hiện có; chỉ stage những tệp cần bàn giao, rồi commit chúng nếu muốn README, nhật ký AI và release notes nằm trong bản nộp.
2. Push nhánh `main` lên `origin` để SHA `1030936fa46a510751a44d3055cd8f5d61b0e841` truy cập được trên GitHub và các thay đổi cần nộp được cập nhật.
3. Sau khi GitHub Pages deploy xong, mở URL Pages và kiểm tra Network với cache tắt; xác nhận ảnh, các mục điều hướng, xác thực form và trang kết quả.
4. Ghi SHA thực tế được deploy cùng kết quả kiểm thử vào release notes khi đã xác minh; không đánh dấu lỗi ảnh là đã sửa nếu chưa có kết quả kiểm tra.
