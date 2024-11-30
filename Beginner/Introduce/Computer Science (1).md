- Tính năng Snapshot : VirtualBox cung cấp tính năng Snapshot. Tính năng này cho phép bạn lưu trạng thái của máy ảo và nhanh chóng khôi phục về trạng thái đó khi cần. Theo cách này, nếu có sự cố hoặc lỗi xảy ra khi sử dụng máy ảo, bạn có thể dễ dàng quay lại trạng thái trước đó.
- Hacking là hành động áp dụng kiến ​​thức khoa học máy tính này để khám phá và khai thác lỗ hổng trong một chương trình hoặc hệ thống.
- Hệ thống số (Các dạng biểu diễn số).
- Bit và Byte:
  + Bit có ý nghĩa nhất (MSB), Bit có ý nghĩa ít nhất (LSB).
  + Thứ tự byte: Dữ liệu 2 byte trở lên được lưu trữ liên tiếp trong bộ nhớ. Cách sắp xếp từng byte trong bộ nhớ được gọi là thứ tự byte.
- Big-endianness: Nó được lưu trữ ở địa chỉ thấp hơn trong bộ nhớ, bắt đầu từ byte ngoài cùng bên trái (lớn nhất).
- Little-endianness: Nó được lưu trữ ở địa chỉ thấp hơn trong bộ nhớ, bắt đầu từ byte ngoài cùng bên phải (nhỏ nhất).
- Các phép toán Bitwise:
  + Các phép toán logic:
    
  ![Screenshot 2024-11-29 224335](https://github.com/user-attachments/assets/3a98a661-ffa9-451e-a4f1-605f207d9918)

  + Toán tử Bitwise:
    
  ![Screenshot 2024-11-29 224347](https://github.com/user-attachments/assets/3f1e2700-4d65-4cfd-adb1-0ca279f6c899)

  + Toán tử Dịch chuyển (Shift Operators):

  ![Screenshot 2024-11-29 231246](https://github.com/user-attachments/assets/66e2a565-89fd-4a9d-93a9-8338022a2ce4)

- Encoding (Mã hóa) and Decoding (Giải mã):
  + Mã ASCII (America Standard Code Information Interchange): là một tiêu chuẩn để mã hóa kí tự (chuyển đổi chữ cái thành chữ số). Một kí tự ASCII có kích thước 1 byte, gồm 7 bit để biểu diễn kí tự và 1 bit để kiếm tra lỗi. Điều này tạo ra 128 biễu diễn kí tự có thể từ 0 -> 127.
  + Unicode: à một mã chuẩn quốc tế gán các số duy nhất cho các ký tự trong mọi ngôn ngữ trên thế giới, không chỉ tiếng Anh. Nó được tạo ra để giải quyết vấn đề về các ký tự không tương thích khi sử dụng các ngôn ngữ khác nhau. Hiện tại Unicode có thể biểu diễn hơn 143000 kí tự (32 bit 1 kí tự) với 128 kí tự đầu tiên giống với mã ASCII.
    * UTF-<số bit> là các định dạng mã hóa của Unicode trong đó UTF-8 được sử dụng phổ biến nhất (hầu hết các kí tự có thể thấy trên máy tính hiện nay) - biểu diễn 1 kí tự có kích thước 1 -> 4 byte.
  + URL Encoding (Percent Encoding): Mã hóa chuỗi thành định dạng có thể truyền qua Internet. URL được sử dụng trên web, nó chỉ chấp nhận một loại ký tự cụ thể (bao gồm chữ cái, chữ số, và một số kí tự đặc biệt).
    * Mã hóa URL được biểu diễn bằng dấu %, theo sau là giá trị thập lục phân của mã ASCII cho ký tự. Hãy lấy ký tự khoảng trắng làm ví dụ: nếu URL chứa khoảng trắng, nó sẽ được chuyển đổi thành +ký hiệu hoặc %20. Đây %20là kết quả của mã hóa URL.
  + Base64 Encoding: là một phương pháp mã hóa chuyển đổi dữ liệu nhị phân thành văn bản bao gồm các ký tự ASCII. Nó được đặt tên vậy vì tổng cộng có kí tự ASCII được sử dụng (bao gồm 52 chữ cái, 10 chữ số, + và /.)
