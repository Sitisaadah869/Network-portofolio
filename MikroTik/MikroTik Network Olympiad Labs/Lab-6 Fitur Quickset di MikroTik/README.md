Fitur Quicksetdi MikroTik merupakan sebuah menu praktis di MikroTik utuk mengkonfigurasi router dalam satu halaman.

A. Sumber Internet IP Static

Topologi:
<p align=center">
<img width="700" alt="topologi quickset1 drawio" src="https://github.com/user-attachments/assets/485fd45f-e241-47fe-b65f-b874198c8482" /></p>

Langkah-langkah;

1). Koneksikan MikroTik ke internet melalui Wireless

2). Buka menu Quickset.

3). Masukan Ip Address 172.16.16.1/25 di Local Network.
<p align=center">
<img width="700" alt="WhatsApp Image 2026-07-01 at 18 30 54" src="https://github.com/user-attachments/assets/b0823418-2392-4ff7-9dcf-53e13c56e780" /></p>

4). Buka menu Firewal, dan tambahkan:
Chain= srcnat
Out.Interfae= wlan1
Action= masquerade
<p align=center">
<img width="700" alt="WhatsApp Image 2026-07-01 at 18 30 54 (1)" src="https://github.com/user-attachments/assets/9888dbbc-cc43-4300-80d1-710b8be75255" /></p>

5). Buka Network & Interet Settings 
6).

7).
8).
