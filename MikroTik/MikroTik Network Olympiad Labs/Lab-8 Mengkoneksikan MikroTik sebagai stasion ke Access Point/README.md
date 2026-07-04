Topologi:
<p align="center">
<img width="508" alt="topologiwlan drawio" src="https://github.com/user-attachments/assets/b11e15c4-2d3a-493b-b996-77c1e5faf130" />
</p>
Langkah-langkah:

1). Buka menu Wireless, klik Security Profile, klik + General lalu isi:

Name: belajar
Mode: dynamic keys
Authenttication Types: WPA2 PSK, WPA2 EAP
WPA2 Pre-Shared Key: Semangat45

Apply lalu OK

2). Klik menu Inteface>>Wireless, ubah Security Profile-default menjadi belajar, jika sudah klik scan>>start



3). Klik SSID Belajar-Mikrotik, lalu klik connect
<p align="center">
<img width="497" alt="WhatsApp Image 2026-07-04 at 11 30 56" src="https://github.com/user-attachments/assets/ef8cc797-8f6c-44d4-a8a7-60016b29e10f" /></p>

4). Buka IP-DHCP Client, klik New lalu ubah Interface>>Wlan1, Apply lalu Ok, Pastikan sudah ada tulisan Bound
<p align="center">
<img width="536" alt="WhatsApp Image 2026-07-04 at 11 31 08" src="https://github.com/user-attachments/assets/492b2c9a-2acc-4739-94af-639f75fcb652" /></p>
<p align="center">
<img width="400" alt="WhatsApp Image 2026-07-04 at 11 31 09 (1)" src="https://github.com/user-attachments/assets/9b740dde-fdcc-4c84-8adf-8c254fc332bd" /></p>

5). Buka New Terminal ketik ping 8.8.8.8, pastikan sudah connect
<p align="center">
<img width="596" alt="WhatsApp Image 2026-07-04 at 11 31 09 (2)" src="https://github.com/user-attachments/assets/165e382a-8aa6-4f16-9af2-fb55c964f023" /></p>

6). Buka IP-Firewal-NAT, isi konfigurasi dengan:

Chain: srcnat
Out.Interface: wlan1
Action: masquerade
<p align="center">
<img width="600" alt="WhatsApp Image 2026-07-04 at 11 31 09" src="https://github.com/user-attachments/assets/c13dafbf-2487-41a0-8277-c8cbafe7d41c" /></p>

7). Buka IP_Address, tambahkan IP 192.168.20.1/24 di ether2 
<p align="center">
<img width="360" alt="WhatsApp Image 2026-07-04 at 11 31 08 (1)" src="https://github.com/user-attachments/assets/6d9a3098-d760-497e-a406-0a9022e71fab" /></p>

8). Buka Network & internet settings, lalu ikuti gambar di bawah ini.
<p align="center">
<img width="440" alt="WhatsApp Image 2026-06-29 at 11 45 25" src="https://github.com/user-attachments/assets/959eb18a-761a-42ca-a039-77e03ee3e6aa" /></p>
<p align="center">
<img width="600" alt="WhatsApp Image 2026-06-29 at 11 45 25 (1)" src="https://github.com/user-attachments/assets/f17e023b-02ba-420b-ba12-4759b67c07ac" /></p>
<p align="center">
<img width="300" alt="WhatsApp Image 2026-07-04 at 11 31 09 (3)" src="https://github.com/user-attachments/assets/e29ed6dc-073d-491b-a8fe-774a7a406e44" />
</p>
9). Buka CMD lalu ketik ping 8.8.8.8 dan tracert 8.8.8.8
<p align="center">
<img width="968" height="504" alt="WhatsApp Image 2026-07-04 at 11 31 08 (2)" src="https://github.com/user-attachments/assets/07c6c2d1-2cee-43f7-be1d-102fee3b8096" />
</p>
Kesimpulan:
Dari materi ini saya bisa menghubungkan mikrotik sebagai stasion ke access point dan mengetahui bahwa mikrotik bisa terhubung ke internet melalui Wifi.
