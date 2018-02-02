### **3 CHẾ ĐỘ MẠNG TRONG VMWARE WORKSTATION 12**
## 1. NAT-Network Address Translation
<img scr="https://imgur.com/a/WH01W">
<ul> 
NAT cung cấp một truy cập máy ảo tới các tài nguyên mạng sử dụng địa chỉ IP của máy chủ lưu trữ.
</ul>
<ul>
 Kết nối dịch vụ địa chỉ mạng được thiết lập tự động nếu bạn theo đường dẫn **Custom** trong "New Virtual Machine Wizard" và chọn  **Use network address translation**.
</ul>
<ul>
 Nếu bạn muốn kết nối với Internet hoặc các mạng TCP / IP khác sử dụng mạng quay số (**dial-up networking**) hoặc kết nối băng thông rộng(**boardband connection**) của máy chủ và bạn không thể cung cấp cho máy ảo một địa chỉ IP trên mạng bên ngoài, NAT thường là cách dễ nhất để cung cấp cho máy ảo của bạn truy cập vào mạng đó. 
</ul>
<ul> 
NAT cũng cho phép bạn kết nối với một mạng TCP / IP sử dụng bộ chuyển đổi Token Ring trên máy chủ
</ul>
<ul>
Nếu bạn sử dụng NAT, máy ảo của bạn sẽ không có địa chỉ IP riêng trên mạng bên ngoài. Thay vào đó, một mạng riêng tư riêng được thiết lập trên máy chủ. Máy ảo của bạn nhận được một địa chỉ trên mạng đó từ máy chủ DHCP ảo VMware. Thiết bị NAT VMware truyền dữ liệu mạng giữa một hoặc nhiều máy ảo và mạng bên ngoài. Nó xác định các gói tin dữ liệu đến cho mỗi máy ảo và gửi chúng đến đúng đích.
</ul>