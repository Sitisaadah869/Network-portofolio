Fitur Quicksetdi MikroTik merupakan sebuah menu praktis di MikroTik utuk mengkonfigurasi router dalam satu halaman.

A. Sumber Internet IP Static

Topologi:
<p align=center">
<img width="700" alt="topologi quickset1 drawio" src="https://github.com/user-attachments/assets/485fd45f-e241-47fe-b65f-b874198c8482" /></p>

Langkah-langkah;

1). Koneksikan MikroTik ke internet melalui Wireless

2). Buka menu Quickset.

3). Masukan Ip Address 172.16.16.1/25 di Local Network lalu klik Apply dan OK.
<p align=center">
<img width="700" alt="WhatsApp Image 2026-07-01 at 18 30 54" src="https://github.com/user-attachments/assets/b0823418-2392-4ff7-9dcf-53e13c56e780" /></p>

4). Buka menu Firewal, dan tambahkan:
Chain= srcnat
Out.Interfae= wlan1
Action= masquerade
<p align=center">
<img width="700" alt="WhatsApp Image 2026-07-01 at 18 30 54 (1)" src="https://github.com/user-attachments/assets/9888dbbc-cc43-4300-80d1-710b8be75255" /></p>

5). Buka Network & internet settings, lalu ikuti gambar di bawah ini.
<p align="center">
<img width="440" alt="WhatsApp Image 2026-06-29 at 11 45 25" src="https://github.com/user-attachments/assets/959eb18a-761a-42ca-a039-77e03ee3e6aa" /></p>
<p align="center">
<img width="800" alt="WhatsApp Image 2026-06-29 at 11 45 25 (1)" src="https://github.com/user-attachments/assets/f17e023b-02ba-420b-ba12-4759b67c07ac" /></p>
<p align="center">
<img width="700" alt="WhatsApp Image 2026-07-01 at 18 30 54 (3)" src="https://github.com/user-attachments/assets/9e4d3cc6-8970-4fd3-8131-953c95dc891d" /></p>

  6). Buka CMD (Command Prompt) lalu lakukan ping.
<p align="center">
<img width="700" alt="WhatsApp Image 2026-07-01 at 18 30 54 (2)" src="https://github.com/user-attachments/assets/02fc9b3a-7224-4504-be71-13eaaff80575" /></p>

B. Sumber Internet IP-DHCP

Topologi:
<p align="center">
<img width="700" alt="topoogi quickset2 drawio" src="https://github.com/user-attachments/assets/3864d14d-f094-49a1-8f86-7822a4f73272" />
</p>
Langkah-langkah:

1). Koneksikan MikroTik ke internet melalui Wireless

2). Buka menu Quickset.

3). Masukan Ip Address 172.16.16.1/25 di Local Network, centang DHCP Server dan NAT.
DHCP Server Range= 172.16.16.10-172.16.16.20
Klik Apply dan Ok
<p align="center">
<img width="700" alt="WhatsApp Image 2026-07-01 at 18 30 53" src="https://github.com/user-attachments/assets/f21628bb-52af-4dd6-8925-71d58aaaf1c2" /></p>

4). Buka Network & internet settings, lalu ikuti gambar di bawah ini.
<p align="center">
<img width="440" alt="WhatsApp Image 2026-06-29 at 11 45 25" src="https://github.com/user-attachments/assets/959eb18a-761a-42ca-a039-77e03ee3e6aa" /></p>
<p align="center">
<img width="800" alt="WhatsApp Image 2026-06-29 at 11 45 25 (1)" src="https://github.com/user-attachments/assets/f17e023b-02ba-420b-ba12-4759b67c07ac" /></p>
<p align="center">


5). Buka CMD (Command Prompt) lalu lakukan ping.
<p align="center">
<img width="700" alt="WhatsApp Image 2026-07-01 at 18 30 55" src="https://github.com/user-attachments/assets/2a86870f-8746-4dc9-8a2d-c6a85f6d1836" /></p>
