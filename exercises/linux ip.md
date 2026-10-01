Cybersecurity Lab Report: Linux IP Address Identification
**Author:** Abiye Fred
**Course:** OCO
**Date:** 01-10-2026
**Environment:** Kali, Command prompt, VSCode
---
##Table of content
1. Executive summary
2. Objective
3. Scope and Limitation
4. Environment and Tools
5. Methodology
6. Results and Evidence
7. Analysis and Findings 
8. Risk Assessment
9. Recommendations
10. Verification plan
11. Conlusion
12. References
13. Appendices
---
## 1. Cover Page and Metadata
Field	Details
Report title	Identification of a Linux IPv4 Loopback Address
Prepared by	Abiye Fred
Date	1 October 2026
Lab environment	Kali Linux, Visual Studio Code, Command Prompt, GitHub
Address identified	127.0.0.1/8
Report status	Preliminary


## 2. Executive Summary
This report documents the identification of the IP address 127.0.0.1/8 in a Linux lab environment. The address 127.0.0.1 is the commonly used IPv4 loopback address. The 127.0.0.0/8 range is reserved for traffic that loops back within the local host; it does not identify a machine’s ordinary LAN or public Internet address. (RFC 1122, Section 3.2.1.3)
The information provided confirms that the address was identified, but no command output, screenshots, service scans, or other test evidence was supplied. This report therefore makes no claims about open ports, running services, vulnerabilities, or the system’s overall security posture.
## 3. Objectives
- Record the Linux IP address identified during the lab.
- Explain the address and its /8 prefix.
- Document the tools used and the limits of the available evidence.
- Identify next steps if the goal is to find the machine’s network-facing address.
## 4. Scope and Limitations
Scope
This report covers the address 127.0.0.1/8 and its role as an IPv4 loopback address.
Limitations
The following information was not provided:
- The command used to identify the address
- Terminal output or screenshots
- Linux distribution and version
- Date and time of the address discovery
- Any scan results or service observations
No other host, network, service, or application was assessed.
## 5. Environment and Tools
The following tools or environments were reported:
- Kali Linux
- Visual Studio Code
- Windows Command Prompt
- GitHub
The specific role of each tool in identifying the address was not provided.
## 6. Methodology
The report records the address supplied by the user and interprets it using IPv4 addressing conventions and the loopback designation in RFC 1122. No additional testing is represented as having been performed.
For reproducibility, add the command used and its complete output to Appendix A. On Linux, ip address can display addresses assigned to network interfaces.
## 7. Results and Evidence
Finding	Observation	Interpretation
IPv4 address and prefix	127.0.0.1/8	127.0.0.1 is within the 127.0.0.0/8 loopback block.
Evidence provided	Address reported by the user	No terminal output, screenshot, or scan result was supplied.


The loopback block is reserved for host-internal use and does not identify a machine’s ordinary network address. (IETF RFC 5735)
## 8. Analysis
The reported address is consistent with a Linux host’s local loopback interface. Software on the same machine can use this interface to communicate with local services or processes.
The address does not show that the Linux host is reachable by other devices. The /8 prefix describes the loopback block; it does not establish that every address in that block was tested.
## 9. Risk and Impact
Assessment: Informational, based on the available evidence.
Finding a loopback address is expected behavior and is not, on its own, evidence of a vulnerability or security incident. The address alone does not reveal whether local services are listening, how they are configured, or what address the host uses on a LAN.
## 10. Mitigation and Recommendations
- If the objective is to find the Linux machine’s LAN address, inspect the output of ip address and identify the address assigned to the active network interface.
- Do not use 127.0.0.1 as the machine’s LAN address; it refers to the local host.
- Save the command used, its full output, the collection date and time, and a screenshot or text capture as evidence.
- If the lab also requires service assessment, document the authorized target, scope, commands, and results separately.
- Consider whether a public IP address should be included before sharing the report.
## 11. Conclusion
The address provided, 127.0.0.1/8, identifies the IPv4 loopback address and its reserved address block. It does not identify the Linux host’s network-facing IP address. Further conclusions about services or security posture require additional authorized testing and supporting evidence.
## 12. References
1. Special Use IPv4 Addresses.
## 13. Appendices
Appendix A — Evidence
*Command*:
ip addr

Output:
[127.0.0.1/8]
Appendix B — Details to Complete
- *Name*: Abiye Fred
- *Course or lab*: OCO
- *Linux distribution and version*: Kali GNU/Linux
- *Lab objective*: Identify and document the IPv4 address reported by the Linux system
- *Date and time of collection*: 01-10-2026/1:00 pm


