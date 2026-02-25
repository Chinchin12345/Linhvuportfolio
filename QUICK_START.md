# ⚡ Quick Start - Option 2 (15 phút)

## 🎯 Mục Tiêu
Import portfolio vào Figma tự động bằng plugin html.to.design

---

## ✅ Checklist Trước Khi Bắt Đầu

- [ ] Có Figma account (Free hoặc Pro)
- [ ] Đã cài Figma Desktop HOẶC dùng Web
- [ ] Có Terminal/Command Prompt
- [ ] Portfolio files đầy đủ trong folder "Cursor Port"

---

## 🚀 3 Bước Chính

```
Step 1: Start Local Server  →  Step 2: Install Plugin  →  Step 3: Import
   (2 phút)                        (2 phút)                  (5-10 phút)
```

---

## 📋 STEP 1: Start Local Server

### Mac/Linux:

```bash
# 1. Mở Terminal (Cmd + Space, gõ "Terminal")

# 2. Di chuyển đến folder
cd "/Users/linh/Documents/2026/00. Portfolio/Cursor Port"

# 3. Start server
python3 -m http.server 8000

# ✅ Thấy "Serving HTTP on..." = Success!
```

### Windows:

```bash
# 1. Mở Command Prompt (Win + R, gõ "cmd")

# 2. Di chuyển đến folder
cd "C:\Users\...\Cursor Port"

# 3. Start server
python -m http.server 8000

# ✅ Thấy "Serving HTTP on..." = Success!
```

### ✅ Test:
- Mở browser: `http://localhost:8000`
- Thấy portfolio? → ✅ Ready!
- **KHÔNG TẮT Terminal!** Giữ nó chạy.

---

## 📋 STEP 2: Install Plugin

### Trong Figma:

```
1. Mở Figma (Desktop hoặc Web)

2. Tạo file mới
   - Click "New design file"
   - Đặt tên: "Linh Vu Portfolio"

3. Mở Plugin Browser
   - Menu → Plugins → Browse plugins in Community
   - HOẶC: Right-click → Plugins → Browse...

4. Search & Install
   - Gõ: "html.to.design"
   - Click plugin (by BuilderX)
   - Click "Install" (nút xanh)

✅ Done! Plugin installed.
```

---

## 📋 STEP 3: Import Portfolio

### Trong Figma file vừa tạo:

```
1. Run Plugin
   - Menu → Plugins → html.to.design
   - HOẶC: Right-click → Plugins → html.to.design

2. Enter URL
   📌 QUAN TRỌNG: Nhập chính xác

   URL: http://localhost:8000

   (Không có dấu "/" ở cuối)

3. Click "Fetch"
   - Plugin sẽ load HTML
   - Đợi 5-10 giây

4. Configure (Optional)
   ✅ Import images: ON
   ✅ Import styles: ON
   ✅ Create components: ON
   Width: 1440px

5. Click "Import"
   - Đợi 2-5 phút
   - Plugin đang convert HTML → Figma

✅ Done! Portfolio imported.
```

---

## 🎉 Kết Quả

Bạn sẽ thấy:
```
Portfolio Frames:
├── Navigation
├── Hero Section
├── Project 01 - AEON Mall
├── Project 02 - Yatabe Arena
├── Project 03 - TOTO Showroom (với 6 ảnh)
├── Project 04 - Toyota
├── Project 05 - Minato Residence
├── Project 06 - Luxury Interiors
├── Project 07 - Hotel Suite
├── Project 08 - MEDRING Dental
├── About Section (với TOTO image grid)
├── Contact Section
└── Footer
```

---

## 🛠️ Immediate Actions

### 1. Organize (2 phút)
```
- Select all frames
- Press: Cmd/Ctrl + G (Group)
- Rename group: "Portfolio Import"
```

### 2. Setup Container (1 phút)
```
- Select group
- Press: Shift + A (Auto Layout)
- Direction: Vertical
- Spacing: 0
```

### 3. Quick Clean (3 phút)
```
- Remove duplicate layers
- Delete empty frames
- Rename sections clearly
```

---

## 🎨 Customize Time!

Bây giờ bạn có thể:

✏️ **Edit Colors**
- Select element
- Change fill colors
- Use: #D4AF37 (gold), #2C2C2C (dark)

📝 **Edit Text**
- Double-click text
- Edit content
- Change fonts

🖼️ **Replace Images**
- Drag new images vào Figma
- Right-click image → Replace image

📐 **Adjust Layout**
- Drag elements
- Resize frames
- Change spacing

---

## 🐛 Troubleshooting

### "Cannot connect to URL"
```
❌ Problem: Server không chạy hoặc sai URL

✅ Fix:
1. Check Terminal - còn chạy?
2. Test: http://localhost:8000 trong browser
3. Restart server nếu cần
4. Try import lại
```

### "Images not imported"
```
❌ Problem: Plugin không load được local images

✅ Fix:
1. Manual: Drag images từ assets/images/ vào Figma
2. Replace trong frames
```

### "Layout looks broken"
```
❌ Problem: Plugin không convert perfect CSS

✅ Fix:
1. Bình thường! Plugin có giới hạn
2. Use imported version làm reference
3. Recreate sections với Auto Layout
4. Follow DESIGN_GUIDE.md
```

---

## ⏱️ Timeline

```
🕐 0:00  - Start server
🕐 0:02  - Open Figma, create file
🕐 0:04  - Install plugin
🕐 0:06  - Enter URL, configure
🕐 0:08  - Click Import
🕐 0:08-0:15 - Wait for import
🕐 0:15  - ✅ Done! Start customizing
```

**Total: ~15 phút**

---

## 📚 Detailed Guides

Nếu cần chi tiết hơn:
- **Server setup**: `START_SERVER.md`
- **Plugin guide**: `FIGMA_PLUGIN_GUIDE.md`
- **Design system**: `DESIGN_GUIDE.md`

---

## 💡 Pro Tips

1. **Keep Terminal Open**
   - Cần server chạy trong khi import
   - Có thể tắt sau khi import xong

2. **Save Progress**
   - Figma auto-saves
   - Nhưng đặt tên file rõ ràng
   - "Linh Vu Portfolio - v1"

3. **Duplicate Before Edit**
   - Cmd/Ctrl + D to duplicate frames
   - Giữ original làm backup
   - Edit trên copy

4. **Use Components**
   - Convert repeated elements → Components
   - Easier to update globally

---

## ✅ Success!

Khi thấy portfolio trong Figma:
- ✅ All sections imported
- ✅ Images visible
- ✅ Text readable
- ✅ Layout reasonable

→ **Ready to customize! 🎉**

---

**Need help? Check:**
- START_SERVER.md
- FIGMA_PLUGIN_GUIDE.md
- DESIGN_GUIDE.md

**Good luck! 🚀✨**
