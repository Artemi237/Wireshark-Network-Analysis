# Wireshark-Network-Analysis
basic network traffic analysis using Wireshark in a virtualized environment
The objective was to capture, observe and understand how devices communicate over a network using different protocols.

---

## Environment

- Operating System: Kali Linux  
- Virtualization: VirtualBox  
- Network configuration: NAT + Host-Only  
- Tool used: Wireshark  

---

## Objectives

- Capture real network traffic  
- Identify different protocols (ICMP, DNS, TCP)  
- Understand how communication happens between a client and external servers  
- Analyze packets and interpret their meaning  

---

## Packet Capture

Wireshark was used to capture network traffic on the `eth0` interface.  
Traffic was generated using ping commands and web browsing.

---

## ICMP Analysis

ICMP packets were captured during a ping test to `google.com`.

- Source: 10.0.2.15 (local machine)  
- Destination: external server (Google)  
- Protocol: ICMP  

This shows that the local machine can communicate with external servers and receive responses.

---

## DNS Analysis

DNS traffic was observed when resolving domain names.

- Source: 10.0.2.15  
- Destination: 8.8.8.8 (DNS server)  
- Protocol: DNS (UDP)  

The machine sends a request to the DNS server to resolve a domain name into an IP address.  
The DNS server responds with the corresponding IP.

---

## TCP / HTTPS Analysis

TCP traffic using TLS was captured during web browsing.

- Protocol: TCP  
- Port: 443 (HTTPS)  
- Encryption: TLSv1.2  

This demonstrates secure communication between the client and web servers.

---

## Troubleshooting

During the setup, the virtual machine did not receive an IP address via DHCP, which prevented internet connectivity.

To resolve this issue, a manual network configuration was applied:

- Static IP assignment  
- Default gateway configuration  
- DNS server configuration  

This allowed proper network connectivity and enabled packet capture.

---

## Conclusion

This project provided a practical introduction to network traffic analysis.  
It demonstrated how different protocols (ICMP, DNS, TCP) are used in real communication.

The troubleshooting phase also helped develop problem-solving skills related to network configuration.

---

## Skills Demonstrated

- Network traffic capture using Wireshark  
- Packet analysis (ICMP, DNS, TCP)  
- Understanding of network protocols  
- Troubleshooting network configuration issues  
- Virtual machine network setup  

---
