# Nmap Cheat Sheet

Nmap is a powerful tool for network discovery and security auditing. 

## Basics

!nmap {IP}


Copy code
**Example**: `!nmap 192.168.1.1`

Scans the specified IP address. Replace `{IP}` with the IP address you want to scan.

## Scan Types

!nmap -sS {IP}


Copy code
**Example**: `!nmap -sS 192.168.1.1`

Performs a SYN scan. It's fast and unobtrusive.

!nmap -sT {IP}


Copy code
**Example**: `!nmap -sT 192.168.1.1`

Performs a TCP connect scan. It's slower but more thorough.

## Port Scanning

!nmap -p {port} {IP}


Copy code
**Example**: `!nmap -p 22 192.168.1.1`

Scans a specific port on the IP address. Replace `{port}` with the port number you want to scan.

## Service Detection

!nmap -sV {IP}


Copy code
**Example**: `!nmap -sV 192.168.1.1`

Detects the services running on the IP address.

## OS Detection

!nmap -O {IP}


Copy code
**Example**: `!nmap -O 192.168.1.1`

Attempts to detect the operating system running on the IP address.

> Note: Always use Nmap responsibly and only scan networks and systems you have permission to scan.