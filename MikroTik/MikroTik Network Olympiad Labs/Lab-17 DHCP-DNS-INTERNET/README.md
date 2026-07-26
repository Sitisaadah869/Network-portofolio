Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Konfigurasi Ip Address:

Buka menu IP>>Addresses

Klik + lalu tambahkan

Address: 192.168.10.1/24 

Interface: ether2

<p align="center"><img width="376" alt="WhatsApp Image 2026-07-26 at 19 24 17" src="https://github.com/user-attachments/assets/36fabea2-cd9f-439f-b558-8261f42a3b53" /></p>

3). Buka menu IP-DHCP Client, klik New lalu ubah Interface>>Wlan1, Apply lalu Ok, Pastikan sudah ada tulisan Bound

4). Buka menu IP>>DHCP Server, klik DHCP setup, pilih interface ether2 lalu klik next sampai muncul tulisan DNS, isi DNS dengan 8.8.8.8 dan 8.8.4.4 lalu klik next sampai selesai. 

<img width="500" height="288" alt="WhatsApp Image 2026-07-26 at 19 24 15" src="https://github.com/user-attachments/assets/1008d285-4b4d-46f1-b1e8-6f3e106d60c0" />

<div style="display: flex; gap: 10px;"><img width="500" alt="WhatsApp Image 2026-07-26 at 19 24 16" src="https://github.com/user-attachments/assets/08b0d5b5-d82d-490a-9d15-198ad5fc1f9c" />
<img width="500" alt="WhatsApp Image 2026-07-26 at 19 24 17 (2)" src="https://github.com/user-attachments/assets/abf3ba0f-8c87-492f-b165-86a2b4d6f132" /></div>

5). Buka menu IP-Firewal-NAT, isi konfigurasi dengan:

Chain: srcnat Out.Interface: wlan1 Action: masquerade

<p align="center"><img width="600" alt="WhatsApp Image 2026-07-26 at 19 24 17 (1)" src="https://github.com/user-attachments/assets/47bea15b-3b13-4414-a948-e589a48977f8" /></p>

6). Pengujian

<p align="center"><img width="612" alt="WhatsApp Image 2026-07-26 at 19 24 17 (3)" src="https://github.com/user-attachments/assets/dca45c96-0506-45c3-bc2b-35be2c7353d3" /></p>


Kesimpulan:

DHCP berfungsi untuk memberikan IP secara otomatis kepada client, sedangkan DNS digunakan untuk menerjemahkan nama domain menjadi alamat IP. Sehingga client bisa terhubung ke internet
