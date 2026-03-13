# 🐾 PetGoSpa - AI Chăm Sóc Thú Cưng Lưu Động 🚐


**PetGoSpa** là nền tảng khởi nghiệp đột phá kết hợp giữa dịch vụ chăm sóc thú cưng tận nhà và Trí tuệ nhân tạo (AI). Dự án giải quyết nỗi lo về thời gian và sự an toàn cho các "Sen" bằng mô hình phục vụ lưu động chuyên nghiệp.

---

## ✨ Tính Năng Nổi Bật

- 📱 **Đặt lịch thông minh**: Giao diện Mobile App thân thiện, đặt dịch vụ chỉ với vài điểm chạm.
- 🤖 **AI Diagnosis**: Tích hợp AI phân tích tình trạng lông và da qua hình ảnh để tư vấn gói dịch vụ phù hợp.
- 🎥 **Real-time Tracking**: Theo dõi lộ trình di chuyển của Groomer và xem trực tiếp quá trình chăm sóc qua Body-cam.
- 💳 **Thanh toán linh hoạt**: Tích hợp các cổng thanh toán điện tử hiện đại.

---

## 🛠 Tech Stack

### Backend
- **Core:** ASP.NET Core MVC 8.0
- **Database:** Microsoft SQL Server
- **ORM:** Entity Framework Core
- **Real-time:** SignalR (dành cho tính năng theo dõi lộ trình)

### UI/UX Concept
- **Styling:** Bootstrap 5, FontAwesome 6
- **Design:** Figma (Mockup dựa trên phong cách hiện đại, tone màu cam chủ đạo)

---

## 🏗 Cấu Trúc Database

Dự án sử dụng SQL Server với các bảng chính:
- `Services`: Lưu thông tin các gói spa (Tắm sấy, cắt tỉa...).
- `Groomers`: Quản lý hồ sơ nhân viên và đánh giá sao.
- `Bookings`: Quản lý lịch hẹn và trạng thái phục vụ.

---

## 🚀 Hướng Dẫn Cài Đặt (Local)

### 1. Yêu cầu hệ thống
- Visual Studio 2022 (v17.8 trở lên)
- .NET 8.0 SDK
- SQL Server Management Studio (SSMS)

### 2. Thiết lập Database
Chạy script SQL sau trong SSMS:
```sql
CREATE DATABASE CatGoSpaDB;
-- (Chạy tiếp các script tạo bảng trong thư mục /Database/Scripts)
###3. Cấu hình Connection String
Cập nhật file appsettings.json trong dự án:"ConnectionStrings": {
  "DefaultConnection": "Server=YOUR_SERVER;Database=CatGoSpaDB;Trusted_Connection=True;TrustServerCertificate=True;"
}
