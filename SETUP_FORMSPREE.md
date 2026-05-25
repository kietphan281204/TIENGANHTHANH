# 🚀 HƯỚNG DẪN SETUP FORMSPREE - TỪNG BƯỚC CHI TIẾT

## ⏱️ Tổng thời gian: 2-3 phút

---

## 📝 BƯỚC 1: Đăng ký Formspree (1 phút)

1. **Mở trình duyệt** và truy cập: https://formspree.io/
2. Click nút **"Get Started"** (màu xanh, góc trên bên phải)
3. Chọn **"Sign up with Google"** → Chọn tài khoản Gmail của bạn
4. Cho phép Formspree truy cập (bấm "Allow")
5. **Xong!** Bạn đã đăng nhập thành công

---

## 📝 BƯỚC 2: Tạo Form mới (30 giây)

1. Sau khi đăng nhập, bạn sẽ thấy **Dashboard**
2. Click nút **"+ New Form"** (màu xanh, góc trên bên phải)
3. Điền thông tin:
   - **Form name**: `Quiz Results` (hoặc tên gì cũng được)
   - **Email to receive submissions**: `tienganhthanh06@gmail.com`
4. Click **"Create Form"**

---

## 📝 BƯỚC 3: Lấy Endpoint (10 giây)

1. Sau khi tạo form, bạn sẽ thấy trang **Form Settings**
2. Tìm dòng **"Form endpoint"** hoặc **"Your form's POST endpoint"**
3. Bạn sẽ thấy một URL như: `https://formspree.io/f/abc123xyz`
4. **Copy toàn bộ URL này** (bấm Ctrl+C hoặc click vào nút copy)

**Ví dụ endpoint:**
```
https://formspree.io/f/xpzgkqwn
```

---

## 📝 BƯỚC 4: Cập nhật code (10 giây)

1. Mở file `index.html` trong Cursor/VS Code
2. Tìm dòng **332** (gần dòng có `const FORMPREE_ENDPOINT`)
3. Bạn sẽ thấy:
   ```javascript
   const FORMPREE_ENDPOINT = "YOUR_FORMPREE_ENDPOINT";
   ```
4. Thay `YOUR_FORMPREE_ENDPOINT` bằng endpoint bạn vừa copy

**Ví dụ:**
```javascript
const FORMPREE_ENDPOINT = "https://formspree.io/f/xpzgkqwn";
```

5. **Lưu file** (Ctrl+S)

---

## ✅ KIỂM TRA

1. Mở file `index.html` trong trình duyệt
2. Làm quiz và bấm **"Nộp bài"**
3. Kiểm tra email `tienganhthanh06@gmail.com`
4. Bạn sẽ nhận được email với kết quả quiz! 🎉

---

## 🆘 GẶP VẤN ĐỀ?

### ❌ Không nhận được email?
- Kiểm tra thư mục **Spam/Junk**
- Đảm bảo đã copy đúng endpoint (có `https://`)
- Kiểm tra Console (F12) xem có lỗi không

### ❌ Lỗi "Form not found"?
- Kiểm tra lại endpoint đã copy đúng chưa
- Đảm bảo endpoint có dạng: `https://formspree.io/f/xxxxx`

### ❌ Không thấy nút "New Form"?
- Đảm bảo đã đăng nhập thành công
- Refresh lại trang Dashboard

---

## 📸 HÌNH ẢNH MINH HỌA

### Bước 2: Tạo Form
```
Dashboard → + New Form → Điền thông tin → Create Form
```

### Bước 3: Copy Endpoint
```
Form Settings → Form endpoint → Copy URL
```

### Bước 4: Dán vào code
```javascript
// Tìm dòng này trong index.html (dòng ~332)
const FORMPREE_ENDPOINT = "YOUR_FORMPREE_ENDPOINT";

// Thay bằng endpoint của bạn
const FORMPREE_ENDPOINT = "https://formspree.io/f/xxxxx";
```

---

## 🎯 TÓM TẮT NHANH

1. ✅ Đăng ký: https://formspree.io/ → Sign up with Google
2. ✅ Tạo form: + New Form → Email: tienganhthanh06@gmail.com
3. ✅ Copy endpoint: `https://formspree.io/f/mvzybwzp`
4. ✅ Dán vào code: Dòng 332 trong `index.html`
5. ✅ Test: Làm quiz → Nộp bài → Kiểm tra email

---

**Chúc bạn thành công! Nếu gặp khó khăn, cứ hỏi mình nhé! 😊**
