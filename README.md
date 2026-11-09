# HƯỚNG DẪN XUẤT BẢN TRANG PHÁP LÝ LÊN GITHUB PAGES
**Dự án:** My Fit AI (`vn.cttlabs.myfit`)  
**Tổ chức phát triển:** CTT Labs  

Thư mục `docs/` này chứa toàn bộ tài liệu pháp lý bắt buộc theo quy định của Google Play Store:
1. `index.html`: Cổng trang chủ đa năng, tự động chuyển tab giữa Privacy Policy, Terms of Service, Medical Disclaimer, và Account & Data Deletion.
2. `privacy-policy.md`: Bản markdown Chính sách Quyền riêng tư.
3. `terms-of-service.md`: Bản markdown Điều khoản Dịch vụ.
4. `medical-disclaimer.md`: Bản markdown Khuyến cáo Y tế & Miễn trừ trách nhiệm.

---

## 🚀 Các Bước Xuất Bản Lên GitHub Pages (Hoạt Động 24/7 Miễn Phí)

### Cách 1: Xuất bản trực tiếp từ Kho lưu trữ hiện tại (Khuyên dùng)

1. **Đẩy mã nguồn lên GitHub:**
   Đảm bảo thư mục `docs/` đã được commit và push lên nhánh `main` (hoặc `master`) của GitHub Repository:
   ```bash
   git add docs/
   git commit -m "docs: add legal compliance documents for Google Play"
   git push origin main
   ```

2. **Kích hoạt GitHub Pages trong Cài đặt Kho lưu trữ (Repository Settings):**
   - Truy cập vào GitHub Repository của bạn trên trình duyệt.
   - Nhấn vào tab **Settings** (Cài đặt) ở thanh trên cùng.
   - Ở thanh điều hướng bên trái, chọn mục **Pages**.
   - Tại mục **Build and deployment > Branch**:
     - Chọn nhánh: **`main`** (hoặc `master`).
     - Chọn thư mục: **`/docs`** (quan trọng: chọn đúng `/docs`, không chọn `/ (root)`).
   - Nhấn **Save** (Lưu).

3. **Lấy Đường Dẫn URL Công Khai:**
   - Sau khoảng 1-2 phút, GitHub sẽ hoàn tất triển khai.
   - Bạn sẽ nhận được đường dẫn công khai có dạng:
     ```text
     https://<your-github-username>.github.io/<repository-name>/
     ```
   *(Ví dụ: `https://cttlabs.github.io/myfit/`)*

---

### Cách 2: Tạo Kho Lưu Trữ Riêng Cho Pháp Lý (Tùy chọn)

Nếu kho mã nguồn chính là kho riêng tư (Private Repository) và tài khoản GitHub chưa đăng ký gói Pro, bạn có thể tạo một kho công khai (Public Repository) mới mang tên `myfit-privacy` hoặc `myfit-legal`:
1. Tạo repo công khai mới: `https://github.com/new`
2. Sao chép toàn bộ các tệp trong thư mục `docs/` này vào repo mới.
3. Vào **Settings > Pages > Branch: `main` > Folder: `/ (root)` > Save**.
4. Đường dẫn sẽ là: `https://<your-username>.github.io/myfit-privacy/`.

---

## 📋 Hướng Dẫn Điền Vào Google Play Console

Khi tải bản phát hành `.aab` lên Google Play Console, tại mục **Chính sách và chương trình (App Content)**, hãy điền các thông tin sau:

| Mục trên Play Console | Đường dẫn cần điền |
| :--- | :--- |
| **Chính sách quyền riêng tư (Privacy Policy URL)** | `https://<your-domain>/` (hoặc `https://<your-domain>/#privacy`) |
| **Xóa tài khoản và dữ liệu (Account Deletion URL)** | `https://<your-domain>/#deletion` |
| **Email hỗ trợ nhà phát triển (Developer Contact Email)** | `ctt.labs@gmail.com` |

---

## ✅ Tiêu Chí Đã Được Đáp Ứng 100% Theo Chính Sách Google Play
- [x] Có URL công khai, truy cập được 24/7 không cần đăng nhập.
- [x] Định danh rõ ràng Tên ứng dụng (`My Fit AI`), Application ID (`vn.cttlabs.myfit`) và Nhà phát triển (`CTT Labs`).
- [x] Nêu rõ các loại dữ liệu thu thập (tài khoản, thể lực, dinh dưỡng, ảnh chụp) và lưu trữ cục bộ.
- [x] Công bố rõ SDK bên thứ ba: Google Play Services, Google AdMob, Cloudflare AI.
- [x] Tích hợp hướng dẫn xóa tài khoản & dữ liệu (Account Deletion) 2 phương thức: Trực tiếp trong app và Gửi email yêu cầu.
- [x] Tuyên bố miễn trừ y tế (Medical Disclaimer) rõ ràng nhằm loại trừ rủi ro pháp lý về sức khỏe và chấn thương thể thao.
