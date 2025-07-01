# Task5-Elevate-Labs

# 📡 Task 5: Capture and Analyze Network Traffic Using Wireshark

## 🎯 Objective
To capture live network traffic using Wireshark and analyze basic protocols such as ICMP, DNS, TCP, HTTP, and TLS.

---

## 🛠 Tools Used
- 🐧 **Kali Linux**
- 🧪 **Wireshark** (GUI network packet analyzer)
- 💻 **Linux Terminal** (for generating traffic via `ping` and browsing)

---

## ✅ Steps Performed

1. Opened **Wireshark** and selected the active network interface (`wlan0`).
2. Started packet capture and:
   - Used `ping google.com` to generate ICMP packets.
   - Opened websites to trigger DNS, HTTP, and TLS traffic.
3. Stopped the capture after ~30 seconds.
4. Applied filters like `icmp`, `dns`, `tcp`, and `http` to analyze packet details.
5. Saved the capture as `packets.pcapng`.
6. Took multiple screenshots highlighting key packets and protocol data.

---

## 🔍 Protocols Identified

| Protocol   | Description                                                                 |
|------------|-----------------------------------------------------------------------------|
| **ICMP**   | Internet Control Message Protocol used by `ping` for connectivity checks.   |
| **DNS**    | Domain Name System queries and responses for hostname resolution.           |
| **TCP**    | Transmission Control Protocol used for reliable connections (e.g., HTTP/HTTPS). |
| **HTTP**   | Unencrypted web traffic with visible `GET` and `200 OK` headers.            |
| **TLSv1.3**| Encrypted HTTPS communication protocol, part of the secure browsing process.|

---

## 📷 Screenshots

### 🖼 ICMP (Ping) Traffic
![ICMP Screenshot](screenshots/Screenshot_2025-07-01_09_07_49.png)  
Captured ICMP echo replies from `ping google.com` showing round-trip times and IPv6 addresses.

---

### 🖼 DNS Query & Response
![DNS Screenshot](screenshots/Screenshot_2025-07-01_09_06_21.png)  
Captured DNS query and response for resolving the domain `www.squadhelp.com`.

---

### 🖼 TCP and TLS Handshake
![TLS Screenshot](screenshots/Screenshot_2025-07-01_09_06_05.png)  
Captured TCP handshake (`SYN`, `ACK`) and encrypted TLSv1.3 session initialization packets.

---

### 🖼 HTTP GET Request
![HTTP Screenshot](screenshots/Screenshot_2025-07-01_09_05_50.png)  
Captured a plaintext HTTP/1.1 `GET` request and a `200 OK` response showing response headers.

---

## 📌 Learning Outcome

- Learned to capture and analyze real-time network traffic.
- Gained hands-on exposure to core internet protocols.
- Understood how to filter and interpret packets in Wireshark.
- Recognized the differences between plaintext and encrypted traffic.
