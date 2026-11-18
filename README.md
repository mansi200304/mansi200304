<div align="center">

<img src="assets/header.svg" width="100%" alt="Mansi Ganga Nayak — security engineer and AI-security researcher" />

<br/>

**Observe quietly. Understand deeply. Build relentlessly.**

[◆ Portfolio](https://mansi200304.github.io/mansi-s_portfolio/) · [LinkedIn](https://linkedin.com/in/mansiganganayak) · [Email](mailto:mnayak12@asu.edu)

[⌁ Research](#02--research-desk) · [◉ Builds](#03--live-tools--builds) · [⚑ Hackathons](#04--hackathons) · [⌘ Signals](#06--systems--signals)

</div>

---

## 01 / The operator

I'm an **MS Computer Science (Cybersecurity)** candidate at **Arizona State University** (expected **December 2027**), and a **graduate research assistant in AI security** with **Prof. Gail-Joon Ahn**. I work across security engineering, digital forensics, cloud security, cryptography, and the security of AI systems.

My work moves between two questions:

- How do we make complex systems more secure?
- How do we make their decisions more understandable, verifiable, and trustworthy?

I've shipped browser-based security tools, event-driven incident-response pipelines on AWS, and explainable ML — and published across AI governance, biomedical AI, cryptography and blockchain.

<sub>TEMPE, ARIZONA · SECURITY ENGINEERING · AI SECURITY · DIGITAL FORENSICS</sub>

---

## 02 / Research desk

**9 peer-reviewed papers · 1 patent filed · 1 provisional in preparation** — spanning Carnegie Mellon IDeaS, Stanford PAI26 / NeurIPS, Yale BMES, Springer, DRDO and IJARESM.

| Work | Venue | Role |
|---|---|---|
| [**Hippo** — An Explainable, Security-by-Design Platform for Health Insurance](https://mansi200304.github.io/mansi-s_portfolio/) | Yale Biomedical Engineering Conference · 2026 | co-author · *provisional patent filing Jan 2027* |
| [**Autonomous Cyber Weapons as AI-Enabled Digital Harms**](https://www.cmu.edu/ideas-social-cybersecurity/events/ideas-conferences/2026_ideas_conference_paper__18.pdf) | IDeaS 2026, Carnegie Mellon University | first &amp; corresponding author |
| [**Democratic Accountability for Autonomous Systems**](https://www.cmu.edu/ideas-social-cybersecurity/events/ideas-conferences/2026_ideas_conference_paper__17.pdf) | IDeaS 2026, Carnegie Mellon University | co-author (equal contribution) |
| [**JetMAE** — How Colour Factors Explain 96% of a Neural Tagger's Decisions](https://openreview.net/attachment?id=nlt2r1P7yU&name=pdf) | PAI26, Stanford University / NeurIPS 2026 | co-author |
| [**Improving Situational Awareness of Autonomous Vehicles**](https://link.springer.com/chapter/10.1007/978-3-032-14156-9_35) | Springer Nature · Feb 2026 | author |
| [**Future Trends in Cybersecurity and Blockchain**](https://link.springer.com/chapter/10.1007/978-3-032-14156-9_37) | Springer Nature · Feb 2026 | author |
| **Quantum Cryptographic Encryption for P2P Robot Communication** | DRDO Centre for AI &amp; Robotics · 2024 | co-author |
| [**Enhancing Data Verification Through Privacy-Preserving Techniques**](https://ijaresm.com/uploaded_files/document_file/Mohammed_Emad_Sultan_SiddiqipInA.pdf) | IJARESM · 2024 | co-author |
| **Real Estate Price Predictor &amp; Minor Extractable Values (Front-Running)** | 2023 | author |

**Patent** · *SafeCount — Two-Step Verification Secure Voting System* · India, 2024 (filed).

> **Hippo** is in my AI-security wheelhouse: a three-tier architecture (Compare / Verify / Operations) that confines an LLM assistant to public plan data and computes rankings deterministically outside the model, so identity and health records stay behind authenticated verification — the assistant never touches protected data.

---

## 03 / Live tools &amp; builds

Two security tools you can run in the browser, plus the cloud and ML systems behind them. **[Try the live tools in the portfolio ↗](https://mansi200304.github.io/mansi-s_portfolio/)**

<table>
<tr>
<td width="50%" valign="top">

### ⌁ TriageLens — file forensics
`JavaScript` · `Web Crypto API`

Zero-upload triage: streams a file in the browser, computes SHA-256 / SHA-1, identifies true type across **18 magic-byte signatures**, flags extension spoofing, and scores Shannon entropy over a 256-bin histogram. Nothing ever leaves the page.

</td>
<td width="50%" valign="top">

### ⛨ IAMSentry — IAM least-privilege auditor
`JavaScript` · `AWS IAM`

Static analyzer that parses IAM policy JSON, compiles action wildcards to regex, and flags **30 privilege-escalation patterns** plus data-exfiltration, defense-evasion, public and cross-account exposure — scored 0–100, zero credentials, zero API calls.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ☁ Cloud Forensics Pipeline on AWS
`Lambda` · `EventBridge` · `GuardDuty` · `SSM` · `Python`

Event-driven IR: a GuardDuty finding triggers EBS snapshots, SSM memory capture, and EC2 isolation in seconds, each step written to an **append-only, hash-chained** chain-of-custody ledger on S3 with an independent verifier. &nbsp;[Repo ↗](https://github.com/mansi200304/cloud-forensics-pipeline)

</td>
<td width="50%" valign="top">

### ◉ Cloud Fraud &amp; Abuse Analyzer
`Python` · `XGBoost` · `Isolation Forest` · `SHAP`

ML pipeline detecting 5 cloud-abuse patterns (account takeover, crypto-mining, IAM escalation, exfiltration, API recon); Isolation Forest + XGBoost + K-Means into a 0–100 hourly per-account risk score with SHAP on every alert.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ⬡ BankSim Fraud-Detection Ensemble
`Python` · `pandas` · `scikit-learn`

Built three detectors on the BankSim dataset — Category Risk (**ROC-AUC 0.98**), Category Novelty (0.86), Time Gap (0.67). The novelty and time-gap detectors use no fraud labels, only each customer's earlier transactions — no leakage.

</td>
<td width="50%" valign="top">

### ⧉ Security Incident Response Framework
`Python` · `Sigma` · `YARA-L` · `Splunk`

Six MITRE ATT&amp;CK-mapped playbooks (phishing, ransomware, insider threat, lateral movement, cloud misconfig, DDoS) with Claude-API alert triage. &nbsp;[Repo ↗](https://github.com/mansi200304/security-incident-response-plan)

</td>
</tr>
</table>

---

## 04 / Hackathons

| Project | Event | What I did |
|---|---|---|
| **Sinkronized** | NASA Space Apps 2026 (*Dancing with the SARs* / NISAR) | Interactive map &amp; engineering — InSAR land-subsidence across five Arizona basins, validated against state radar (0.94–0.99 correlation). [Live](https://sinkronized.vercel.app/web/) · [Repo](https://github.com/mansi200304/NASA-Hackathon) |
| **Orbit** | Cubbie Hackathon · DevHacks ASU | Agent-to-agent coordination Skill — friends' assistants negotiate study times through a privacy-first relay, confirming once. [Live](https://orbit-cubbie.vercel.app) · [Repo](https://github.com/Manavpatel06/Orbit) |
| **ARC** | Devils Invent 2026 · Honeywell Aerospace × ASU | Owned the security &amp; radio layer — Ed25519 anti-spoofing caught all 7 attacks (ROC AUC 0.986), 0 false flags on 31 real aircraft. [Repo](https://github.com/Manavpatel06/FLOCK) |
| **Rice Matters** | AIR Spark Hackathon · ASU | Open-source OpenCode plugin that watches an AI coding agent and flags blocked, failed or falsely-completed tasks. [Repo](https://github.com/QuaanNguyen/border-collie) |

---

## 05 / GitHub

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=mansi200304&show_icons=true&hide_border=false&title_color=7a1f30&icon_color=3f6d93&text_color=2a0f16&bg_color=f3ecdf&border_color=d8c7b0" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mansi200304&layout=compact&langs_count=8&hide_border=false&title_color=7a1f30&text_color=2a0f16&bg_color=f3ecdf&border_color=d8c7b0" alt="Top languages" />

</div>

---

## 06 / Systems &amp; signals

**Security &amp; investigation**
![Incident Response](https://img.shields.io/badge/Incident_Response-7a1f30?style=flat-square&logoColor=f3ecdf)
![Digital Forensics](https://img.shields.io/badge/Digital_Forensics-7a1f30?style=flat-square)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-7a1f30?style=flat-square)
![Splunk](https://img.shields.io/badge/Splunk-7a1f30?style=flat-square&logo=splunk&logoColor=f3ecdf)
![YARA](https://img.shields.io/badge/YARA--L-7a1f30?style=flat-square)
![Sigma](https://img.shields.io/badge/Sigma-7a1f30?style=flat-square)

**Cloud &amp; infrastructure**
![AWS](https://img.shields.io/badge/AWS-7a1f30?style=flat-square&logo=amazonwebservices&logoColor=f3ecdf)
![Lambda](https://img.shields.io/badge/Lambda-7a1f30?style=flat-square&logo=awslambda&logoColor=f3ecdf)
![Docker](https://img.shields.io/badge/Docker-7a1f30?style=flat-square&logo=docker&logoColor=f3ecdf)
![Linux](https://img.shields.io/badge/Linux-7a1f30?style=flat-square&logo=linux&logoColor=f3ecdf)
![CI/CD](https://img.shields.io/badge/CI%2FCD-7a1f30?style=flat-square)

**Languages**
![Python](https://img.shields.io/badge/Python-7a1f30?style=flat-square&logo=python&logoColor=f3ecdf)
![Java](https://img.shields.io/badge/Java-7a1f30?style=flat-square&logo=openjdk&logoColor=f3ecdf)
![C++](https://img.shields.io/badge/C%2B%2B-7a1f30?style=flat-square&logo=cplusplus&logoColor=f3ecdf)
![JavaScript](https://img.shields.io/badge/JavaScript-7a1f30?style=flat-square&logo=javascript&logoColor=f3ecdf)
![SQL](https://img.shields.io/badge/SQL-7a1f30?style=flat-square&logo=postgresql&logoColor=f3ecdf)

**AI &amp; data**
![PyTorch](https://img.shields.io/badge/PyTorch-7a1f30?style=flat-square&logo=pytorch&logoColor=f3ecdf)
![scikit-learn](https://img.shields.io/badge/scikit--learn-7a1f30?style=flat-square&logo=scikitlearn&logoColor=f3ecdf)
![XGBoost](https://img.shields.io/badge/XGBoost-7a1f30?style=flat-square)
![SHAP](https://img.shields.io/badge/SHAP-7a1f30?style=flat-square)

**Cryptography**
![Post-Quantum](https://img.shields.io/badge/Post--Quantum-7a1f30?style=flat-square)
![AES RSA ECC](https://img.shields.io/badge/AES_RSA_ECC-7a1f30?style=flat-square)
![Differential Privacy](https://img.shields.io/badge/Differential_Privacy-7a1f30?style=flat-square)

---

## 07 / Certifications

AWS Academy Cloud Foundations · AI Fluency: Framework &amp; Foundations (Anthropic) · Palo Alto Networks Cybersecurity Fundamentals · Google — Networks &amp; Network Security · Google — Manage Security Risks · Cybersecurity for Everyone (University of Maryland)

---

<div align="center">

**MANSI GANGA NAYAK**

<sub>RESEARCH WITH INTENT · ENGINEERING WITH PRECISION</sub>

[◆ Portfolio](https://mansi200304.github.io/mansi-s_portfolio/) · [LinkedIn](https://linkedin.com/in/mansiganganayak) · [Email](mailto:mnayak12@asu.edu)

</div>
