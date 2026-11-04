# BẢN TIN MỘC. — Website báo điện tử demo

Website tạp chí/bản tin tiếng Việt, thiết kế theo tinh thần editorial với bảng màu:

- Trắng ngà `#EEEAE6`
- Be `#D7B689`
- Vàng đất `#C38C55`
- Đỏ gạch `#813527`

**Điều kiện:** HTML + CSS + JavaScript thuần. Không cần mua hosting, không cài Node/npm, không dùng cơ sở dữ liệu. Có thể chạy trên GitHub Pages.

**Đây là dự án học tập / bản trình diễn.** Toàn bộ bài viết, ngày, tác giả và xếp hạng đọc nhiều là nội dung minh họa; đây không phải nguồn tin đã kiểm chứng, không liên kết hoặc đại diện cho CNN, Dân Trí, Tuổi Trẻ.

## Bắt đầu ở đây

👉 Xem file **`HUONG-DAN-TU-A-DEN-Z.md`** để được hướng dẫn tạo GitHub, đưa web lên mạng, sửa bài và đổi màu từng bước.

### Có những chức năng gì?

- Trang chủ với grid biên tập 3 cột và bài tiêu điểm.
- Các trang chuyên mục tự lấy bài từ dữ liệu.
- Trang đọc bài, gợi ý bài liên quan, thông tin tác giả.
- Tìm kiếm nội dung (chạy trực tiếp trong trình duyệt).
- Lưu/bỏ lưu bài trên thiết bị qua `localStorage` (không đồng bộ giữa thiết bị).
- Menu mobile, giao diện responsive, nút chia sẻ/sao chép liên kết.
- 18 bài demo; ảnh Unsplash khi có Internet và 12 SVG minh họa dự phòng.

## Cấu trúc thư mục

```text
ban-tin-moc/
├── index.html                 <- TRANG CHỦ (phải ở thư mục gốc của GitHub)
├── chuyen-muc.html            <- Trang chuyên mục
├── bai-viet.html              <- Trang đọc bài
├── tim-kiem.html              <- Trang tìm kiếm
├── da-luu.html                <- Các bài được lưu
├── gioi-thieu.html            <- Về dự án
├── assets/
│   ├── css/style.css         <- Giao diện, bốn màu nằm trên cùng
│   ├── js/data.js            <- Tên báo, chuyên mục, bài viết
│   ├── js/app.js             <- Logic website, không cần sửa nếu mới học
│   └── images/               <- Logo favicon, ảnh minh họa SVG
├── HUONG-DAN-TU-A-DEN-Z.md
├── BAT-DAU.txt
└── README.md
```

## Thay đổi nhanh

- **Đổi tên:** `assets/js/data.js` → `SITE.name`, `brandMain`, `brandAccent`, `shortName`.
- **Đổi màu:** `assets/css/style.css` → bốn biến `--ivory`, `--beige`, `--ochre`, `--brick` ở đầu file.
- **Sửa bài:** `assets/js/data.js` → `ARTICLES`.
- **Dùng tranh SVG thay ảnh mạng:** `assets/js/data.js` → `useOnlinePhotos: false`.

## Giới hạn thực tế

Đây là web **tĩnh**: không có trang đăng nhập quản trị, không có đăng bài bằng form, không có bình luận máy chủ, không có database. Cập nhật bài bằng việc sửa `data.js` và đẩy tệp lên GitHub. GitHub Pages yêu cầu public repository đối với GitHub Free và có giới hạn sử dụng. Để làm báo điện tử quy mô lớn/hoạt động thương mại, cần giải pháp hosting và CMS phù hợp hơn.

## Tham khảo chính thức

- [GitHub Pages — Creating a site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
- [Configuring publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [Uploading files](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
- [GitHub Pages limits](https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits)

## Bản quyền

Bộ mã website và minh họa SVG trong gói được tạo mới cho bản demo. Nếu dùng ảnh Unsplash hiển thị từ máy chủ ảnh bên ngoài, hãy tuân thủ điều khoản sử dụng và quyền riêng tư của nhà cung cấp. Khi thay ảnh bằng ảnh của m, hãy đảm bảo có quyền sử dụng.
