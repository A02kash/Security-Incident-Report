# Security-Incident-Report

This project centered on an exhaustive analysis of DNS and ICMP traffic in transit, leveraging data extracted from the `tcpdump` utility. The primary focus was identifying and addressing the `UDP Port 53 Unreachable` issue encountered within the network infrastructure.

## Scenario

### Incident Description

You are a cybersecurity analyst at a company specializing in IT consultant services. Several customers contacted your company reporting their inability to access the company website [`Yummy Recipes for Me`](https://www.yummyrecipesforme.com/). They encountered the error message “destination port unreachable” after waiting for the page to load. You are tasked with analyzing the situation and determining which network protocol was affected during this incident. 

### `tcpdump` log file
![image](https://github.com/A02kash/Security-Incident-Report/assets/131836019/afe94a45-ffe2-4b5c-b63b-4dd5b30e6c13)

### Investigative Steps Taken

1. **Initial Report Reception:** Noted multiple customer complaints regarding website inaccessibility.
2. **Error Observation:** Identified the error message `destination port unreachable` during attempted access to the website.
3. **Packet Analysis:** Initiated packet sniffing tests using `tcpdump` to delve into the network traffic.
4. **Findings:** Discovered the root issue pointing to the unavailability of UDP Port 53, the standard DNS port.
5. **Hypotheses:** Suspected misconfigurations within the firewall or a potential DoS attack targeting the DNS server.

### Next Steps and Resolution

- **Immediate Action:** Engaging the Network Security team to comprehensively investigate firewall configurations.
- **DNS Server Assessment:** Verification and analysis of the DNS server's operational status post-suspected attack.
- **Mitigation Strategy:** Implementing measures to rectify firewall misconfigurations and fortify against possible DoS attacks.

## License

> This project is licensed under [`Google Cybersecurity Professional Certificate`](https://www.coursera.org/professional-certificates/google-cybersecurity?isNewUser=true#testimonials).
