---
layout: default
---

# Projects

Here are some of the key cybersecurity projects I've worked on:

1. **Python Keylogger with Payload Techniques**  
   Developed a Python-based keylogger with various payload delivery methods, including phishing emails and a USB drop attack. The keylogger captured keystrokes and sent the data via an email server, while employing steganography to hide malicious code in images for added stealth.  
   [Read the full write-up on Medium](https://medium.com/@seiferboado101/exploring-advanced-cybersecurity-techniques-my-keylogger-project-966ce2e310d9)
   [Github Repository](https://github.com/Xei-pher/Python-Keylogger)

2. **Cybersecurity Home Lab**  
   This project documents my journey into creating a home lab, a sandboxed environment for testing cybersecurity tools and techniques. I set up **Metasploitable 2/3 and vulnerable Windows VMs**, alongside **Ubuntu Server** for Blue Team activities and **Kali Linux VM** for offensive security testing. I configured virtual networking, assigned static IPs, and fine-tuned Linux systems for tasks like user management, firewall configuration, and package installations.  
   The lab is a powerful setup for running future projects, simulating attacks, and testing intrusion detection systems. It provided valuable experience in networking fundamentals and Linux administration.  
   [Read the full article on Medium](https://medium.com/@seiferboado101/building-my-first-cybersecurity-home-lab-a-journey-into-networking-linux-configurations-and-cc2ffd9a762b)

3. **DVWA Hacking**  
   A comprehensive exploration of vulnerabilities using the Damn Vulnerable Web Application (DVWA). This project included exploiting various vulnerabilities such as SQL Injection, XSS, and CSRF.
   [Read the full write-up on my Google Docs](https://docs.google.com/document/d/1spQaani_Yim1mr6mZuLNBMtGrXUjybJybZJnKVvWEAg/edit?usp=sharing)

4. **Client Website Monitoring Service with Grafana and Prometheus**  
   Demonstrated blue teaming capabilities by deploying a comprehensive website monitoring service using **Grafana** and **Prometheus**. This service monitored the health of client websites when I was an intern in SHIELD Foundry, checked SSL certificate expiry, tracked uptime status, and alerted for any issues. Deployed using **Docker** and **Docker Compose** for containerization. This solution ensured real-time observability and proactive website maintenance.

5. **OWASP Juice Shop Hacking**  
   Ethical hacking challenges with OWASP Juice Shop, identifying security vulnerabilities in an intentionally vulnerable web app.
   [Read the full write-up on my Google Docs](https://docs.google.com/document/d/1QjhROyB7c9D9RwvVYzOvMfIyITKEc47xMU5rteW5kMc/edit?usp=sharing)

6. **Wireshark Malware Analysis of OskiStealer**  
   In this project, I analyzed network traffic to identify indicators of compromise (IoCs) for the **OskiStealer** malware. Using **Wireshark**, I examined HTTP traffic from an infected host, and with tools like **VirusTotal** and **MalwareBazaar**, I uncovered how the malware exfiltrates data while evading detection. I also utilized **steganography** techniques and forensic analysis to investigate the malware’s behavior on the system.  
   [Read the full article on Medium](https://medium.com/@seiferboado101/from-network-packets-to-malware-insights-analyzing-oskistealer-through-forensics-7f7a97191a08)

7. **Building a SIEM with Azure Sentinel**  
   Developed a **Security Information and Event Management (SIEM)** system using **Microsoft Azure Sentinel**. The project involved setting up log collection, threat detection, and dashboards for real-time monitoring of Windows devices. I configured custom analytics rules and visualizations for tracking security events and potential threats, gaining hands-on experience in cloud security and incident response.  
   [Read the full article on Medium](https://medium.com/@seiferboado101/building-a-siem-with-threat-intelligence-using-microsoft-azure-sentinel-39f9c4ece87a)

8. **Enhancing Security with OSSEC: Comprehensive Setup and Testing**  
   Set up **OSSEC** as a host-based intrusion detection system (HIDS) in a virtualized environment. The project involved configuring the OSSEC server and Web UI on an Ubuntu VM, linking it to a Windows 10 VM agent, and simulating attacks from a Kali Linux VM to validate OSSEC’s detection capabilities. Successfully detected and logged simulated attacks such as those using **Metasploit** and **EternalBlue** exploits.  
   [Read the full article on Medium](https://medium.com/@seiferboado101/enhancing-security-with-ossec-a-comprehensive-setup-and-testing-guide-f92822f287df)

[Back to About Me](./index.md)
