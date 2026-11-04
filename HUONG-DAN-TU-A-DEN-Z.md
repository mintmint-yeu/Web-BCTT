# HƯỚNG DẪN TỪ A ĐẾN Z — ĐƯA WEB BÁO ĐIỆN TỬ LÊN MẠNG FREE 100%

> Dành cho người chưa biết lập trình. Hướng dẫn theo giao diện GitHub hiện tại (các nút trên GitHub thường hiển thị bằng tiếng Anh).

## PHẦN A — XEM THỬ WEB TRÊN MACBOOK

**Bước 1.** Tải file ZIP đi kèm, bấm đúp để giải nén. M sẽ thấy thư mục `ban-tin-moc`.

**Bước 2.** Mở thư mục đó, tìm file `index.html`, bấm đúp để mở bằng trình duyệt. Nếu muốn chọn Chrome: nhấn chuột phải → **Mở bằng** → **Google Chrome**.

**Bước 3.** Thử bấm một bài nổi bật, chọn các chuyên mục, gõ từ khóa trong ô tìm kiếm, mở menu trên điện thoại và nút lưu bài.

**Bước 4.** Nếu ảnh không hiện khi mất Internet, hệ thống sẽ tự dùng tranh minh họa SVG có sẵn. Mặc định website thử lấy một số ảnh từ Unsplash khi có kết nối mạng. Toàn bộ chức năng chính hoạt động từ file local.

**Cần nhớ:** `index.html` là trang chủ. Không được đổi tên file này thành `trangchu.html` nếu muốn GitHub Pages nhận diện tự động.

## PHẦN B — ĐĂNG KÝ GITHUB MIỄN PHÍ

**Bước 5.** Mở https://github.com/ → bấm **Sign up** nếu chưa có tài khoản. Có tài khoản thì bấm **Sign in**.

**Bước 6.** Đăng ký tài khoản và xác minh email theo hướng dẫn của GitHub.

**Bước 7.** Sau khi đăng nhập, nhấn biểu tượng **+** ở góc trên bên phải (hoặc nút **New**) → chọn **New repository**.

**Bước 8.** Điền:

- **Repository name:** `ban-tin-moc` (có thể chọn tên khác nhưng không dấu, không khoảng trắng).
- **Description:** `Website tạp chí điện tử demo bằng HTML CSS JavaScript` (không bắt buộc).
- **Visibility:** chọn **Public** (bắt buộc nếu dùng GitHub Free để xuất bản qua Pages).
- **Add a README file:** không cần bật, vì bộ web đã có sẵn `README.md`.

Nhấn **Create repository**.

## PHẦN C — TẢI WEB LÊN GITHUB

**Bước 9.** Tại repository mới, tìm đường dẫn **uploading an existing file**. Nếu đã có file trong repo, chọn **Add file → Upload files**.

**Bước 10.** Mở Finder trên Mac → mở thư mục `ban-tin-moc` đã giải nén.

**Bước 11.** Chọn **toàn bộ nội dung bên trong thư mục** (`index.html`, `bai-viet.html`, `assets`, ...), rồi kéo thả vào khu vực upload trên GitHub. Có thể kéo thả nguyên thư mục vào vùng upload rồi kiểm tra danh sách tệp trước khi xác nhận. Quan trọng: GitHub phải hiển thị `index.html` ở **cấp gốc** của repository, cùng cấp với thư mục `assets`.

**KHÔNG làm:** chỉ upload file `.zip` hoặc upload nhầm cả thư mục cha để tạo đường dẫn `ban-tin-moc/index.html`. Làm thế GitHub Pages sẽ không tìm được trang chủ ở `/`.

**Bước 12.** Kéo xuống, tại **Commit message**, nhập `Upload website lan dau` → chọn **Commit changes** hoặc **Propose changes** tùy giao diện. Nếu có lựa chọn nhánh, hãy chọn cập nhật trực tiếp nhánh `main` của chính m để dễ nhất.

**Bước 13.** Trở lại tab **Code** của repository, kiểm tra cấu trúc tối thiểu phải là:

```text
index.html
bai-viet.html
chuyen-muc.html
tim-kiem.html
da-luu.html
gioi-thieu.html
assets/
  css/style.css
  js/data.js
  js/app.js
  images/...
```

**Bước 14.** File `.nojekyll` là file ẩn nên có thể không nhìn thấy trong Finder. Không sao: dự án này vẫn có thể chạy khi thiếu nó. Nếu muốn thêm, tạo file tên `.nojekyll` ở cấp gốc trên GitHub.

## PHẦN D — BẬT GITHUB PAGES (QUAN TRỌNG NHẤT)

