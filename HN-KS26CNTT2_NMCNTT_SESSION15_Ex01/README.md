# 5.Yêu cầu đầu ra
- Báo cáo phân tích: Sơ đồ luồng dữ liệu từ local SSD lên Cloud
  - Thu nhập dữ liệu data từ ổ cứng SSD -> Nén dữ liệu và Mã hóa đầu ra -> Truyền dữ liệu lên Cloud thông qua mạng Internet với đường dẫn riêng -> Lối vào của đường dẫn riêng xác thực thông tin tiếp nhận luồng thông tin -> Lưu trữ các dữ liệu vào trong kho
  - Cơ chế xử lý xung đột phiên bản: Hệ thống sẽ xử lý khi 2 người cùng bị mất kết nối mà cloud lưu trong thời gian thực thì sẽ giữ lại cả 2 phiên bản và tự động tạo ra một file riêng có tên thiết bị, thời gian, khi có mạng trở lại thì họ sẽ mở file để kiểm tra, tổng hợp các chi tiết mới nhất lưu lại phiên bản mới hoàn chỉnh nhất.
- Quy trình thực thi: 
  - Bước 1: Tạo một file gốc 
  - Bước 2: Thiết lập phần mềm vào thư mục lưu trữ
  - Bước 3: Bật tính năng đồng bộ và kiểm tra phần Version History