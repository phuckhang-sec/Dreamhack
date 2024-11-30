- Cú pháp: ssh user@HOST -p PORT -i [PATH TO PRIVATE KEY FILE]
  + Thay "user" bằng tên tài khoản muốn sử dụng, thay "HOST" bằng tên ip máy chủ.
  + Nếu bạn muốn kết nối với một cổng cụ thể, hãy sử dụng "-p" tùy chọn.
- Có 2 phương pháp xác thực:
  + Xác thực bằng mật khẩu: ssh user@HOST
  + Lưu trữ khóa công khai trên máy chủ từ xa và chỉ định khóa riêng cho máy khách để xác minh danh tính của người dùng (An toàn hơn). Có thể tạo cặp khóa công khai-riêng bằng lệnh.
  
