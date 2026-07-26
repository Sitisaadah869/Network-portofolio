Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Lakukan Basic Configuration:

Ip Address ether 2 : 192.168.20.1/24

DHCP Client : 

Interface: wlan1 

add default route: yes

DHCP Server : ether 2

3). Firewall-nat : 

Chain: srcnat

Out.Interface: wlan1

Action: src-nat

To Addresses: 10.47.117.147 (IP Address interface WAN)
<p align="center">
<img width="500" alt="WhatsApp Image 2026-07-26 at 20 06 44" src="https://github.com/user-attachments/assets/33e42738-4577-435e-81db-5ac6f3aa2f63" /></p>

4). Pengujian 

<p align="center"><img width="500" alt="WhatsApp Image 2026-07-26 at 20 06 44 (1)" src="https://github.com/user-attachments/assets/7e44cc78-cac1-45d8-bdc4-298df5fad00c" /></p>



apply, ok

4). Ping
