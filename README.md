# Portfolio CV cá nhân

- **Tác giả:** Đào Duy Thương
- **Mô tả:** Website portfolio CV giới thiệu bản thân, kỹ năng, dự án, quá trình học tập và thông tin liên hệ. Trang được xây dựng bằng HTML và CSS.

## Liên kết

- **Website:** [K20 Portfolio](https://daoduythuong.github.io/K20_Portfolio_CNTT20-04/)
- **Mã nguồn:** [GitHub repository](https://github.com/daoduythuong/K20_Portfolio_CNTT20-04)
- **Hồ sơ tác giả:** [github.com/daoduythuong](https://github.com/daoduythuong)
- **Minh chứng:** [Trang giới thiệu](https://daoduythuong.github.io/K20_Portfolio_CNTT20-04/#gioi-thieu), [dự án](https://daoduythuong.github.io/K20_Portfolio_CNTT20-04/#du-an), [liên hệ](https://daoduythuong.github.io/K20_Portfolio_CNTT20-04/#lien-he)

## Cấu trúc thư mục

```text
.
├── index.html          # Trang portfolio chính
├── ket-qua.html        # Trang kết quả của form liên hệ
├── README.md           # Tài liệu dự án
├── AI log.md           # Nhật ký và ghi nhận kiểm tra
├── css/
│   └── style.css       # Giao diện và bố cục responsive
└── assets/
	├── 7-74849_gangster-sticker-dead-man-walking-logo-hd-png.png
	├── avatar.svg
	├── du-an-1.svg
	├── du-an-2.svg
	└── du-an-3.svg
```

## Chạy trên máy local

Website không cần cài thư viện. Mở terminal tại thư mục dự án và chạy:

```powershell
py -m http.server 8000
```

Mở [http://localhost:8000](http://localhost:8000) trên trình duyệt. Dừng máy chủ bằng `Ctrl+C`.

## Xuất bản

Website công khai trên GitHub Pages tại liên kết ở phần **Liên kết**. Dự án đặt `index.html` ở thư mục gốc; cấu hình phù hợp với cấu trúc hiện tại là xuất bản từ nhánh `main`, thư mục `/(root)`. Có thể xác nhận nguồn đang được cấu hình tại **Settings → Pages** của repository.

## Kiểm tra sản phẩm

1. Mở trang chính và kiểm tra menu đến các mục Giới thiệu, Kỹ năng, Dự án, Học tập và Liên hệ.
2. Tại mục Dự án, xác nhận ba hình minh họa tải được.
3. Trong form liên hệ, thử gửi thiếu trường bắt buộc hoặc nhập dữ liệu sai để kiểm tra xác thực HTML5. Sau đó nhập họ tên từ 2 ký tự, email hợp lệ và lời nhắn từ 10 đến 500 ký tự để mở trang `ket-qua.html`.
4. Xác nhận dữ liệu gửi bằng phương thức GET có thể xuất hiện trên URL. Form chỉ phục vụ thực hành: không gửi email và không lưu dữ liệu lên máy chủ.

**Lưu ý khi kiểm tra:** `ket-qua.html` hiện hiển thị tên “Việt Anh/Trần Việt Anh”, chưa đồng nhất với tên Đào Duy Thương trên trang chính.
