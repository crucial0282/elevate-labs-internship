# 📄 Packet Capture Summary Report

Internship Task: Live Network Traffic Analysis
Tool Used: Wireshark
Capture File: wireshark-capture.pcapng
Duration: ~1 Minute
## 🔍 Summary of Observed Network Activities
The captured network traffic reveals a mix of IPv4 and IPv6 communications, involving several key protocols and interactions:
### 1. UDP Communication

    Traffic was observed between 192.168.1.7 and 224.77.77.77 over port 12177.

    Packet content includes XML-like data referencing "ASUS_ARMOURY_CRATE", indicating communication from ASUS software related to device management or telemetry.

### 2. ARP Resolution

    Multiple ARP requests and replies show IP-to-MAC address mapping activities.

    Example: 192.168.1.7 was resolved to MAC 14:d4:24:90:21:bf.

    Indicates active discovery or validation of local network hosts.

### 3. ICMPv6 Interactions

    Includes Neighbor Solicitations and Advertisements, which are part of IPv6’s address resolution process.

    Involves link-local and global addresses such as:

        fe80::1, fe80::3907:173:601c:d32b

        2402:e280:2203:110::1, 2402:e280:2203:110:1b94:9fbd:5546:339

### 4. TCP and TLSv1.3 Connections

    TCP 3-way handshakes were followed by TLSv1.3 encrypted sessions.

    Notable SNI (Server Name Indication) included: assets.msn.com.

    Suggests secure communication with Microsoft services.

    Presence of TLS continuation segments indicates ongoing data transfer over encrypted channels.

### 5. Device Identification

    Devices involved had MAC addresses linked to:

        AzureWave Technologies (e.g., 14:d4:24:90:21:bf) – common in Wi-Fi modules.

        Taicang T&W Electronics (e.g., 40:33:06:94:af:f0) – likely a networked device or access point.

## 📌 Conclusion

The packet capture reflects normal device activity on a home or office network. It includes multicast software communication (ASUS Armoury Crate), local device discovery (ARP and ICMPv6), and secure access to external services (TLS to assets.msn.com).
