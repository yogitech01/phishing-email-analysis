# Phishing Email Analysis

## Objective
Analyze a sample phishing email and identify indicators of phishing based on sender details, links, urgency, and overall content.

---

## Sample Email (Attached)
See `phishing_email.txt` for the full content.

**Sample Content Preview:**


Subject: Urgent - Your account will be suspended!
From: support@secure-paypal.com

Dear Customer,

We noticed unusual activity in your PayPal account.
Click the link below to verify your account or it will be suspended within 24 hours:

http://paypal-verification-login.com

Thank you,
PayPal Security Team



---

## Findings

### 1. Sender Address Spoofing
- **Observed:** `support@secure-paypal.com`
- **Expected:** Official PayPal emails come from `@paypal.com`.
- **Risk:** Attackers use similar-looking domains to trick users.

### 2. Suspicious Links
- **Observed:** `http://paypal-verification-login.com`
- **Expected:** Official PayPal domain is `https://www.paypal.com`.
- **Risk:** Likely leads to a fake website designed to steal credentials.

### 3. Urgent / Threatening Language
- **Observed:** “Your account will be suspended within 24 hours.”
- **Risk:** Designed to create panic and force quick, careless actions.

### 4. Generic Greeting
- **Observed:** “Dear Customer” (instead of the user’s real name).
- **Risk:** Indicates a bulk/phishing email rather than a legitimate targeted message.

### 5. Grammar and Style
- **Observed:** Slightly unnatural language and formatting.
- **Risk:** Often seen in phishing campaigns.

### 6. Attachments
- **Observed:** None in this sample.
- **Risk:** Many phishing emails contain malicious attachments (e.g., `.zip`, `.exe`).

---

## Conclusion
This sample email clearly shows multiple phishing indicators:
- Spoofed sender address  
- Fake login link  
- Urgency and threatening language  
- Generic greeting  

These traits confirm that this email is **phishing** and should be treated as malicious. Users should avoid clicking on any links or providing personal information.

---

## Tools Used
- Manual inspection of email content
- Optional: Online email header analyzer (e.g., MxToolbox)

---

**Internship Task Completed ✅**

