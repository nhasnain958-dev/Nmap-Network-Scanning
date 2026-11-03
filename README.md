# Nmap Network Scanning

## Project Overview
This project demonstrates basic network scanning and service detection using Nmap 7.993 on a local Windows computer.

## Objective
- Identify the target IP address.
- Perform a basic Nmap scan.
- Identify open ports.
- Detect available services.
- Perform service and version detection.

## Tools Used
- Nmap 7.993
- Windows 10
- Command Prompt (CMD)
- Notepad

## Target Information
- Target IP: 127.0.0.1
- Hostname: localhost
- Operating System: Windows 10
- Scan Type: Localhost TCP Scan

## Commands Used

### 1. Check Nmap Version
```cmd
nmap --version
```

### 2. Identify IP Address
```cmd
ipconfig
```

### 3. Basic Nmap Scan
```cmd
nmap 127.0.0.1
```

### 4. Service and Version Detection
```cmd
nmap -sV 127.0.0.1
```

### 5. Save Scan Results
```cmd
nmap -sV -oN nmap_results.txt 127.0.0.1
```

## Scan Results

| Port | State | Service | Version / Details |
|---|---|---|---|
| 135 | Open | MSRPC | Microsoft Windows RPC |
| 445 | Open | Microsoft-DS | Unidentified |
| 5357 | Open | HTTP | Microsoft HTTPAPI 2.0 |
| 5432 | Open | PostgreSQL | Unidentified |
| 8000 | Open | HTTP-Alt | Splunkd |
| 8089 | Open | Unknown | Unidentified |
| 8194 | Open | SSL/HTTP | Golang net/http server |

## Findings
- The target host was successfully detected as active.
- Seven open TCP ports were identified.
- Microsoft Windows RPC was detected.
- PostgreSQL database service was detected.
- Splunkd was detected on port 8000.
- Some services could not be fully identified.

## Learning Points
1. Learned IP address identification.
2. Understood basic network scanning.
3. Learned open and closed TCP ports.
4. Practiced service and version detection.
5. Learned to save scan results.

## Screenshots
Screenshots of target IP identification, basic scanning, service detection, and scan results are available in the Screenshots folder.

## Conclusion
This project provided practical experience with Nmap network scanning, open port identification, and service detection on a local Windows computer.

## Disclaimer
This scan was performed on my own local computer for educational purposes only.
