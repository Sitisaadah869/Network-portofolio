Default Configuration adalah konfigurasi bawaan yang sudah tersedia pada router MikroTik setelah di reset atau pertama kali digunakan.

Langkah-langkah:

1). Login ke MikroTik menggunakan WinBox.

2). Pilih menu System-Reset Configuration.
<p align="center">
<img width="500" alt="cpyan " src="https://github.com/user-attachments/assets/ac1357bc-eca1-416f-bcc8-32b0bcd5f81e" />
</p>
3). Lalu klik Reset Configuration.
<p align="center">
<img width="500" alt="Screenshot (115)" src="https://github.com/user-attachments/assets/b46dbfc1-4ea4-4e19-acf4-14b584bb6752" />
</p>
4). Setelah selesai melakukan Reset Conguration, login kembali menggunakan WinBox.

5) Login dengan IP 182.168.88.1, user "admin", password kosongkan, lalu klik connect.
<p align="center">
<img width="600" alt="Screenshot (118)" src="https://github.com/user-attachments/assets/16477220-663d-43f7-8331-971b00afa5bd" /></p>

Default Configuration berisi:

a. IP Address 192.168.88.1/24.

<img width="500" alt="Screenshot 2026-06-23 124012" src="https://github.com/user-attachments/assets/0d04caad-2131-4fc5-b97f-ba20bae4bbbb" />

b. Username "admin", password kosong.

c. DHCP Client aktif pada ether1
<p align="center">
<img width="600" alt="Screenshot (123)" src="https://github.com/user-attachments/assets/9be6d386-cb63-4a5e-9950-8d1d7d2c17e7" />
</p>
d. Bridge ports untuk menggabungkan beberapa interface menjadi satu segmen jaringan.
<p align="center">
<img width="600" alt="Screenshot (125)" src="https://github.com/user-attachments/assets/d2a9de2a-becb-45d2-be82-0691e86aa1ea" />
</p>

e. NAT untuk menghubungkan jaringan lokal ke internet.
<p align="center">
<img width="600" alt="Screenshot (127)" src="https://github.com/user-attachments/assets/dbd9db63-16cf-4ded-b592-7d600a80dd54" />
</p>
Kesimpulan:
Default Configuration pada MikroTik berisi pengaturan awal yang membantu saat mulai melakukan konfigurasi.