**Bước 15.** Trên repository, chọn tab **Settings** (Cài đặt).

**Bước 16.** Nhìn thanh menu trái, kéo xuống tìm **Pages** (trong nhóm Code and automation).

**Bước 17.** Tại **Build and deployment**:

1. **Source:** chọn **Deploy from a branch**.
2. **Branch:** chọn `main`.
3. **Folder:** chọn `/(root)`.
4. Nhấn **Save**.

**Bước 18.** Quay lại trang **Settings → Pages**, khi GitHub hiển thị **Visit site** thì nhấn để mở website. Nếu chưa có đường dẫn, làm mới trang Pages và kiểm tra mục **Actions** để xem tác vụ xuất bản.

**Đường dẫn website thường có dạng:**

```text
https://TEN-TAI-KHOAN.github.io/ban-tin-moc/
```

Thay `TEN-TAI-KHOAN` bằng username GitHub của m. Nếu repository của m có tên khác, thay luôn phần `ban-tin-moc` bằng tên repository thực tế. Đây là URL mẫu, không phải đường dẫn đã được tạo.

**Bước 19.** Mở website bằng chế độ ẩn danh hoặc điện thoại để kiểm tra thật: thử bấm Trang chủ, Chuyên mục, Đọc bài, Tìm kiếm và Bài đã lưu. HTTPS và tên miền phụ `github.io` được GitHub cung cấp.

## PHẦN E — ĐỔI TÊN WEBSITE & LOGO

Mở repository trên GitHub, lần lượt bấm `assets` → `js` → `data.js`. Tìm biểu tượng hình cây bút **Edit this file** (Chỉnh sửa tệp).

Ở gần đầu file có:

```js
window.SITE = {
  name: 'BẢN TIN MỘC',
  brandMain: 'BẢN TIN',
  brandAccent: 'MỘC.',
  shortName: 'MỘC.',
  tagline: 'Đọc chậm một chút. Hiểu sâu hơn một chút.',
  // ...
};
```

Ví dụ muốn tên **THỜI KHẮC.** thì sửa:

```js
name: 'THỜI KHẮC',
brandMain: 'THỜI',
brandAccent: 'KHẮC.',
shortName: 'KHẮC.',
tagline: 'Tin tức trong một góc nhìn mới.',
```

Bấm **Commit changes** để lưu. Không cần sửa toàn bộ các file HTML.

**Lưu ý:** favicon (chữ M trong tab trình duyệt) vẫn là logo minh họa. Nếu muốn đổi, mở `assets/images/favicon.svg` để sửa chữ M hoặc tải lên icon khác cùng tên.

## PHẦN F — THAY BẢNG MÀU

Mở `assets/css/style.css`, bấm nút cây bút và tìm ở những dòng đầu:

```css
--ivory:#EEEAE6;
--beige:#D7B689;
--ochre:#C38C55;
--brick:#813527;
```

Thay các mã HEX theo ý muốn → **Commit changes**. Toàn website sẽ đổi màu theo, không cần chỉnh từng mục một.

## PHẦN G — SỬA BÀI VIẾT HOẶC THÊM BÀI MỚI

Mở `assets/js/data.js`, kéo đến phần `window.ARTICLES = [`.

Mỗi bài có mẫu như sau:

```js
{
  id:'bai-viet-moi',
  category:'van-hoa',
  views:100,
  title:'Tiêu đề của bài viết mới',
  excerpt:'Một đoạn mô tả ngắn về bài viết.',
  author:'Tên tác giả',
  date:'2026-11-04',
  image:'culture',
  reading:4,
  body:[
    'Đoạn mở đầu của bài viết.',
    'Đoạn nội dung thứ hai.',
    'Đoạn nội dung thứ ba.'
  ]
},
```

**Để thay bài hiện có:** tìm tiêu đề trong file, sửa `title`, `excerpt`, `body`, `author`, `date` rồi Commit changes.

**Để thêm bài:** sao chép một khối `{ ... },` từ bài khác, dán vào cuối danh sách *trước dấu `];`*, đổi `id` thành mã mới **không trùng** và cập nhật các trường. Lưu ý dấu phẩy giữa các bài và dấu nháy đơn trong chuỗi JavaScript. Nếu chưa quen code, m nên sửa một bài có sẵn trước.

Các giá trị `category` hợp lệ:

`thoi-su`, `doi-song`, `giao-duc`, `van-hoa`, `cong-nghe`, `kinh-te`, `goc-nhin`, `moi-truong`, `du-lich`, `suc-khoe`.

Bài sẽ **tự xuất hiện** trong chuyên mục tương ứng. Trang chủ sắp bài theo `date` từ mới đến cũ. Không cần tạo một trang HTML riêng cho từng bài.

