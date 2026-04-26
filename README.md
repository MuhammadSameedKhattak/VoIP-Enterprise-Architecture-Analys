# Enterprise VoIP Architecture & Traffic Analysis

📌 **Project Overview**
Designed and deployed a Cisco Call Manager Express (CME) environment to establish intra-network SIP routing. Conducted live packet analysis on an Ubuntu machine to verify Layer 7 signaling and Layer 4 RTP media streams, ensuring optimal network health parameters (latency, jitter, and packet loss) for enterprise voice traffic.

---

🏗️ **Topology & Infrastructure (Packet Tracer)**

![Packet Tracer Topology](your-topology-image-name.png)

* **Infrastructure**: Built using a Cisco 2811 Router (CME) and 2960 Switch.
* **Voice VLANs**: Configured to separate telephony traffic from standard data.
* **DHCP Option 150**: Deployed to direct endpoints to the TFTP server for configuration.
* **Dial-Peers**: Configured Layer 3 routing between extensions 1001 and 1002.

![Phones Connected](your-connected-phones-image-name.png)
*Visual confirmation of successful registration and active call connection.*

---

🔍 **Live Traffic Analysis (Wireshark)**

![SIP Signaling Analysis](your-wireshark-image-name.png)

* **SIP Handshake**: Captured and analyzed live signaling on Ubuntu loopback interface.
* **Protocol Flow**: Verified the sequence of `INVITE`, `180 Ringing`, and `CANCEL` teardown.
* **NOC Troubleshooting**: Demonstrates the ability to diagnose call setup failures at the packet level.
