# Portfolio - 3D Architectural Design

Trang portfolio hiện đại và chuyên nghiệp để trưng bày các dự án thiết kế kiến trúc 3D của bạn.

## Tính năng

- ✨ Thiết kế sang trọng, tối giản theo phong cách DeGraw & DeHaan
- 📱 Responsive hoàn toàn (desktop, tablet, mobile)
- 🎨 Hiệu ứng hover và animations mượt mà
- 🖼️ Gallery dự án với masonry layout
- 📧 Form liên hệ tích hợp
- ⚡ Performance tối ưu
- 🎯 Navigation mượt mà với scroll spy

## Cấu trúc file

```
Cursor Port/
├── index.html          # Trang chính
├── styles.css          # Stylesheet
├── script.js           # JavaScript cho tương tác
├── assets/
│   └── images/         # Thư mục chứa hình ảnh
└── README.md          # Tài liệu hướng dẫn
```

## Các section trong trang

1. **Navigation** - Menu điều hướng fixed với hiệu ứng
2. **Hero Section** - Banner chào mừng với CTA buttons
3. **Projects** - Gallery trưng bày các dự án với 6 projects:
   - AEON Shopping Mall
   - Contemporary Gas Station
   - TOTO Premium Showroom
   - Toyota Dealership
   - Commercial Complex
   - Luxury Interior Spaces
4. **About** - Giới thiệu với statistics
5. **Contact** - Form liên hệ và thông tin
6. **Footer** - Footer với social links

## Cách sử dụng

### 1. Xem trang web

Mở file `index.html` trong trình duyệt web:
- Click đúp vào file `index.html`
- Hoặc kéo thả file vào trình duyệt
- Hoặc sử dụng Live Server trong VS Code

### 2. Chỉnh sửa nội dung

#### Thay đổi tiêu đề và mô tả:
Mở `index.html` và tìm các phần:
- Hero title: Dòng ~35
- Project descriptions: Dòng ~70+
- About section: Dòng ~180+
- Contact info: Dòng ~220+

#### Thêm/xóa dự án:
- Copy một `<div class="project-card">...</div>`
- Thay đổi hình ảnh trong thẻ `<img src="...">`
- Cập nhật category, title, và description

#### Thay đổi màu sắc:
Mở `styles.css` và chỉnh sửa các biến CSS (dòng ~9-16):
```css
:root {
    --primary-color: #2c2c2c;
    --accent-color: #d4af37;
    ...
}
```

### 3. Thêm hình ảnh mới

1. Đặt file hình ảnh vào thư mục `assets/images/`
2. Cập nhật đường dẫn trong `index.html`:
   ```html
   <img src="assets/images/ten-hinh-moi.png" alt="Mô tả">
   ```

### 4. Tùy chỉnh fonts

Hiện tại sử dụng Google Fonts:
- **Playfair Display** - Cho tiêu đề
- **Inter** - Cho nội dung

Để thay đổi, cập nhật link trong `<head>` của `index.html`

## Tùy chỉnh nâng cao

### Thay đổi layout grid

Trong `styles.css`, tìm `.projects-grid` (dòng ~353):
```css
.projects-grid {
    grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
    gap: 30px;
}
```

### Tắt/bật hiệu ứng

Trong `script.js`:
- Tắt parallax: Comment dòng 100-107
- Tắt custom cursor: Comment dòng 119-170
- Tắt stats counter: Comment dòng 190-213

### Form submission

Hiện tại form chỉ show alert. Để tích hợp với backend:
1. Mở `script.js`
2. Tìm function form submission (dòng ~90)
3. Thay thế bằng AJAX call hoặc service như Formspree, EmailJS

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers

## Performance Tips

1. Tối ưu hình ảnh trước khi upload (sử dụng TinyPNG, ImageOptim)
2. Sử dụng format WebP cho hình ảnh hiện đại
3. Enable caching nếu deploy lên server
4. Minify CSS và JS cho production

## Deploy

### GitHub Pages
1. Push code lên GitHub repository
2. Settings → Pages → Deploy from main branch
3. Website sẽ có tại: `https://username.github.io/repo-name`

### Netlify
1. Kéo thả thư mục vào Netlify Drop
2. Hoặc connect với Git repository
3. Tự động deploy khi có changes

### Vercel
1. Import GitHub repository
2. Configure build settings (không cần)
3. Deploy tự động

## Liên hệ

Nếu cần hỗ trợ hoặc có câu hỏi, vui lòng liên hệ qua form trong trang web.

## License

Free to use for personal and commercial projects.
