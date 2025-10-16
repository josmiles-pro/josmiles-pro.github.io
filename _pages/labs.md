---
layout: single
title: "Lab Challenges"
permalink: /labs/
author_profile: true
toc: true
toc_label: "Challenges"
toc_icon: "flask"
---

## Featured Security Lab Challenges

---

## 🔴 FakeBank Web Application Penetration Test

**Platform:** TryHackMe | **Difficulty:** Easy | **Date:** September 2025

### Challenge Brief
Conduct security assessment of FakeBank application to identify access control vulnerabilities in financial transaction systems.

### Methodology
- Directory enumeration using Gobuster
- Identified hidden `/bank-transfer` endpoint
- Exploited missing authentication controls
- Executed unauthorized $2,000 transfer between accounts

### Tools Used
Gobuster, Burp Suite, Firefox DevTools, Kali Linux

### Key Finding
**Critical Vulnerability:** Unprotected administrative interface (CVSS 9.1)
- No authentication required for financial transactions
- Complete bypass of authorization controls

### Impact
Demonstrated direct monetary theft capability and complete transaction control without credentials.

![FakeBank Exploitation](../assets/images/fakebank-exploit.png)

**Skills:** Web exploitation, Access control testing, Impact assessment

---

## 🟢 Passive Reconnaissance & OSINT

**Platform:** TryHackMe | **Difficulty:** Easy | **Date:** October 2025

### Challenge Brief
Perform comprehensive intelligence gathering on target domains using only passive techniques without alerting targets.

### Methodology
- WHOIS analysis for domain registration intel
- DNS enumeration (TXT, MX, A records)
- Subdomain discovery via DNSDumpster
- Global infrastructure analysis using Shodan

### Tools Used
whois, nslookup, DNSDumpster, Shodan.io

### Key Findings
✅ Identified domain registered July 5, 2018 (NameCheap/Cloudflare)  
✅ Discovered 5 subdomains including `remote.tryhackme.com` (VPN portal)  
✅ Retrieved TXT flag: `THM{a5b83929888ed36acb0272971e438d78}`  
✅ Analyzed 76M+ servers: US leads Apache (4.3M), China leads nginx (13.2M)

### Impact
Mapped complete attack surface and identified high-value remote access targets without direct system interaction.

![Passive Recon Results](../assets/images/passive-recon-results.png)

**Skills:** OSINT, DNS analysis, Threat intelligence, Attack surface mapping

---

## 🔵 Web Application Security Assessment

**Platform:** TryHackMe | **Difficulty:** Medium | **Date:** September 2025

### Challenge Brief
Identify and exploit OWASP Top 10 vulnerabilities in test web applications including authentication bypass, injection, and broken access control.

### Methodology
- SQL injection for authentication bypass
- Cross-Site Scripting (XSS) for session hijacking  
- IDOR exploitation for unauthorized data access
- Source code analysis for credential exposure

### Tools Used
Burp Suite, SQLMap, Browser DevTools, OWASP ZAP

### Key Vulnerabilities Exploited
✅ **SQL Injection:** Bypassed login with `admin' OR '1'='1'--`  
✅ **Stored XSS:** Stole session cookies via `<script>` injection  
✅ **IDOR:** Accessed user ID 9 (Database Admin) via parameter manipulation  
✅ **Sensitive Data Exposure:** Found credentials in HTML comments  
✅ **Business Logic:** Exploited negative amounts for financial gain

### Impact
Demonstrated multiple critical paths to full application compromise and data breach.

![Web Security Exploitation](../assets/images/web-security-exploit.png)

**Skills:** OWASP Top 10, SQLi/XSS exploitation, Access control testing, Vulnerability chaining

---

## 📊 Skills Summary

| **Category** | **Skills Demonstrated** |
|-------------|------------------------|
| **Web Security** | SQLi, XSS, IDOR, Authentication bypass |
| **Network** | DNS enumeration, Subdomain discovery |
| **OSINT** | WHOIS, Shodan, Passive intelligence |
| **Tools** | Burp Suite, Gobuster, nslookup, SQLMap |
| **Reporting** | Risk assessment, Impact analysis |

**Total Challenges:** 25+ | **Platforms:** TryHackMe, HackTheBox | **Points:** 500+

---

## 📂 View More

**GitHub:** [Complete Lab Reports](https://github.com/yourusername/security-labs)  
**TryHackMe:** [Profile & Badges](https://tryhackme.com/p/yourusername)
