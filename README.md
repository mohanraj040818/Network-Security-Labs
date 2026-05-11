# Nmap Network Scanning & Security Analysis
This repository contains a comprehensive analysis of network scanning phases conducted as part of my Cybersecurity studies at UNISEL.  
Project Overview
The objective was to perform various scanning techniques on a target host (10.11.15.11) to identify active services and determine the operating system through fingerprinting.  
Key Scanning TasksHost Discovery: 
Successfully identified live hosts on the target network with low latency (0.0060s).  
SYN Stealth Scan (-sS): Performed half-open scans to identify open ports (135, 139, 445, 2869) while remaining difficult for basic security systems to detect.  
TCP Connect Scan (-sT): Completed full three-way handshakes to confirm service availability.  
Xmas & FIN Scans: Analyzed how the Windows TCP/IP stack responds to non-standard flag combinations for the purpose of OS Fingerprinting.  
Service & OS Detection: Confirmed the target was running Microsoft Windows 11 24H2 and identified specific versions of active services like icslap and netbios-ssn.  
Reflection & ComparisonReliability: The Full Connect Scan is the most reliable but easiest to detect by administrators.  
Efficiency: The SYN Scan is the most useful tool for cybersecurity assessments as it provides a fast, accurate map of open ports without high overhead.  
Deep Defense: Service/OS detection is critical for identifying specific patch levels and known vulnerabilities.  
