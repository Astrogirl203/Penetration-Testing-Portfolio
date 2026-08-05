# Network Scanning with Nmap

## Objective
Scan my home lab network to find open ports and running services.

## Scan Results

### Machines Scanned
- 192.168.1.100 (Ubuntu Linux)
- 192.168.1.101 (Windows 10)

### Key Findings

**Machine 1: 192.168.1.100**
- Port 22 (SSH) - OPEN
- Port 80 (HTTP) - OPEN
- Port 443 (HTTPS) - OPEN
- Port 3306 (MySQL) - OPEN

**Risk:** MySQL is exposed to network! Should be restricted.

**Machine 2: 192.168.1.101**
- Port 135 (RPC) - OPEN
- Port 139 (NetBIOS) - OPEN
- Port 445 (SMB) - OPEN

**Risk:** SMB allows file sharing - check access controls.

## Commands Used
```bash
nmap -A -p- 192.168.1.100
nmap -sV 192.168.1.0/24
