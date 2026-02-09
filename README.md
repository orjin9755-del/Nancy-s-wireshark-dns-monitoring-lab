# Nancy's wireshark-dns-monitoring-lab Very basic DNS traffic analysis using Wireshark (SOC & GRC perspective).

# Wireshark DNS Monitoring Lab

## Overview
This lab demonstrates basic DNS traffic analysis using Wireshark. The objective is to observe normal network behavior, understand DNS queries, and relate network monitoring activities to SOC operations and GRC controls.



## Tools Used
- Kali Linux (VMware)
- Wireshark



## Lab Objectives
- Capture live network traffic
- Filter and analyze DNS packets
- Identify normal DNS behavior
- Understand how DNS monitoring supports security controls



## Procedure

1. Launched Kali Linux in VMware.
2. Opened Wireshark and selected the active network interface.
3. Started packet capture.
4. Generated normal traffic by visiting common websites.
5. Applied DNS filter (`dns`) to isolate DNS traffic.
6. Observed DNS queries and responses.



## Observations
- DNS queries were made to legitimate and recognizable domains such as search engines and informational websites (mozilla firefox, google.com)
- Traffic used UDP port 53, which is standard for DNS.
- No suspicious or anomalous domain names were observed during the capture.



## SOC Perspective
From a Security Operations (SOC) perspective, DNS traffic analysis helps:
- Detect suspicious or malicious domain communication
- Establish a baseline of normal network behavior
- Support incident detection and investigation



## GRC Perspective
From a Governance, Risk, and Compliance (GRC) perspective:
- DNS monitoring serves as a detective control.
- Packet capture logs act as evidence of monitoring activities.
- Continuous monitoring reduces the risk of undetected malicious communication.



## Risk Consideration
If DNS traffic is not monitored, malicious domains may be accessed without detection, potentially leading to data exfiltration or malware communication.



## Conclusion
This lab demonstrates how basic network monitoring contributes to both technical security operations and organizational risk management.
