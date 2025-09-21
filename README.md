# Assignment6_Embedded_System
Giao tiếp I2C (I2C Communication)

Dự án này trình bày cách cấu hình và sử dụng vi điều khiển STM32 làm thiết bị Master trong giao tiếp I2C. Chương trình sẽ thực hiện đọc/ghi dữ liệu với một thiết bị Slave bên ngoài (ví dụ: cảm biến, EEPROM) và hiển thị kết quả lên máy tính để giám sát.

Yêu cầu:
Cấu hình ngoại vi I2C trên STM32 hoạt động ở chế độ Master.

Cấu hình UART để gửi dữ liệu về máy tính.

Viết các hàm để thực hiện giao tiếp (đọc/ghi một hoặc nhiều byte) với một thiết bị I2C Slave cụ thể.

Trong vòng lặp chính, chương trình sẽ đọc dữ liệu từ Slave một cách định kỳ và hiển thị lên terminal.

Phần cứng sử dụng
Board phát triển STM32F103C8T6.

Một thiết bị I2C Slave, ví dụ:

Cảm biến gia tốc/gyro MPU-6050.

EEPROM AT24C256.

Mạch chuyển USB-to-TTL để giao tiếp UART.

Mạch nạp và gỡ lỗi ST-Link V2.

LED (dùng để báo trạng thái hoạt động).

Dây cắm.
