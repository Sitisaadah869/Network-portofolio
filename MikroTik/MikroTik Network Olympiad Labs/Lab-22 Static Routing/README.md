Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Lakukan Basic Configuration:

Ip Address ether 2 : 192.168.20.1/24

DHCP Client : 

Interface: wlan1 

add default route: no

<p align="center"><img width="540" alt="WhatsApp Image 2026-07-26 at 19 51 14" src="https://github.com/user-attachments/assets/d17097c5-80d6-4949-bf91-504e1385ddda" /></p>

DHCP Server : ether 2

Firewall-nat : 

Chain: srcnat

Out. Interface: wlan1

Action: Masquerade

3). IP>>Route: new+

<p align="center"><img width="440" alt="WhatsApp Image 2026-07-26 at 19 51 14 (1)" src="https://github.com/user-attachments/assets/4fe572c8-1a5c-4e3b-8120-b10c33593822" /></p>

dst-address: 8.8.8.0

gateway: 10.47.117.50
<p align="center">
<img width="500" alt="WhatsApp Image 2026-07-26 at 19 51 15 (1)" src="https://github.com/user-attachments/assets/ef89ce46-d14f-4b84-8057-2a61b172f955" /></p>

apply, ok

4). cara melihat gateway

Buka New Terminal

Ketikan perintah : ip dhcp-client print detail

<p align="center"><img width="500" alt="WhatsApp Image 2026-07-26 at 19 51 15" src="https://github.com/user-attachments/assets/685f1561-0b8a-4af0-a75d-bda201dbfc75" /></p>

5). Pengujian

<p align="center"><img width="500" alt="WhatsApp Image 2026-07-26 at 19 51 15 (2)" src="https://github.com/user-attachments/assets/cd0d033a-4f5e-4a18-b162-6c2f02e780d6" /></p>
