# Wireshark Traffic Analysis Report

## 🎯 Objective:
To capture and analyze live network traffic using Wireshark and identify various protocols used during communication over the internet.

## 📁 File Captured:
- **Filename:** network_capture.pcap
- **Tool Used:** Wireshark
- **Capture Duration:** ~1 minute
- **Interface Used:** Wi-Fi (active interface)
- **Total Packets Captured:** Varies based on traffic (e.g., 300-1500)

---

## ✅ Protocols Identified:

### 1. **DNS (Domain Name System)**
- Purpose: Resolves domain names to IP addresses.
- Observed Activity: Requests to resolve websites like `google.com`, `openai.com`.
- Example Filter Used: `dns`

### 2. **TCP (Transmission Control Protocol)**
- Purpose: Provides reliable, ordered, and error-checked delivery of data.
- Observed Activity: 3-way handshakes, HTTP traffic.
- Example Filter Used: `tcp`

### 3. **HTTP (HyperText Transfer Protocol)**
- Purpose: Transfers web pages and resources.
- Observed Activity: Browsing unencrypted websites.
- Example Filter Used: `http`

### 4. **ICMP (Internet Control Message Protocol)**
- Purpose: Used for diagnostic functions (e.g., ping).
- Observed Activity: Ping to google.com
- Example Filter Used: `icmp`

---

## 🔍 Filters Used:
```text
dns
http
tcp
icmp
