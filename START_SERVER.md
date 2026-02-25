# 🚀 Start Local Server - Quick Guide

## Method 1: Python (Khuyên dùng - Có sẵn trên Mac)

### Bước 1: Mở Terminal
- Press `Cmd + Space`
- Gõ "Terminal"
- Press Enter

### Bước 2: Di chuyển đến thư mục Portfolio
```bash
cd "/Users/linh/Documents/2026/00. Portfolio/Cursor Port"
```

### Bước 3: Start server
```bash
python3 -m http.server 8000
```

**Bạn sẽ thấy:**
```
Serving HTTP on :: port 8000 (http://[::]:8000/) ...
```

### Bước 4: Test trong browser
- Mở Chrome/Safari
- Vào: `http://localhost:8000`
- Portfolio sẽ hiển thị!

### ⚠️ LƯU Ý:
- **KHÔNG TẮT Terminal** - Giữ nó chạy!
- Cần server chạy để plugin Figma có thể fetch
- Để dừng server: Press `Ctrl + C` trong Terminal

---

## Method 2: Node.js (Nếu có cài)

```bash
# Cài http-server (chỉ cần 1 lần)
npm install -g http-server

# Start server
cd "/Users/linh/Documents/2026/00. Portfolio/Cursor Port"
http-server -p 8000
```

---

## Method 3: VS Code (Nếu dùng VS Code)

1. Mở thư mục "Cursor Port" trong VS Code
2. Install extension "Live Server"
3. Right-click vào `index.html`
4. Chọn "Open with Live Server"
5. Sẽ mở tại `http://127.0.0.1:5500`

**Lưu ý:** Nếu dùng Live Server, URL sẽ là `http://127.0.0.1:5500` thay vì `http://localhost:8000`

---

## ✅ Kiểm Tra Server Đã Chạy Chưa

### Test 1: Mở Browser
- Vào: `http://localhost:8000`
- Nếu thấy portfolio → ✅ Success!

### Test 2: Check Terminal
- Thấy message "Serving HTTP..." → ✅ Running
- Có error → ❌ Check lại commands

---

## 🐛 Troubleshooting

### Error: "Address already in use"
**Nghĩa là:** Port 8000 đang được dùng

**Giải quyết:** Dùng port khác
```bash
python3 -m http.server 8080
# Sau đó dùng: http://localhost:8080
```

### Error: "python3: command not found"
**Nghĩa là:** Python chưa cài

**Giải quyết:** Dùng Python 2
```bash
python -m SimpleHTTPServer 8000
```

### Error: "No such file or directory"
**Nghĩa là:** Sai đường dẫn

**Giải quyết:**
```bash
# Kiểm tra đường dẫn
pwd

# Nếu sai, cd đúng thư mục
cd "/Users/linh/Documents/2026/00. Portfolio/Cursor Port"
```

---

## 🎯 Ready for Figma!

Khi server đã chạy:
- ✅ Terminal vẫn mở và hiển thị "Serving HTTP..."
- ✅ Browser mở `http://localhost:8000` thấy portfolio
- ✅ Sẵn sàng cho bước tiếp theo!

**→ Chuyển sang Bước 2: Install Plugin trong Figma**

---

**💡 Tip:** Bookmark `http://localhost:8000` để test dễ dàng!
