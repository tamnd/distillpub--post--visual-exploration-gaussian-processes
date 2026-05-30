# Cách mở trang tiếng Việt ở máy local

Trang tiếng Việt nằm tại `public/index_vi.html`.

Từ thư mục gốc repository, chạy:

```sh
cd public
python3 -m http.server 8000
```

Sau đó mở:

```text
http://localhost:8000/index_vi.html
```

Lý do nên dùng local server thay vì mở file trực tiếp là trang Distill tải template
và các asset tương tác qua request HTTP. Nếu chỉ mở `index_vi.html` bằng `file://`,
một số phần nhúng có thể không hiển thị đúng.
