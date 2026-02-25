# 🎨 Figma Plugin Installation & Import Guide

## 📋 Bước 2: Install Plugin "html.to.design"

### Option A: Install từ Figma Desktop/Web

**Bước 1: Mở Figma**
- Desktop: Mở app Figma
- Web: Đi tới https://figma.com

**Bước 2: Tạo File mới**
- Click vào profile/team của bạn
- Click "New design file"
- Đặt tên: "Linh Vu Portfolio"

**Bước 3: Browse Plugins**
- Menu bar → **Plugins** → **Browse plugins in Community**
- Hoặc: Right-click → **Plugins** → **Browse plugins in Community**

**Bước 4: Search & Install**
1. Trong search box, gõ: **"html.to.design"**
2. Click vào plugin (by BuilderX)
3. Click nút **"Install"** (màu xanh)
4. ✅ Done! Plugin đã được cài

---

## 📋 Bước 3: Import Portfolio vào Figma

### Chuẩn bị:
- ✅ Server đang chạy tại `http://localhost:8000`
- ✅ Plugin đã cài trong Figma
- ✅ File Figma mới đã tạo

### Import Process:

**Bước 1: Mở Plugin**
- Trong Figma, menu: **Plugins** → **html.to.design**
- Hoặc: Right-click → **Plugins** → **html.to.design**

**Bước 2: Nhập URL**

Plugin sẽ hiển thị popup. Bạn có 2 options:

**Option A: Import từ URL (Khuyên dùng)**
```
1. Chọn tab "URL"
2. Nhập: http://localhost:8000
3. Click "Fetch"
4. Đợi plugin load HTML
```

**Option B: Import từ HTML Code**
```
1. Chọn tab "Code"
2. Copy toàn bộ nội dung file index.html
3. Paste vào box
4. Click "Import"
```

**Bước 3: Configure Settings (Optional)**

Plugin có thể hỏi settings:
- ✅ **Import images**: Check (để import ảnh)
- ✅ **Import styles**: Check (để giữ colors, fonts)
- ✅ **Create components**: Check (tạo components tự động)
- 📐 **Width**: 1440px (Desktop size)

**Bước 4: Click "Import"**

Plugin sẽ bắt đầu convert:
```
⏳ Parsing HTML...
⏳ Fetching images...
⏳ Creating frames...
⏳ Applying styles...
```

**Thời gian:** 2-5 phút (tùy portfolio size)

---

## ✨ Sau Khi Import

### Bạn sẽ thấy:

**1. Frames Structure:**
```
📁 Portfolio
├── 🖼️ Navigation
├── 🖼️ Hero
├── 🖼️ Projects
│   ├── AEON Mall
│   ├── Yatabe Arena
│   ├── TOTO Showroom
│   ├── Toyota
│   ├── Minato Residence
│   ├── Luxury Interiors
│   ├── Hotel Suite
│   └── MEDRING Dental
├── 🖼️ About
├── 🖼️ Contact
└── 🖼️ Footer
```

**2. Layers Panel:**
- Tất cả sections được convert thành Frames
- Text layers với đúng content
- Images đã được imported
- Colors từ CSS

---

## 🛠️ Bước 4: Clean Up & Organize

### Ngay sau import, làm những việc này:

**1. Rename Frames**
```
Frame 1 → Navigation
Frame 2 → Hero Section
Frame 3 → Project 01 - AEON
...
```

**2. Group Related Elements**
- Select multiple layers: `Cmd + Click` (Mac) / `Ctrl + Click` (Win)
- Group: `Cmd + G` / `Ctrl + G`

**3. Create Main Container**
```
1. Select tất cả frames
2. Frame selection: `Cmd + Option + G` / `Ctrl + Alt + G`
3. Rename: "Portfolio - Desktop 1440px"
```

**4. Setup Auto Layout**
```
1. Select container frame
2. Click "+" button bên cạnh "Auto layout"
3. Hoặc: Shift + A
4. Settings:
   - Direction: Vertical
   - Spacing: 0 (sections đã có padding riêng)
   - Padding: 0
```

---

## 🎨 Bước 5: Apply Design System

### Colors

**Tạo Color Styles:**
```
1. Rectangle tool (R)
2. Fill với color: #2C2C2C
3. Select fill swatch → Right-click → "Create style"
4. Name: "Primary/Dark"
5. Repeat cho tất cả colors:
   - Primary/Dark: #2C2C2C
   - Accent/Gold: #D4AF37
   - Secondary/Light: #F5F5F5
   - Text/Dark: #1A1A1A
   - Text/Light: #666666
```

