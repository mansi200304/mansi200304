<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,40:1a1f6e,100:00c6ff&height=220&section=header&text=Mansi%20Ganga%20Nayak&fontSize=48&fontColor=ffffff&fontAlignY=40&desc=Cybersecurity%20Researcher%20%E2%80%A2%20AI%20Security%20%E2%80%A2%20Published%20Author%20%E2%80%A2%20Stanford%20PAI26&descSize=14&descAlignY=60&animation=fadeIn" width="100%"/>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/mansiganganayak)
[![Portfolio](https://img.shields.io/badge/Cybersecurity%20Portfolio-%23FF6B6B.svg?style=for-the-badge&logo=githubpages&logoColor=white)](https://mansi200304.github.io/Cybersecurity-Portfolio---Mansi-Ganga-Nayak)
[![XR Portfolio](https://img.shields.io/badge/XR%20%26%20Security%20Portfolio-%238A2BE2.svg?style=for-the-badge&logo=githubpages&logoColor=white)](https://mansi200304.github.io/XR-and-Cybersecurity-Portfolio/)
[![Email](https://img.shields.io/badge/Email-%23D14836.svg?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mnayak12@asu.edu)

</div>

---

## About Me

MS Cybersecurity student at Arizona State University (GPA 4.0) with research published across Stanford, Springer, and DRDO — and a patent filed for a cryptographic voting system. I work at the intersection of AI, security engineering, and research: building detection pipelines, securing military robot communications, training immersive VR security environments, and applying ML interpretability to real-world threat analysis. Five peer-reviewed publications. One patent. Presented at Stanford PAI26 2026 alongside Anthropic, MIT, and Berkeley Lab.

I care about building systems that are not just functional but explainable — because in security, knowing *why* something was flagged matters as much as the flag itself.

📍 Tempe, AZ &nbsp;|&nbsp; F-1 · OPT May 2027 · No sponsorship required at start

---

## Research & Publications

> 5 peer-reviewed papers · 1 patent · Stanford · Springer · DRDO · IJARESM

<br/>

### [JetMAE: How Colour Factors Explain 96% of a Neural Tagger's Decisions](https://openreview.net/attachment?id=nlt2r1P7yU&name=pdf)
**PAI26 Stanford University / NeurIPS 2026** &nbsp;·&nbsp; *Mansi Ganga Nayak, Samarjeet Malik, Mugdha Raje Ashiya, Gaurav Harit*

We introduce JetMAE, a masked autoencoder (MAE) that treats each of 12 hand-crafted jet observables as an independent token and pre-trains by masked reconstruction before fine-tuning for quark/gluon classification on 1 million LHC jets. MAE pre-training yields AUC 0.8769 — a statistically significant gain of +1.35% ± 0.28% over random initialisation (paired t-test p=0.014). SHAP attribution identifies constituent multiplicity as the dominant discriminator, consistent with the QCD colour-factor ratio CA/CF = 9/4. PySR symbolic regression then distils 95.9% of neural AUC into a single closed-form expression in multiplicity alone — making the model fully interpretable without sacrificing performance. The interpretability pipeline (SHAP + symbolic distillation) has direct application to AI hallucination detection and decision transparency in agentic security systems.

`Transformer` `Masked Autoencoder` `SHAP` `Symbolic Regression` `PyTorch` `scikit-learn`

<br/>

### [Quantum Cryptographic Encryption for P2P Robot Communication](https://drive.google.com/file/d/1y1S-4z8VWZj9rMacXHrjvW3rh4hd9Lzg/view)
**DRDO Centre for AI and Robotics, 2024** &nbsp;·&nbsp; *Under Prof. Sandeep Shukla, IIT Kanpur*

This paper presents a multi-layered cryptographic framework securing peer-to-peer communications across five DRDO military robots — DAKSH, NETRA, CSROV, SROV, and UXOR. We designed and deployed 8+ protocols including CRYSTALS-Kyber post-quantum key encapsulation, AES-256 symmetric encryption, RSA-4096 asymmetric encryption, ECC, SHA-256 integrity hashing, and Diffie-Hellman key exchange. Three legacy unencrypted communication channels were identified and eliminated with zero breach incidents during the deployment window. The framework establishes a replicable security architecture for autonomous systems operating in adversarial environments where classical encryption is vulnerable to quantum attacks.

`CRYSTALS-Kyber` `Post-Quantum Cryptography` `AES-256` `RSA-4096` `ECC` `P2P Security` `Linux`

<br/>

### [Enhancing Data Verification through Privacy-Preserving Techniques](https://ijaresm.com/uploaded_files/document_file/Mohammed_Emad_Sultan_SiddiqipInA.pdf)
**IJARESM, September 2024**

This paper investigates privacy-preserving mechanisms for large-scale data verification workflows where traditional approaches expose sensitive information during the validation process. We implement and evaluate differential privacy mechanisms — calibrated Laplace and Gaussian noise addition — alongside secure multi-party computation (SMPC) protocols that allow multiple parties to jointly verify data correctness without revealing their individual inputs. The work demonstrates measurable accuracy-privacy trade-offs across dataset scales, providing a framework for organisations that must satisfy regulatory requirements (GDPR, HIPAA) while maintaining analytical utility. Findings are benchmarked against standard non-private baselines.

`Differential Privacy` `Secure Multi-Party Computation` `Python` `Cryptography` `GDPR` `HIPAA`

<br/>

### [Improving Situational Awareness of Autonomous Vehicles to Ensure Safe Navigation](https://link.springer.com/chapter/10.1007/978-3-032-14156-9_35)
**Springer, February 2026**

This paper addresses the challenge of real-time environmental perception in autonomous vehicles operating under adverse conditions — sensor noise, occlusion, and adversarial interference. We propose a multi-modal situational awareness framework that fuses LiDAR, camera, and radar inputs through a late-fusion architecture, applying attention mechanisms to weight sensor reliability dynamically. The framework improves object detection accuracy in low-visibility scenarios and introduces a threat-scoring module that flags potentially adversarial objects in the vehicle's path. Results are evaluated on standard AV safety benchmarks with improvements in both detection latency and false negative rate for critical obstacle classes.

`Autonomous Vehicles` `Sensor Fusion` `LiDAR` `Computer Vision` `Attention Mechanisms` `Safety`

<br/>

### [Future Trends in Cybersecurity and Blockchain](https://link.springer.com/chapter/10.1007/978-3-032-14156-9_37)
**Springer Book Chapter, February 2026**

This chapter provides a structured analysis of converging trends shaping the next decade of cybersecurity and blockchain technology. We examine the threat landscape evolution driven by AI-powered attacks, the transition to post-quantum cryptographic standards (NIST PQC), and the role of zero-trust architecture in distributed enterprise environments. On the blockchain side, we analyse smart contract vulnerability patterns, consensus mechanism security trade-offs, and the emerging use of blockchain for tamper-evident audit trails in regulated industries. The chapter synthesises findings across academic literature and industry threat intelligence to produce actionable projections for practitioners and researchers.

`Post-Quantum Cryptography` `Zero-Trust` `Blockchain Security` `Smart Contracts` `Threat Intelligence`

<br/>

**Patent:** SafeCount — Two-Step Verification Based Secure Voting System &nbsp;·&nbsp; *Filed, India, 2024*

---

## Projects

<table>
<tr>
<td width="50%" valign="top">

**🌐 VR Security Training — Jarvis Cyber Command Center**
`Three.js` `WebXR` `GLSL Shaders` `Web Speech API` `Vitest`

Browser-based immersive cybersecurity training simulator — no headset required, stable 90fps with only 19 draw calls via instanced rendering. Features a rotating holographic threat globe with live cyber attack routes, concentric orbit rings, pulsating radar wavefronts, and a vocal AI narrator (native SpeechSynthesis) that announces threats in real time. Scrolling glassmorphic telemetry panel outputs live firewall and intrusion events. Compiles with 0 errors, passes all 6 custom Vitest unit tests.

</td>
<td width="50%" valign="top">

**🛡️ Security Incident Response Framework**
`Python` `YARA-L` `Sigma` `Splunk` `NIST SP 800-61r2`

Enterprise-grade IR framework with 6 MITRE ATT&CK-mapped playbooks covering phishing, ransomware, insider threat, lateral movement, cloud misconfiguration, and DDoS. Includes hand-written YARA-L and Sigma detection rules, Python automation for host isolation and ticket creation, escalation matrix, RCA templates, and a KPI tracker with MTTD/MTTR dashboards. Mean detection time under 2 minutes on simulated intrusion scenarios.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**☁️ Cloud-Based SIEM System**
`AWS` `Splunk` `Python` `Lambda` `CloudWatch` `EC2` `S3`

Scalable SIEM deployed on AWS aggregating 10,000+ daily log events across endpoint, network, and cloud sources. Six custom detection rules covering brute force, lateral movement, privilege escalation, data exfiltration, C2 beaconing, and unauthorized access. Real-time alerting, anomaly detection dashboards, and automated log ingestion via Lambda.

</td>
<td width="50%" valign="top">

**🗳️ SafeCount — Secure EVM Voting System**
`Blockchain` `RFID` `Biometrics` `Solidity` `RBAC` `Cryptography`

**Patent filed (India, 2024).** 3-factor authenticated electronic voting machine combining RFID, facial recognition, and fingerprint biometrics with blockchain-based vote verification and tamper-evident audit trails. RBAC enforces role separation across all user tiers. Deployed in 1 institutional pilot — eliminated 100% of identified proxy voting vectors.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**🔍 AWS Cloud Fraud Detection & Abuse Pattern Analyzer**
`Python` `AWS` `XGBoost` `Isolation Forest` `SHAP` `spaCy` `Streamlit`

End-to-end ML pipeline detecting cloud account fraud — account takeover, crypto mining abuse, IAM privilege escalation, data exfiltration, and API reconnaissance. Three-model ensemble (Isolation Forest + XGBoost + K-Means) produces a 0–100 risk score per account per hour. SHAP explainability on every alert. Live Streamlit dashboard for analyst and executive views. Built entirely from scratch.

</td>
<td width="50%" valign="top">

**🤖 CyberGuard AI Security Assistant**
`Python` `NLP` `spaCy` `REST API` `Web Speech API`

*In development.* AI-powered security training platform generating 15+ adaptive threat scenarios covering phishing, social engineering, ransomware, and lateral movement. Custom NLP pipeline with spaCy IOC extraction, Jinja2 scenario templates, and output validation. Voice-activated JARVIS interface via Web Speech API.

</td>
</tr>
</table>

---

## Skills

<div align="center">

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C/C++](https://img.shields.io/badge/C%2FC%2B%2B-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)
![GLSL](https://img.shields.io/badge/GLSL-Shaders-5C3EE8?style=flat-square&logoColor=white)

**AI & Machine Learning**
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-0073B7?style=flat-square&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-Explainability-6C3483?style=flat-square&logoColor=white)
![spaCy](https://img.shields.io/badge/spaCy-NLP-09A3D5?style=flat-square&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white)

**Security Tools**
![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![Palo Alto](https://img.shields.io/badge/Palo%20Alto%20NGFW-FA582D?style=flat-square&logo=paloaltonetworks&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp%20Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-2596CD?style=flat-square&logoColor=white)
![YARA-L](https://img.shields.io/badge/YARA--L-Rules-CC0000?style=flat-square&logoColor=white)
![Sigma](https://img.shields.io/badge/Sigma-Rules-4A90D9?style=flat-square&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-4682B4?style=flat-square&logoColor=white)

**Cloud & Infrastructure**
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**3D & Immersive**
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=three.js&logoColor=white)
![WebXR](https://img.shields.io/badge/WebXR-7B2FBE?style=flat-square&logoColor=white)
![Unity](https://img.shields.io/badge/Unity-000000?style=flat-square&logo=unity&logoColor=white)
![Blender](https://img.shields.io/badge/Blender-F5792A?style=flat-square&logo=blender&logoColor=white)

**Visualization**
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)
![PowerBI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)

**Frameworks & Standards**
![MITRE ATT&CK](https://img.shields.io/badge/MITRE%20ATT%26CK-E50914?style=flat-square&logoColor=white)
![NIST](https://img.shields.io/badge/NIST%20CSF-003087?style=flat-square&logoColor=white)
![ISO 27001](https://img.shields.io/badge/ISO%2027001-005F99?style=flat-square&logoColor=white)
![SOC 2](https://img.shields.io/badge/SOC%202-6C3483?style=flat-square&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP%20Top%2010-000000?style=flat-square&logo=owasp&logoColor=white)
![HIPAA](https://img.shields.io/badge/HIPAA-2E86AB?style=flat-square&logoColor=white)

</div>

---

## Certifications

<div align="center">

![Anthropic AI Fluency](https://img.shields.io/badge/Anthropic-AI%20Fluency%20Framework-C15B27?style=flat-square&logoColor=white)
![Claude 101](https://img.shields.io/badge/Anthropic-Claude%20101-C15B27?style=flat-square&logoColor=white)
![Palo Alto](https://img.shields.io/badge/Palo%20Alto-Cybersecurity%20Fundamentals-FA582D?style=flat-square&logo=paloaltonetworks&logoColor=white)
![Google](https://img.shields.io/badge/Google-Networks%20%26%20Network%20Security-4285F4?style=flat-square&logo=google&logoColor=white)
![Google](https://img.shields.io/badge/Google-Manage%20Security%20Risks-4285F4?style=flat-square&logo=google&logoColor=white)
![Maryland](https://img.shields.io/badge/U%20of%20Maryland-Cybersecurity%20for%20Everyone-CC0000?style=flat-square&logoColor=white)
![IBM](https://img.shields.io/badge/IBM-Generative%20AI%20%26%20Prompt%20Engineering-052FAD?style=flat-square&logo=ibm&logoColor=white)
![Vanderbilt](https://img.shields.io/badge/Vanderbilt-Prompt%20Engineering-000000?style=flat-square&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-Cloud%20Foundations-232F3E?style=flat-square&logo=amazonaws&logoColor=white)

</div>

---

## GitHub Stats

<div align="center">

<img height="170em" src="https://github-readme-stats.vercel.app/api?username=mansi200304&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&title_color=00c6ff&icon_color=00c6ff&text_color=c9d1d9&bg_color=0d1117"/>
<img height="170em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mansi200304&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&title_color=00c6ff&text_color=c9d1d9&bg_color=0d1117"/>

<br/>

![Streak](https://github-readme-streak-stats.herokuapp.com/?user=mansi200304&theme=tokyonight&hide_border=true&ring=00c6ff&fire=00c6ff&currStreakLabel=00c6ff)

</div>

---

## Open To

<div align="center">

![SOC Analyst](https://img.shields.io/badge/SOC%20Analyst-00C853?style=for-the-badge)
![Security Engineer](https://img.shields.io/badge/Security%20Engineer-00C853?style=for-the-badge)
![AI Security](https://img.shields.io/badge/AI%20%26%20ML%20Security-00C853?style=for-the-badge)
![Security BA](https://img.shields.io/badge/Security%20Business%20Analyst-00C853?style=for-the-badge)
![Threat Intelligence](https://img.shields.io/badge/Threat%20Intelligence-00C853?style=for-the-badge)
![Cloud Security](https://img.shields.io/badge/Cloud%20Security-00C853?style=for-the-badge)
![Fraud Analytics](https://img.shields.io/badge/Fraud%20%26%20Risk%20Analytics-00C853?style=for-the-badge)

**📍 Tempe, AZ &nbsp;·&nbsp; Night shift available (7:30 pm – 7:30 am ET) &nbsp;·&nbsp; F-1 OPT May 2027 &nbsp;·&nbsp; No sponsorship required at start**

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00c6ff,100:1a1f6e&height=120&section=footer" width="100%"/>

![Views](https://komarev.com/ghpvc/?username=mansi200304&color=00c6ff&style=flat-square&label=profile+views)
</div>
