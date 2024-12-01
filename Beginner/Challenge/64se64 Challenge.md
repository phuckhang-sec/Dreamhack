- Challenge link: https://dreamhack.io/wargame/challenges/872
- Khi down file về giải nén sẽ được 1 trang web, kiểm tra Source file của web đó, ta thấy 1 đoạn dữ liệu đáng ngờ có dạng base64:
IyEvdXNyL2Jpbi9lbnYgcHl0aG9uMwphc2M9WzY4LCA3MiwgMTIzLCA5OCwgMTAxLCA0OCwgNTIsIDU0LCA5OCwgNTUsIDUzLCA1MCwgNTAsIDk3LCA5NywgNTAsIDEwMSwgNTAsIDU2LCAxMDIsIDUwLCA1NSwgNTQsIDEwMSwgNDgsIDk5LCA1NywgNDksIDQ4LCA1MywgNTAsIDQ5LCAxMDIsIDUwLCA1MSwgOTcsIDQ4LCA1MywgNTYsIDU1LCA0OCwgNDgsIDUzLCA5NywgNTYsIDUxLCA1NSwgNTUsIDUxLCA1NSwgNDgsIDk3LCA0OSwgNDksIDEwMSwgNTMsIDEwMSwgNTIsIDEwMCwgOTksIDQ5LCA1MywgMTAyLCA5OCwgNTAsIDk3LCA5OCwgMTI1XQphcnI9WzAgZm9yIGkgaW4gcmFuZ2UoNjgpXQpmb3IgaSBpbiByYW5nZSgwLDY4KToKICAgIGFycltpXT1jaHIoYXNjW2ldKQpmbGFnPScnLmpvaW4oYXJyKQpwcmludChmbGFnKQ==
- Thử giải mã đoạn dữ liệu đó bằng python:
  + Khai báo thư viện chứa hàm b64decode.
  + Khởi tạo biến để lưu chuỗi -> đưa biến vào hàm b64decode để xử lí dể đưa dữ liệu Base64 về byte.
  + Đưa byte về dạng chuỗi kí tự bằng hàm decode('utf-8')

  ![Screenshot 2024-11-30 201037](https://github.com/user-attachments/assets/75b133c8-6bcf-4f09-a7d3-1431dde748bc)

  - Kết quả được đoạn code bằng python và khi chạy đoạn code đó ta được flag:

  ![Screenshot 2024-11-30 200138](https://github.com/user-attachments/assets/ecb37e54-0d5e-4925-83e2-feb63f53f433)

  - Flag: DH{be046b7522aa2e28f276e0c910521f23a0587005a8377370a11e5e4dc15fb2ab}

 
    


    




