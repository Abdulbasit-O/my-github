# Small Office Network with DHCP,DNS and VLANs (Cisco Packet Tracer)
This project is a small office network i built using Cisco Packet Tracer.
It includes VLANs for seperating departments, a DDHCP for automatic IP addresses, a DNS server for name resolution.
The goal was to understand how small network works and how to troubleshoot them.
## What I Built 
- Two VLAN (Admin & Support)
- A router using Router on a stick for inter VLAN communication
- A DHCP server that gives PCs their ip adresses automatically
- A DNS server thatr resolves a custom domain name 
- 10 PCs connected to their respective VLANs
## IP Setup 
- VLAN 10 - Admin:**192.168.10.0/24**
- VLAN 20 - Support:**192.168.20.0/24**
- Router Gateways:**192.168.10.1**, **192.168.10.2**
## Testing 1 Performed 
- PCs succesfully received IP addresses via the DHCP
- Devices in the same VLAN communicated efficiently
- Inter VLAN communication worked through the router
- DNS resolved 'office.local' correctly
## Troubleshooting I Practiced
- wrong VLAN Assignments
- Incorrect trunk configuration
- wrong gateways in DHCP settings
## How To Use The Project
- Download the '.pkt' file from this repositery
- Open it in cisco packet tracer
- Power on all devices
- Test pings between PCs
- Explore the DHCP and DNS settings
