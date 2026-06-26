Menghubungkan MikroTik ke internet menggunakan WLAN 

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


Agar PC/Laptop mendapatkan internet, bisa mengikuti cara-cara berikut:

1). Buka IP-Address klik + masukkan ip 192.168.10.1/24 ether2, jika sudah klik Apply dan Ok.
<p align="center">
<img width="700" alt="Screenshot (168)" src="https://github.com/user-attachments/assets/083f04b8-8baf-4ec9-93f4-4ab15ec4b10a" /></p>

2). Buka IP-DHCP Server, klik DHCP-Setup, Interface "ether2", lalu klik Next sampai selesai.
<p align="center">
<img width="700" alt="Screenshot (169)" src="https://github.com/user-attachments/assets/fa944193-27dc-4e5e-a4c6-77c60398553a" /></p>

3). Buka Network & Internet Setting double klik ethernet yang akan dihubungkan, lalu ikuti gambar di bawah ini.
<p align="center">
<img width="500" alt="Screenshot (172)" src="https://github.com/user-attachments/assets/5ef84448-bcb7-43bd-a834-6f6237ea8926" /></p>
<p align="center">
<img width="500" alt="Screenshot (174)" src="https://github.com/user-attachments/assets/e109d235-0468-4f6b-9ed9-9403efba62fa" /></p>

4). Buka CMD (Command Prompt), lalu ketik ping google.com atau ping 8.8.8.8
<p align="center">
<img width="500" alt="Screenshot (176)" src="https://github.com/user-attachments/assets/6896f3b6-ec22-4a3b-90a0-131878847cbf" /></p>
