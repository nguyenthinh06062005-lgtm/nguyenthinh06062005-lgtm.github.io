---
title: "Hệ thống giám sát nhiệt độ đa kênh LM35"
excerpt: "Dự án sử dụng Arduino để đọc dữ liệu nhiệt độ từ 3 cảm biến LM35, chuẩn hóa dữ liệu đầu ra định dạng JSON và quản lý mã nguồn bằng Git."
collection: portfolio
---

## 📝 Tổng quan dự án
Dự án tập trung vào việc thu thập và xử lý tín hiệu tương tự (Analog) từ các cảm biến nhiệt độ LM35 phổ biến, sau đó chuyển đổi sang độ C và truyền dữ liệu lên máy tính thông qua giao tiếp Serial.

## 🛠️ Công nghệ sử dụng
* **Phần cứng:** Arduino Uno R3, 3 cảm biến LM35.
* **Ngôn ngữ:** C++.
* **Quản trị mã nguồn:** Git/GitHub.
* **Định dạng dữ liệu:** JSON.

## 💡 Các tính năng chính
1. **Đọc dữ liệu đa kênh:** Sử dụng các chân ADC (A0, A1, A2) để theo dõi nhiệt độ tại 3 vị trí khác nhau đồng thời.
2. **Chuẩn hóa dữ liệu:** Thay vì gửi các dòng text thô, hệ thống đóng gói dữ liệu vào định dạng **JSON**, giúp dễ dàng tích hợp với các ứng dụng IoT khác.
3. **Quản lý phiên bản:** Toàn bộ quá trình phát triển được kiểm soát chặt chẽ bằng Git, thực hiện đầy đủ các thao tác Commit, Branching và xử lý Merge Conflict.

## 🔗 Liên kết dự án
Bạn có thể xem chi tiết mã nguồn tại đây:
[Link Repository Arduino LM35](https://github.com/nguyenthinh06062005-lgtm/arduino-lm35)