>1. What file type is a text-based DOS script used to perform tasks from the cli? (answer with the file extension, e.g. '.something')
P/s .bat
>2.  What Windows exploit was dropped as a part of the Shadow Brokers leak? (Format: ms bulletin number, e.g. MSxx-xxx)
P/s MS17-010
>3.  Gain a shell on the vulnerable target, then submit the contents of the flag.txt file that can be found in C:\
Mở msf trong command
Sử dụng payload exploit/windows/smb/ms17_010_psexec
![alt text](image.png)
Thiết lập các thông số cho payload
![alt text](image-1.png)
Bắt đầu khai thác
![alt text](image-2.png)
Khởi tạo shell tương tác 
![alt text](image-3.png)
Tìm được file flag
![alt text](image-4.png)
![alt text](image-5.png)
P/s:EB-Still-W0rk$