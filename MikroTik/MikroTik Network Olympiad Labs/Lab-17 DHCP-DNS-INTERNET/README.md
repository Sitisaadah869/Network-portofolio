Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Konfigurasi Ip Address:

Buka menu IP>>Addresses
Klik + lalu tambahkan
Address: 192.168.10.1/24 
Interface: ether2

3). Buka menu IP-DHCP Client, klik New lalu ubah Interface>>Wlan1, Apply lalu Ok, Pastikan sudah ada tulisan Bound

4). Buka menu IP>>DHCP Server, klik DHCP setup, pilih interface ether2 lalu klik next sampai muncul tulisan DNS, isi DNS dengan 8.8.8.8 dan 8.8.4.4 lalu klik next sampai selesai. 

5). Buka menu IP-Firewal-NAT, isi konfigurasi dengan:

Chain: srcnat Out.Interface: wlan1 Action: masquerade

6). Pengujian


Kesimpulan:

DHCP berfungsi untuk memberikan IP secara otomatis kepada client, sedangkan DNS digunakan untuk menerjemahkan nama domain menjadi alamat IP. Sehingga client bisa terhubung ke internet
