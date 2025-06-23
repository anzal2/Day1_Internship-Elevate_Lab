# Day1_intership-elevate_labs-
DAY 1 – INTERNSHIP
==================

Tasks Performed:
----------------
1. Downloaded Nmap on Linux using the terminal.
2. Performed a TCP SYN Scan on my own IP using:
   Command: nmap -sS 192.168.208.64
3. Discovered open ports:
   - FTP (Port 21)
   - SSH (Port 22)
   - HTTP-Proxy (Port 8080)
4. Captured network packets using Wireshark for analysis.

Service and Port Analysis:
--------------------------

➤ FTP – Port 21
   - Use: Unencrypted file transfers.
   - Risk: High
     • Allows anonymous login
     • Transfers credentials in plaintext
     • Vulnerable to brute-force attacks
   - Recommendation:
     • Disable FTP if not needed
     • Use SFTP (Secure FTP over SSH) as a secure alternative

➤ SSH – Port 22
   - Use: Secure remote login and system administration.
   - Risk: Medium
     • Weak passwords or default credentials
     • Password-based login enabled
     • Service exposed to the internet
   - Recommendation:
     • Use SSH key-based authentication
     • Disable root login
     • Use tools like Fail2Ban to prevent brute-force
     • Optionally change default SSH port

➤ HTTP-Proxy – Port 8080
   - Use: Web applications, development servers, or proxy services.
   - Risk: Varies (High if vulnerable apps are exposed)
     • May expose internal tools
     • Could allow unauthorized access to admin panels
   - Recommendation:
     • Restrict access using firewall rules
     • Secure the application with authentication
     • Keep software up to date

