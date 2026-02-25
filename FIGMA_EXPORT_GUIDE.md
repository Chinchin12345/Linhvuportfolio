# 🎨 Hướng Dẫn Xuất Portfolio sang Figma

## 📌 Các Phương Pháp

### ✅ Phương Pháp 1: Sử dụng Plugin "html.to.design" (Khuyên dùng)

**Bước 1: Cài đặt Plugin**
1. Mở Figma Desktop hoặc Web
2. Menu → Plugins → Browse plugins in Community
3. Tìm "html.to.design"
4. Click "Install"

**Bước 2: Host Website Local**
```bash
# Trong thư mục Cursor Port
python3 -m http.server 8000
# Hoặc
python -m SimpleHTTPServer 8000
```

**Bước 3: Import vào Figma**
1. Mở Figma, tạo file mới
2. Plugins → html.to.design
3. Nhập URL: `http://localhost:8000`
4. Click "Import"

**Lưu ý:**
- Plugin sẽ convert HTML/CSS thành Figma frames
- Có thể mất vài phút với portfolio lớn
- Cần chỉnh sửa lại một số elements

---

### ✅ Phương Pháp 2: Screenshot + Manual Design (Chính xác nhất)

**Bước 1: Chụp Screenshots**
- Mở `index.html` trong Chrome
- Sử dụng extension "GoFullPage" hoặc "Awesome Screenshot"
- Chụp full page screenshot

**Bước 2: Import vào Figma**
1. Tạo Frame mới (Desktop: 1440x...)
2. Kéo screenshot vào làm reference layer
3. Lock layer này (Cmd/Ctrl + Shift + L)
4. Set opacity: 50%

**Bước 3: Recreate**
- Trace từng section theo screenshot
- Sử dụng DESIGN_GUIDE.md cho colors, fonts, spacing
- Tạo components cho elements tái sử dụng

---

### ✅ Phương Pháp 3: Copy Images & Manual Layout

**Bước 1: Chuẩn bị Assets**
```bash
# Tất cả ảnh đã có trong:
Cursor Port/assets/images/
```

**Bước 2: Setup Figma File**
1. Tạo file mới: "Linh Vu Portfolio"
2. Tạo Pages:
   - 🎨 Design System
   - 🖥️ Desktop (1440px)
   - 📱 Mobile (375px)
   - 📦 Components

**Bước 3: Setup Design System**

**Colors:**
```
Primary Dark:    #2C2C2C
Secondary Light: #F5F5F5
Accent Gold:     #D4AF37
Text Dark:       #1A1A1A
Text Light:      #666666
White:           #FFFFFF
```

**Typography:**
```
Headings: Playfair Display
Body:     Inter

H1: 56px / Bold
H2: 48px / Bold
H3: 32px / Semi-bold
Body: 18px / Regular
Small: 14px / Medium
```

**Bước 4: Tạo Layout**
- Frame: 1440px width
- Columns: 12 columns, 80px margins, 30px gutter
- Auto Layout cho sections

---

## 🎯 Template Structure trong Figma

```
📁 Linh Vu Portfolio
├── 🎨 Design System
│   ├── Colors
│   ├── Typography
│   ├── Spacing
│   └── Components
│
├── 🖥️ Desktop
│   ├── Navigation
│   ├── Hero
│   ├── Projects (8 sections)
│   ├── About
│   ├── Contact
│   └── Footer
│
├── 📱 Tablet (768px)
│   └── [Same sections, responsive]
│
└── 📱 Mobile (375px)
    └── [Same sections, mobile layout]
```

---

## 🛠️ Components cần tạo trong Figma

### 1. Navigation Bar
- Auto Layout (Horizontal)
- Logo (Text)
- Menu Items (Component với hover state)
- Hamburger (Mobile variant)

### 2. Buttons
- Primary Button (Component)
  - Default state
  - Hover state
  - Pressed state
- Secondary Button (Variant)

### 3. Project Card
- Auto Layout (Horizontal or Vertical)
- Image container
- Text content
- Number badge
- Category tag

### 4. Contact Item
- Auto Layout (Horizontal)
- Label
- Value
- Divider line
- Hover state

---

## 📋 Checklist Export

### Files cần có:
- ✅ `index.html` - Đã có
- ✅ `styles.css` - Đã có
- ✅ `script.js` - Đã có
- ✅ `DESIGN_GUIDE.md` - Đã có
- ✅ `README.md` - Đã có
- ✅ Tất cả ảnh trong `assets/images/`

### Design Elements:
- ✅ 8 Project sections với mô tả chi tiết
- ✅ TOTO gallery (6 ảnh)
- ✅ About section với image grid
- ✅ Contact section minimal design
- ✅ Responsive breakpoints

---

## 💡 Tips Quan Trọng

### Khi Recreate trong Figma:

1. **Sử dụng Auto Layout**
   - Tất cả sections dùng Auto Layout
   - Dễ dàng responsive và chỉnh sửa spacing

2. **Tạo Components**
   - Button, Card, Nav item → Components
   - Hover states → Variants
   - Responsive → Variants

3. **Organize Layers**
   ```
   Section
   ├── Container (Auto Layout)
   │   ├── Content (Auto Layout)
   │   │   ├── Number
   │   │   ├── Category
   │   │   ├── Title
   │   │   └── Description
   │   └── Image
   ```

4. **Use Constraints**
   - Container: Left & Right (stretch)
   - Content: Center
   - Images: Scale (cover)

5. **Grid Setup**
   - Desktop: 12 columns, 80px margin
   - Tablet: 8 columns, 40px margin
   - Mobile: 4 columns, 20px margin

---

## 🚀 Quick Start

### Option A: Nhanh (30 phút)
1. Screenshot full website
2. Import vào Figma
3. Trace sections chính
4. Chỉnh sửa theo ý muốn

### Option B: Professional (2-3 giờ)
1. Setup Design System
2. Tạo Components library
3. Build từng section với Auto Layout
4. Add interactions và prototypes

### Option C: Full Migration (1 ngày)
1. Host website + use html.to.design
2. Clean up imported layers
3. Organize và tạo components
4. Setup variants và responsive
5. Add prototypes đầy đủ

---

## 📞 Resources

- **Figma Plugin**: html.to.design
- **Chrome Extension**: GoFullPage (screenshots)
- **Font Files**:
  - [Playfair Display](https://fonts.google.com/specimen/Playfair+Display)
  - [Inter](https://fonts.google.com/specimen/Inter)
- **Design Guide**: Xem `DESIGN_GUIDE.md`

---

## ✨ Sau khi Export

Trong Figma, bạn có thể:
- ✏️ Chỉnh sửa colors, fonts, spacing
- 🎨 Thử nghiệm layouts mới
- 📱 Tạo mobile/tablet versions
- 🔗 Add prototypes và interactions
- 👥 Share với clients để feedback
- 📤 Export cho developers

---

**Chúc bạn thành công với Figma! 🎉**

Questions? Check DESIGN_GUIDE.md for details.
