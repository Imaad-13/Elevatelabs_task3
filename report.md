# 📋 Vulnerability Report Summary (Nessus Essentials)

## 🎯 Target
- **IP Address:** 192.168.1.10
- **Scanner:** Nessus Essentials
- **Scan Date:** May 29, 2025

---

## 🔴 Critical Vulnerability

### 1. Node.js Multiple Vulnerabilities (Feb 14, 2024)
- **Plugin ID:** 190856
- **CVSS v3 Score:** 9.8
- **Description:** Outdated Node.js versions contain severe vulnerabilities that may allow remote code execution or denial-of-service (DoS).
- **Affected Versions:** < 18.19.1 / 20.11.1 / 21.6.2

---

## 🟠 Medium Vulnerabilities

### 2. SSL Certificate Cannot Be Trusted
- **Plugin ID:** 51192
- **CVSS Score:** 6.5
- **Description:** The SSL certificate is self-signed or from an untrusted CA, which could allow man-in-the-middle (MITM) attacks.

### 3. Node.js Multiple Vulnerabilities (May 14, 2025)
- **Plugin ID:** 236766
- **CVSS Score:** 6.2
- **Description:** Newer vulnerabilities in Node.js allowing potential DoS or memory exploits.
- **Affected Versions:** < 20.19.2 / 22.15.1 / 23.11.1 / 24.0.2
