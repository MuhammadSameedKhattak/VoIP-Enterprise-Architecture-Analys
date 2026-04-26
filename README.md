ni# Enterprise VoIP Architecture & Traffic Analysis

📌 **Project Overview**
Designed and deployed a Cisco Call Manager Express (CME) environment to establish intra-network SIP routing. Conducted live packet analysis on an Ubuntu machine to verify Layer 7 signaling and Layer 4 RTP media streams, ensuring optimal network health parameters (latency, jitter, and packet loss) for enterprise voice traffic.

---

🏗️ **Topology & Infrastructure (Packet Tracer)**

![Packet Tracer Topology](https://github.com/MuhammadSameedKhattak/VoIP-Enterprise-Architecture-Analys/blob/main/Screenshot%20from%202026-04-26%2005-21-12.png?raw=true.png)

* **Infrastructure**: Built using a Cisco 2811 Router (CME) and 2960 Switch.
* **Voice VLANs**: Configured to separate telephony traffic from standard data.
* **DHCP Option 150**: Deployed to direct endpoints to the TFTP server for configuration.
* **Dial-Peers**: Configured Layer 3 routing between extensions 1001 and 1002.

![Phones Connected](https://github.com/MuhammadSameedKhattak/VoIP-Enterprise-Architecture-Analys/blob/main/Screenshot%20from%202026-04-26%2004-45-44.png?raw=true.png)
*Visual confirmation of successful registration and active call connection.*

---

🔍 **Live Traffic Analysis (Wireshark)**

![SIP Signaling Analysis](https://github.com/MuhammadSameedKhattak/VoIP-Enterprise-Architecture-Analys/blob/main/Screenshot%20from%202026-04-26%2005-24-10.png?raw=true.png)

* **SIP Handshake**: Captured and analyzed live signaling on Ubuntu loopback interface.
* **Protocol Flow**: Verified the sequence of `INVITE`, `180 Ringing`, and `CANCEL` teardown.
* **Troubleshooting**: Demonstrates the ability to diagnose call setup failures at the packet level.
