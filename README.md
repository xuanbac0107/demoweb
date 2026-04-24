# Website Việt Nan - Nhập Hàng Chính Ngạch Trung Quốc

Website giới thiệu dịch vụ nhập hàng chính ngạch Trung Quốc - Việt Nam, được thiết kế responsive, sẵn sàng triển khai lên internet.

## Tính Năng

- **Responsive Design** – hiển thị tốt trên mobile, tablet, desktop
- **Smooth scroll** giữa các section
- **Sticky header** tự động thay đổi khi cuộn trang
- **Active navigation** tự động highlight menu theo vị trí cuộn
- **Counter animation** cho các con số thống kê
- **Fade-in animations** khi cuộn đến các phần nội dung
- **Mobile menu** với hamburger icon
- **Back to top** button
- **SEO-friendly** với meta tags đầy đủ
- **Font Awesome icons** (via CDN)
- **Google Fonts** – Be Vietnam Pro

## Cấu Trúc Dự Án

```
demowebsite/
├── index.html          # Trang chủ
├── css/
│   └── style.css       # Toàn bộ styles
├── js/
│   └── main.js         # JavaScript cho tương tác
├── images/             # Thư mục chứa hình ảnh (có thể thêm)
└── README.md
```

## Chạy Website Trên Máy

### Cách 1: Mở trực tiếp
Kéo thả `index.html` vào trình duyệt (Chrome/Firefox/Edge).

### Cách 2: Dùng Live Server (khuyến nghị)
1. Mở dự án trong **VS Code**
2. Cài extension **Live Server**
3. Chuột phải vào `index.html` → **Open with Live Server**

### Cách 3: Dùng Python server
```bash
cd demowebsite
python -m http.server 8000
```
Mở trình duyệt: `http://localhost:8000`

## Triển Khai Lên Internet

### GitHub Pages (miễn phí)
```bash
cd demowebsite
git init
git add .
git commit -m "Initial website"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```
Vào **Settings** → **Pages** → chọn branch `main` → Save.

### Netlify (miễn phí – dễ nhất)
1. Đăng ký tại [netlify.com](https://www.netlify.com/)
2. Kéo thả thư mục `demowebsite` vào **Netlify Drop**
3. Nhận URL public ngay lập tức

### Vercel (miễn phí)
1. Cài CLI: `npm i -g vercel`
2. Chạy: `vercel` trong thư mục dự án
3. Follow hướng dẫn

## Tùy Chỉnh

### Đổi màu chủ đạo
Mở [css/style.css](css/style.css), sửa biến CSS trong `:root`:

```css
:root {
    --primary: #1a4ec7;     /* Màu xanh chủ đạo */
    --red: #e53935;          /* Màu đỏ nhấn */
}
```

### Đổi thông tin liên hệ
Tìm và thay trong [index.html](index.html):
- Số điện thoại: `0936 123 456`
- Email: `info@vietnan.com.vn`
- Địa chỉ: `Số 12, Nguyễn Văn Linh, Long Biên, Hà Nội`

### Thêm hình ảnh thật
Thay ảnh SVG mẫu ở hero section bằng ảnh thật trong thư mục [images/](images/):

```css
.hero::before {
    background-image: url('../images/hero-bg.jpg');
}
```

## Trình Duyệt Hỗ Trợ

Chrome / Edge / Firefox / Safari (phiên bản 2 năm trở lại).

## License

Dùng tự do cho mục đích cá nhân hoặc thương mại.
