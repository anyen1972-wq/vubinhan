# 💰 SpendWise — Web Quản Lý Chi Tiêu Cá Nhân Thông Minh

Ứng dụng web Single Page Application (SPA) giúp theo dõi thu chi cá nhân, phân tích ngân sách theo danh mục, trực quan hóa dữ liệu qua biểu đồ và xuất báo cáo Excel chuyên nghiệp.

![SpendWise Banner](https://img.shields.io/badge/SpendWise-v1.0-6C63FF?style=for-the-badge&logo=wallet)
![Tech](https://img.shields.io/badge/HTML5-CSS3-VanillaJS-orange?style=for-the-badge)
![Storage](https://img.shields.io/badge/Storage-localStorage-00C897?style=for-the-badge)

---

## ✨ Tính Năng Nổi Bật

### 1. 💵 Quản Lý Thu Chi (Core CRUD)
- Thêm, sửa, xóa các khoản thu/chi linh hoạt có xác nhận an toàn.
- Phân loại 14 danh mục trực quan (Ăn uống, Di chuyển, Mua sắm, Lương, Freelance...).
- Bộ lọc nhanh theo loại: **Tất cả / Chi tiêu / Thu nhập**.
- Tự động tính số dư tức thì, cảnh báo khi số dư âm.

### 2. 📊 Trực Quan Hóa Dữ Liệu (Chart.js)
- **Biểu đồ tròn (Doughnut Chart):** Cơ cấu tỷ lệ % chi tiêu theo từng nhóm danh mục.
- **Biểu đồ cột kép (Grouped Bar Chart):** So sánh trực tiếp biến động giữa Thu nhập và Chi tiêu.
- **Biểu đồ đường (Line Chart):** Xu hướng chi tiêu lũy kế theo thời gian.
- **Bộ lọc chu kỳ:** Xem theo **Tuần này**, **Tháng này**, hoặc **Năm nay**.

### 3. 🎯 Quản Lý Ngân Sách & Cảnh Báo
- Thiết lập hạn mức chi tiêu hàng tháng cho từng danh mục riêng biệt.
- Thanh tiến độ hiển thị trực quan tỷ lệ đã chi kèm nhãn trạng thái (*Ổn định / Sắp chạm hạn mức / Vượt hạn mức*).
- Tự động kích hoạt cảnh báo Toast thông minh khi chi tiêu đạt $\ge 85\%$ hoặc $\ge 100\%$ hạn mức.

### 4. 📑 Báo Cáo & Dữ Liệu
- **Xuất file Excel (`.xlsx`):** Sử dụng SheetJS, hỗ trợ định dạng cột và tiêu đề tiếng Việt chuẩn.
- **Xuất file CSV:** Định dạng UTF-8 BOM hiển thị chuẩn tiếng Việt không lỗi font.
- **Sao lưu & Khôi phục JSON:** Tải file backup về máy và nạp lại bất cứ lúc nào.
- **Web Notification:** Hẹn giờ nhắc nhở ghi chép chi tiêu mỗi ngày (Web Notification API).

### 5. 🎨 Giao Diện & Trải Nghiệm
- Chế độ **Sáng / Tối (Light & Dark Mode)** tự động đồng bộ cả biểu đồ.
- Thiết kế **Mobile-first Responsive**, hoạt động mượt mà trên điện thoại, máy tính bảng và PC.
- Không cần cài đặt `npm` hay build tool phức tạp — mở là chạy ngay trên mọi trình duyệt.

---

## 🚀 Hướng Dẫn Sử Dụng

1. Mở thư mục dự án `D:\web số 1\`.
2. Nhấp đúp chuột vào file **`index.html`** để chạy trực tiếp trên trình duyệt (Chrome, Edge, Firefox, Safari...).

---

## 🛠️ Công Nghệ Sử Dụng

- **Frontend:** HTML5, CSS3 (CSS Variables, Flexbox, Grid), Vanilla JavaScript (ES6+)
- **Thư viện:**
  - [Chart.js v4](https://www.chartjs.org/) — Vẽ biểu đồ phân tích
  - [SheetJS (xlsx)](https://sheetjs.com/) — Xuất báo cáo bảng tính Excel
  - [Font Awesome 6](https://fontawesome.com/) — Bộ icon giao diện
  - [Google Fonts (Inter)](https://fonts.google.com/specimen/Inter) — Typography hiện đại
- **Lưu trữ:** Trình duyệt `localStorage`
