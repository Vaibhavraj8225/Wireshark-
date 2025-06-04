🕵️ Wireshark Network Traffic Analysis
📘 Overview
This project demonstrates how to capture and analyze live network traffic using Wireshark. The goal is to identify key protocols like ICMP, DNS, and TCP by generating traffic and observing how data moves across the network.

🎯 Objective
Capture packets using Wireshark.

Generate traffic using ping 8.8.8.8.

Identify at least 3 network protocols.

Export results and summarize findings.

🛠️ Tools
Wireshark (free, open-source)

Terminal/Command Prompt (for ping command)

📝 Steps
Launch Wireshark and start capturing on the active network interface.

Run ping 8.8.8.8 to create ICMP traffic.

Optionally, browse a website to capture DNS/TCP/HTTP traffic.

Stop the capture after ~1 minute.

Use filters like icmp, dns, or tcp to isolate protocol traffic.

Export the capture as a .pcap file.

Analyze packets and write a short report.

📊 Protocols Observed
ICMP – Used for the ping test.

DNS – Captures domain lookups from browsing.

TCP – Shows connections to websites or services.

📁 Files
ping_8_8_8_8_capture.pcap – Saved packet capture file.

report.md – Summary of identified protocols and packet details.

✅ Outcome
This task helps build foundational skills in network analysis, packet inspection, and understanding how common protocols function at a low level.

