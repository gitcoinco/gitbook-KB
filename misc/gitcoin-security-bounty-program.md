---
description: >-
  Gitcoin Security Bounty Program Responsible Disclosure Policy & Bug Bounty
  Guidelines Version 2.0  |  Effective: Oct 2026  |  Scope: https://gitcoin.co
---

# Gitcoin Security Bounty Program

### 1. Purpose & Mission

Gitcoin is an open-source marketplace that funds public goods and connects developers with meaningful work. We manage real economic value on behalf of our users — including grant funding, bounty payouts, and contributor rewards. The security of our platform directly protects that value.

This Security Bounty Program exists because we believe the security community plays a critical role in keeping our platform safe. Responsible researchers who identify and privately disclose vulnerabilities protect our users before malicious actors can exploit them. In recognition of that contribution, we compensate researchers fairly for valid, in-scope findings.

We are committed to acting in good faith toward researchers who act in good faith toward us — acknowledging your reports promptly, communicating our findings clearly, and paying bounties in a timely manner once vulnerabilities are confirmed.

### 2. Program Scope

The bounty program applies exclusively to the primary Gitcoin web application and its authenticated/unauthenticated surfaces. Only the following domain is in scope:

https://gitcoin.co  (all paths under the primary domain)

**Out of Scope**

The following are explicitly excluded from the program:

* Subdomains not operated by Gitcoin (e.g., third-party integrations)
* Third-party services (Slack, WordPress, Intercom, cloud infrastructure providers, etc.)
* Vulnerabilities in past/unsupported versions of the software
* Issues affecting only deprecated features with documented end-of-life
* Bugs requiring physical access to a user's device
* Vulnerabilities affecting only outdated browsers (EOL browsers, IE 11, etc.)

### 3. Vulnerability Severity & Payout

Severity is assessed using the OWASP Risk Rating Methodology, which evaluates both the likelihood of exploitation and the impact on users, data, and platform integrity. The Gitcoin security team makes all final determinations on severity and payout eligibility.

**Payout Schedule**

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top"><strong>Severity</strong></td><td valign="top"><strong>Description</strong></td><td valign="top"><strong>Payout</strong> (<strong>USD</strong>)</td></tr><tr><td valign="top"><mark style="color:$danger;"><strong>Critical</strong></mark></td><td valign="top">Full account takeover, authentication bypass, RCE, mass data exfiltration, payment/fund manipulation</td><td valign="top">$800</td></tr><tr><td valign="top"><mark style="color:$warning;"><strong>High</strong></mark></td><td valign="top">Significant data exposure, privilege escalation, stored XSS impacting many users, IDOR with broad impact</td><td valign="top">$420</td></tr><tr><td valign="top"><mark style="color:pink;"><strong>Medium</strong></mark></td><td valign="top">Limited data leaks, CSRF on sensitive actions, reflected XSS, SSRF with limited impact</td><td valign="top">$200</td></tr><tr><td valign="top"><mark style="color:blue;"><strong>Low</strong></mark></td><td valign="top">Information disclosure, low-impact CSRF, self-XSS requiring unusual conditions, minor logic flaws</td><td valign="top">$50</td></tr></tbody></table>

Payouts are made in USDC. You must provide a valid Ethereum wallet address when submitting a report. Payouts will only be made to the first researcher who submits a qualifying report for a given vulnerability.

### 4. Eligible Vulnerability Types

The following represent examples of in-scope vulnerability classes. This list is not exhaustive — any significant, novel vulnerability affecting the platform's security may qualify.

* **Remote Code Execution (RCE):** Any vulnerability allowing arbitrary code execution on Gitcoin infrastructure.
* **SQL Injection:** Injections that expose, modify, or destroy database contents.
* **Authentication & Session Bypass:** Flaws allowing unauthorized access to accounts or bypassing login controls.
* **Broken Authorization / IDOR:** Accessing or modifying resources belonging to other users.
* **Privilege Escalation:** Gaining elevated permissions beyond what is authorized.
* **Stored Cross-Site Scripting (XSS):** Persistent script injection affecting other users.
* **Reflected Cross-Site Scripting (XSS):** Non-persistent script injection with meaningful user impact.
* **Cross-Site Request Forgery (CSRF):** Forcing authenticated users to perform unintended actions.
* **Server-Side Request Forgery (SSRF):** Making the server issue requests to internal or external systems.
* **Sensitive Data Exposure:** Unintended disclosure of PII, credentials, tokens, or financial data.
* **Business Logic Flaws:** Manipulation of application flows to gain unintended financial or platform advantages.
* **Mass Assignment / Parameter Pollution:** Modifying object properties not intended to be user-controlled.
* **Open Redirect (to phishing):** Redirects that enable credential harvesting from Gitcoin's domain.

### 5. Ineligible Issues

The following will not qualify for a payout under any circumstances:

* Denial of Service (DoS/DDoS) attacks or rate limiting
* Social engineering, phishing, or spear-phishing attacks
* Physical access attacks
* Self-XSS (requires the victim to execute the payload themselves)
* Clickjacking without a demonstrable, high-impact attack chain
* Man-in-the-Middle (MiTM) attacks requiring local network access
* Cache poisoning without meaningful user impact
* Missing security headers without a demonstrated exploit
* Missing DNS records (SPF, DMARC, etc.) without demonstrated exploit
* Brute force attacks against login or other endpoints
* Vulnerabilities in third-party services or platforms not operated by Gitcoin
* Stack traces, verbose errors, or debug information without exploitable impact
* SSL/TLS configuration issues without a practical attack scenario
* Open ports without a demonstrated exploit path
* CSV injection / formula injection without a practical attack
* Automated scan results submitted without a proof of concept

### 6. Submission Process & Flow

