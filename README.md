<div align="center">

# 🛡️ Cybersecurity Audits

### Security Assessments · Web Application Security · Network Analysis · Technical Reporting

**Paloma Casabona** · Cybersecurity Analyst (SOC) · Software Developer

*From evidence to actionable security improvements.*

[![Focus](https://img.shields.io/badge/Focus-Security%20Auditing-0d9488?style=flat-square)](#about-this-repository)
[![Methodology](https://img.shields.io/badge/Methodology-OWASP-2563eb?style=flat-square)](#methodology)
[![Documentation](https://img.shields.io/badge/Documentation-Technical%20Reports-475569?style=flat-square)](#featured-security-assessment)

</div>

---

## 🔎 About this repository

This repository brings together my hands-on cybersecurity work, including **security assessments, web application analysis, network traffic inspection, controlled laboratory exercises, technical evidence, and remediation guidance**.

My approach emphasizes not only identifying potential weaknesses, but also **interpreting their actual impact, distinguishing automated findings from verified vulnerabilities, and proposing practical safeguards**.

The collection includes coursework from information security auditing modules alongside independent, authorized assessments.

## ⭐ Featured security assessment

### Web Security Assessment — palomacasabona.com | November 2026

**Scope:** My own public portfolio website, with an additional comparison against a locally served build.  
**Approach:** OWASP ZAP baseline / passive assessment; review of HTTP responses and security configuration.  
**Tools:** OWASP ZAP, Docker, HTTP inspection.

| Production scan summary | Result |
|:--|--:|
| URLs assessed | 41 |
| High-risk alert categories | **0** |
| Medium-risk alert categories | **4** |
| Low-risk alert categories | **2** |
| Informational alert categories | **5** |

**Topics reviewed:** CSRF protections on a public contact form; Content Security Policy (`style-src 'unsafe-inline'`); Cross-Origin Resource Sharing (`Access-Control-Allow-Origin: *`); Subresource Integrity for third-party stylesheets; Cross-Origin-Embedder-Policy; HTTP Strict Transport Security; caching behavior and informational disclosures.

> **Interpretation:** These figures represent automated alert categories, **not 11 confirmed exploitable vulnerabilities**. Findings require context-specific validation. Some are hardening recommendations or low-impact observations for public static content.

### 📑 Assessment deliverables

| Language | Report |
|:--|:--|
| 🇪🇸 Spanish | [Security assessment (PDF)](Informe_Auditoria_Seguridad_Paloma_Casabona_2026.pdf) |
| 🇬🇧 English | Translation planned |
| 🇷🇺 Russian | Translation planned |
| 🇸🇦 Arabic | Translation planned |
| 🇨🇳 Simplified Chinese | Translation planned |

*The Spanish PDF link assumes the file is stored alongside this README. Update the relative path if you place it in a subfolder.*

---

## 🧰 Tools & technologies

| Area | Tools / environments |
|:--|:--|
| Web security assessment | OWASP ZAP, Burp Suite, OWASP Juice Shop |
| Network inspection | Wireshark, Nmap |
| HTTP and discovery | cURL, FFUF |
| Systems and laboratories | Kali Linux, Ubuntu, Docker |
| Documentation and version control | Git, GitHub, Markdown, PDF reporting |

*Tools are listed as part of the repository's broader practical work; they were not all used in the featured ZAP assessment.*

---

## 🧭 Methodology

```text
Define authorized scope
         ↓
Reconnaissance and asset review
         ↓
Passive assessment / controlled testing
         ↓
Analyze and validate findings
         ↓
Assess context, likelihood and impact
         ↓
Recommend safeguards and remediation
         ↓
Document evidence and retest where applicable
```

Findings are assessed in context. Reports distinguish **observed configuration**, **potential risk**, **verification status**, and **recommended remediation**.

---

## 📂 Areas covered

- **Web application security:** HTTP headers, browser security policies, exposed endpoints, and configuration review.
- **Network traffic analysis:** Packet inspection and protocol analysis with Wireshark.
- **Security laboratories:** Authorized exercises using OWASP Juice Shop and Burp Suite.
- **Technical reporting:** Scope, methodology, findings, evidence, risk interpretation, and preventive controls.
- **Defensive improvement:** Mitigation recommendations, hardening, and validation steps.

---

## 🎯 Skills demonstrated

Security assessment · Technical documentation · Network traffic analysis · Web security fundamentals · Evidence handling · Risk interpretation · Remediation planning · Linux and Docker environments

---

## ⚖️ Responsible use & authorization

All practical assessments documented here are intended for educational, defensive, or professional development purposes.

Testing is performed **only on systems I own, controlled lab environments, or systems with explicit authorization**.

Public reports are reviewed to avoid disclosing credentials, tokens, sensitive data, or information that would unnecessarily increase risk.

---

## 👩‍💻 Author

**Paloma Casabona**  
Cybersecurity Analyst (SOC) · Software Developer

[GitHub Profile](https://github.com/nawras2967)

---

<div align="center">

*Security is not only about detecting issues — it is about understanding, prioritizing, and reducing risk.*

</div>
