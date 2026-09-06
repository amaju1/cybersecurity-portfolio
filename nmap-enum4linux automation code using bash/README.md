
Automated Network Reconnaissance with Bash

Overview

This project is a Bash-based network reconnaissance script that automates initial host and service enumeration using Nmap and Enum4linux.

The script first performs an Nmap scan to identify open ports. If SMB port 445 is detected as open, it automatically runs Enum4linux to perform additional SMB enumeration.

Workflow

Target IP
   ↓
Nmap Port Scan
   ↓
Identify Open Ports
   ↓
Is Port 445 Open?
   ↓
 ┌───────────────┐
 │      Yes      │ → Run Enum4linux SMB Enumeration
 └───────────────┘
        ↓
   Save/Review Results

Tools Used

* Bash – Automation and scripting
* Nmap – Network and port scanning
* Enum4linux – SMB/Windows network enumeration
* Kali Linux – Testing environment

Features

* Accepts a target IP address.
* Automates Nmap scanning.
* Detects open network ports.
* Checks specifically for SMB port 445.
* Automatically launches Enum4linux when SMB is detected.
* Reduces repetitive manual enumeration tasks.

Example Workflow

./recon.sh <target-ip>

The script performs the Nmap scan and, when port 445 is open, proceeds with SMB enumeration using Enum4linux.

Skills Demonstrated

* Bash scripting
* Security automation
* Network reconnaissance
* Port and service enumeration
* SMB enumeration
* Conditional scripting
* Linux command-line usage
* Penetration-testing workflow automation

Disclaimer

This script was developed and tested in an authorized cybersecurity lab environment. It should only be used against systems for which you have explicit permission to perform security testing.
