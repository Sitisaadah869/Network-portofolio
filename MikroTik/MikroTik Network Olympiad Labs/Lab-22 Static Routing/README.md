Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Lakukan Basic Configuration:

Ip Address ether 2 : 192.168.20.1/24

DHCP Client : 

Interface: wlan1 

add default route: no

DHCP Server : ether 2

Firewall-nat : 

Chain: srcnat

Out. Interface: wlan1

Action: Masquerade

3). IP>>Route: new+

dst-address: 8.8.8.0

gateway: 10.47.117.50

apply, ok

4). cara melihat gateway

Buka New Terminal

Ketikan perintah : ip dhcp-client print detail
