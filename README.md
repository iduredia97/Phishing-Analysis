# Phishing Campaign Analysis

##  Overview
This repository documents my analysis of a financially-themed phishing campaign delivering Agent Tesla (aka MSIL/AgentTesla), a .NET-based credential stealer and ransomware.
## 📑 Full Report
For a detailed write-up of the analysis, including methodology, findings, and recommendations:  
👉 [View the full report (PDF)](https://github.com/iduredia97/Phishing-Analysis/blob/main/From-Inbox-to-Intrusion-Unmasking-a-Phishing-Campaign-Delivering-Agent-Tesla%20(1).pdf)


## 🧰 Tools & Techniques
- **Email analysis:** EML parsing, SPF/DKIM checks  
- **Sandboxing:** Kali Linux VM, safe isolated environment  
- **Threat intelligence:** VirusTotal, IP reputation services  
- **Network analysis:** Wireshark (PCAP review, DNS queries)  
- **Report writing:** Professional-style threat intel report (tactical + strategic recommendations)

## 📊 Key Findings
- Attachment `STATEMENT OF ACCOUNT.zip` → Agent Tesla (50/67 AV detection on VirusTotal)  
- Spoofed sender domain `coretek.cn` with SPF authentication failure  
- Malicious infrastructure: `193.42.33.171` (sender IP), `mail.expertsconsultgh.co` (C2), multiple malicious IPs  
- Risks: credential theft, financial fraud, reputational harm, regulatory compliance exposure  

## 🛡️ Recommendations
- Block/Quarantine identified IOCs  
- Enforce DMARC and strengthen email security policies  
- Deploy attachment sandboxing and EDR for endpoints  
- Provide phishing awareness training targeting finance/accounting staff  

## 📂 Repository Contents
- `report/` → Full professional report + recruiter summary + IOCs  
- `analysis/` → Supporting artifacts (headers, hashes, PCAP notes)  
- `images/` → Screenshots and visualizations  

## Portfolio Relevance
This project demonstrates my ability to:
- Perform technical malware and phishing analysis in a safe lab environment  
- Translate raw findings into **business risk language**  
- Produce **professional, recruiter- and stakeholder-ready reporting**  

## Conclusion
The analyzed email attachment represents a significant security threat containing Agent Tesla malware designed for comprehensive data theft and system compromise. The combination of social engineering tactics, established malware infrastructure, and the sender's association with known malicious networks indicates a sophisticated threat actor operation.

Immediate implementation of the recommended blocking and containment measures is critical to prevent further compromise. Organizations should treat this incident as a high-priority security event requiring comprehensive incident response procedures and enhanced monitoring for potential lateral movement or data exfiltration activities.

The presence of this threat highlights the ongoing need for robust email security controls, user education, and comprehensive endpoint protection strategies to defend against evolving malware distribution campaigns.

The exercise demonstrates end-to-end skills in **email header forensics, malware analysis, IOC extraction, and professional incident reporting**.
