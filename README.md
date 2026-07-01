<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a1f6e,100:00c6ff&height=200&section=header&text=Mansi%20Ganga%20Nayak&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=I%20build%20things%20that%20catch%20bad%20actors%20before%20humans%20can&descSize=15&descAlignY=58&animation=fadeIn" width="100%"/>
</div>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/mansiganganayak)
[![Portfolio](https://img.shields.io/badge/-Cybersecurity%20Portfolio-FF6B6B?style=flat-square&logo=githubpages&logoColor=white)](https://mansi200304.github.io/Cybersecurity-Portfolio---Mansi-Ganga-Nayak)
[![XR Portfolio](https://img.shields.io/badge/-XR%20%26%20Security%20Portfolio-8A2BE2?style=flat-square&logo=githubpages&logoColor=white)](https://mansi200304.github.io/XR-and-Cybersecurity-Portfolio/)
[![Email](https://img.shields.io/badge/-mnayak12@asu.edu-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:mnayak12@asu.edu)

</div>

---

```python
# What I actually do
def mansi():
    return {
        "currently_obsessed_with" : "Building an AWS fraud detection pipeline that catches
                                     crypto miners, account hijackers, and data thieves
                                     before a human analyst even opens their laptop",

        "how_i_think"            : "Like an attacker first, a defender second,
                                     and a data analyst third",

        "tools_i_reach_for"      : ["Python", "AWS", "XGBoost", "SHAP", "spaCy",
                                     "Splunk", "Wireshark", "Three.js", "Streamlit"],

        "things_i_have_shipped"  : ["WebXR security trainer running at 90fps with a
                                     vocal AI narrator and live cyber threat globe",
                                    "SIEM pipeline on AWS detecting intrusions in < 2 min",
                                    "Post-quantum encrypted comms for 5 DRDO military robots",
                                    "Blockchain voting system — patent filed"],

        "random_fact"            : "Presented at Stanford PAI26 2026. The paper uses SHAP
                                     to explain why a neural net makes decisions — same
                                     technique I use to explain why my fraud model flags
                                     an AWS account at 3am.",
    }
```

---

## 🔨 What I'm building right now

### AWS Cloud Fraud Detection & Abuse Pattern Analyzer

Not a tutorial project. An actual end-to-end ML pipeline I'm building from scratch —
every line of code written and owned by me, no black-box APIs, no shortcuts.

**The problem it solves:** AWS accounts get compromised constantly. Attackers spin up GPU
instances to mine crypto, exfiltrate data through S3, escalate IAM privileges, or sell
the stolen credentials. The industry average time to catch this? **197 days.**
My pipeline catches it in **under 30 minutes.**

**How it works:**

```
CloudTrail + GuardDuty + IAM + VPC Flow + Billing API
        ↓
  Lambda ingestion → S3 → Athena (50,000+ events/day)
        ↓
  40+ behavioral features engineered per account per hour
  (velocity, geo-distance, time deviation, cost spikes)
        ↓
  ┌─────────────────────────────────────────┐
  │  Isolation Forest  →  novel anomalies   │
  │  XGBoost           →  fraud type label  │  → weighted ensemble → 0-100 risk score
  │  K-Means           →  ring detection    │
  └─────────────────────────────────────────┘
        ↓
  spaCy + regex IOC extractor
  SHAP waterfall → "why was this account flagged?"
        ↓
  Streamlit dashboard (analyst view + exec view)
  SNS → Slack alert fires when risk score > 70
```

**What I'm detecting:** account takeover · crypto mining · data exfiltration ·
IAM privilege escalation · API reconnaissance · impossible travel · Tor access · billing abuse

**Stack:** `Python` `AWS Lambda` `S3` `CloudTrail` `GuardDuty` `Kinesis` `Athena`
`XGBoost` `scikit-learn` `SHAP` `spaCy` `Streamlit` `MLflow` `Step Functions` `SNS`

**Target:** F1 > 0.92 · FPR < 8% · Detection < 30 min · 500 accounts · 90 days · 45M events

---

## 🚀 Things I've shipped

<table>
<tr>
<td width="50%" valign="top">

### 🌐 VR Security Training — Jarvis Cyber Command Center
[`Three.js`] [`WebXR`] [`GLSL`] [`Web Speech API`]

Built a browser-based immersive cybersecurity training environment —
no headset required, runs at **90fps with only 19 draw calls**
(instanced rendering + zero-allocation render loops).

The fun part: a rotating holographic threat globe, concentric
orbit rings spinning in opposite directions, pulsating radar
wavefronts, and a vocal AI narrator (native `SpeechSynthesis`)
that reads out threats as you resolve them — *"Exposed electrical
cables successfully insulated on Server Rack Four Bravo."*

- ✅ 0 build errors
- ✅ 6/6 Vitest unit tests passing
- ✅ Custom GLSL shader materials for all holographic effects
- ✅ Scrolling live telemetry panel with real-time cyber event feed

</td>
<td width="50%" valign="top">

### ☁️ Cloud SIEM Pipeline
[`AWS`] [`Splunk`] [`Python`] [`Lambda`] [`CloudWatch`]

Deployed a production-equivalent SIEM on AWS aggregating
**10,000+ daily log events** across endpoint, network,
and cloud sources.

Wrote 6 custom detection rules from scratch covering:
brute force · lateral movement · privilege escalation ·
data exfiltration · C2 beaconing · unauthorized access

**Mean detection time: under 2 minutes** on simulated
intrusion scenarios. Everything automated — Lambda triggers,
S3 log storage, CloudWatch alerting, Splunk dashboards.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛡️ Security Incident Response Framework
[`Python`] [`YARA-L`] [`Sigma`] [`Splunk`] [`NIST`]

Built a complete enterprise IR framework — not a template,
an actual working system with:

- 6 MITRE ATT&CK-mapped playbooks (phishing, ransomware,
  insider threat, lateral movement, cloud misconfig, DDoS)
- YARA-L + Sigma detection rules for each scenario
- Python automation: isolate host, block IP, disable account,
  create ticket, page analyst — all triggered automatically
- KPI tracker: MTTD/MTTR per incident, SLA compliance,
  false positive rate trends

Frameworks: NIST SP 800-61r2 · MITRE ATT&CK · ISO 27001 · SOC 2

</td>
<td width="50%" valign="top">

### 🗳️ SafeCount — Secure Voting System
[`Blockchain`] [`RFID`] [`Biometrics`] [`Solidity`] [`RBAC`]

**Patent filed (India, 2024)**

3-factor authenticated EVM: RFID + facial recognition +
fingerprint. Every vote is blockchain-verified with a
tamper-evident audit trail.

Deployed in 1 institutional pilot.
Result: **100% of identified proxy voting vectors eliminated.**

The patent covers the novel security architecture combining
hardware biometrics with on-chain vote verification.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔐 Post-Quantum Robot Comms — IIT Kanpur / DRDO
[`CRYSTALS-Kyber`] [`AES-256`] [`Python`] [`Linux`]

Secured P2P communications across **5 DRDO military robots**
(DAKSH, NETRA, CSROV, SROV, UXOR) using 8+ cryptographic
protocols including CRYSTALS-Kyber post-quantum encryption.

Eliminated 3 legacy unencrypted communication channels.
Zero breach incidents during deployment.

Published 3 papers from this work. Filed 1 patent.
Under Professor Sandeep Shukla (now Director, IIIT Hyderabad).

</td>
<td width="50%" valign="top">

### 🤖 CyberGuard AI Security Assistant
[`Python`] [`NLP`] [`REST API`] [`Web Speech API`]

*In active development*

Security training platform with 15+ adaptive threat scenarios
covering phishing, social engineering, ransomware, and lateral
movement. JARVIS voice interface, IOC extraction pipeline,
and output validation layer.

Built with a custom NLP pipeline — spaCy for entity extraction,
Jinja2 templates for structured scenario generation, regex
IOC extractor for IPs, hashes, domains, and ARNs.

</td>
</tr>
</table>

---

## 🧠 How I think about problems

I don't just use tools — I understand why they work.

**Detection engineering:** I write YARA-L and Sigma rules by hand because I understand
the log structures they're matching against. I know why `failed_api_rate` is a better
fraud signal than `total_api_calls`.

**ML for security:** I chose an ensemble of three models for fraud detection because
each one catches a different thing — Isolation Forest for novel patterns (no labels needed),
XGBoost for known fraud types (supervised), K-Means for coordinated rings (clustering).
One model would miss two of those three.

**Explainability matters:** I use SHAP on every ML alert because in a security context,
"the model flagged it" is not an answer. You need to say "this account was flagged because
`impossible_travel_flag` fired, `gpu_instance_count` spiked 24x, and `failed_api_rate`
was 3.2x above baseline." That's what SHAP gives you.

**Physics → Security:** My Stanford paper applied SHAP to explain why a neural net
classifies particle jets. Same interpretability technique, same mathematical framework —
just applied to fraud instead of quarks.

---

## 🛠️ Full toolkit

<div align="center">

**I write code in**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)
![C/C++](https://img.shields.io/badge/C%2FC%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![GLSL](https://img.shields.io/badge/GLSL-Shaders-5C3EE8?style=for-the-badge&logoColor=white)

**I do ML with**

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-0073B7?style=for-the-badge&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-Explainability-6C3483?style=for-the-badge&logoColor=white)
![spaCy](https://img.shields.io/badge/spaCy-NLP-09A3D5?style=for-the-badge&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)

**I deploy on**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

**I detect threats with**

![Splunk](https://img.shields.io/badge/Splunk-000000?style=for-the-badge&logo=splunk&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Palo Alto](https://img.shields.io/badge/Palo%20Alto%20NGFW-FA582D?style=for-the-badge&logo=paloaltonetworks&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp%20Suite-FF6633?style=for-the-badge&logo=burpsuite&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=for-the-badge&logoColor=white)
![YARA](https://img.shields.io/badge/YARA--L-Rules-CC0000?style=for-the-badge&logoColor=white)
![Sigma](https://img.shields.io/badge/Sigma-Rules-4A90D9?style=for-the-badge&logoColor=white)

**I visualize data with**

![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
![PowerBI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

**I think in**

![MITRE ATT&CK](https://img.shields.io/badge/MITRE%20ATT%26CK-E50914?style=for-the-badge&logoColor=white)
![NIST](https://img.shields.io/badge/NIST%20CSF-003087?style=for-the-badge&logoColor=white)
![ISO 27001](https://img.shields.io/badge/ISO%2027001-005F99?style=for-the-badge&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP%20Top%2010-000000?style=for-the-badge&logo=owasp&logoColor=white)

**I render 3D with**

![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white)
![WebXR](https://img.shields.io/badge/WebXR-VR%2FAR-7B2FBE?style=for-the-badge&logoColor=white)
![Unity](https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white)
![Blender](https://img.shields.io/badge/Blender-F5792A?style=for-the-badge&logo=blender&logoColor=white)

</div>

---

## 📚 Published research

**[JetMAE — PAI26 Stanford / NeurIPS 2026](https://openreview.net/attachment?id=nlt2r1P7yU&name=pdf)**

Trained a masked autoencoder on jet physics observables (1M jets, LHC data).
Used SHAP to show that **one variable — constituent multiplicity — explains 96%
of the neural network's decisions.** Then used symbolic regression (PySR) to
distill the entire neural net into a single formula: `(0.663 − 0.229n)²`

AUC 0.8769 · pre-training gain +1.35% ± 0.28% (p=0.014) · statistically significant

*Why this matters for security:* The same SHAP + symbolic distillation pipeline
I used to explain a particle physics model is what I now use to explain why my
fraud detection model flags an AWS account. Interpretability is interpretability.

---

**[Quantum Crypto for Military Robot Comms — DRDO 2024](https://drive.google.com/file/d/1y1S-4z8VWZj9rMacXHrjvW3rh4hd9Lzg/view)**
CRYSTALS-Kyber post-quantum encryption across 5 live DRDO robots · 3 unencrypted channels eliminated

**[Privacy-Preserving Data Verification — IJARESM 2024](https://ijaresm.com/uploaded_files/document_file/Mohammed_Emad_Sultan_SiddiqipInA.pdf)**
Differential privacy + secure multi-party computation for large-scale analytics

**[Autonomous Vehicle Situational Awareness — Springer 2026](https://link.springer.com/chapter/10.1007/978-3-032-14156-9_35)**

**[Future Trends in Cybersecurity & Blockchain — Springer 2026](https://link.springer.com/chapter/10.1007/978-3-032-14156-9_37)**

**Patent:** SafeCount — Two-Step Verification Based Secure Voting System *(Filed India, 2024)*

---

## 📊 Stats

<div align="center">

<img height="170em" src="https://github-readme-stats.vercel.app/api?username=mansi200304&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&title_color=00c6ff&icon_color=00c6ff&text_color=c9d1d9&bg_color=0d1117"/>
<img height="170em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mansi200304&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&title_color=00c6ff&text_color=c9d1d9&bg_color=0d1117"/>

</div>

<div align="center">

![Streak](https://github-readme-streak-stats.herokuapp.com/?user=mansi200304&theme=tokyonight&hide_border=true&ring=00c6ff&fire=00c6ff&currStreakLabel=00c6ff)

</div>

---

## 📍 What I'm looking for

I want to work somewhere that has **real data, real threats, and real stakes.**
I'm not looking to watch dashboards — I want to build the systems that feed them.

Open to: SOC Analyst · Security Engineer · AI/ML Security · Security Business Analyst
· Threat Intelligence · Cloud Security · Fraud & Risk Analytics · Internship

📍 Tempe, AZ · Night shift available · F-1 OPT May 2027 · No sponsorship required

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00c6ff,100:1a1f6e&height=100&section=footer" width="100%"/>

![Views](https://komarev.com/ghpvc/?username=mansi200304&color=00c6ff&style=flat-square&label=profile+views)

</div>
