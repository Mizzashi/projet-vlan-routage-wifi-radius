# projet-vlan-routage-wifi-radius
This project involves designing and configuring a complete network infrastructure that includes VLAN management, routing, DHCP and RADIUS services, as well as a secure Wi-Fi network.

The network is segmented into three VLANs:

- VLAN 10 – Staff Room: for standard users, with the SSID sale and the key key_sale.

- VLAN 20 – Management: for executives, with the SSID pa-direction and RADIUS authentication.

- VLAN 200 – Administration: reserved for network administration and infrastructure devices.

The R1 router provides inter-VLAN routing and hosts the DHCP service. The S1 switch, configured as a trunk link to R1, handles VLAN assignment across switch ports.
The Wi-Fi access point, configured in bridge mode, allows wireless clients to connect to the appropriate VLANs.
Finally, a RADIUS server secures access for management users through centralized authentication.

This architecture delivers clear service separation, improved security, and simplified local network administration.


![Schéma réseau](Diagramme%20TP-Wifi.jpg)

```bash
ping 8.8.8.8
