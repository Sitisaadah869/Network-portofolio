Export dan Import pada mikrotik

Langkah-langkah:

1). Login ke MikroTik menggunakan WinBox

2). Klik Menu New Terminal

3). Ketikan perintah untuk export file

export file=nama-file, nama file=konfigurasi1, jika sudah tekan Enter.

4). Reset Configuration dengan cara:

Klik System>>Reset Configuration

Ceklis Do Not Backup dan No Default Configuration
<p align="center">
<img width="500" alt="Screenshot (283)" src="https://github.com/user-attachments/assets/0a2638a7-40f6-45c6-8237-8469df14a52c" />
</p>
5). Login kembali ke Mikrotik menggunakan WinBox

6). Klik menu New Terminal

7). Ketikan perintah untuk import file

import file-name=konfigurasi1.rsc
<p align="center">
<img width="650" alt="WhatsApp Image 2026-07-10 at 21 16 46" src="https://github.com/user-attachments/assets/36abbf27-fcbd-4ea2-8444-76bc40c74a4a" /></p>

Tekan Enter

8). Lalu lakukan Reboot dengan cara:

System>>Reboot
<p align="center">
<img width="500" alt="WhatsApp Image 2026-07-10 at 21 16 45" src="https://github.com/user-attachments/assets/a71a8ecd-8a4f-476b-991e-a0f45e03a92c" /></p>

9). Jika sudah melakukan Reboot, konfigurasi yang di export sudah ada kembali
<p align="center">
<img width="650" alt="WhatsApp Image 2026-07-10 at 21 16 46 (1)" src="https://github.com/user-attachments/assets/a67a23bd-0b74-478c-a0a1-0f9b75ddaa8f" /></p>

Kesimpulan:

Export dan Import pada mikrotik berfungsi untuk menyimpan dan mengembalikan konfigurasi router MikroTik agar pengguna tidak perlu melakukan konfigurasi ulang.

