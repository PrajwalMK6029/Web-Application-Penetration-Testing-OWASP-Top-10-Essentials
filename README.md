# Project 3: Web Application Penetration Testing – OWASP Top 10 Essentials

## Overview
This project provides a structured workflow and reporting toolkit for assessing a deliberately vulnerable web application in an authorised, isolated lab. The project brief focuses on OWASP Juice Shop or bWAPP and asks for application mapping, vulnerability identification, proof-of-concept evidence, and remediation guidance.

This repository is a **documentation and assessment scaffold**. It does not claim that vulnerabilities have already been tested or confirmed. Add your own observations, screenshots, Burp Suite state file, ZAP session, and final report after completing the lab.

## Objectives
- Map application pages, forms, endpoints, and API calls.
- Review common web-application weakness categories using manual testing first.
- Use automated tools as supporting evidence and only within the approved lab scope.
- Document verified findings with reproduction steps, impact, severity, evidence, and remediation.
- Produce a developer-friendly penetration-test report.

## Lab target
Use only a deliberately vulnerable application that you own or have explicit permission to test, such as:
- OWASP Juice Shop
- bWAPP

Use an isolated lab address supplied by your instructor. Do not test public websites or real users without written authorisation.

## Tools listed in the brief
- Burp Suite Community Edition
- OWASP ZAP
- Browser developer tools
- Wappalyzer or manual technology fingerprinting
- sqlmap only as a cautious follow-up after manual validation
- SecLists / directory discovery tools only when explicitly in scope

## Repository structure
```text
webapp-pentest-project-3/
├── README.md
├── .gitignore
├── requirements.txt
├── docs/
│   ├── lab-safety.md
│   ├── workflow.md
│   ├── owasp-test-matrix.md
│   └── remediation-reference.md
├── templates/
│   ├── authorisation-and-scope.md
│   ├── finding-template.md
│   ├── pentest-report-template.md
│   ├── evidence-register.csv
│   └── testing-log.csv
└── evidence/
    └── README.md
```

## Suggested workflow
1. Complete `templates/authorisation-and-scope.md`.
2. Set up the approved vulnerable application and record the lab URL.
3. Map the app manually and with Burp/ZAP; save tool session files locally.
4. Test the categories in `docs/owasp-test-matrix.md` using safe, lab-only test cases.
5. Record only reproducible observations; distinguish confirmed findings from hypotheses.
6. Capture screenshots or short recordings that avoid exposing real secrets.
7. Score findings using the severity method required by your instructor and explain the rationale.
8. Complete the report template and include practical remediation advice.
9. Review `docs/lab-safety.md` before sharing the repository publicly.

## Deliverables checklist
- [ ] Burp Suite state file (if supported by your setup and required by the brief)
- [ ] OWASP ZAP session
- [ ] Evidence screenshots/videos grouped by finding ID
- [ ] Comprehensive report with executive summary
- [ ] Remediation recommendations for each verified issue

## Important
Do not commit real credentials, session cookies, API keys, personal information, or unredacted sensitive traffic. Replace lab-only secrets with placeholders in screenshots and reports. This repository is a starter framework, not proof that testing has been performed.
