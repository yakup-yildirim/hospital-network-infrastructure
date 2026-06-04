# Hospital Network Infrastructure

## Short Description

This project simulates a hospital network infrastructure created in Cisco Packet Tracer. It includes multiple hospital departments, VLANs, routing, WAN links, DHCP, NAT, ACL rules, and a Site-to-Site IPsec VPN tunnel for a remote medical center.

The project was created for learning and GitHub portfolio purposes as a Computer Science student project. It does not use any real hospital data and is not intended to represent a production-ready network.

## Main Features

- Department-based network segmentation using VLANs
- Router-on-a-stick configuration for inter-VLAN routing
- WAN links between multiple routers
- OSPF routing between the main hospital routers
- DHCP services for department clients
- NAT/PAT for simulated internet access
- ACL rules for basic access control
- IPsec VPN tunnel between the Emergency network and a remote Turkey Medical Center
- Public web server simulation
- Basic SSH configuration for device management

## Network Topology Overview

The topology represents a regional hospital network with several departments connected through routers and switches. The main hospital network contains IT, Admin, Laboratory, Polyclinics, and Emergency departments.

The core routers are connected using WAN links to simulate a hospital backbone. The Emergency router is also connected to a remote Turkey Medical Center using an IPsec VPN tunnel. A separate internet/NAT section is used to simulate external network access.

Main network areas:

- IT Department
- Admin Department
- Laboratory
- Polyclinics
- Emergency
- Turkey Remote Medical Center
- Internet / public web server simulation

## VLAN and IP Addressing Table

| Network Area | VLAN | Network Address | Default Gateway |
|---|---:|---|---|
| IT Department | 10 | 192.168.10.0/24 | 192.168.10.1 |
| Admin Department | 11 | 192.168.11.0/24 | 192.168.11.1 |
| Laboratory | 20 | 192.168.20.0/24 | 192.168.20.1 |
| Polyclinics | 30 | 192.168.30.0/24 | 192.168.30.1 |
| Emergency | 40 | 192.168.40.0/24 | 192.168.40.1 |
| Turkey Remote Medical Center | 50 | 192.168.50.0/24 | 192.168.50.1 |

## Main Devices and Services

- Multiple Cisco routers and switches
- Department PCs and printers
- Hospital file/database server
- DNS / web server
- Public web server
- DHCP pools for departments
- NAT for simulated internet access
- ACL rules for access control
- IPsec VPN tunnel for the remote medical center
- WAN links between routers

## Technologies and Concepts Used

- Cisco Packet Tracer
- VLANs
- Router-on-a-stick
- IPv4 addressing and subnetting
- OSPF routing
- DHCP
- NAT/PAT
- Standard and extended ACLs
- WAN connections
- Site-to-Site IPsec VPN
- SSH remote access
- Basic network security concepts

## How to Open the Project

1. Install Cisco Packet Tracer.
2. Download or clone this repository.
3. Open the `.pkt` file with Cisco Packet Tracer.
4. Review the topology, device configurations, VLANs, routing, ACLs, NAT, and VPN settings.

## What I Learned

While working on this project, I practiced how to design and configure a network for a multi-department organization. I learned how VLANs can separate departments, how routers can connect different networks, and how OSPF can be used for routing between multiple routers.

I also practiced DHCP configuration, NAT for internet access, ACL-based traffic control, SSH access, and IPsec VPN configuration for a remote site.

## Future Improvements

- Add more detailed documentation for each router and switch configuration
- Add a cleaner topology diagram image to the repository
- Add more detailed verification screenshots
- Add monitoring or logging features
- Add redundant internet access or backup routing paths
- Expand the remote medical center with more devices

## Note

This project was created only for learning and portfolio purposes. It does not contain real hospital data and should not be considered a production-ready network design.

