# Task-2
Email Analysis 

🛡️ Task 2: Analyze a Phishing Email Sample

🎯 Objective

To analyze a suspicious email and identify common phishing indicators, helping improve email security awareness and threat detection skills.

---

🧰 Tools Used

- 📧 Email Client (e.g., Google mail,Outloo,kThunderbird) or Sample Email Viewer
- 🕵️‍♂️ [MxToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- 🔬 [VirusTotal](https://www.virustotal.com/)
- 📝 Text Editor or Email Viewer

---

📂 Sample Email File

> ⚠️ This file is for educational analysis only. Do not open in an active inbox. Use a **sandbox** or offline viewer.

---

📝 Steps Followed

1. Obtain a Sample Phishing Email
A phishing email was collected from my spam folder of mail for educational purpose only and saved as `.eml`.

2. Examine the Sender
- domain: `support@nqt-exam.com` pretending to be `nqt-exam.com`, `ggzc5.r.sp1-brevo.net`
- IP address: `77.32.149.27`

3. Analyze Email Headers
Used MxToolbox Header Analyzer:

🖼️ ![Header Analysis](screenshots/header-analysis.png)

- SPF: ❌ Fail  
- DKIM Authenticated : ❌ Fail  
- Return-Path: `bounces-ggzc5-support=nqt-exam.com@shared-p100-i27.d.sp1-brevo.net`

4. Review Links & Attachments
- Hovered over embedded links:
🖼️ ![Link Hover Analysis](screenshots/suspicious-link-hover.png)
		1. https://ggzc5.r.sp1-brevo.net/mk/cl/f/sh/1t6Af4OiGsE8LH4vhmZMmLkiFOHM7N/t9g_FkxBVMrl
		2. https://ggzc5.r.sp1-brevo.net/mk/cl/f/sh/1t6Af4OiGsDg0YsVJQTRc5gsrZIcPJ/naF38sxg-dWt
		3. ggzc5.r.sp1-brevo.net

- VirusTotal confirms the link is flagged:
🖼️ ![VirusTotal Scan](screenshots/virustotal-url-scan.png)

5. Language Analysis
- Found urgency and fear-based language


---

📄 Sample Report Summary

| Indicator            | Found | Details                                      |
|----------------------|-------|----------------------------------------------|
| Sender               | ✅    | `support@nqt-exam.com`                       |
| SPF/DKIM Fail        | ✅    | Email auth failed (see headers)              |
| Suspicious Links     | ✅    | Hover reveals non-suspicious URL             |
| Threatening Language | ✅    | “Act now to avoid suspension”                |


📌 Conclusion: This is a confirmed it's not a phishing email, and the url are also not malicious link.

---

📸 Screenshots

| Description                        | Screenshot |
|-----------------------------------|------------|
| Header Analysis                   | ![Header](screenshots/header-analysis.png) |
| Suspicious Link Hover             | ![Link Hover](screenshots/suspicious-link-hover.png) |
| VirusTotal URL Scan               | ![VirusTotal](screenshots/virustotal-url-scan.png) |

---

✅ Key Takeaways

- Check SPF/DKIM to verify sender authenticity.
- Look for urgency, bad grammar, and mismatched URLs.
- Hover links `before clicking`.
- Scan links/files on [VirusTotal](https://www.virustotal.com/).

---

⚠️ Legal & Ethical Use

This project is for **educational and research** purposes only.  
**Do not open** `.eml` files in a live inbox or interact with suspicious links.



