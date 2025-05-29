# 🛡️ Mitigation Plan for Identified Vulnerabilities

This document outlines recommended remediation steps for the critical and medium vulnerabilities discovered in the Nessus scan of the host `192.168.1.10`.

---

## 🔴 Critical Vulnerability

### 1. Node.js Multiple Vulnerabilities (Feb 14, 2024)
- **Plugin ID:** 190856
- **Severity:** Critical
- **CVSS v3 Score:** 9.8
- **Affected Versions:** Node.js < 18.19.1 / < 20.11.1 / < 21.6.2
- **Threat:** Allows attackers to execute arbitrary code, crash the system via denial-of-service, or bypass security restrictions.

#### ✅ Recommended Mitigation:
- **Update Node.js** to the latest secure version.
  - Visit: [https://nodejs.org](https://nodejs.org)
- **Linux Install (Ubuntu/Debian):**
  ```bash
  sudo apt update
  sudo apt install -y nodejs npm

---

## 🟠 Medium Vulnerabilities

---

### 2. SSL Certificate Cannot Be Trusted
- **Plugin ID:** 51192  
- **Severity:** Medium  
- **CVSS Score:** 6.5  

#### ⚠️ Threat
The server is using a **self-signed** or **untrusted SSL certificate**. This could allow **man-in-the-middle (MITM)** attacks or impersonation of the server.

#### ✅ Recommended Mitigation
- Replace the certificate with one issued by a **trusted Certificate Authority (CA)**.
- Use **Let's Encrypt** (a free SSL provider):  
  🔗 [https://letsencrypt.org](https://letsencrypt.org)

#### 📥 Example with Certbot:
```bash
sudo apt install certbot
sudo certbot certonly --standalone