**Để đưa bài mới lên vùng đầu trang:** sửa `date` thành ngày mới nhất. Dòng `featured:true` là metadata để mở rộng về sau; vùng tiêu điểm hiện chọn bài mới nhất theo ngày.

## PHẦN H — THAY ẢNH BẰNG ẢNH CỦA M

M có 2 lựa chọn:

**Cách 1 — Dùng minh họa có sẵn, luôn chạy kể cả offline:** đổi `useOnlinePhotos: true` thành `useOnlinePhotos: false` trong `data.js`. File SVG được lưu sẵn trong `assets/images`.

**Cách 2 — Dùng ảnh thật của riêng m:**

1. Tải ảnh `.jpg`, `.png` hoặc `.webp` lên thư mục `assets/images/` trong repository.
2. Trong bài tương ứng ở `assets/js/data.js`, thêm trường `photo` như sau:

```js
photo:'./assets/images/anh-trang-chu.jpg',
```

3. Bấm Commit changes. Ảnh riêng sẽ được ưu tiên hơn ảnh Unsplash mặc định.
4. Nên dùng ảnh nén dưới khoảng 300–600 KB nếu có thể, để website tải nhanh.

Đặt tên ảnh không dấu, không có khoảng trắng. Ví dụ: `ha-noi-sang.jpg`.

**Quyền ảnh:** chỉ dùng ảnh m sở hữu hoặc có giấy phép phù hợp. Các link Unsplash mặc định trong bộ demo là ảnh minh họa từ bên thứ ba và cần Internet.

## PHẦN I — WEBSITE BỊ LỖI THÌ LÀM GÌ?

| Triệu chứng | Nguyên nhân thường gặp | Cách xử lý |
|---|---|---|
| Vào URL thấy trang 404 | Chưa bật Pages hoặc `index.html` bị nằm trong thư mục con | Vào Settings → Pages, kiểm tra `main / (root)` và vị trí file |
| Giao diện chỉ còn chữ, không có màu | Thiếu file CSS | Kiểm tra `assets/css/style.css` trong repository |
| Trang trống, không có bài | Thiếu `data.js`, `app.js` hoặc code sai dấu | Kiểm tra cả hai file và sửa cú pháp vừa chỉnh |
| Ảnh tải không lên | Ảnh online lỗi hoặc địa chỉ ảnh tự thêm sai | Đổi `useOnlinePhotos:false` để dùng SVG, hoặc kiểm tra file ảnh |
| Menu chạy nhưng trang bài viết lỗi | Link `id` không khớp bài trong dữ liệu | Kiểm tra `id` duy nhất của bài |
| Đã sửa nhưng chưa thấy thay đổi | Trình duyệt còn cache hoặc Pages chưa cập nhật | Làm mới trang, thử ẩn danh và kiểm tra tác vụ Actions |
| Bài lưu biến mất khi đổi máy | Lưu trong bộ nhớ trình duyệt của một máy | Đây là giới hạn thiết kế tĩnh, không có đồng bộ tài khoản |

## PHẦN J — ĐIỀU GÌ FREE VÀ ĐIỀU GÌ CHƯA CÓ?

**Miễn phí:** mã HTML/CSS/JS, giao diện desktop/mobile, trang chủ và trang bài, tìm kiếm nội bộ, lưu bài cục bộ, hosting GitHub Pages ở repository Public, đường dẫn `github.io`.

**Không có sẵn:** bảng quản trị như WordPress, tài khoản độc giả, bình luận lưu trên máy chủ, analytics chuyên nghiệp, gửi email thật, database, hệ thống phân quyền nhiều biên tập viên.

**Giới hạn GitHub Pages:** website tĩnh này phù hợp demo, học tập, portfolio/dự án nội dung nhỏ; không nên coi là hosting miễn phí không giới hạn cho báo thương mại quy mô lớn. GitHub có quota và điều khoản sử dụng riêng.

**Lưu ý minh bạch:** website hiện ghi rõ *Bản trình diễn / Nội dung minh họa*, vì các tiêu đề và bài viết là nội dung giả lập. Khi vận hành thật, thay bằng thông tin đã được xác minh, trích nguồn và tuân thủ quy định liên quan.

## NGUỒN CHÍNH THỨC

- GitHub Pages: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- Bật xuất bản bằng nhánh: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- Upload file/folder: https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
- Giới hạn và điều khoản: https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits

Chỉ cần làm đúng **PHẦN A → B → C → D** là đưa được bản website lên Internet. Các phần sau để m tùy chỉnh theo ý mình.
