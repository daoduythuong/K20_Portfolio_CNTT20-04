# Portfolio CV cá nhân — Đào Duy Thương

## Sản phẩm này là gì?

Website portfolio CV cá nhân giới thiệu bản thân, kỹ năng, dự án học tập, quá trình học tập và thông tin liên hệ của sinh viên ngành Công nghệ Thông tin.

## Demo

https://daoduythuong.github.io/K20_Portfolio_CNTT20-04/

## Tính năng

- Giới thiệu bản thân và các kỹ năng đang học.
- Hiển thị ba dự án học tập cùng hình minh họa.
- Trình bày một số học phần và sản phẩm học tập.
- Có thông tin liên hệ và form lời nhắn với xác thực trường bắt buộc, email, độ dài họ tên và lời nhắn.

## Cách mở

1. Mở [website demo](https://daoduythuong.github.io/K20_Portfolio_CNTT20-04/).
2. Dùng menu đầu trang để chuyển đến Giới thiệu, Kỹ năng, Dự án, Học tập hoặc Liên hệ.
3. Ở mục Liên hệ, có thể thử form; dữ liệu hợp lệ sẽ mở trang kết quả và xuất hiện trên URL. Form không gửi email thật.

## Cấu trúc thư mục

```text
.
├── index.html
├── ket-qua.html
├── css/
│   └── style.css
├── assets/
└── docs/
    ├── evidence-index.md
    └── AI_LOG.md
```

## Đã kiểm tra

Tài liệu [docs/evidence-index.md](docs/evidence-index.md) hiện chưa có nội dung minh chứng.

## Hạn chế / Chưa kiểm tra

- Form liên hệ chỉ là form thực hành: không gửi email và không lưu dữ liệu lên máy chủ; dữ liệu được gửi bằng phương thức GET.
- Trang kết quả `ket-qua.html` còn hiển thị tên “Việt Anh/Trần Việt Anh”, chưa đồng nhất với tên trên trang chính.
- Các liên kết GitHub trong phần dự án được ghi là cần cập nhật.
- Việc hiển thị ảnh và trạng thái tải ảnh trên trình duyệt chưa được xác minh bằng DevTools; xem [docs/AI_LOG.md](docs/AI_LOG.md).

## Khai báo AI

Xem [docs/AI_LOG.md](docs/AI_LOG.md).
