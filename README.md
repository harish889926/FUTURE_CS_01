# FUTURE_CS_01 — Vulnerability Assessment Report

## Target
- **Website:** https://demo.testfire.net
- **Application:** Altoro Mutual (Demo Banking App by HCL Technologies)
- **Assessment Type:** Passive, read-only — no exploitation

## Tools Used
| Tool | Purpose |
|------|---------|
| Nmap 7.98 | Port scanning & service detection |
| OWASP ZAP 2.17.0 | Passive vulnerability scanning |
| Firefox DevTools | Manual header & cookie inspection |

##  Findings Summary
| Risk Level | Count |
|------------|-------|
|  High    | 3     |
|  Medium  | 4     |
|  Low     | 7     |
| **Total**  | **14**|

##  Vulnerabilities Found
| # | Vulnerability | Location | Risk |
|---|--------------|----------|------|
| 1 | Cross-Site Scripting (XSS) | Search Bar | High |
| 2 | Cross-Site Scripting (XSS) | Feedback Page |  High |
| 3 | Missing Anti-CSRF Tokens | Feedback Form |  High |
| 4 | Missing CSP Header | All Pages |  Medium |
| 5 | Missing Anti-Clickjacking Header | All Pages |  Medium |
| 6 | Sub Resource Integrity Missing | JS Scripts |  Medium |
| 7 | Exposed Swagger REST API | /swagger/index.html |  Medium |
| 8 | Server Version Disclosure | HTTP Headers |  Low |
| 9 | Cookie Without SameSite | JSESSIONID |  Low |
| 10 | Missing HSTS Header | All Pages |  Low |
| 11 | X-Content-Type-Options Missing | All Pages |  Low |
| 12 | Sensitive Info in HTML Comments | /login.jsp |  Low |
| 13 | Debug Error Messages | Swagger JSON |  Low |
| 14 | Autocomplete on Password Field | /login.jsp |  Low |

##  Repository Structure
FUTURE_CS_01/
├── README.md
├── screenshots/     ← All evidence screenshots
├── report/          ← Full PDF report (Canva)
└── notes/           ← Raw findings notes

##  Intern Details
- **Track:** Cyber Security (CS)
- **Organization:** Future Interns
- **Task:** Task 1 — Vulnerability Assessment Report