Follow the steps below to submit a report. Reports that do not follow this process, or that are disclosed publicly before a fix is deployed, will be disqualified.

**Step 1 — Verify the issue**  Confirm the vulnerability exists, is reproducible, and falls within the scope defined in Section 2. Do not test on accounts or data you do not own.

**Step 2 — Prepare your report** Write up a complete report using the template in Section 7 below. Ensure your proof of concept is clear, reproducible, and does not cause data loss or service disruption.

**Step 3 — Submit via email**  Email support@gitcoin.co with the subject line: \[SECURITY] \<short vulnerability title>. Encrypt your email if it contains sensitive credentials or PII.

**Step 4 — Await acknowledgment**  You will receive an acknowledgment within 7 business days confirming receipt and providing a reference ID. Do not follow up before this window closes.

**Step 5 — Triage & severity review**  The Gitcoin security team will reproduce your finding and assess severity using the OWASP Risk Rating Methodology. You will receive a triage decision within 14 business days of acknowledgment.

**Step 6 — Remediation**  Gitcoin will work to remediate validated findings within the SLA defined in Section 8. We may request your assistance testing the fix prior to deployment.

**Step 7 — Payout** Once the fix is confirmed and deployed, your bounty will be issued in USDC at the end of that calendar month.

**Step 8 — Coordinated disclosure** After remediation is complete, you are free to publish your research. We ask that you coordinate the timing with the Gitcoin team and give us at least 30 days after fix deployment before public disclosure.

### 7. Required Report Template

All submissions must include the following information. Incomplete reports will be returned for revision and may lose priority in the queue.

**Vulnerability Title:** _A concise, descriptive title (e.g., "Stored XSS in grant description field allows session hijacking")_

**Severity (Self-Assessed):** _Critical / High / Medium / Low — based on the OWASP model. Include your reasoning._

**Affected URL / Endpoint:** _The exact URL(s) or API endpoint(s) where the vulnerability exists._

**Vulnerability Type:** _The CWE or category (e.g., CWE-79 XSS, CWE-89 SQL Injection, CWE-352 CSRF)._

**Description:** _A clear explanation of the vulnerability: what it is, why it exists, and what an attacker can do with it._

**Impact:**  _The realistic worst-case impact if exploited in production — who is affected, what data is at risk, what actions can be taken._

**Steps to Reproduce:** _A numbered, step-by-step walkthrough that allows the Gitcoin team to reproduce the issue independently. Include all required preconditions (e.g., account type, specific page state)._

**Proof of Concept:** _One or more of the following: screenshot(s), screen recording, working exploit code, or a test payload. PoC must be non-destructive and must not access real user data._

**Suggested Remediation:**  _(Optional) Your recommendation for fixing the issue._

**Your Ethereum Address:** _Required for payout._

**Discovery Date:**  _When you first identified this vulnerability._

**Tools Used:** _(Optional) Any scanning tools, browser extensions, or proxies used during research._

### 8. Service Level Agreements (SLAs)

Gitcoin commits to the following response timelines for valid, in-scope reports. All timelines are in business days from the date of original submission.

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top"><strong>Milestone</strong></td><td valign="top"><strong>All</strong> <strong>Severities</strong></td><td valign="top"><strong>Critical</strong> (<strong>Expedited</strong>)</td></tr><tr><td valign="top">Initial Acknowledgment</td><td valign="top">7 business days</td><td valign="top">3 business days</td></tr><tr><td valign="top">Triage &#x26; Severity Confirmed</td><td valign="top">14 business days</td><td valign="top">7 business days</td></tr><tr><td valign="top">Fix Deployed (Critical)</td><td valign="top">—</td><td valign="top">30 calendar days</td></tr><tr><td valign="top">Fix Deployed (High)</td><td valign="top">60 calendar days</td><td valign="top">—</td></tr><tr><td valign="top">Fix Deployed (Medium / Low)</td><td valign="top">90 calendar days</td><td valign="top">—</td></tr></tbody></table>

### 9. Researcher Guidelines

Participation in this program requires adherence to the following rules. Violations will result in immediate disqualification and may be reported to law enforcement.

**You Must:**

* Use only your own account(s) for testing in the production environment.
* Obtain written permission before testing on any account other than your own.
* Stop testing immediately if you accidentally access another user's data, and disclose this access in your report.
* Provide enough detail for the Gitcoin team to reproduce and fix the issue.
* Maintain strict confidentiality — do not share, publish, or discuss the vulnerability until a fix is deployed.
* Coordinate public disclosure timing with the Gitcoin team (minimum 30 days post-fix).

**You Must Not:**

* Access, download, modify, or destroy data belonging to other users.
* Execute attacks that degrade service availability (DoS, DDoS, resource exhaustion).
* Conduct social engineering or phishing attacks against Gitcoin employees or users.
* Exploit vulnerabilities beyond the minimum necessary to prove impact.
* Disclose any vulnerability publicly or to any third party before remediation.
* Use automated scanning tools in ways that impact production performance.
* Make threats, ransom demands, or use unprofessional language in any communications.
* Submit reports for issues already known to the Gitcoin team or submitted by another researcher.

The Gitcoin team retains sole discretion over all bounty determinations, including severity classification, payout amounts, and eligibility. We value good-faith researchers and will treat them accordingly.

### **10. Contact**

Submit all security vulnerability reports privately and directly to:

support@gitcoin.co

Subject line format: \[SECURITY] \<short vulnerability title>

Reports must not be submitted publicly, posted to social media, filed as GitHub issues, or shared with any third party. Public disclosure of a vulnerability before a fix is deployed will automatically disqualify the submission from any payout.

_Gitcoin Security Bounty Program v2.0  |  support@gitcoin.co  |  https://gitcoin.co_
