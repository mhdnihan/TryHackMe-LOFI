# TryHackMe-LOFI
A practical walkthrough of network enumeration and path traversal exploitation in the TryhackMe Lo-Fi room

TryHackMe – Lo-Fi

Overview

Completed the Lo-Fi room on TryHackMe, focusing on network enumeration and identifying a Path Traversal vulnerability in a web application.

The objective was to enumerate the target, investigate the web service, identify the vulnerability, and retrieve the root flag.

Tools Used

* Nmap – Network and port enumeration
* Web Browser – Web application inspection
* Linux Terminal – Command-line interaction

Methodology

1. Network Enumeration

* Started by scanning the target machine using Nmap.
* Identified open ports and the services running on them.
* Found an accessible HTTP service and proceeded with web application enumeration.

2. Web Application Enumeration

* Accessed the HTTP service through a browser.
* Inspected the application and examined its URL structure.
* Identified a potential file path manipulation vulnerability.

3. Path Traversal Exploitation

* Tested the URL for directory traversal.
* Manipulated the file path to access files outside the intended web directory.
* Successfully accessed the root.txt file and retrieved the root flag.

Vulnerability Identified

Path Traversal (Directory Traversal)

Path Traversal is a vulnerability that occurs when an application does not properly validate user-controlled file paths. An attacker may manipulate file paths using sequences such as ../ to access files outside the intended directory.

Impact

* Unauthorized access to sensitive files.
* Exposure of system information.
* Potential disclosure of configuration files and credentials.

Key Takeaways

* Practiced network reconnaissance using Nmap.
* Improved web application enumeration skills.
* Understood how path traversal vulnerabilities work.
* Learned how improper file path validation can expose sensitive system files.

