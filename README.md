# FUTURE_CS_03 – API Security Risk Analysis Report

**Author:** NORAH CYPRIAN NGILIULE  
**CIN ID:** FIT/MAY26/CS8136  
**Date:** 21-05-2026  
**Task:** API Security Risk Analysis – Future Interns Task 3  

---

## Overview
This project focuses on API Security Risk Analysis, where different API security risks are identified, analyzed, and documented. The aim is to understand how insecure APIs can expose systems to cyberattacks and how to mitigate these risks effectively.

---

## Tools Used
- Postman / Insomnia  
- Browser Developer Tools  
- Sample Public APIs (Test/Demo APIs)  
- Google Docs / MS Word  
- PDF Export Tools  

---

## Skills Gained
- API security analysis  
- Authentication & authorization assessment  
- Risk identification and evaluation  
- Security documentation writing  
- SaaS security fundamentals  

---

## Key Features
- Identification of insecure API endpoints and data exposure risks  
- Analysis of authentication & authorization issues (tokens, API keys, access control)  
- Detection of missing rate-limiting and input validation weaknesses  
- Clear explanation of API risks in simple, business-friendly language  

---

## Deliverable
A professional API Security Risk Analysis Report containing:
- Identified API security risks  
- Impact analysis of each risk  
- Recommended mitigation strategies  
- Documented and uploaded to GitHub repository  

---

## API Tested

Name: JSONPlaceholder  
URL: https://jsonplaceholder.typicode.com  
Type: Public REST API for testing and learning  

---

## Methodology

This assessment was conducted using a structured, read-only security analysis approach. The API was evaluated by reviewing documentation, sending controlled requests to selected endpoints, and analyzing responses and HTTP security headers. The goal was to identify potential security weaknesses based on OWASP API Security Top 10 principles without performing any malicious or disruptive testing.

---

## Endpoints Tested

1. GET /users - Check authentication requirement  
2. GET /users/1 - Test single user access  
3. GET /users/2 - Test IDOR vulnerability  
4. GET /posts - Check data exposure  
5. POST /posts - Test write access without authentication  
6. HEAD /users - Inspect security headers  

---

## Findings Summary

Finding API-01: No authentication required for any endpoint  
Severity: MEDIUM  

Finding API-02: IDOR vulnerability – can access any user by changing sequential ID  
Severity: MEDIUM  

Finding API-03: Missing security headers (CSP, X-Frame-Options, X-Content-Type-Options)  
Severity: LOW  

Finding API-04: No rate limiting – unlimited requests allowed  
Severity: LOW  

Total Findings: 4  
Medium Risk: 2  
Low Risk: 2  

---

## Conclusion

JSONPlaceholder is a test API intentionally designed for learning. However, if this were a production API, the security issues identified would be unacceptable for a business.

Key takeaways from this assessment:
- APIs must require authentication for sensitive data  
- Sequential IDs create IDOR vulnerabilities  
- Security headers should never be missing  
- Rate limiting protects against abuse  

Ethical Compliance Statement: All testing was performed in read-only scope. No exploitation, brute force, or denial-of-service attacks were conducted.  

---

## Links

GitHub Repository: https://github.com/NorahCyprian/FUTURE_CS_03 
API Tested: https://jsonplaceholder.typicode.com  
OWASP API Security Top 10: https://owasp.org/www-project-api-security/
