A **Network** is a group of interconnected devices (computers, phones, servers, etc.) that can communicate with each other.

**Key Networking Components**

 **Devices:** Anything that sends or receives data on a network (laptops, servers, smartphones, smart TVs, etc.).

 **Switches:** Intelligent devices that connect other devices within a **LAN**, efficiently directing traffic.
 
 **Routers:** Devices that connect different networks, like connecting your home network to the internet. They intelligently route data packets between networks.

 **Cables/Wireless:** The physical medium that provides the connection. This can be Ethernet cables, fiber optic cables, or wireless signals (Wi-Fi)


**IP Addresses:** Every device on a network has a unique IP address (like 192.168.1.10). Think of it as the device's "mailing address" for data.
- IPv4: - 
	- The older and most common internet protocol.
	- Uses 32-bit addresses.
	- Provides approximately 4.3 billion unique IP addresses.
- IPv6: 
	- -The newer standard, designed to address the limitations of IPv4.
	- Uses 128-bit addresses.
	- Provides an astronomically large address space (340 undecillion addresses!).
	- More complex format with colons separating groups of hexadecimal digits.
	- 
**IP Allocation:**
1. **Manually(Static):** The network administrator assigns a specific fixed IP address to each device on the network. This involves manually configuring network settings on the device itself.
2. **Dynamically(DHCP):**  Dynamic Host Configuration Protocol server is set up on the network. Devices configured for DHCP automatically request an IP address from this server when they connect. The DHCP server leases an available IP address from a pool for a set period.

**Packets:** Small chunks of data aka packets. Each packet has the sender's and receiver's IP address and other information to help it travel.

**Protocols:** These are like the "rules of the road" governing how data is formatted, transmitted, and received (examples: TCP, HTTP, DNS).

## Commands

- `ping`
- `host`
- `nslookup`
- `dig`
- `ipconfig`
- `ip`
- `route or ip route`
- `traceroute`
- `netstat`
- `ethtool`
- `tcpdump`
- `nmap`