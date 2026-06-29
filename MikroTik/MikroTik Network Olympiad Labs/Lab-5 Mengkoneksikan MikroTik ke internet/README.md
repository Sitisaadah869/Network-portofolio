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
<p align="center">
<img width="596" height="408" alt="WhatsApp Image 2026-06-29 at 11 34 44" src="https://github.com/user-attachments/assets/e12cec5a-7db5-4521-b253-d4348578c99e" /></p>

9). Masukan IP Address 192.168.10.1/24 pada ether2

<p align="center">
<img width="528" height="380" alt="WhatsApp Image 2026-06-29 at 11 45 24" src="https://github.com/user-attachments/assets/edbcfc52-433c-42d9-84c1-a6bd2a2babd6" /></p>


10). Buka menu IP, klik DHCP Server, klik DHCP setup, pilih interface ether2 lalu klik next sampai selesai.
<p align="center">
<img width="868" height="372" alt="WhatsApp Image 2026-06-29 at 11 45 24 (1)" src="https://github.com/user-attachments/assets/763eb4c0-5a0e-46a6-9ec1-5d24b7f92da3" /></p>

11). Buka Network & internet settings, lalu ikti gambar di bawah ini.
<p align="center">
<img width="440" alt="WhatsApp Image 2026-06-29 at 11 45 25" src="https://github.com/user-attachments/assets/959eb18a-761a-42ca-a039-77e03ee3e6aa" /></p>
<p align="center">
<img width="800" alt="WhatsApp Image 2026-06-29 at 11 45 25 (1)" src="https://github.com/user-attachments/assets/f17e023b-02ba-420b-ba12-4759b67c07ac" /></p>
<p align="center">
<img width="396" alt="WhatsApp Image 2026-06-29 at 11 45 25 (2)" src="https://github.com/user-attachments/assets/5a5fb7f3-1634-4d74-a942-13ad1a344515" /></p>

12). Buka CMD (Command Prompt), lalu ping ke 8.8.8.8
<p align="center">
<img width="700" alt="WhatsApp Image 2026-06-29 at 11 45 26 (1)" src="https://github.com/user-attachments/assets/8c7e7c19-7ff0-4b8e-875a-b787a4ea6450" /></p>

B. Sumber internet IP Statis

Topologi:
<p align="center">
<img width="350" alt="topologi2 drawio" src="https://github.com/user-attachments/assets/d76fce7b-f7de-4e68-9d06-adcc94b86ab2" /></p>
