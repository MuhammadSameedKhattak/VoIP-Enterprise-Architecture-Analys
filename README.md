# Enterprise VoIP Architecture & Traffic Analysis

📌 **Project Overview**
Designed and deployed a Cisco Call Manager Express (CME) environment to establish intra-network SIP routing. Conducted live packet analysis on an Ubuntu machine to verify Layer 7 signaling and Layer 4 RTP media streams, ensuring optimal network health parameters (latency, jitter, and packet loss) for enterprise voice traffic.

🏗️ **Topology & Infrastructure (Packet Tracer)**
![Packet Tracer Topology](put-your-packet-tracer-filename-here.png)
* Configured Voice VLANs to separate telephony traffic from standard data.
* Deployed DHCP pools with Option 150 to direct endpoints to the TFTP server.
* Configured Layer 3 Dial-Peers to establish call routing between extensions.

🔍 **Live Traffic Analysis (Wireshark)**
![SIP Signaling Analysis](put-your-wireshark-sip-filename-here.png)
* Captured and analyzed live SIP signaling, verifying the 3-way handshake (`INVITE`, `200 OK`, `ACK`) and graceful session teardown. 
* Monitored RTP UDP streams to confirm zero packet loss and acceptable jitter thresholds, simulating standard NOC troubleshooting procedures for degraded audio issues.
