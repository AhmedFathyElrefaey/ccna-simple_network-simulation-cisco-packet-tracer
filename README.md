# CCNA Enterprise Network Simulation

A practical enterprise network simulation developed using Cisco Packet Tracer as part of my CCNA learning journey.

## Project Overview

This project simulates a small enterprise network consisting of two IPv4 network segments.

The topology includes routers, switches, PCs, printers, and dedicated DHCP servers.

The main goal of the project was to apply CCNA networking concepts in a practical environment and gain hands-on experience with network configuration and troubleshooting.

## Network Topology

The network consists of two main network segments.

Each network contains:

- 1 Router
- 2 Switches
- 4 PCs
- 2 Printers
- 2 DHCP Servers

## IPv4 Addressing

The original network was:

192.168.40.0/24

It was divided into two equal /25 subnets.

### Network 1

- Network: `192.168.40.0/25`
- Subnet Mask: `255.255.255.128`
- Default Gateway: `192.168.40.1`
- DHCP Server: `192.168.40.2`
- DHCP Client Range: `192.168.40.3 - 192.168.40.126`
- Broadcast: `192.168.40.127`

### Network 2

- Network: `192.168.40.128/25`
- Subnet Mask: `255.255.255.128`
- Default Gateway: `192.168.40.129`
- DHCP Server: `192.168.40.130`
- DHCP Client Range: `192.168.40.131 - 192.168.40.254`
- Broadcast: `192.168.40.255`

## Technologies and Concepts

- IPv4 Addressing
- IPv4 Subnetting
- CIDR
- DHCP
- Static IP Addressing
- Default Gateway
- Cisco IOS
- Layer 2 Switching
- Layer 3 Routing
- Network Troubleshooting
- Cisco Packet Tracer

## Troubleshooting

During the implementation, the PCs initially failed to obtain IP addresses through DHCP.

The issue was identified as an incorrect DHCP Server IP configuration.

After assigning static IP addresses to the DHCP servers and configuring the correct subnet mask and default gateway, the PCs successfully obtained their IP addresses.

This troubleshooting process helped reinforce the importance of understanding how DHCP and network addressing work together.

## Verification

The network was verified using:

```bash
ipconfig
ping
