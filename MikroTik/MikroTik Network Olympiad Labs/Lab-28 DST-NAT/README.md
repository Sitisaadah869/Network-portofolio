Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Lakukan Basic Configuration:

Ip Address ether 2 : 192.168.20.1/24

DHCP Client : 

Interface: wlan1 

add default route: yes

DHCP Server : ether 2

3). Firewall-nat : 

Chain: dstnat

Dst. Address: 10.47.117.50

Protocol: 6(tcp) 

Dst. Port: 8081

<p align="center"><img width="600" alt="WhatsApp Image 2026-07-26 at 20 06 45" src="https://github.com/user-attachments/assets/e5303166-f389-434d-9213-90ee1b66abc8" /></p>

Action: dst-nat

To Address: 192.168.20.1

To Port: 80

<p align="center"><img width="600" alt="WhatsApp Image 2026-07-26 at 20 06 45 (1)" src="https://github.com/user-attachments/assets/40420aca-03a8-45b6-9f03-53ffb1b5778c" /></p>

apply, ok

4). Pengujian
<p align="center">
<img width="600" alt="WhatsApp Image 2026-07-26 at 20 06 45 (2)" src="https://github.com/user-attachments/assets/9e853f9b-1e2a-4b0d-a4f7-677c71797e44" /></p>
<div style="display: flex; gap: 10px;">
<img width="500" alt="WhatsApp Image 2026-07-26 at 20 06 45 (3)" src="https://github.com/user-attachments/assets/a2fbc57c-17b8-43d2-8b55-2eb7883e2438" />
<img width="500" alt="WhatsApp Image 2026-07-26 at 20 06 46" src="https://github.com/user-attachments/assets/b44c6f08-8ddc-497c-9d98-98ade668e2e0" /></div>
