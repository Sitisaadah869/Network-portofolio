Topologi:
<p align="center">
<img width="508" alt="topologiwlan drawio" src="https://github.com/user-attachments/assets/b11e15c4-2d3a-493b-b996-77c1e5faf130" />
</p>
Langkah-langkah:

1). Buka menu Wireless, klik Security Profile, klik + General lalu isi:

Name: belajar
Mode: dynamic keys
Authenttication Types: WPA2 PSK, WPA2 EAP
WPA2 Pre-Shared Key: Semangat45

Apply lalu OK

2). Klik menu Inteface>>Wireless, ubah Security Profile-default menjadi belajar, jika sudah klik scan>>start



3). Klik SSID Belajar-Mikrotik, lalu klik connect


4). Buka IP-DHCP Client, klik New lalu ubah Interface>>Wlan1, Apply lalu Ok, Pastikan sudah ada tulisan Bound


5). Buka New Terminal keti ping 8.8.8.8, pastikan sudah connect


6). Buka IP-Firewal-NAT, isi konfigurasi dengan:

Chain: srcnat
Out.Interface: wlan1
Action: masquerade

7). Buka IP_Address, tambahkan IP 192.168.20.1/24 di ether2 


8). Buka Network 


9). Buka CMD lalu ketik ping 8.8.8.8 dan tracert 8.8.8.8
