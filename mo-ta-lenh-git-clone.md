# Mô tả câu lệnh `git clone`

## Cú pháp

```
git clone <đường-dẫn-repository>
git clone <đường-dẫn-repository> <tên-thư-mục>
```

Ví dụ trong bài thực hành:

```
git clone https://github.com/codegym-vn/wf-hello.git
```

## Ý nghĩa

`git clone` dùng để sao chép toàn bộ một Remote Repository có sẵn (trên GitHub) về máy tính, tạo thành một Local Repository.

Khi chạy lệnh, Git sẽ:

1. Tạo một thư mục mới trên máy, tên trùng với tên repository (ví dụ `wf-hello`). Nếu muốn đặt tên khác, thêm `<tên-thư-mục>` ở cuối lệnh.
2. Tải về toàn bộ mã nguồn và lịch sử commit của dự án.
3. Tự động tạo thư mục ẩn `.git` để theo dõi thay đổi.
4. Tự động kết nối Local Repository với Remote Repository gốc bằng tên `origin`, nên sau đó có thể dùng `git pull` và `git push` ngay.

## Các bước đã thực hiện

1. Mở trang https://github.com/codegym-vn/wf-hello, bấm nút **Code** (trước đây gọi là "Clone or download") và copy đường dẫn của repository.
2. Mở Terminal, dùng lệnh `cd` để di chuyển đến thư mục muốn chứa repository.
3. Chạy `git clone https://github.com/codegym-vn/wf-hello.git`.
4. Mở thư mục `wf-hello` vừa sao chép về để xem các file bên trong.

## Phân biệt `git init` và `git clone`

| Lệnh | Khi nào dùng |
|---|---|
| `git init` | Tạo repository mới từ đầu trên máy, chưa có sẵn trên GitHub. |
| `git clone` | Lấy về một repository đã có sẵn trên GitHub. |
