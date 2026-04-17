# 🛡️ Zorvyn Phishing Case Study

### Real-World SOC Investigation Report

---

## 📌 Overview

This repository contains a real-world cybersecurity investigation into a suspicious internship offer that turned out to be a **coordinated phishing campaign targeting freshers**.

The case demonstrates how modern scams use **professional design, cloud infrastructure, and social engineering** to appear legitimate.

---

## 🎯 Objective

* Analyze suspicious email and offer letter
* Investigate domains and infrastructure
* Correlate OSINT findings
* Identify phishing indicators
* Document a SOC-style investigation

---

## 📥 Incident Summary

* Platform: LinkedIn
* Role: Cybersecurity Analyst Intern
* Key Observations:

  * No application submitted
  * Direct selection
  * No interview process
  * Offer letter with high stipend

---

## 📧 Email & Offer Letter Findings

* Professional formatting
* Pre-generated login credentials
* Immediate onboarding
* Reimbursement-based expense model

⚠️ **Red Flag:** Financial trap disguised as reimbursement

---

## 🌐 Domain Analysis

### zorvyn.io

* Status: `clientHold` (suspended)
* Hidden ownership

### zorvyn.live

* Newly registered (same timeline as attack)
* Used for onboarding and communication

🚨 **Key Insight:** Domain rotation strategy observed

---

## 🌐 Infrastructure Analysis

* Hosted on Microsoft Azure
* Multiple IP addresses used
* Inconsistent configuration across servers

### Findings:

* Domain mismatch
* Self-signed SSL certificate
* Public SSH exposure
* Unrelated hostname mapping

---

## 🧪 Threat Intelligence (VirusTotal)

* Some URLs → Clean
* Some → Suspicious
* Some → Phishing

⚠️ Mixed results indicate **inconsistent reputation**

---

## 🌍 OSINT Findings

* Multiple LinkedIn users reported:

  * Same workflow
  * Same domains
  * Payment requests

---

## 🕸️ Attack Flow

1. Unsolicited email
2. Fake assessment
3. Direct selection
4. Offer letter
5. Onboarding portal
6. Trust building
7. Payment request (inferred stage)

---

## 📊 Indicators of Compromise (IOCs)

### Domains:

* zorvyn.live
* zorvyn.io
* employeesupport.zorvyn.live

### IPs:

* 20.84.233.22
* 20.193.150.182

### Email:

* [hr@zorvyn.live](mailto:hr@zorvyn.live)

---

## ⚖️ Final Verdict

🔴 **Confirmed Phishing / Job Scam Campaign**

---

## 🛡️ Key Learnings

* Professional design ≠ legitimacy
* Cloud hosting ≠ trust
* Domain age matters
* Always verify before trusting

---

## 📸 Evidence

Screenshots included:

* Offer letter
* Email content
* VirusTotal results
* WHOIS data
* Shodan analysis
* LinkedIn reports

---

## ⚠️ Ethical Note

This investigation was conducted without engaging in risky actions (such as signing documents or making payments), ensuring safe and responsible analysis.

---

## 🚀 Author
Sana Mujawar
Cybersecurity Enthusiast | SOC Analyst Learner

---

## ⭐ If you found this useful

Consider starring the repo and sharing to spread awareness.
