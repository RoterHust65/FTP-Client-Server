# FTP-Client-Server
- Dự án này bao gồm hai chương trình: FTP client và FTP server. FTP client dùng để kết nối với FTP server và thực hiện các thao tác FTP như tải lên, tải xuống, liệt kê thư mục,... FTP server dùng để cung cấp dịch vụ FTP cho các client.
## Yêu cầu dự án 
- Hệ điều hành: Windows, Linux, macOS
- Cài đặt ngôn ngữ C
## Cài đặt
1. Tải project xuống
```git clone https://github.com/RoterHust65/FTP-Client-Server.git```
2. Biên dịch server 
```
cd server
gcc server.c FTP_Server.c -o ftpserver 
```
3. Biên dịch client
```
cd client
gcc client.c FTP_Client.c -o ftpclient 
```
4. Chạy chương trình
- 4.1 Chạy server ```./ftpserver```
- 4.2 Chạy client ```./ftpclient```
## Sử dụng 
### FTP client:
Để sử dụng FTP client, bạn cần kết nối với FTP server:
```./ftpclient 127.0.0.1 ```
- Địa chỉ IP của server kết nối
- Đăng nhập bằng `user` `pass`
- Sử dụng các câu lệnh FTP
  - ls: liệt kê danh sách file ở thư mục hiện tại
  - cd: chuyển đổi thư mục
  - put: upload lên server
  - get: dow file ở thư mục server
### FTP server:
Để sử dụng FTP server, bạn cần chạy chương trình:
```./ftpserver```