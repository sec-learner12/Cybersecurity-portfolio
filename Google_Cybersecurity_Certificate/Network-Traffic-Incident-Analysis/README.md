# Network Traffic Incident Analysis

This case study investigates a service outage affecting the website www.yummyrecipesforme.com. 
Customers reported the site was unreachable, and tcpdump analysis revealed repeated 
"UDP port 53 unreachable" ICMP messages. This indicated that DNS requests were not reaching 
the DNS server, suggesting a possible DDoS attack or a misconfiguration blocking DNS traffic.

## Key Skills Demonstrated
- Network traffic analysis using tcpdump
- Identifying DNS and ICMP-related failures
- Recognizing indicators of DDoS activity
- Root cause analysis and incident documentation

## Tools / Concepts Used
- tcpdump
- DNS (UDP port 53)
- ICMP error messages
- Firewall and server health investigation

## Full Report
See the attached PDF in this folder.
