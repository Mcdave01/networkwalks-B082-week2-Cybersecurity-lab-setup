
# B082 Week 2 — Penetration Testing Report

**Name:** Atanda Oluwagbenga  
**Batch:** B082-Week2  
**Week:** 2

## Overview
This repository contains my Week 2 cybersecurity practical report covering reconnaissance, footprinting, DNS enumeration, web technology fingerprinting, HTTP header inspection, and network discovery using Kali Linux tools.

## Scope
- Domain reconnaissance: `networkwalks.com`
- Local network discovery using supplied Zenmap/Nmap evidence
- WHOIS, WhatWeb, nslookup, curl, DNSRecon and Zenmap/Nmap

## Key Results

| Tool | Purpose | Observation |
|---|---|---|
| WHOIS | Domain reconnaissance | Registrar, domain dates and name-server information were observed. |
| WhatWeb | Web fingerprinting | Apache, WordPress 7.1, WP Download Manager 3.3.58, Bootstrap 7.1, jQuery 3.7.1 and other technologies were identified. |
| nslookup | DNS resolution | `networkwalks.com` resolved to `192.232.216.135` using DNS server `8.8.8.8`. |
| curl `-I` | HTTP header inspection | HTTP/2 200 and WordPress-related HTTP information were observed. |
| DNSRecon | DNS enumeration | NS, MX, A, TXT/SPF and SRV records were observed. |
| Zenmap/Nmap | Network discovery | The supplied topology showed `192.168.16.1`, `localhost`, and `192.168.16.254`. |

## Risk Summary
The assessment identified information that could assist further reconnaissance, including web technology information, the public web-server IP, HTTP/WordPress-related information, DNS infrastructure information, and visible local-network nodes.

These are **observations, not confirmed vulnerabilities**.

## Recommendations
- Keep WordPress, plugins and supporting components updated.
- Review unnecessary technology/version exposure.
- Review HTTP response headers.
- Regularly review public DNS records.
- Monitor DNS and web infrastructure for unexpected changes.
- Perform authorized internal network discovery.
- Investigate unknown devices on internal networks.
- Maintain current network topology documentation.
- Perform deeper vulnerability validation only within an authorized scope.

## Repository Structure

```text
B082-Week2/
├── README.md
├── Report/
│   ├── Atanda_Oluwagbenga_B082_Week2_Penetration_Testing_Report.pdf
│   └── Atanda_Oluwagbenga_B082_Week2_Penetration_Testing_Report.docx
└── Evidence/
    ├── whois.png
    ├── whatweb.png
    ├── nslookup.png
    ├── curl.png
    ├── dnsrecon.png
    └── zenmap.png
```

## Authorization Notice
All reconnaissance and scanning should be performed only against systems and networks for which appropriate authorization has been granted.
