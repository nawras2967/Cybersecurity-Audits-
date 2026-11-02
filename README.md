<div align="center">

# 🛡️ CYBERSECURITY AUDITS

### Security Research · Vulnerability Assessment · Web Application Security · Network Analysis

**PALOMA CASABONA**

Cybersecurity Analyst (SOC) | Software Developer

*Security assessments grounded in evidence, risk analysis and actionable remediation.*

![Cybersecurity](https://img.shields.io/badge/CYBERSECURITY-SECURITY%20ASSESSMENT-0A192F?style=for-the-badge)
![OWASP](https://img.shields.io/badge/METHODOLOGY-OWASP-00A6A6?style=for-the-badge)
![Status](https://img.shields.io/badge/STATUS-ACTIVE-22C55E?style=for-the-badge)

**[Security Assessments](#-featured-security-assessment) · [Methodology](#-assessment-methodology) · [Technical Stack](#-technical-stack) · [Documentation](#-technical-documentation)**

</div>

---

## 01 / OVERVIEW

This repository documents my practical work in **cybersecurity auditing, vulnerability assessment, network traffic analysis and web application security**.

It combines academic security auditing projects with independent assessments performed in controlled environments and on systems under my ownership or authorization.

My work focuses on the complete assessment lifecycle:

**Asset identification → Security analysis → Evidence collection → Risk evaluation → Remediation planning → Technical reporting**

The objective is not simply to identify potential security weaknesses, but to understand their technical implications, assess their actual relevance and recommend appropriate preventive and corrective security controls.

### Core areas

| Domain | Focus |
|---|---|
| **Web Application Security** | HTTP security headers, browser security policies, exposed resources and configuration assessment |
| **Vulnerability Assessment** | Automated findings, contextual analysis, risk classification and remediation |
| **Network Security** | Traffic inspection, protocol analysis and service discovery |
| **Security Operations** | Security monitoring concepts, event interpretation and defensive investigation |
| **Technical Reporting** | Evidence documentation, executive summaries, technical findings and mitigation plans |
| **Security Laboratories** | Controlled practical exercises using intentionally vulnerable environments |

---

## 02 / FEATURED SECURITY ASSESSMENT

### 🔎 Web Application Security Assessment

**Target:** `www.palomacasabona.com`  
**Assessment date:** November 2, 2026  
**Assessment type:** Automated passive web security assessment  
**Primary tool:** OWASP ZAP 2.17.0  
**Infrastructure:** Cloudflare, web application deployment and local testing environment

#### Assessment overview

A security assessment was performed against my professional portfolio website to examine HTTP response security, browser security policies, exposed resources and potential configuration weaknesses.

The assessment included a comparison between a locally served static build and the publicly deployed website.

The objective was to identify security-relevant findings, distinguish configuration observations from confirmed vulnerabilities and establish a prioritized remediation strategy.

#### Security assessment results

| Metric | Production environment |
|---|---:|
| Endpoints observed | **41** |
| High-severity alert categories | **0** |
| Medium-severity alert categories | **4** |
| Low-severity alert categories | **2** |
| Informational alert categories | **5** |
| Assessment method | Passive baseline scan |

> **Assessment limitation:** These results represent automated alert categories, not confirmed exploitable vulnerabilities. No manual exploitation or comprehensive penetration testing was performed.

#### Technical findings

| ID | Finding | ZAP severity | Assessment |
|---|---|---|---|
| F01 | Missing anti-CSRF tokens in contact form | Medium | Requires contextual verification |
| F02 | CSP permits `unsafe-inline` styles | Medium | Confirmed configuration observation |
| F03 | Permissive CORS policy | Medium | Context-dependent risk |
| F04 | Missing Subresource Integrity attributes | Medium | Third-party resource hardening |
| F05 | Missing Cross-Origin-Embedder-Policy | Low | Optional architectural control |
| F06 | Inconsistent HSTS headers on API responses | Low | Requires route-level verification |

#### Defensive recommendations

The assessment identified several opportunities for improving the application's security posture:

- Review server-side validation and anti-abuse protections on the contact endpoint.
- Evaluate CORS configuration independently for public assets and API responses.
- Reduce reliance on inline CSS and progressively strengthen Content Security Policy.
- Consider self-hosting third-party font resources.
- Verify consistent HTTPS security policies across application routes.
- Evaluate additional cross-origin isolation controls only when technically justified.

**Outcome:** A documented security baseline and a prioritized remediation plan, with explicit distinctions between observed configurations, potential risks and findings requiring further verification.

---

## 03 / TECHNICAL DOCUMENTATION

### 🌍 Multilingual security reporting

Security documentation is intended to be accessible to both technical and non-technical audiences.

The featured assessment is available in Spanish, with adapted translations prepared in English, Russian, Arabic and Simplified Chinese.

| Language | Document |
|---|---|
| 🇪🇸 **Spanish** | `Informe_Auditoria_Seguridad_Paloma_Casabona_2026.pdf` |
| 🇬🇧 **English** | `Informe_Auditoria_Paloma_Casabona_EN.pdf` |
| 🇷🇺 **Russian** | `Informe_Auditoria_Paloma_Casabona_RU.pdf` |
| 🇸🇦 **Arabic** | `Informe_Auditoria_Paloma_Casabona_AR.pdf` |
| 🇨🇳 **Simplified Chinese** | `Informe_Auditoria_Paloma_Casabona_ZH.pdf` |

*Documents should be accessed through the repository's file browser. Availability depends on which PDFs have been uploaded.*

### Report structure

The technical assessment documentation covers:

1. Executive summary and assessment scope.
2. Local and production environment comparison.
3. Security findings and technical interpretation.
4. Risk classification and assessment limitations.
5. Preventive controls and security safeguards.
6. Prioritized remediation recommendations.
7. Verification procedures and monitoring indicators.
8. Technical glossary and supporting references.

---

## 04 / ASSESSMENT METHODOLOGY

Security assessments follow a structured, evidence-based workflow.

```text
                  SECURITY ASSESSMENT WORKFLOW

                           ┌──────────────┐
                           │ DEFINE SCOPE │
                           └──────┬───────┘
                                  │
                           ┌──────▼───────┐
                           │ RECONNAISSANCE│
                           └──────┬───────┘
                                  │
                           ┌──────▼───────┐
                           │   ANALYSIS   │
                           └──────┬───────┘
                                  │
                           ┌──────▼───────┐
                           │   VALIDATE   │
                           │   FINDINGS   │
                           └──────┬───────┘
                                  │
                           ┌──────▼───────┐
                           │ ASSESS RISK  │
                           └──────┬───────┘
                                  │
                           ┌──────▼───────┐
                           │  RECOMMEND   │
                           │  CONTROLS    │
                           └──────┬───────┘
                                  │
                           ┌──────▼───────┐
                           │   DOCUMENT   │
                           │   & REPORT   │
                           └──────────────┘
```

### Assessment principles

**Evidence before conclusions.** Automated alerts are reviewed in context and are not automatically classified as confirmed vulnerabilities.

**Risk-based prioritization.** Findings are assessed according to their potential impact, likelihood and relevance to the target architecture.

**Defensive value.** Reports emphasize practical safeguards, configuration improvements and remediation procedures.

**Reproducibility.** Assessment scope, tools, limitations and supporting evidence are documented whenever available.

**Responsible testing.** Testing is restricted to authorized systems and controlled environments.

---

## 05 / TECHNICAL STACK

### Security assessment and analysis

| Technology | Application |
|---|---|
| **OWASP ZAP** | Automated passive web security assessment |
| **Burp Suite** | Web application security testing and HTTP analysis |
| **Wireshark** | Network packet capture and protocol inspection |
| **Nmap** | Network discovery and service enumeration |
| **FFUF** | Web content discovery in authorized environments |
| **cURL** | HTTP request and response inspection |

### Infrastructure and environments

| Technology | Application |
|---|---|
| **Kali Linux** | Security testing environment |
| **Ubuntu** | Linux administration and laboratory environments |
| **Docker** | Containerized tools and isolated test environments |
| **OWASP Juice Shop** | Intentionally vulnerable web application laboratory |
| **Git & GitHub** | Version control and technical documentation |

*The table represents technologies used across the broader body of work, not exclusively in the featured assessment.*

---

## 06 / SECURITY LABORATORIES & PRACTICAL WORK

### Web application security

Practical exercises involving HTTP request analysis, web security concepts, application behavior and controlled vulnerability assessment.

**Tools:** Burp Suite, OWASP Juice Shop and supporting HTTP utilities.

### Network traffic analysis

Traffic capture and inspection to examine network protocols, communications and security-relevant observations.

**Tool:** Wireshark.

### Network reconnaissance

Authorized exercises involving host discovery, service identification and the interpretation of network enumeration results.

**Tools:** Nmap and Linux networking utilities.

### Technical audit reporting

Development of structured security reports documenting objectives, methodology, technical evidence, findings, risk interpretation and recommended safeguards.

**Deliverables:** PDF assessments, supporting evidence and technical documentation.

---

## 07 / RISK MANAGEMENT & REMEDIATION

A security finding becomes operationally useful when it can be interpreted, prioritized and addressed.

The reporting process distinguishes:

| Classification | Meaning |
|---|---|
| **Observed finding** | A configuration or behavior supported by collected evidence |
| **Potential vulnerability** | A weakness requiring further validation |
| **Confirmed vulnerability** | A security weakness demonstrated through sufficient verification |
| **False positive** | An alert determined to be inapplicable after review |
| **Residual risk** | Risk remaining after controls or remediation |

### Remediation priorities

**P1 — Review first:** Contact endpoint protections and API-specific CORS behavior.

**P2 — Planned hardening:** Content Security Policy, external resource dependencies and HSTS consistency.

**P3 — Architecture-dependent:** Cross-origin isolation controls such as COEP.

**Continuous improvement:** Reassessment after changes, evidence preservation and monitoring of relevant security indicators.

---

## 08 / PROFESSIONAL COMPETENCIES

`Security Auditing` · `Web Application Security` · `Vulnerability Assessment` · `Network Traffic Analysis` · `HTTP Security` · `Risk Assessment` · `Technical Reporting` · `Linux` · `Docker` · `Security Hardening` · `Remediation Planning`

---

## 09 / ETHICAL & LEGAL NOTICE

All security assessments and practical exercises documented in this repository are conducted for legitimate educational, research and defensive purposes.

Testing is performed exclusively against:

- Systems under my ownership.
- Controlled and intentionally vulnerable laboratory environments.
- Systems for which explicit authorization has been granted.

No unauthorized access, exploitation or testing of third-party infrastructure is endorsed.

Sensitive information, authentication credentials and private operational data should not be included in public documentation.

---

## 10 / AUTHOR

<div align="center">

### Paloma Casabona

**Cybersecurity Analyst (SOC) | Software Developer**

Security Auditing · Defensive Security · Web Application Security

[![GitHub](https://img.shields.io/badge/GitHub-nawras2967-181717?style=for-the-badge&logo=github)](https://github.com/nawras2967)

</div>

---

<div align="center">

### SECURITY IS A PROCESS, NOT A CHECKLIST.

*Identify. Analyze. Validate. Mitigate. Document.*

**© 2026 Paloma Casabona**

</div>
