

DESCRIPTION:

This project is a Python-based Penetration Testing Toolkit designed to assist ethical hackers and security testers by offering multiple basic penetration testing modules in a single script. It uses core libraries like socket, requests, paramiko, and argparse.

Features:
Port Scanner
Scans common ports (21, 22, 25, 80, 443, 3306) on the specified target IP or domain to identify open services.

SSH Brute-Forcer
Performs brute-force attacks against SSH servers using a given username and a password wordlist file. Built using paramiko for secure SSH handling.

Vulnerability Scanner
Tests for basic SQL Injection and Cross-Site Scripting (XSS) vulnerabilities by injecting payloads into a URL and checking for reflections.

Usage:
You can run the toolkit using various options:


python toolkit.py -p <target_ip>      # Port Scan
python toolkit.py -b <target> <username> <wordlist.txt>   # SSH Brute Force
python toolkit.py -v <url>             # Vulnerability Scan
Libraries Used:
socket for network connections (port scanning)

paramiko for SSH login attempts

requests for web vulnerability scanning

argparse for modular command-line interaction

Important Points:
Simple, Lightweight: No heavy libraries needed — only standard and widely-used ones.

Modular Design: Each tool (scanner/brute-forcer/vuln-scanner) is a separate function for easier maintenance.

Extensible: You can add new modules (like FTP brute-force, web directory brute-force, etc.) easily by following the same structure.

OUTPUT:


![Image](https://github.com/user-attachments/assets/6cfa38ad-b9ec-4b01-8fc4-fedf3f7c7a40)
