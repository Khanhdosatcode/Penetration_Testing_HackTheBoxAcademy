 RDP to with user "htb-student" and password "HTB_@cademy_stdnt!"
1. When establishing a reverse shell session with a target, will the target act as a client or server?
P/s : client
2. Connect to the target via RDP and establish a reverse shell session with your attack box then submit the hostname of the target box. 
Kết nối từ xa tới máy chủ mục tiêu bằng xfreerdp 
![alt text](image.png)
Kết nối thành công 
![alt text](image-1.png)
Vô hiệu hóa Anti virus 
![alt text](image-2.png)
Trên máy tấn công lắng nghe cổng 443
![alt text](image-3.png)
Trên máy chủ mục tiêu gửi tín hiệu về cổng 443 của máy tấn công tạo reverse shell
![alt text](image-4.png)
Tạo reverse shell thành công xem hostname
![alt text](image-6.png)
P/s:Shells-Win10

