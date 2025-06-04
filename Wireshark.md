Capture and Analyze Network Traffic Using Wireshark
Objective
Capture live network packets and identify basic protocols and traffic types using Wireshark.
________________________________________
Tools Used
•	Wireshark – Network protocol analyzer (https://www.wireshark.org/)
________________________________________
Steps Taken
1. Wireshark Installation
Wireshark was downloaded and installed from the official website.
![Image](https://github.com/user-attachments/assets/2b328524-38e1-4ab1-af3b-a7ec07ea187e)
________________________________________
2. Capture Setup
•	Launched Wireshark.
•	Selected the active network interface (e.g., Ethernet or Wi-Fi) to begin capture.
![Image](https://github.com/user-attachments/assets/8b41f92b-1814-40a1-bd35-8006a72d8383)
________________________________________
3. Traffic Generation
To generate network traffic:
•	Opened a terminal or command prompt.
•	Executed the following command:
ping 8.8.8.8
This created ICMP packets (ping).
![Image](https://github.com/user-attachments/assets/d5a19233-c8eb-407f-b220-325392324cd2)
________________________________________
4. Capture Duration
•	Let the capture run for about 1 minute while pinging.
•	Then stopped the capture using the red square “Stop” button in Wireshark.
![Image](https://github.com/user-attachments/assets/28f8e26b-1c0a-4d4e-a572-30d184e8a24e)
________________________________________
5. Filtering Protocols
Used the following filters in Wireshark to identify traffic:
•	icmp – for ping requests/replies.
•	dns – for domain name resolution traffic.
•	http – for web browsing (if applicable).
•	tcp and udp – transport layer protocols.
![Image](https://github.com/user-attachments/assets/18509e7c-1001-4ec6-a190-6e4fec2b5846)
________________________________________
6. Protocols Identified
Protocol	Description	Details
ICMP	Internet Control Message Protocol	Used by the ping command to test connectivity.
DNS	Domain Name System	Translates domain names to IP addresses.
TCP	Transmission Control Protocol	Reliable, connection-oriented protocol used by HTTP/HTTPS.
![Image](https://github.com/user-attachments/assets/e06e3fec-bfbd-414d-a6cc-f25a2c924455)
________________________________________
7. Export Capture
The capture was exported as a .pcap file:
File name: ping_8_8_8_8_capture.pcap
![Image](https://github.com/user-attachments/assets/fb8c3ea4-36d4-429f-b672-01caf1f4a15e)
________________________________________
8. Summary of Findings
•	The ICMP packets showed the request and reply from 8.8.8.8 (Google DNS).
•	DNS queries occurred when browsing or accessing websites.
•	TCP traffic was observed during browser activities.
Sample Packet Details (ICMP)
•	Source IP: 192.168.1.x (local machine)
•	Destination IP: 8.8.8.8
•	Type: Echo (ping) request and reply
•	Size: ~74 bytes per ICMP packet
![Image](https://github.com/user-attachments/assets/006db986-67d6-44b0-a14c-059f223531e5)
________________________________________
Conclusion
This exercise provided hands-on experience with capturing and analyzing network traffic using Wireshark. The ping to 8.8.8.8 successfully generated ICMP packets, and other basic protocols such as DNS and TCP were also identified.

