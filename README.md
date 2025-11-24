# basic-nmap-risk-assessment
Network Security Assessment: Basic Nmap Scanning & Risk Analysis

This  project demonstrates a fundamental cybersecurity workflow: performing network reconnaissance using Nmap and conducting risk analysis. It bridges technical penetration testing skills with Governance, Risk, and Compliance (GRC) principles.

Target: Home Network (10.45.37.x)
Scanner:Kali Linux VM
Target Host: Windows 11 Physical Machine

Objectives
- Perform network discovery and service enumeration
- Identify potential security risks
- Document findings in a professional risk assessment report
- Demonstrate understanding of both technical and analytical cybersecurity skills

Tools Used
- Nmap (Network Mapper) 7.94
- Kali Linux (VirtualBox VM)
- Windows 11 (Target Host)
- Git & GitHub (Documentation)

Images that shows example of Nmap Command execution in Kali Linux  and windows network interface identified prior to scanning are attactched.
 Scanning Process
1. Host Discovery: `nmap -sn 10.45.37.0/24`
2.Service Enumeration: `nmap -sS -sV 10.45.37.xxx`
3. Vulnerability Assessment: `nmap -sC 10.45.37.xxx`


 Key Findings
- Open Ports: 135, 139, 445,1055,2179,3306
-Services Identified: RPC, NetBIOS, SMB,mysql, flexlm
- Risk Level: Medium
- Primary Concern: SMB service exposure, outdated service versions

Report
Comprehensive risk analysis available in: [RISK_ASSESSMENT_REPORT.md](RISK_ASSESSMENT_REPORT.md)

How to Reproduce
1. Ensure you have permission to scan the target network
2. Set up Kali Linux in bridged networking mode
3. Identify target IP using `ipconfig` on Windows
4. Run Nmap scans as documented in the report
5. Analyze results and document findings

Disclaimer
This assessment was conducted on a **private, owned home network**. Unauthorized scanning of networks is illegal and unethical. Always obtain explicit permission before conducting any security assessment.