**Apply to Existing Elements:**
```
1. Select element with color
2. Click fill swatch
3. Choose color style vừa tạo
```

### Typography

**Tạo Text Styles:**
```
1. Text tool (T)
2. Set font: Playfair Display, 56px, Bold
3. Select text → Right-click → "Create style"
4. Name: "H1 / Display"
5. Repeat cho:
   - H1 / Display: Playfair Display, 56px, Bold
   - H2 / Section: Playfair Display, 48px, Bold
   - H3 / Project: Playfair Display, 32px, Semi-bold
   - Body / Large: Inter, 18px, Regular
   - Body / Regular: Inter, 16px, Regular
   - Label / Small: Inter, 14px, Medium
```

---

## 🐛 Troubleshooting

### Issue 1: Plugin không load được URL

**Nguyên nhân:** Server không chạy hoặc sai URL

**Giải quyết:**
```
1. Check Terminal - Server còn chạy không?
2. Test browser: http://localhost:8000
3. Nếu không mở được → Restart server
4. Try lại trong plugin
```

### Issue 2: Images không import

**Nguyên nhân:** Plugin không fetch được local images

**Giải quyết:**
```
Option A: Manual import
1. Drag images từ thư mục assets/images/ vào Figma
2. Replace trong frames

Option B: Use absolute paths
1. Ensure server running
2. Images phải accessible qua http://localhost:8000/assets/images/
```

### Issue 3: Layout bị broken

**Nguyên nhân:** Plugin không convert hoàn hảo CSS

**Giải quyết:**
```
1. Đây là bình thường với CSS phức tạp
2. Use imported version làm reference
3. Recreate sections với Auto Layout
4. Follow DESIGN_GUIDE.md
```

### Issue 4: Fonts không đúng

**Nguyên nhân:** Figma chưa có fonts

**Giải quyết:**
```
1. Download fonts:
   - Playfair Display: https://fonts.google.com/specimen/Playfair+Display
   - Inter: https://fonts.google.com/specimen/Inter
2. Install fonts trên máy
3. Restart Figma
4. Apply lại text styles
```

---

## 🎯 Next Steps

Sau khi import thành công:

**1. Review & Clean:**
- [ ] Check tất cả sections imported đúng
- [ ] Remove unnecessary layers
- [ ] Group và organize

**2. Setup Design System:**
- [ ] Create color styles
- [ ] Create text styles
- [ ] Create component library

**3. Create Components:**
- [ ] Button components
- [ ] Navigation components
- [ ] Project card components
- [ ] Contact item components

**4. Add Auto Layout:**
- [ ] Apply to all sections
- [ ] Setup responsive constraints
- [ ] Test resizing

**5. Create Variants:**
- [ ] Desktop (1440px)
- [ ] Tablet (768px)
- [ ] Mobile (375px)

**6. Add Prototypes:**
- [ ] Navigation links
- [ ] Button interactions
- [ ] Hover states
- [ ] Scroll animations

---

## 💡 Pro Tips

### Speed Up Workflow:

1. **Keyboard Shortcuts:**
```
R = Rectangle
T = Text
F = Frame
A = Auto Layout
Cmd/Ctrl + D = Duplicate
Cmd/Ctrl + G = Group
Option/Alt + Drag = Duplicate while moving
```

2. **Use Plugins:**
- **Unsplash** - Replace images
- **Iconify** - Add icons
- **Content Reel** - Fill text content
- **Anima** - Export to code

3. **Components Best Practices:**
- Create master components page
- Use variants for states
- Name clearly: "Button/Primary/Default"
- Use auto layout for flexibility

---

## ✅ Success Checklist

Import thành công khi:
- ✅ Tất cả sections hiển thị trong Figma
- ✅ Images đã imported
- ✅ Text content đầy đủ
- ✅ Colors gần giống website
- ✅ Layout structure đúng

**→ Bạn đã sẵn sàng customize trong Figma! 🎉**

---

## 📞 Need Help?

**Resources:**
- Plugin docs: https://www.builder.io/c/docs/import-from-figma
- Figma help: https://help.figma.com
- Design guide: Xem `DESIGN_GUIDE.md`

---

**Good luck với Figma! 🚀✨**
