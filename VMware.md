# **3 CHẾ ĐỘ MẠNG TRONG VMWARE WORKSTATION 12**
=======================================================================
## 1. NAT-Network Address Translation

<img scr="https://github.com/Tuantrung/FIL-Tuantrung/blob/master/New%20folder/Screenshot_1.png" >


- NAT cung cấp một truy cập máy ảo tới các tài nguyên mạng sử dụng địa chỉ IP của máy chủ lưu trữ.

- Kết nối dịch vụ địa chỉ mạng được thiết lập tự động nếu bạn theo đường dẫn **Custom** trong "New Virtual Machine Wizard" và chọn  **Use network address translation**

- Nếu bạn muốn kết nối với Internet hoặc các mạng TCP / IP khác sử dụng mạng quay số (**dial-up networking**) hoặc kết nối băng thông rộng(**boardband connection**) của máy chủ và bạn không thể cung cấp cho máy ảo một địa chỉ IP trên mạng bên ngoài, NAT thường là cách dễ nhất để cung cấp cho máy ảo của bạn truy cập vào mạng đó. 

- NAT cũng cho phép bạn kết nối với một mạng TCP / IP sử dụng bộ chuyển đổi Token Ring trên máy chủ

- Nếu bạn sử dụng NAT, máy ảo của bạn sẽ không có địa chỉ IP riêng trên mạng bên ngoài. Thay vào đó, một mạng riêng tư riêng được thiết lập trên máy chủ. Máy ảo của bạn nhận được một địa chỉ trên mạng đó từ máy chủ DHCP ảo VMware. Thiết bị NAT VMware truyền dữ liệu mạng giữa một hoặc nhiều máy ảo và mạng bên ngoài. Nó xác định các gói tin dữ liệu đến cho mỗi máy ảo và gửi chúng đến đúng đích.

- Nếu bạn chọn NAT, máy ảo có thể sử dụng nhiều giao thức TCP / IP tiêu chuẩn để kết nối với các máy khác trên mạng bên ngoài. Ví dụ, bạn có thể sử dụng HTTP để duyệt các trang web, FTP để chuyển các tập tin và Telnet để đăng nhập vào các máy tính khác. Trong cấu hình mặc định, máy tính trên mạng bên ngoài không thể bắt đầu kết nối với máy ảo. Điều đó có nghĩa là, ví dụ, cấu hình mặc định không cho phép bạn sử dụng máy ảo như một máy chủ Web để gửi các trang web tới các máy tính trong mạng bên ngoài.

- Nếu bạn thực hiện một số lựa chọn khác trong New Virtual Machine Wizard và sau đó quyết định sử dụng NAT, bạn có thể thực hiện thay đổi đó trong trình biên tập cài đặt máy ảo (**VM** > **Settings**).

## 2. Bridged Networking

<img scr="https://github.com/Tuantrung/FIL-Tuantrung/blob/master/New%20folder/Screenshot_2.png" >