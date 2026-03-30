# Investigation 002 - Nmap Port Scan Detection

## Date
2026-03-30

## Objective
Perform and detect a port scan using Nmap

## Scan Command Used
sudo nmap -sV localhost

## Open Ports Discovered
- 22/tcp - SSH (OpenSSH 10.2p1)
- 8000/tcp - HTTP (Splunkd)
- 8089/tcp - HTTPS (Splunkd)
- 8194/tcp - HTTPS (Golang)

## Screenshot
![Splunk Search] [../screenshots/nmap.png]

## Findings
Four open ports discovered. SSH on port 22 is a common
attack target. In a real environment this information
would help an attacker plan their next move.

## Conclusion
Port scanning is typically the first step in an attack.
Detecting it early in a SOC environment is critical.
