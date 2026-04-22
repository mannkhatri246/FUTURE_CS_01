## Overview
A passive, read-only security audit conducted on http://demo.testfire.net (Altoro Mutual - IBM Demo Banking Application) as part of the Future Interns Cybersecurity Internship 2026.

## Target Information
- Website: http://demo.testfire.net
- Application: Altoro Mutual (IBM Demo Banking App)
- IP Address: 65.61.137.117
- Server: Apache-Coyote/1.1
- Assessment Date: April 13, 2026
- Assessment Type: Passive / Read-Only

## Tools Used
- SecurityHeaders.com - HTTP security header analysis
- Browser DevTools (Chrome) - Network and cookie inspection
- Manual Testing - XSS and SQL Injection detection

## Summary of Findings
- Critical: 3
- High: 6
- Medium: 3
- Total: 12

## Vulnerabilities Found

### 1. Critical
- Cross-Site Scripting (XSS)
- SQL Injection - Authentication Bypass
- Broken Access Control

### 2. High
- Missing Content-Security-Policy
- Missing X-Frame-Options
- No HTTPS Enforcement
- Server Version Disclosed
- Missing SameSite Cookie Attribute
- Session Cookie Never Expires

### 3. Medium
- Missing X-Content-Type-Options
- Missing Referrer-Policy
- Missing Permissions-Policy

## Remediation Summary

### Immediate Actions (Critical)
- Fix SQL Injection using parameterized queries
- Fix XSS with input validation and output encoding
- Fix Broken Access Control with server-side authentication checks

### Short-Term Actions (High)
- Enable HTTPS with SSL/TLS certificate
- Add Security Headers (CSP, X-Frame-Options)
- Fix Session Management (SameSite, session timeout)
- Hide Server Version from HTTP response headers

### Medium-Term Actions (Medium)
- Add X-Content-Type-Options header
- Add Referrer-Policy header
- Add Permissions-Policy header

## Disclaimer
This assessment was conducted strictly for educational purposes as part of a cybersecurity internship. Only passive, read-only techniques were used on an intentionally vulnerable demo application authorized for security testing. No data was modified, extracted, or damaged.

## Prepared By
- Name: Khatri Mann Jatinkumar
- Organization: Future Interns
- Email: mannkhatri2464@gmail.com
- Internship: Cyber Security Internship 2026
