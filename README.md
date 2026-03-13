# Multi-Cloud Deployment & Security Hardening Lab   

A practical graduation project focusing on deploying and securing infrastructure across Microsoft Azure and Amazon Web Services (AWS).

[Screenshots doc]

### 📌 Project Overview   
This project demonstrates the ability to architect, deploy, and secure cloud environments. It includes virtual network configuration, virtual machine hardening, honeypot deployment, and centralized logging.

### 🛠 Tech Stack   
* Cloud Providers: Microsoft Azure, AWS

* Operating Systems: Ubuntu/Windows Server

* Security Tools: Azure Network Security Groups (NSG), AWS Security Groups, Microsoft Sentinel

* Monitoring: Log Analytics Workspace (LAW), Azure Monitor

### 🚀 Key Features   
Part 1: Microsoft Azure

* Network Architecture: Deployed a custom Virtual Network (VNet) with a 10.0.0.0/16 address space and specific subnets.

* Security Hardening: Configured NSGs to restrict management ports (SSH/RDP) to a single administrative IP.

* Honeypot Deployment: Created a sacrificial VM (CNA-Honeypot) running Apache/IIS to monitor potential unauthorized traffic.

* SIEM Integration: Established a Log Analytics Workspace and enabled Microsoft Sentinel for threat detection.

Part 2: Amazon Web Services (AWS)

* Compute Instance: Provisioned EC2 instances t3.micro with public IP accessibility.

* Firewall Configuration: Implemented strict inbound rules within AWS Security Groups.

* Secure Storage: Configured S3 buckets with "Block Public Access" enabled to prevent data leaks.

* Connectivity Testing: Validated network pathing using ping and traceroute.

### 📝 Troubleshooting & Observations
* Logging Challenges: During the Azure phase, the Azure Monitor Agent (AMA) was unavailable in the selected region. I documented multiple onboarding attempts via extensions and portal wizards, showcasing an ability to troubleshoot cloud-native deployment issues.

* Security Validation: Performed "fail-tests" by removing security rules to ensure connectivity was correctly blocked

### 🎓 Certification
This project was completed as part of the CyberNova Academy Graduation Assessment.
