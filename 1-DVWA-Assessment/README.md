# DVWA Vulnerability Assessment

## Objective
I tested the Damn Vulnerable Web Application (DVWA) to find and document security vulnerabilities.

## Vulnerabilities Found

### 1. SQL Injection (HIGH RISK)
**Location:** Login page  
**Description:** The login form doesn't check user input properly  
**What I did:** I entered `admin' OR '1'='1` and bypassed login  
**How to fix:** Use prepared statements in the code  

### 2. Cross-Site Scripting (XSS) (MEDIUM RISK)
**Location:** User input form  
**Description:** Can inject JavaScript code  
**What I did:** Entered `<script>alert('XSS')</script>`  
**How to fix:** Sanitize all user input  

### 3. Weak Passwords (MEDIUM RISK)
**Description:** Default credentials still active  
**What I did:** Logged in with admin/password  
**How to fix:** Change default credentials  

## Tools Used
- Burp Suite Community Edition
- Firefox Browser
- DVWA Application

## Time Spent
3 days

## Key Learnings
- How to identify input validation issues
- Understanding HTTP requests
- Basics of web security testing

## Screenshots
[I'll add screenshots later]
