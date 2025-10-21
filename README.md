# 🛡️ Phishing Email Analysis — Task 2

This repository presents the analysis of a **real phishing email impersonating Banco do Bradesco (Bradesco Livelo)**.  
It was created as part of a **Cybersecurity Internship Project — Task 2**, focusing on real-world **email threat forensics** and **phishing detection** techniques.

---

## 📘 Overview

Phishing attacks continue to be one of the most common and dangerous social engineering threats.  
In this task, a fraudulent email was analyzed in detail to uncover **spoofing**, **authentication failures**, and **social engineering tactics** designed to deceive users.

The analyzed email falsely claims that *Bradesco Livelo points are about to expire*, using **urgency** to push recipients into clicking malicious links.

---

## 🎯 Objectives

- Identify **spoofing** and **impersonation** techniques  
- Analyze **email headers** for anomalies  
- Decode and inspect **HTML and Base64 content**  
- Highlight **urgency-based manipulation** tactics  
- Document technical findings in a **forensic report**

---

## 🧰 Tools & Techniques Used

- 🧾 **MXToolbox** — DNS, SPF, DKIM, and header validation  
- 🔍 **Whois & IP Lookup** — Trace sender origin  
- 🧩 **Base64 Decoding** — Reveal hidden HTML payloads  
- 🕵️ **Manual Header Inspection** — Identify spoofing and authentication failures  
- 💻 **Text & HTML Analysis** — Extract and verify embedded URLs

---

## 📂 Repository Structure

```
📦 Final_Phishing_Email_Analysis_Task2
├── 📁 data
│   └── phishing_email.eml            # Raw email file
├── phishing_email_sample.txt         # Raw phishing email sample
├── Phishing_Email_Analysis_Report.md # Detailed technical analysis
└── README.md                         # Project overview (this file)
```

---

## 🔍 Key Findings

| Indicator | Description |
|------------|--------------|
| 🕵️ **Spoofed Domain** | The sender pretends to be Bradesco but uses `@atendimento.com.br` |
| ⚠️ **Return Path Mismatch** | Real Bradesco emails would return to `@bradesco.com.br` |
| ❌ **SPF/DKIM/DMARC Failures** | Authentication mechanisms failed or missing |
| ⚡ **Urgent Tone** | Subject line: *"Your points expire today!"* — triggers emotional response |
| 🌐 **Suspicious IP Origin** | Originated from DigitalOcean (not affiliated with Bradesco) |
| 🔗 **Fake Links** | Redirects to unrelated domain `blog1seguimentmydomine2bra.me` |

---

## 🧠 Summary of the Phishing Email

**Subject:** “CLIENTE PRIME - BRADESCO LIVELO: Seu cartão tem 92.990 pontos expirando hoje!”  
**From:** `BANCO DO BRADESCO LIVELO <banco.bradesco@atendimento.com.br>`  
**Return Path:** `root@ubuntu-s-1vcpu-1gb-35gb-intel-sfo3-06`  
**Origin IP:** `137.184.34.4` (DigitalOcean VPS, not Bradesco)

The message creates a false sense of urgency and includes links disguised as Bradesco resources, leading to a **credential harvesting page**.

---

## 🚀 Internship Context

This project was developed as part of a **Cybersecurity Internship (Task 2)** to demonstrate:
- Practical understanding of **phishing forensics**
- Hands-on experience with **email authentication analysis**
- Real-world skills in **threat documentation and communication**

---

## 📌 How to Use

1. Open `phishing_email_sample.txt` to view the raw phishing email.  
2. Use **MXToolbox** or manual header inspection for authentication checks.  
3. Decode Base64 segments (if any) to extract HTML or hidden URLs.  
4. Review `Phishing_Email_Analysis_Report.md` for complete technical findings.  
5. Apply insights to **train users** or **enhance email security filters**.

---

## 🧩 Learning Outcomes

- Gained practical knowledge of **phishing email structures**  
- Enhanced ability to **detect spoofing and header anomalies**  
- Improved **technical reporting and documentation** skills  
- Strengthened understanding of **email-based social engineering**

---
  
### **Author**
- **Cybersecurity Intern – Task 2** 
- Your Name : DHANUSH S 
- Date: 21 Oct 2025

