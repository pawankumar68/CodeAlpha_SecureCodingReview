# Secure Coding Review

A security review project built for the **CodeAlpha Cyber Security Internship - Task 3**.

## 📌 Description

This project contains a small, intentionally vulnerable Admin Login page (HTML, CSS, and JavaScript) along with a full security review report documenting the vulnerabilities found, how each one was confirmed, its impact, and recommended fixes.

The goal of this task was to practice identifying common, real-world security mistakes in front-end code — the same kind of mistakes that show up in actual beginner projects — and to document them the way a security analyst would.

## 🛠 Tools Used

- HTML, CSS, JavaScript (the sample application under review)
- Google Chrome DevTools (Console, Elements) — used to test and confirm each vulnerability
- Microsoft Word (review report)

## 🔗 Live Demo

Try the vulnerable login page yourself: [Live Demo](https://pawankumar68.github.io/CodeAlpha_SecureCodingReview/)

**Credentials:** username `admin`, password `admin123`

⚠️ This is intentionally insecure — feel free to try bypassing the login using browser DevTools (see the review report for how).

## 📂 Contents

- `index.html` — the sample admin login page
- `dashboard.html` — the page shown after login
- `style.css` — shared styling for both pages
- `Secure_Coding_Review_Report.docx` — the full review report, written in simple language (5 vulnerabilities, with screenshots as proof)
- `Secure_Coding_Review_Report.pdf` — PDF version for quick preview (viewable directly on GitHub)

## 🔍 Vulnerabilities Identified

| ID | Vulnerability | Severity |
|----|---------------|----------|
| VULN-01 | Hardcoded credentials in client-side JavaScript | High |
| VULN-02 | Authentication enforced only on the client side (bypassed using browser console) | High |
| VULN-03 | Unsanitized URL input rendered as HTML (XSS) | Medium |
| VULN-04 | Password hint disclosed directly on the login page | Medium |
| VULN-05 | Session state stored in an unprotected, client-editable cookie | Low |

Full details, proof-of-concept steps, screenshots, and fix recommendations for each vulnerability are in the review report.

## ▶️ How to Run

1. Download `index.html`, `dashboard.html`, and `style.css` into the same folder
2. Open `index.html` in any browser
3. Login with username `admin` and password `admin123`

⚠️ This app is intentionally insecure and is for educational/demonstration purposes only — it should never be deployed or used for real authentication.

## 🎓 What I Learned

- How easily front-end-only authentication can be bypassed using nothing more than browser DevTools
- Why credentials and session validation must always be handled on a server, never trusted to client-side code
- How unsanitized user input leads to Cross-Site Scripting (XSS) vulnerabilities
- How to document a security finding clearly: location, proof of concept, impact, and fix

---
**Internship:** CodeAlpha - Cyber Security Domain
**Task:** Task 3 - Secure Coding Review
