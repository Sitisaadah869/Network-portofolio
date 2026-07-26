Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Lakukan Basic Configuration:

Ip Address ether 2 : 192.168.20.1/24

DHCP Client : 

Interface: wlan1 

add default route: no

<p align="center"><img width="500" alt="WhatsApp Image 2026-07-26 at 19 51 14" src="https://github.com/user-attachments/assets/6b629287-e1b4-41ae-a8a8-bd860b72ebc5" /></p>

DHCP Server : ether 2

Firewall-nat : 

Chain: srcnat

Out. Interface: wlan1

Action: Masquerade

3). IP>>Route: new+

<p align="center"><img width="440" alt="WhatsApp Image 2026-07-26 at 19 51 14 (1)" src="https://github.com/user-attachments/assets/319e8d9d-0f64-47fc-8c2d-b850aa6c36fe" /></p>

dst-address: 0.0.0.0/0

gateway: 10.47.117.50

<img width="620" height="580" alt="WhatsApp Image 2026-07-26 at 19 51 16" src="https://github.com/user-attachments/assets/06decd16-c39b-433b-b3fd-8d98b765c3f2" />
<img width="824" height="200" alt="WhatsApp Image 2026-07-26 at 19 51 16 (1)" src="https://github.com/user-attachments/assets/12c0706f-8b35-4b06-8b3a-b7668596ae28" />

apply, ok

4). cara melihat gateway

Buka New Terminal

Ketikan perintah : ip dhcp-client print detail

<p align="center"><img width="500" alt="WhatsApp Image 2026-07-26 at 19 51 15" src="https://github.com/user-attachments/assets/ebe193d7-6a3f-4da2-9fa0-7016cc782709" /></p>

5). Pengujian

<p align="center"><img width="500" alt="WhatsApp Image 2026-07-26 at 19 51 16 (2)" src="https://github.com/user-attachments/assets/b5d3a394-1ecc-4020-842e-0ddb579ce979" /></p>
