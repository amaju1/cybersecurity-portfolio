
DVWA Stored XSS & BeEF Browser Exploitation Lab

Overview

This project demonstrates the security impact of a Stored Cross-Site Scripting (XSS) vulnerability using Damn Vulnerable Web Application (DVWA) and the Browser Exploitation Framework (BeEF) in an isolated lab environment.

A BeEF hook was injected through DVWA’s Stored XSS functionality. After the vulnerable browser was successfully hooked, BeEF was used to demonstrate browser manipulation by changing the hooked browser’s displayed page to a simulated Google email login page.

Lab Environment

* Attacker: Kali Linux
* Target Application: DVWA
* Browser Exploitation Framework: BeEF
* Virtualization: VirtualBox
* Network: Isolated laboratory environment

Methodology

1. Configured DVWA in an isolated testing environment.
2. Identified the Stored XSS functionality within DVWA.
3. Injected a BeEF hook through the vulnerable input field.
4. Accessed the affected page using a separate page.
5. Confirmed that the website page appeared as a hooked client within BeEF.
6. Used BeEF to demonstrate browser-side manipulation.
7. Replaced the displayed page with a simulated Google email login page.
8. Documented the results and security implications.

Result

The Stored XSS vulnerability successfully allowed the injected JavaScript to execute in the victim browser context.

After the browser was hooked, BeEF demonstrated that an attacker could interact with and manipulate the browser environment. The simulated email login page illustrated how browser compromise could potentially be used for social-engineering and phishing scenarios.

Result: Successful lab demonstration ✅

Security Impact

Stored XSS can allow malicious JavaScript to execute whenever users access a compromised page. Depending on the application’s security controls and the victim’s browser context, this can potentially lead to:

* Website session manipulation
* Unauthorized browser actions
* Phishing and social-engineering attacks
* Theft of sensitive information in vulnerable scenarios
* Further browser-based exploitation

Mitigation

Developers can reduce Stored XSS risk by implementing:

* Strict input validation where appropriate
* Context-aware output encoding
* Content Security Policy (CSP)
* Secure cookie attributes such as HttpOnly and SameSite
* Avoiding unsafe handling of user-supplied HTML/JavaScript
* Regular security testing and code review

Skills Demonstrated

* Stored XSS identification and exploitation
* JavaScript injection
* BeEF framework usage
* Web application security assessment
* Understanding of client-side attack techniques
* Security impact analysis
* Penetration-testing documentation

Disclaimer

This project was performed exclusively in an authorized, isolated cybersecurity laboratory using DVWA, an intentionally vulnerable application.

The phishing page used in the demonstration was simulated for educational purposes and was not used to collect real credentials or target real users.
