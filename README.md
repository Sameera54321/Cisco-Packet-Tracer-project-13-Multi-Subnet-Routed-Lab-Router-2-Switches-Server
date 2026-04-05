# Cisco-Packet-Tracer-project-13-Multi-Subnet-Routed-Lab-Router-2-Switches-Server

I’m happy to share a clean, practical networking project – a multi‑subnet routed network built in Cisco Packet Tracer.

![image alt](https://github.com/Sameera54321/Cisco-Packet-Tracer-project-13-Multi-Subnet-Routed-Lab-Router-2-Switches-Server/blob/main/19.png?raw=true)

## 📌 Summary

### Multi‑Subnet Routed Lab is a Cisco Packet Tracer simulation that models a small enterprise network with three separate IP subnets interconnected by a single router. The network consists of:

    1 router (Router0) – with three LAN interfaces (or subinterfaces)

    2 switches (Switch1, Switch2) – Cisco 2968‑24TT (access layer)

    2 PCs (PC0, PC1) – end users

    1 server (Server0) – providing network services

### IP addressing :

| Device | Interface/IP | Subnet |
| :--- | :--- | :--- |
| Router0 (int to Switch1) | 172.16.31.1 | 172.16.31.0/24 |
| PC0 | 172.16.31.12 | 172.16.31.0/24 |
| Router0 (int to Switch2) | 192.168.50.1 | 192.168.50.0/24 |
| PC1 | 192.168.50.252 | 192.168.50.0/24 |
| Router0 (int to Server) | 10.10.10.1 | 10.10.10.0/24 |
| Server0 | 10.10.10.10 | 10.10.10.0/24 |

### The project focuses on:

    Router configuration – assigning IP addresses to interfaces, enabling routing (directly connected routes handle inter‑subnet communication automatically)

    Switch configuration – connecting PCs and server to the correct VLAN (or default VLAN 1)

    End‑device settings – static IP addresses with correct default gateways (the router’s interface IP on each subnet)

    Connectivity verification – using ping from PC0 (172.16.31.12) to Server0 (10.10.10.10) and PC1 (192.168.50.252)

    Optional server services – configure DHCP, DNS, or HTTP on Server0 to serve all subnets

## ✨ Features

    ✅ Three separate IP subnets – 172.16.31.0/24, 192.168.50.0/24, 10.10.10.0/24

    ✅ Router0 – inter‑subnet routing (directly connected routes)

    ✅ Two Cisco 2968 switches – access layer connectivity

    ✅ Server0 – can provide DHCP, DNS, HTTP, or FTP services

    ✅ PCs – realistic end‑user devices for testing

    ✅ Full Packet Tracer file (.pkt) – ready to open and practice

    ✅ Documentation – IP addressing table, router config, switch configs

## 🛠️ Built With

    Cisco Packet Tracer – version 8.x

    CLI – router and switch configurations

## 🤝 Contributing

Contributions are welcome! To extend this lab:

    Fork the repository.

    Add dynamic routing (RIP/OSPF/EIGRP) if more routers are added.

    Implement VLANs on the switches and router‑on‑a‑stick.

    Configure the server as a DHCP server for all three subnets (using DHCP relay).

    Add access control lists (ACLs) to restrict traffic between subnets.

    Open a pull request with a clear description.

## 📜 License

Distributed under the MIT License. See the LICENSE file for more information.
Free to use, modify, and share for educational purposes.
