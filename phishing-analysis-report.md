# 🛡️ Phishing Email Analysis Report

## 📧 Subject: 
**Mion's live TV appearance threatens his career: explore his story**

## 🕵️ Phishing Characteristics Identified:

| # | Indicator | Details |
|--|-----------|---------|
| 1 | **Suspicious Sender Domain** | The email was sent from `ifdlae@inbridgepvt.com`, which is not a trusted or known domain. |
| 2 | **Unusual Subject Line** | The subject seems clickbait and emotionally manipulative to lure users in. |
| 3 | **Suspicious Links** | Links in the HTML body redirect to `https://ncmtrading.com/...` — unrelated to the claimed content. Hover reveals mismatch. |
| 4 | **Language & Urgency** | Body uses fear tactics like "threatens his career" to provoke emotional clicks. |
| 5 | **URL Obfuscation** | URL parameters (`ryQvSfXqYr=...`) are encoded to hide true purpose and make it harder to read. |
| 6 | **Tracking Pixel** | `<img src="...1px..." />` is used to track if the email was opened. Typical in malicious campaigns. |
| 7 | **No Personalization** | The email is generic and does not mention the recipient's name. |
| 8 | **HTML-only Format** | No plaintext version is included — commonly used in phishing to hide content in plain view. |
| 9 | **Spoofed Look** | The sender appears legitimate (uses TLS, SPF passed), but the email content is socially engineered. |
| 10 | **Unsubscribe Link** | Often fake — leads back to same suspicious domain. A trap to confirm active emails. |

---

## 🔍 Header Analysis Summary

- **SPF:** ✅ Passed (Domain authorized the IP to send)
- **DKIM:** ❌ Not Signed
- **DMARC:** 🟡 Best-guess pass — not strict validation
- **Sender IP:** `23.83.212.50` — linked to relay/mailchannels.net
- **Return Path:** `ifdlae@inbridgepvt.com`
- **User Agent:** `smtpclient.apple` — suspicious & spoofed

Tool used: [https://mxtoolbox.com/EmailHeaders.aspx](https://mxtoolbox.com/EmailHeaders.aspx)

---

## 💡 Conclusion

This email uses **social engineering**, **spoofed headers**, and **malicious redirection** to manipulate recipients. It demonstrates typical phishing tactics — emotionally charged subject, shady links, and tracking.

---

## 📂 Files in This Repo

- `phishing-email-headers.txt`: Raw phishing email and header
- `phishing-analysis-report.md`: Report of analysis
- `README.md`: Project overview
