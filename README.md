# CyberFlux
### See the Flow. Decode the Network.

**CyberFlux** is a Python-based network traffic monitoring and packet analysis tool that captures live network packets and analyzes communication between devices. It extracts useful packet information such as source IP, destination IP, protocol, ports, packet size, timestamp, and payload representation.

Built using **Python and Scapy**, CyberFlux helps users understand network communication, inspect traffic patterns, and explore packet-level networking concepts.

---

## Overview

Network communication happens through packets that carry data between devices. CyberFlux captures these packets and converts their technical details into a readable format, making network traffic easier to observe and analyze.

## Features

- **Live Packet Capture** — Capture network packets in real time.
- **IP Address Analysis** — Identify source and destination IP addresses.
- **Protocol Detection** — Identify TCP, UDP, ICMP, and other protocols.
- **Port Inspection** — Extract source and destination ports when available.
- **Packet Size Monitoring** — Measure the size of captured packets.
- **Payload Inspection** — Display payload data in hexadecimal representation.
- **Timestamp Tracking** — Record when packets are captured.
- **CSV Logging** — Save packet information for further analysis.
- **Lightweight & Simple** — Built with Python and Scapy.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Scapy | Packet capture and analysis |
| CSV | Store captured packet information |
| Npcap | Windows packet capture support |

## Project Structure

\`\`\`text
CyberFlux/
│
├── main.py
├── requirements.txt
├── README.md
│
└── logs/
    └── packets.csv
\`\`\`

## Installation

### 1. Clone the repository

\`\`\`bash
git clone https://github.com/your-username/CyberFlux.git
cd CyberFlux
\`\`\`

### 2. Install dependencies

\`\`\`bash
pip install -r requirements.txt
\`\`\`

### 3. Install Npcap (Windows)

Windows users may need Npcap to enable live packet capture.

Download it from:

https://npcap.com/

### 4. Run CyberFlux

Run your terminal with the required network capture permissions, then execute:

\`\`\`bash
python main.py
\`\`\`

The program will begin capturing packets. Press **Ctrl + C** to stop the capture.

## Sample Output

\`\`\`text
=============================================================
                  CYBERFLUX
           Network Traffic Analyzer
=============================================================

Packet Number : 1
Timestamp    : 16:30:15
Source IP   : 192.168.1.10
Destination  : 142.250.183.14
Protocol     : TCP
Source Port  : 51234
Dest Port   : 443
Packet Size  : 74 bytes
Payload     : Hexadecimal Data
\`\`\`

## Packet Information

CyberFlux analyzes the following information from captured packets:

| Field | Description |
|---|---|
| Timestamp | Capture time of the packet |
| Source IP | IP address sending the packet |
| Destination IP | IP address receiving the packet |
| Protocol | Communication protocol |
| Source Port | Sender's port number, if applicable |
| Destination Port | Receiver's port number, if applicable |
| Packet Size | Total packet size in bytes |
| Payload | Packet payload represented in hexadecimal |

## How It Works

1. CyberFlux listens on a network interface.
2. Scapy captures packets passing through the monitored interface.
3. The application analyzes packet headers and identifies protocols.
4. Relevant packet details are extracted.
5. Packet information is displayed in the terminal.
6. Captured information is stored in a CSV log file.

## Future Improvements

- Graphical user interface (GUI)
- Real-time traffic statistics and graphs
- Protocol-based packet filtering
- IP address filtering
- Packet search and analysis
- Network traffic visualization
- Capture start/stop controls
- Export and reporting features
- Basic suspicious traffic indicators

## Security & Ethical Use

CyberFlux is intended for educational purposes, network troubleshooting, and authorized network monitoring.

- Capture traffic only on networks you own or have permission to monitor.
- Packet capture may require administrator/root privileges.
- Encrypted traffic, such as HTTPS, cannot generally be decrypted by packet capture alone.
- Avoid collecting, storing, or exposing sensitive network data.

## Author

**Developer:** Pushkar Singh

## License

This project is intended for educational and research purposes. Licensing details can be added as the project evolves.

---

> **CyberFlux — See the Flow. Decode the Network.**
