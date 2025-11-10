# Networking Basics

This file contains basic notes on networking concepts and common troubleshooting commands.

## 1. IP Addresses
- An IP address is a unique identifier for a device on a network.
- Example: `192.168.1.1`
- IPv4 format: 4 numbers separated by dots (0-255)

## 2. Subnetting
- Subnetting divides a network into smaller segments.
- Example: `192.168.1.0/24` → 256 addresses (0-255)
- Common subnet masks:
  - /24 → 255.255.255.0
  - /16 → 255.255.0.0

## 3. Ping & Traceroute
- **Ping**: Test connectivity to another device.
  ping 8.8.8.8

Traceroute: See the path packets take to reach a device.

traceroute 8.8.8.8    # Linux/macOS
tracert 8.8.8.8       # Windows

## 4. DNS Basics
DNS (Domain Name System) converts domain names to IP addresses.

Example: google.com → 142.250.190.14

Useful troubleshooting commands:
nslookup google.com
dig google.com 

#ping google.com
#ipconfig /flushdns
#netsh int ip reset
#netsh winsock reset


