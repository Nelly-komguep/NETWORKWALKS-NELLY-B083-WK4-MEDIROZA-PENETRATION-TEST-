# 🛡️ Mediroza General Hospital — Web Application Penetration Testing

### NetworkWalks Cybersecurity Internship — Week 4

![Security](https://img.shields.io/badge/Assessment-Authorized%20Pentest-red)
![Batch](https://img.shields.io/badge/Batch-B083-blue)
![Target](https://img.shields.io/badge/Target-medirozahospital.com-green)
![Methodology](https://img.shields.io/badge/Methodology-Black--Box-orange)

---

## 📋 Assessment Overview

This repository documents my Week 4 penetration testing project conducted as part of the NetworkWalks Cybersecurity Internship.

The assessment focused on the authorized black-box security evaluation of the Mediroza General Hospital web application.

| Parameter              | Details                                    |
| ---------------------- | ------------------------------------------ |
| **Target**             | `https://medirozahospital.com`             |
| **Organization**       | Mediroza General Hospital                  |
| **Assessment Type**    | Black-Box Web Application Penetration Test |
| **Program**            | NetworkWalks Cybersecurity Internship      |
| **Batch**              | B083                                       |
| **Duration**           | 5 Days                                     |
| **Testing Scope**      | Authorized target domain only              |
| **Testing Model**      | External / Black-Box                       |
| **Authorization**      | Written authorization provided             |
| **DoS Testing**        | Not performed                              |
| **Social Engineering** | Not performed                              |

---

# 🎯 Objectives

The assessment was designed around four main milestones:

### M1 — Initial Access

Identify exposed entry points, analyze the authentication mechanism and demonstrate access to the restricted patient area within the authorized laboratory environment.

**Expected deliverable:**

* Proof of access
* Three patient laboratory PDF reports

### M2 — Data Extraction

Analyze the protection mechanisms applied to the retrieved PDF documents and recover their contents using appropriate offline analysis techniques.

**Expected deliverable:**

* Recovered contents of all three documents
* Evidence of the recovery process

### M3 — Critical Data Exposure

Analyze the information obtained during the previous phases and investigate additional exposure resulting from files, metadata, directories or legacy resources.

**Expected deliverable:**

* Evidence of staff salary information
* Evidence of shareholder information
* Documentation of the exposure chain

### M4 — Professional Pentest Report

Produce a professional penetration testing report containing:

* Executive Summary
* Scope and Methodology
* Findings and Proof of Exploitation
* Risk Classification
* Recommendations and Remediation

---

# 🧭 Methodology

The assessment followed a structured penetration-testing workflow:

```text
Reconnaissance
      │
      ▼
Application Mapping
      │
      ▼
Authentication Analysis
      │
      ▼
Initial Access
      │
      ▼
Data Retrieval
      │
      ▼
Offline Document Analysis
      │
      ▼
Metadata / Legacy Resource Analysis
      │
      ▼
Sensitive Data Exposure
      │
      ▼
Risk Assessment
      │
      ▼
Reporting & Remediation
```

The methodology was informed by established penetration-testing and web-application security practices, including OWASP testing principles and structured penetration-testing phases.

---

# 🛠️ Tools Used

| Tool               | Purpose                                 |
| ------------------ | --------------------------------------- |
| Kali Linux         | Security testing environment            |
| Burp Suite         | HTTP traffic interception and analysis  |
| cURL               | HTTP reconnaissance                     |
| Browser            | Manual application exploration          |
| `file`             | File identification                     |
| `pdfinfo`          | PDF structure analysis                  |
| ExifTool           | Metadata analysis                       |
| QPDF               | PDF verification/decryption             |
| NetworkWalks tools | Authorized laboratory document analysis |
| Git / GitHub       | Documentation and version control       |

---

# 🔎 Assessment Phases

## M1 — Initial Access

📁 [`M1-INITIAL-ACCESS/`](./M1-INITIAL-ACCESS/)

The first phase focused on:

* Web reconnaissance
* `robots.txt` analysis
* Application directory discovery
* Patient portal identification
* Authentication analysis
* HTTP request/response analysis using Burp Suite
* Access validation
* Retrieval of the three laboratory reports

---

## M2 — Data Extraction

📁 [`M2-DATA-EXTRACTION/`](./M2-DATA-EXTRACTION/)

The second phase focused on:

* Identification of PDF protection mechanisms
* File analysis
* Extraction of relevant cryptographic information
* Offline password recovery
* PDF decryption/verification
* Validation of recovered contents

---

## M3 — Critical Data Exposure

📁 [`M3-CRITICAL-DATA-EXPOSURE/`](./M3-CRITICAL-DATA-EXPOSURE/)

The third phase focused on:

* File metadata analysis
* Identification of operational information
* Analysis of exposed directories
* Investigation of legacy resources
* Identification of staff information
* Identification of shareholder information
* Documentation of the complete exposure chain

---

## M4 — Final Penetration Testing Report

📁 [`M4-PENTEST-REPORT/`](./M4-PENTEST-REPORT/)

The final deliverable consolidates:

1. Executive Summary
2. Scope and Methodology
3. Technical Findings
4. Evidence and Proof of Exploitation
5. Risk Classification
6. Business Impact
7. Recommendations
8. Remediation Roadmap
9. Conclusion

---

# 📊 Findings Overview

| ID     | Finding                                      | Category                        | Risk |
| ------ | -------------------------------------------- | ------------------------------- | ---- |
| MED-01 | Authentication weakness                      | Authentication                  | TBD  |
| MED-02 | Insufficient protection of patient documents | Cryptographic / Data Protection | TBD  |
| MED-03 | Sensitive information disclosure             | Information Disclosure          | TBD  |
| MED-04 | Exposed legacy resources                     | Security Misconfiguration       | TBD  |
| MED-05 | Sensitive organizational data exposure       | Data Exposure                   | TBD  |

> Risk levels will be assigned after completing the technical analysis and evaluating likelihood, impact and exploitability.

---

# 📸 Evidence

All screenshots and supporting evidence are organized according to the corresponding milestone.

```text
M1 → Initial Access
M2 → Data Extraction
M3 → Critical Data Exposure
M4 → Final Report
```

Sensitive personal information should be masked or redacted before publication.

---

# 🔐 Authorization & Rules of Engagement

This assessment was performed exclusively within the scope defined by the NetworkWalks Week 4 Mediroza General Hospital penetration-testing project.

Testing was restricted to the authorized target:

`https://medirozahospital.com`

The following activities were excluded:

* Denial-of-Service testing
* Social engineering
* Phishing
* Testing unrelated external systems
* Testing outside the authorized target scope

All testing activities documented in this repository were performed for educational and authorized security-assessment purposes.

---

# 📚 References

* OWASP Web Security Testing Guide
* OWASP Top 10
* Penetration Testing Execution Standard (PTES)
* NIST SP 800-115

---

# 👩🏽‍💻 Author

**Nelly**

Software Engineering Student
Cybersecurity / Offensive Security

**Program:** NetworkWalks Cybersecurity Internship
**Batch:** B083
**Week:** 4 — Web Application Penetration Testing

---

## ⚠️ Responsible Disclosure

The information contained in this repository is intended strictly for educational and authorized security-testing purposes.

Do not reproduce testing activities against systems without explicit authorization.
