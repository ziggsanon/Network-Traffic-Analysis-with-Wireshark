# Network-Traffic-Analysis-with-Wireshark 
Analyzing network traffic using Wireshark with a focus on SMTP PCAPs.
# Wireshark Network Traffic Analysis: SMTP PCAP (Still in progress)

## Project Overview

In this project, I performed a **network traffic analysis** using **Wireshark**, focusing on **SMTP** (Simple Mail Transfer Protocol) traffic. The analysis involves **decoding base64 data**, examining **SMTP commands**, and mapping key findings to the **MITRE ATT&CK** framework to identify potential security risks and attack vectors.

## Objective

- Analyze **SMTP traffic** captured in a **PCAP file**.
- Decode **base64-encoded data** to extract sensitive information.
- Investigate **SMTP commands** and email headers to identify security risks.
- **Map findings** to the **MITRE ATT&CK** framework for better understanding of potential vulnerabilities.

## Methodology

1. **Wireshark Setup**: Loaded the PCAP file into Wireshark and filtered SMTP traffic using the `smtp` filter.
2. **Base64 Decoding**: Identified and decoded base64-encoded content, including usernames and passwords.
3. **SMTP Command Analysis**: Analyzed SMTP commands like `EHLO`, `AUTH`, `MAIL FROM`, and `RCPT TO` to identify suspicious activity.
4. **MITRE ATT&CK Mapping**: Mapped the captured traffic to MITRE ATT&CK tactics such as **Credential Dumping** and **Phishing** to assess potential vulnerabilities.

## Example Analysis

### SMTP Command Exchange:

Captured SMTP commands, including authentication and email data:




## MITRE ATT&CK Mapping

This analysis maps the SMTP traffic to several MITRE ATT&CK techniques:

- **T1071**: Application Layer Protocol - SMTP.
- **T1071.001**: Application Layer Protocol: Web Protocols - Email-based phishing.
- **T1110**: Brute Force (if brute force is attempted during authentication).

## Tools Used

- **Wireshark**: For capturing and analyzing network traffic.
- **Base64 Decoding Tool**: For decoding encoded data.
- **MITRE ATT&CK Framework**: For mapping captured actions to known attack techniques.

## Conclusion

This project demonstrates how **SMTP traffic analysis** can uncover critical vulnerabilities, such as **credential theft** and **phishing attempts**. By mapping findings to the **MITRE ATT&CK framework**, we can understand attack tactics and strengthen security posture.

## Next Steps

- Perform additional **network traffic analysis** on different protocols to explore broader attack surfaces.
- Integrate automated tools for detecting **email-based threats** in enterprise environments.
- Continue to update this project with new findings and insights.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

