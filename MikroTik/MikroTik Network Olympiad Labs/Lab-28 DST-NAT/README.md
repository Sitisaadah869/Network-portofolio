Langkah-langkah

1). Login ke MikroTik menggunakan WinBox

2). Lakukan Basic Configuration:

Ip Address ether 2 : 192.168.20.1/24

DHCP Client : 

Interface: wlan1 

add default route: yes

DHCP Server : ether 2

3). Firewall-nat : 

Chain: dstnat

Dst. Address: 10.47.117.50

Protocol: 6(tcp) 

Dst. Port: 8081

Action: dst-nat

To Address: 192.168.20.1

To Port: 80

apply, ok

4). Pengujian
