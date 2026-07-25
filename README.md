# Growfinix Internship Task 1: Securing Frontend Frameworks (XSS & CSRF)

## Overview
This repository contains the demonstration and fix for Cross-Site Scripting (XSS) and Cross-Site Request Forgery (CSRF) vulnerabilities in a React + Tailwind CSS web application.

---

## 1. Vulnerability Demonstration (XSS Exploitation)

### Vulnerable Code Pattern
Previously, user inputs were rendered directly using unsanitized HTML insertion:
```jsx
// VULNERABLE CODE
<div dangerouslySetInnerHTML={{ __html: userSubmittedInput }} />
