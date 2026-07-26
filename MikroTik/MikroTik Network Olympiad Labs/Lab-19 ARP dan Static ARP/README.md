Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Tambahkan Ip Address:

192.168.20.1/24 pada ether 2

<p align="center"><img width="384" alt="WhatsApp Image 2026-07-26 at 20 35 12" src="https://github.com/user-attachments/assets/afe8b6f2-0ca5-457f-b6d1-fef9a28ed8e9" /></p>

3). Menambahkan Static ARP:

IP>>ARP

Klik New+

IP Address: 192.168.20.2

MAC Address: 00-90-F5-C7-5C-5C (MAC Address PC client)

Interface: ether 2

<p align="center"><img width="404" alt="WhatsApp Image 2026-07-26 at 20 35 11" src="https://github.com/user-attachments/assets/c9ffcbde-5b17-47d1-9b07-82ad669a7d06" /></p>

4). Ubah mode ARP di Interface

Interface>>ether2

Ubah opsi ARP: enable menjadi "Reply-only"

<p align="center"><img width="500" alt="WhatsApp Image 2026-07-26 at 20 35 11 (1)" src="https://github.com/user-attachments/assets/d01652aa-0c31-4b8e-bc13-97e0893c1673" /></p>

5). Pengujian
Ubah IP di PC client menjadi 192.168.20.2/24, lalu lakukan ping
<div style="display: flex; gap: 10px;">
<img width="300" alt="WhatsApp Image 2026-07-26 at 20 35 12 (2)" src="https://github.com/user-attachments/assets/a00ef262-e25d-45ae-8e33-1662588594ca" />
<img width="450" alt="WhatsApp Image 2026-07-26 at 20 35 12 (1)" src="https://github.com/user-attachments/assets/beb11318-6440-4e41-b344-2e032a2bcee5" /></div>

Ubah IP di PC client menjadi 192.168.20.2/24 (selain ip yang di masukan di ARP), lalu lakukan ping kembali
<div style="display: flex; gap: 10px;">
<img width="300" alt="WhatsApp Image 2026-07-26 at 20 35 13" src="https://github.com/user-attachments/assets/48139d04-7490-42f7-96a0-e011e248b630" />
<img width="450" alt="WhatsApp Image 2026-07-26 at 20 35 12 (3)" src="https://github.com/user-attachments/assets/e5fae8ab-52e2-4ace-a68d-05dd7c5b8dc9" /></div>
