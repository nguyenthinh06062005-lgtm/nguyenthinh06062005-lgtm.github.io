---
title: "Hệ thống Giám sát Nhiệt độ Đa điểm (Arduino )"
excerpt: "Giải pháp thu thập và trực quan hóa dữ liệu nhiệt độ thời gian thực sử dụng cảm biến LM35 và đóng gói dữ liệu JSON chuyên nghiệp."
header:
  teaser: /images/arduino-project-teaser.png
---

## 📑 Tổng quan dự án
Dự án này tập trung vào việc xây dựng một hệ thống IoT hoàn chỉnh từ tầng thiết bị (Edge) đến tầng ứng dụng (Application). Mục tiêu cốt lõi là giải quyết bài toán thu thập dữ liệu Analog từ nhiều nguồn (3 cảm biến LM35) và truyền tải lên máy tính một cách toàn vẹn, minh bạch.

## 🛠️ Giải pháp Kỹ thuật

### 1. Tầng thiết bị & Nhúng (Firmware)
* **Xử lý tín hiệu:** Sử dụng thuật toán đọc mảng và tính toán giá trị trung bình để giảm thiểu sai số nhiễu từ cổng ADC của Arduino.
* **Đóng gói dữ liệu:** Thay vì truyền chuỗi văn bản thuần túy, tôi đã áp dụng cấu trúc **JSON** (JavaScript Object Notation). Việc này giúp dữ liệu có cấu trúc rõ ràng, dễ dàng mở rộng thêm cảm biến mà không cần sửa đổi giao thức truyền nhận.

### 2. Tầng ứng dụng (PC App)
* **Ngôn ngữ:** Phát triển trên nền tảng C# Windows Forms.
* **Hiển thị:** Tích hợp thư viện **ZedGraph** để vẽ đồ thị thời gian thực cho cả 3 kênh nhiệt độ đồng thời, giúp người dùng theo dõi biến động nhiệt độ một cách trực quan nhất.

### 3. Quy trình quản lý (Git Workflow)
* Tuân thủ quy trình làm việc nhóm chuyên nghiệp: Tách nhánh (Branching), xử lý xung đột (Conflict Resolution) và sử dụng **Atomic Commits** để quản lý lịch sử mã nguồn.

---

## 📊 Thông số Kỹ thuật chính
* **Hardware:** Arduino Uno R3, 03 x LM35 Sensor.
* **Communication:** Serial (UART) - Baudrate 9600.
* **Format:** JSON Structured Data.

🔗 [**Khám phá chi tiết mã nguồn trên GitHub**](https://github.com/nguyenthinh06062005-lgtm/Arduino_LM35_TempMonitor)

---