Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Tambahkan Ip Address:

192.168.20.1/24 pada ether 2

3). Menambahkan Static ARP:

IP>>ARP

Klik New+

IP Address: 192.168.20.2

MAC Address: 00-90-F5-C7-5C-5C (MAC Address PC client)

Interface: ether 2

4). Ubah mode ARP di Interface

Interface>>ether2

Ubah opsi ARP: enable menjadi "Reply-only"

5). Pengujian
Ubah IP di PC client menjadi 192.168.20.2/24, lalu lakukan ping


Ubah IP di PC client menjadi 192.168.20.2/24 (selain ip yang di masukan di ARP), lalu lakukan ping kembali
