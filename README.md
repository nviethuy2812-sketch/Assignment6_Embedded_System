Giao Tiếp I2C Master trên STM32F1
Giới thiệu
Dự án này là bài tập cơ bản về cách triển khai giao thức I²C (Inter-Integrated Circuit) trên vi điều khiển STM32F103C8T6. Chương trình cấu hình STM32 làm thiết bị Master, thực hiện đọc dữ liệu từ một cảm biến Slave (ví dụ: MPU-6050), và sau đó gửi dữ liệu này lên máy tính qua giao tiếp UART để hiển thị và giám sát.

Đây là một kỹ năng nền tảng trong lập trình nhúng, cho phép vi điều khiển giao tiếp với hàng ngàn loại cảm biến, bộ nhớ và các IC ngoại vi khác chỉ bằng hai dây tín hiệu.

Yêu cầu & Tính Năng Chính 🎯
Cấu hình I2C Master: Khởi tạo và cấu hình ngoại vi I2C1 của STM32 để hoạt động ở chế độ Master.

Giao tiếp Slave: Viết các hàm cấp thấp để đọc thành công dữ liệu từ một địa chỉ thanh ghi cụ thể của thiết bị Slave.

Giám sát qua UART: Dữ liệu đọc từ cảm biến được định dạng và gửi lên PC thông qua USART1 (9600-8-N-1) để hiển thị trên terminal.

Báo hiệu Trạng thái: Sử dụng một đèn LED để báo hiệu trạng thái hoạt động của chương trình (ví dụ: nhấp nháy mỗi khi đọc dữ liệu thành công).

Phần Cứng Sử Dụng 🛠️
Board phát triển STM32F103C8T6 ("Blue Pill").

Cảm biến I2C MPU-6050 (Gia tốc kế & Con quay hồi chuyển).

Mạch chuyển USB-to-TTL (CP2102 hoặc FT232).

Mạch nạp ST-Link V2.

1x LED và điện trở hạn dòng (~220Ω).

Dây cắm và Breadboard.

