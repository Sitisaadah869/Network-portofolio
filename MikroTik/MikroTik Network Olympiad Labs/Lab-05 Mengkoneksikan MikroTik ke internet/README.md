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
<img width="800" height="135" alt="WhatsApp Image 2026-06-29 at 12 23 38" src="https://github.com/user-attachments/assets/ed96dc9f-52fb-4e8f-949a-d423d61aefe8" />
</p>

4). Klik Security Profile, isi WPA-2 dengan Password WIFI.
<p align="center">
<img width="525" alt="WhatsApp Image 2026-06-29 at 12 23 14" src="https://github.com/user-attachments/assets/f7fafb3b-d3af-43a8-8651-dc3236fb6511" />
</p>
5). Buka Interface WLAN ubah default menjadi Profile1, Lalu scan dan connect.
<p align="center">
<img width="550" alt="WhatsApp Image 2026-06-29 at 12 22 51" src="https://github.com/user-attachments/assets/d0275329-cb82-42f5-a6e5-f412fa30a2ed" />
</p>

6). Klik IP-DHCP Client, klik New, masukkan interface WLAN1, lalu klik Apply dan Ok.
Pastikan status DHCP Client sudah Bound.
<p align="center">
<img width="600" alt="WhatsApp Image 2026-06-29 at 12 22 27" src="https://github.com/user-attachments/assets/be9eba23-a456-44bc-bd83-fd893da11f36" />
</p>

7). Buka IP-Firewall NAT, sesuaikan isi dengan gambar di bawah ini.
<p align="center">
<img width="600" alt="WhatsApp Image 2026-06-29 at 12 32 20 (1)" src="https://github.com/user-attachments/assets/8b9028b2-cf49-4f88-923a-6a4c62db4a71" />
</p>
<p align="center">
<img width="550" alt="WhatsApp Image 2026-06-29 at 12 36 26" src="https://github.com/user-attachments/assets/0ae1a15f-ffc5-454a-99ad-002a80fecde5" />
</p>

8). Buka New Terminal, ketik ping google.com atau ping 8.8.8.8, jika sudah connect berarti MikroTik sudah terhubung ke internet.
<p align="center">
<img width="596" height="408" alt="WhatsApp Image 2026-06-29 at 11 34 44" src="https://github.com/user-attachments/assets/e12cec5a-7db5-4521-b253-d4348578c99e" /></p>

9). Masukan IP Address 192.168.10.1/24 pada ether2

<p align="center">
<img width="528" height="380" alt="WhatsApp Image 2026-06-29 at 11 45 24" src="https://github.com/user-attachments/assets/edbcfc52-433c-42d9-84c1-a6bd2a2babd6" /></p>


10). Buka menu IP, klik DHCP Server, klik DHCP setup, pilih interface ether2 lalu klik next sampai selesai.
<p align="center">
<img width="868" height="372" alt="WhatsApp Image 2026-06-29 at 11 45 24 (1)" src="https://github.com/user-attachments/assets/763eb4c0-5a0e-46a6-9ec1-5d24b7f92da3" /></p>

11). Buka Network & internet settings, lalu ikuti gambar di bawah ini.
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
<img width="507" height="333" alt="topologi drawio" src="https://github.com/user-attachments/assets/0c95041e-1091-4c0f-b05f-b298dd070605" /></p>

Langkah-langkah:

1). Login ke MikroTik menggunakan WinBox.

2). Buka menu Wireless.

3). Pilih Interface WLAN1, lalu klik tanda centang (enable).
<p align="center">
<img width="800" alt="WhatsApp Image 2026-06-29 at 12 23 38" src="https://github.com/user-attachments/assets/ed96dc9f-52fb-4e8f-949a-d423d61aefe8" /></p>

4). Klik Security Profile, isi WPA-2 dengan Password WIFI.
<p align="center">
<img width="525" alt="WhatsApp Image 2026-06-29 at 12 23 14" src="https://github.com/user-attachments/assets/f7fafb3b-d3af-43a8-8651-dc3236fb6511" />
</p>
5). Buka Interface WLAN ubah default menjadi Profile1, Lalu scan dan connect.
<p align="center">
<img width="550" alt="WhatsApp Image 2026-06-29 at 12 22 51" src="https://github.com/user-attachments/assets/d0275329-cb82-42f5-a6e5-f412fa30a2ed" /></p>

6). Klik IP-DHCP Client, klik New, masukkan interface WLAN1, lalu klik Apply dan Ok.
Pastikan status DHCP Client sudah Bound.
<p align="center">
<img width="600" alt="WhatsApp Image 2026-06-29 at 12 22 27" src="https://github.com/user-attachments/assets/be9eba23-a456-44bc-bd83-fd893da11f36" />
</p>

7). Buka IP-Firewall NAT, sesuaikan isi dengan gambar di bawah ini.
<p align="center">
<img width="600" alt="WhatsApp Image 2026-06-29 at 12 22 27" src="https://github.com/user-attachments/assets/be9eba23-a456-44bc-bd83-fd893da11f36" />
</p>
<p align="center">
<img width="550" alt="WhatsApp Image 2026-06-29 at 12 36 26" src="https://github.com/user-attachments/assets/0ae1a15f-ffc5-454a-99ad-002a80fecde5" /></p>

8). Buka New Terminal, ketik ping google.com atau ping 8.8.8.8, jika sudah connect berarti MikroTik sudah terhubung ke internet.
<p align="center">
<img width="596" height="408" alt="WhatsApp Image 2026-06-29 at 11 34 44" src="https://github.com/user-attachments/assets/e12cec5a-7db5-4521-b253-d4348578c99e" /></p>

9). Masukan IP Address 192.168.10.1/24 pada ether2

<p align="center">
<img width="528" height="380" alt="WhatsApp Image 2026-06-29 at 11 45 24" src="https://github.com/user-attachments/assets/edbcfc52-433c-42d9-84c1-a6bd2a2babd6" /></p>

10). Buka Network & internet settings, lalu ikuti gambar di bawah ini.
<p align="center">
<img width="440" alt="WhatsApp Image 2026-06-29 at 11 45 25" src="https://github.com/user-attachments/assets/959eb18a-761a-42ca-a039-77e03ee3e6aa" /></p>
<p align="center">
<img width="800" alt="WhatsApp Image 2026-06-29 at 11 45 25 (1)" src="https://github.com/user-attachments/assets/f17e023b-02ba-420b-ba12-4759b67c07ac" /></p>
<p align="center">
<img width="392" height="452" alt="WhatsApp Image 2026-06-29 at 11 45 26" src="https://github.com/user-attachments/assets/51a78dce-c150-48a4-9ecc-026b8988d10a" />
</p>
11). Buka CMD (Command Prompt), lalu ping ke 8.8.8.8
<p align="center">
<img width="700" alt="WhatsApp Image 2026-06-29 at 11 45 26 (1)" src="https://github.com/user-attachments/assets/8c7e7c19-7ff0-4b8e-875a-b787a4ea6450" /></p>

Kesimpulan:

MikroTik bisa terhubung ke internet dengan menggunakan dynamic (otomatis) atau static (manual).
