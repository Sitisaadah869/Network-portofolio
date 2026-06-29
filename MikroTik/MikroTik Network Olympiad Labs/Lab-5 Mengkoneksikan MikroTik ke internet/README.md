Menghubungkan MikroTik ke internet menggunakan WLAN 

A. Sumber internet IP Dynamic
Topologi:
<p align="center">
<img width="350" alt="topologi1 drawio" src="https://github.com/user-attachments/assets/4bbefe58-5b75-4ebf-a51b-bc49768db79b" />
</p>
Langkah-langkah:

1). Login ke MikroTik menggunakan WinBox.


2). Buka menu Wireless.

3). Pilih Interface WLAN1, lalu klik tanda centang (enable).
<p align="center">
<img width="600" alt="Screenshot (158)" src="https://github.com/user-attachments/assets/7b335662-4b30-4af1-8bc1-8c7dda4f902c" /></p>

4). Klik Security Profile, isi WPA-2 dengan Password WIFI.
<p align="center">
<img width="600" alt="Screenshot (160)" src="https://github.com/user-attachments/assets/c3e192f5-a123-4781-91b2-8035e6c32696" />
</p>
5). Buka Interface WLAN ubah default menjadi Profile1, Lalu scan dan connect.
<p align="center">
<img width="600" alt="Screenshot (159)" src="https://github.com/user-attachments/assets/16fb970b-c36b-4570-b7a7-114d29d5acb7" /></p>

6). Klik IP-DHCP Client, klik New, masukkan interface WLAN1, lalu klik Apply dan Ok.
Pastikan status DHCP Client sudah Bound.
<p align="center">
<img width="600" alt="Screenshot (162)" src="https://github.com/user-attachments/assets/dd458230-be33-4460-9272-7e03f8584c8d" /></p>

7). Buka IP-Firewall NAT, sesuaikan isi dengan gambar di bawah inni.
<p align="center">
<img width="700" alt="Screenshot (165)" src="https://github.com/user-attachments/assets/e2976095-d1ed-4624-97fa-cd43462304e2" /></p>
<p align="center">
<img width="700" alt="Screenshot (166)" src="https://github.com/user-attachments/assets/d810c273-7e4b-497c-ba22-2e7d290d8d0c" /></p>

8). Buka New Terminal, ketik ping google.com atau ping 8.8.8.8, jika sudah connect berarti MikroTik sudah terhubung ke internet.

