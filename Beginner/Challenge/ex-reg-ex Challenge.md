- Sau khi tải file về và giải né ta được file app.py
- cat app.py ta được như hình bên dưới:

![Screenshot 2024-12-01 200417](https://github.com/user-attachments/assets/7c5d9acc-6cfb-4d37-bfd3-5fb61c0b91e6)

- Dòng dr\w{5,7}e\d+am@[a-z]{3,7}\.\w+ khá đáng ngờ match với input_val, ta sẽ dịch ngược đoạn mã này để tạo ra input:
  + dr: là 1 chuỗi dr
  + \w{5,7}: /w là các kí tự từ a-z, \w{5,7} là 5 đến 7 kí tự a-z ngẫu nhiên
  + e: kí tự e
  + \d+: viết tắt của 1 số, có thể là nhiều số từ 0-9
  + am@: chuỗi am@
  + [a-z]{3,7}: 3-7 kí tự a-z
  + .: kí tự .
  + \w+: 1 vài kí tự từ a-z
- Tạm dịch những đoạn kí tự trên thành: drancdefe123am@abcd.abc
- Nhập vào input ta được Flag: DH{e64a267ab73ae3cea7ff1255b5f08f3e5761defbfa6b99f71cbda74b7a717db3}
