# Hệ thống đặt dịch vụ chăm sóc thú cưng tại nhà

## 1. Mô tả
Dự án xây dựng hệ thống quản lý trung tâm chăm sóc thú cưng, bao gồm frontend (React), backend (ASP.NET Core), và cơ sở dữ liệu (SQL Server). Hệ thống có thể triển khai cục bộ hoặc trên nền tảng Azure.

---

## 2. Các bước cài đặt

### Bước 1: Clone source code từ GitHub
```bash
git clone https://github.com/tlambvq2/ASPNET-DK23TTC11-tranlam-petcare_at_home.git
cd src
```

### Bước 2: Khởi động project
### 2.1. Khởi động backend
- Mở thử mục PetCareSystem.
```bash
cd PetCareSystem
```
- Mở file `PetShopProj.sln` bằng Visual Studio
- Ấn F5 hoặc Ctrl + F5 để khởi động.

### 2.2. Khởi động frontend
- Mở thử mục PCS_front_end.
```bash
cd PCS_front_end
npm install
npm run dev
```

---

## 4. Triển khai trên Azure

### 4.1. Thiết lập Azure Web App
- Tạo một **App Service** trên Azure.
- Cấu hình App Service với:
  - SKU, Scaling
  - Runtime: **.NET 8.0**

#### Triển khai mã nguồn
- Dùng **GitHub Actions** làm CI/CD:
  - Tự động build, run test, deploy API lên Azure App Service.

#### Cấu hình môi trường
- Thiết lập các biến môi trường:
  - Kết nối DB, khóa API, config khác.
- Thiết lập SSL/TLS bảo mật giao tiếp.

### 4.2. Cơ sở dữ liệu trên Azure SQL Server

#### Thiết lập
- Tạo một instance Azure SQL Server.
- Tạo DB mới trên instance này.

#### Triển khai và cấu hình
- Dùng Azure Data Studio để quản lý DB.
- Thiết lập firewall rules cho phép truy cập.

#### Bảo mật và sao lưu
- Kích hoạt:
  - Transparent Data Encryption (TDE)
  - Azure SQL Threat Detection
- Cấu hình sao lưu tự động và phục hồi khi cần.

# Liên hệ với người phát triển:
Email: tlambvq2@gmail.com
SĐT : 0903710403