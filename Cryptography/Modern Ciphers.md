- Nguyên lý Kerckhoff: Một hệ thống mật mã phải an toàn ngay cả khi mọi thứ khác trong hệ thống đều được biết ngoại trừ khóa. AES và RSA cũng là những ví dụ về mật mã có thuật toán mã hóa được công khai nhưng không thể giải mã bằng công nghệ hiện đại nếu không có khóa.
- Confusion and Diffusion (Sự nhầm lẫn và Khuếch tán): Năm 1945, một nhà mật mã học Claude Shannon đã công bố rằng một hệ thống mật mã an toàn phải đáp ứng được các đặc tính của sự nhầm lẫn  và sự khuếch tán . Nhiều hệ thống mật mã hiện đại tuân theo cả hai đặc tính này.
  + Confusion: Sự nhầm lẫn là đặc tính khiến việc nhận dạng các đặc điểm của văn bản thuần túy trong một bản mã trở nên khó khăn.

![image](https://github.com/user-attachments/assets/4c5f2290-5583-46aa-92bf-06f64c7e12d8)

  + Diffusion: Sự khuếch tán là tính chất mà những thay đổi nhỏ trong văn bản gốc dẫn đến những thay đổi lớn trong văn bản mã hóa , và không có trong hầu hết các mật mã cổ điển.

![image](https://github.com/user-attachments/assets/46851692-83a1-4b72-8f06-73cc052ec48c)

- Symmetric-key Cryptosystems (Hệ thống mật mã khóa đối xứng): Hệ thống mật mã khóa đối xứng là hệ thống mật mã sử dụng cùng một khóa để mã hóa và giải mã. Chúng có thể được phân loại thành mã khối và mã luồng.
  + Block Ciphers (Mã khối): là một mã hóa mã hóa một văn bản thuần túy thành các khối có kích thước cố định. 

![image](https://github.com/user-attachments/assets/2f95c768-60fd-4a89-9fec-bfa7b5148df9)

  + Stream Ciphers (Mã luồng): là một mã hóa tạo ra một luồng dữ liệu được chia sẻ bởi người gửi và người nhận và thực hiện một số thao tác nhất định trên văn bản thuần túy để tạo ra văn bản mã hóa. Quá trình giải mã được thực hiện bằng cách đảo ngược các thao tác của quá trình mã hóa.

![image](https://github.com/user-attachments/assets/a199df28-dfc7-4dcf-bd6c-52ae2fc8a248)

![image](https://github.com/user-attachments/assets/e07ddd7b-eb40-44cd-a3c2-12495b7294c1)

  + Ưu/ Nhược điểm của mã hóa khóa đối xứng: Hệ thống mật mã khóa đối xứng thường nhanh hơn hệ thống mật mã khóa công khai, nhưng chúng có hạn chế là người gửi và người nhận phải trao đổi khóa trước. Ngoài ra, trong hệ thống mật mã khóa đối xứng, nếu có nhiều người trong một nhóm, thì phải tạo và sử dụng các khóa khác nhau cho mỗi người.

![image](https://github.com/user-attachments/assets/25fcf7f2-76a3-4ad3-9b10-6d4a5f0719a1)

- Public-key Cryptosystems (Hệ thống mật mã khóa công khai): người gửi mã hóa và gửi dữ liệu đến người nhận bằng khóa công khai của người nhận , và người nhận giải mã dữ liệu bằng khóa riêng của mình . Khóa công khai và khóa riêng được sử dụng trong cùng một hệ thống được gọi là cặp khóa .Sự khác biệt là đối với mật mã khóa đối xứng, người gửi và người nhận phải sử dụng cùng một khóa, trong khi đối với hệ thống mật mã khóa công khai, họ sử dụng các khóa khác nhau. Vì lý do này, hệ thống mật mã khóa công khai đôi khi được gọi là hệ thống mật mã khóa bất đối xứng .
  + Ưu/ Nhược điểm của mã hóa khóa công khai:
    * Ưu: Trong hệ thống mật mã khóa công khai, mọi người trong nhóm tạo khóa công khai và khóa riêng của họ và chỉ cần tiết lộ khóa công khai của họ. Do đó,Ncặp khóa là cần thiết khi bạn cóNnhững người trong một nhóm. Điều này ít hơn nhiều so với hệ thống mật mã khóa đối xứng. Ngoài ra, sau khi đã tạo khóa, bạn không cần phải tạo lại, ngay cả khi bạn đang giao tiếp với người mới.
    * Nhược: Mặt khác, hệ thống mật mã khóa công khai thường chậm hơn hệ thống mật mã khóa đối xứng vì chúng yêu cầu tính toán phức tạp hơn. Chúng cũng yêu cầu khóa dài hơn hệ thống mật mã khóa đối xứng để cung cấp cùng mức bảo mật như hệ thống mật mã khóa đối xứng. Ví dụ, AES, hệ thống mật mã khóa đối xứng, đủ an toàn với khóa 192 bit trở lên, trong khi RSA, hệ thống mật mã khóa công khai, khuyến nghị sử dụng khóa 2048 bit trở lên.
   
    * ![image](https://github.com/user-attachments/assets/e2d50176-5320-4b94-be1d-19c7789d3006)

- Đặc điểm của Modern Ciphers:
   + Bảo mật: người được ủy quyền mới được xem thông tin.
   + Tính toàn vẹn: là khả năng kiểm tra và đảm bảo rằng không có bất kỳ thay đổi nào trong số những thay đổi này đối với dữ liệu xảy ra, hông tin do người gửi gửi đi không thể bị can thiệp. 
   + Xác thực: khả năng xác định danh tính của người mà bạn đang trao đổi thông tin. 
   + Không thể chối cãi: Không thể chối bỏ là khả năng khiến việc phủ nhận thông tin đã được trao đổi sau khi thông tin đã được trao đổi trở nên bất khả thi. Các giao dịch trực tuyến sẽ không thể thực hiện được nếu bên nhận tiền có thể phủ nhận rằng họ đã nhận được tiền khi giao dịch diễn ra.









