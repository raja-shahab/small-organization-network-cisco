# Small Organization Network - README

## Project Overview

This project, titled "Small Organization Network," was created using Cisco Packet Tracer to simulate the network infrastructure of a small organization. The network design aims to connect multiple buildings within two cities (City A and City B) with various VLANs to ensure efficient communication, security, and management of network resources.

## Network Design

The network consists of several buildings, each with its own set of devices, connected through a central main campus switch. The network also includes an email server, an FTP server, and a web server to handle different organizational needs.

### Key Components

1. **Main Campus Switch:** The central switch that interconnects all buildings within the organization.
2. **City Routers:** Routers in City A and City B that facilitate communication between the two cities.
3. **Servers:** 
   - **Email Server:** Located in the cloud.
   - **FTP Server and Web Server:** Located in Building A4.
4. **VLANs:** Virtual LANs to segment the network for better traffic management and security.

### Buildings and VLANs

- **City A:**
  - **Building A1:** VLAN 10 (192.168.1.0/24)
    - PCs: PC0, PC1
    - Printer: Printer0
  - **Building A2:** VLAN 20 (192.168.2.0/24)
    - PCs: PC2, PC3
    - Printer: Printer1
  - **Building A3:** VLAN 30 (192.168.3.0/24)
    - PCs: PC4, PC5
    - Printer: Printer2
  - **Building A4:** VLAN 40 (192.168.4.0/24)
    - Server: FTP Server, Web Server
    - PCs: PC6, PC7
    - Printer: Printer3

- **City B:**
  - **Building B1:** VLAN 80 (192.168.8.0/24)
    - PCs: PC8
    - Printer: Printer4
  - **Building B2:** VLAN 100 (192.168.10.0/24)
    - PCs: PC9
    - Printer: Printer5

## Network Diagram

(images/network_diagram.png)

### Description

- **Cloud Connection:** The email server is placed in the cloud with an IP address of 20.0.0.1/30.
- **City A Router (10.10.10.1/30):** Connects the main campus switch and the cloud.
- **City B Router (10.10.10.2/30):** Connects to the main campus switch and provides communication with City B.
- **Inter-building Connections:** Each building in City A and City B is connected to the main campus switch or respective routers using appropriate switch models (2960, 3560, etc.).
