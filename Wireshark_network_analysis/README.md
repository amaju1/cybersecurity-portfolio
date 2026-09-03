Wireshark Credential Sniffing Lab

Overview

A cybersecurity lab demonstrating how credentials can be exposed when transmitted over an insecure protocol.

Lab Environment

* Kali Linux – penetration testing and analysis
* Metasploitable 2 – vulnerable target
* Wireshark – packet capture and analysis
* VirtualBox – virtual lab environment

What I Did

1. Exploited a vulnerable service on Metasploitable 2 called telnet
2. Started a Wireshark packet capture.
3. Logged into the target service while capturing traffic.
4. Analyzed the packets to identify the transmitted login credentials.
5. Demonstrated the security risk of plaintext authentication.

Key Finding

The login credentials were visible within the captured network traffic because the authentication protocol did not properly encrypt the credentials.

Mitigation

Use encrypted protocols such as HTTPS, SSH, and TLS, and avoid plaintext authentication protocols.

Ethical Notice: This exercise was performed exclusively in my own isolated virtual lab for educational purposes.
