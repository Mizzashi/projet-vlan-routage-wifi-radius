# projet-vlan-routage-wifi-radius
This project involves designing and configuring a complete network infrastructure that includes VLAN management, routing, DHCP and RADIUS services, as well as a secure Wi-Fi network.

The network is segmented into three VLANs:

- VLAN 10 – Sale : for standard users, with the SSID : sale and the key : key_sale.

- VLAN 20 – Direction : for executives, with the SSID : pa-direction and RADIUS with authentication.

- VLAN 200 – Management : reserved for network administration and infrastructure devices.

The R1 router provides inter-VLAN routing and hosts the DHCP service. The S1 switch, configured as a trunk link to R1, handles VLAN assignment across switch ports.
The Wi-Fi access point, configured in bridge mode, allows wireless clients to connect to the appropriate VLANs.
Finally, a RADIUS server secures access for management users through centralized authentication.

This architecture delivers clear service separation, improved security, and simplified local network administration.

Hardware list : 

- Router (R1) : Cisco 1841
- Switch (S1) : Cisco WS-C2950T-24
- Wireless Access Point (AP) : Cisco AIR-CAP2702E-E-K9
- LXC with Radius server on Proxmox LE Hypervisor

Autonomous AP IOS Software” mode (without Wi-Fi controllers).
- Firmware version: `ap3g2-k9w7-tar.153-3.JF10.tar`**

![Schéma réseau](Diagramme%20TP-Wifi.jpg)


