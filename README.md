<div align="center">
  <h1>🛡️ Michael Lannen | CSAP | CySA+ | Security+ | Network+ | AZ-900 | SC-900</h1>
  <p><b>Cybersecurity Specialist | SecOps & Incident Response</b></p>
  <p><i>Incident response, practical threat intelligence pipelines, and real-world infrastructure defense.</i></p>

  [![Email Me](https://img.shields.io/badge/Email-Me-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:Michael.lannen93@gmail.com) 
  [![Download Master CV](https://img.shields.io/badge/Download-Master%20CV-0078D4?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)](./Michael%20Lannen%20Cyber%20Security.pdf)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/michael-lannen-053588167/) 
  [![GitHub](https://img.shields.io/badge/GitHub-Profile-24292e?style=for-the-badge&logo=github)](https://michaelwlannen.github.io)
</div>

---

### 👨‍💻 About Me

Growing up, I knew there were jobs messing around with computers, but coming from a small town, I never really knew what an actual career in tech looked like. I started out working regular jobs—retail, labor, and eventually customer operations at a call center.

While working on the call floor, an old-school IT guy took me under his wing. Whenever he had a spare minute, he showed me the ropes, explained how the systems actually worked, and helped me see that this was something I could build a future around.

When my daughter was born, everything shifted into focus. I enrolled in an intensive 18-month Associate degree program, worked two jobs, DoorDashed with a car seat in the back to pay for diapers, and studied late into the night. I finished the degree with Honors and knocked out five CompTIA certifications before graduating. That stretch proved to me what I'm capable of when I lock in—when I commit to something, I see it through.

I landed at **FMRS Health Systems**, originally brought on for general IT support, but that role transformed quickly. After walking into an active **Qilin ransomware** outbreak and helping isolate and recover systems, I realized defensive security wasn't just a job track—it was where I wanted to be. 

Instead of waiting around for tasks to be handed down, I started hunting down operational gaps across our environment. When I saw our organization lacked centralized visibility, I built and deployed a production **Splunk Enterprise SIEM** across 150+ clinical endpoints from the ground up, setting up Linux LVM storage pools and automating fleet forwarder rollouts. To supercharge our threat intel, I engineered an automated **MISP pipeline** integrated with a local LLM to ingest and enrich IOCs, shooting real-time triage summaries straight to Discord without leaking data to cloud APIs.

I didn't stop at technical telemetry, either. Recognizing our exposure to social engineering, I stood up a custom **GoPhish simulation platform** with tailored login portals and training redirects, measurably cutting our phishing risk. To lock down our operational resilience, I authored full Disaster Recovery Plans and now lead **DRP tabletop exercises directly with organizational stakeholders** to prepare our team for real-world incidents.

I moved way past basic troubleshooting—I actively hunt threats, build automation, and solve defensive problems. I'm always looking to sharpen my skills, learn from experienced practitioners, and share what I know with anyone else working their way up from scratch. If you've got advice, want to talk shop, or have a problem to solve, feel free to reach out. We can learn from each other! DONT GIVE UP!

Galatians 6:9, Philippians 4:13, Joshua 1:9

### 🏆 Certifications
⚡ `CompTIA Security+` | `CompTIA Network+` | `CompTIA CySA+` | `CompTIA CSAP` | `CompTIA ITF+` | `Microsoft AZ-900` | `Microsoft SC-900`

---

### 🛠️ Technical Skills

| 🛡️ Security Operations, IR & OSINT | 🔑 Identity, Cloud & Compliance | 🌐 Systems, Networking & Automation |
| :--- | :--- | :--- |
| • Microsoft Sentinel & Splunk Enterprise<br>• SentinelOne EDR & Wazuh SIEM<br>• Ransomware Containment & Host Isolation<br>• OSINT & Targeted Google Dorking<br>• GoPhish Phishing Simulations<br>• Nessus Professional, VirusTotal, AlienVault OTX | • Entra ID (Azure AD) & Active Directory<br>• Intune MDM, RBAC, MFA & Conditional Access<br>• HIPAA Security Rule & PCI-DSS Compliance<br>• NIST CSF & SP 800-53 Mapping<br>• Email Security (SPF, DKIM, DMARC)<br>• PKI, TLS/SSL & Storage Encryption (AES-256) | • Detection: KQL, SPL, Alert Tuning, IOC Triaging<br>• Scripting: PowerShell, Python, Bash<br>• REST API Ingestion & Local Automation Pipelines<br>• MISP Threat Sharing & STIX/TAXII<br>• pfSense, WireGuard, Site-to-Site VPNs, VLANs<br>• Linux (Ubuntu/Debian) Administration & Docker |

---

### 🗺️ Infrastructure Topology

![Enterprise Infrastructure Topology Map](https://quickchart.io/graphviz?format=png&graph=digraph+G+{+node+[shape=box,fontname="Helvetica",style="filled,rounded",fillcolor="%231e293b",color="%2338bdf8",fontcolor="%23f8fafc"];+edge+[color="%2394a3b8"];+bgcolor="%230f172a";+subgraph+cluster_0+{+label="Enterprise+Perimeter";+fontcolor="%2338bdf8";+color="%2338bdf8";+VLAN_Seg+[label="pfSense+Firewall+%26+WireGuard\n(Secure+VLAN+Segmentation)",shape=diamond,color="%2338bdf8"];+}+subgraph+cluster_1+{+label="Clinical+Footprint+(150%2B+Endpoints)";+fontcolor="%2338bdf8";+WinAD+[label="Entra+ID+/+Active+Directory"];+MultiEndpoints+[label="Multi-Platform+Endpoints\n(NinjaOne+%26+SentinelOne)"];+VLAN_Seg+->+WinAD;+VLAN_Seg+->+MultiEndpoints;+}+subgraph+cluster_2+{+label="Centralized+Security+Core";+fontcolor="%2338bdf8";+color="%2338bdf8";+Splunk+[label="Ubuntu+Linux+Server\nSplunk+Enterprise+SIEM",fillcolor="%232a3439",color="%2338bdf8"];+LVM+[label="1TB+Linux+LVM\nAggregated+Storage+Pool"];+Splunk+->+LVM+[dir=both,label="Log+Sync/IO"];+}+subgraph+cluster_3+{+label="Threat+Intel+%26+Automation";+fontcolor="%2338bdf8";+MISP+[label="MISP+Pipeline"];+LLM+[label="Local+LLM+/+Discord+Alerts"];+MISP+->+LLM;+}+WinAD+->+Splunk+[label="S1+API+/+Event+Logs",fontcolor="%2394a3b8"];+MultiEndpoints+->+Splunk+[label="Sysmon+/+Universal+Forwarder",fontcolor="%2394a3b8"];+})

---

### 🏗️ Featured Project: Local LLM & MISP Threat Intelligence Pipeline
🔗 **[Repository Link](https://github.com/michaelnoobz/Splunk-homelab-and-work-set-up)**

An automated pipeline designed to speed up alert triage without leaking internal incident data to external APIs:
* **Automated IOC Enrichment:** Connects **MISP** directly into **Splunk Enterprise** to flag incoming telemetry against verified IOC lists on the fly.
* **Local AI Triage:** Passes raw alert payloads to a private, locally hosted model (**Dolphin-Mistral / Mistral-7B via Ollama**) to draft immediate triage summaries and remediation steps.
* **Alert Delivery:** Sends enriched alert summaries straight to a designated SOC Discord webhook so analysts have context before opening a ticket.

---

### 🛠️ Projects & Hands-on Work

* **[Production Splunk SIEM Deployment](https://github.com/michaelnoobz/Splunk-homelab-and-work-set-up):** Set up a production Splunk Enterprise instance on Ubuntu across 150+ endpoints. Built custom LVM disk partitions for storage and deployed universal forwarders using NinjaOne REST APIs and PowerShell.
* **[OSINT & Advanced Google Dorking Workflows](https://github.com/michaelnoobz):** Use Google Dorking (`site:`, `filetype:`, `inurl:`) and open-source intelligence methods for threat surface mapping, tracking attacker infrastructure, and locating hidden, unindexed job listings and point-of-contact info.
* **[Azure Honeypot & Sentinel Telemetry](https://github.com/michaelnoobz/MyFirstSEIM):** Stood up an exposed Azure cloud VM to catch live internet attacks; wrote custom **KQL** queries in **Microsoft Sentinel** to track brute-force attempts and source IPs.
* **[Vulnerability Management & Nessus Lab](https://github.com/michaelnoobz/Splunk-homelab-and-work-set-up):** Configured Nessus Professional in an isolated test environment, ran credentialed scans on Windows/Linux hosts, mapped out high-risk CVEs by CVSS score, and applied remediation patches.
* **[GoPhish Simulation Framework](https://github.com/michaelnoobz/Gophish-):** Built realistic phishing tests with GoPhish using custom Microsoft login clones and instant educational landing pages, driving down click rates across staff.
* **[Disaster Recovery Tabletop (Operation Open Jack)](https://github.com/michaelnoobz/DRP-Table-Tops):** Wrote practical incident response and disaster recovery documentation mapped to HIPAA and NIST CSF, including tabletop walkthroughs for physical port compromise.
* **[Malware & Phishing Analysis Labs](https://github.com/michaelnoobz/Pico-CTF-Python-Automation):** Analyzed live phishing emails and malicious files, dissecting email headers, extracting indicators of compromise (IOCs), and checking behaviors in sandbox environments.

---

### 💼 Practical Experience

#### Cybersecurity Specialist / IT Specialist
**FMRS Health Systems** | Beckley, WV | *Nov 2024 – Present*
* **Ransomware Response:** Responded directly to a Qilin ransomware incident that hit an external firewall service; helped isolate affected systems, dug into IOCs, and worked through the containment and recovery steps.
* **Phishing Defense:** Investigated and resolved multiple phishing campaigns, pulling apart headers and malicious URLs to pull IOCs and tighten mail filtering rules.
* **SIEM Build:** Built and deployed a production Splunk environment on Linux, configuring log ingestion from 150+ clinical endpoints for unified log visibility.
* **Fleet Automation:** Wrote custom PowerShell scripts hooked into NinjaOne REST APIs to deploy endpoint security agents across 150+ machines automatically.
* **Directory & Identity Security:** Locked down access for 300+ accounts across Entra ID and Active Directory using least-privilege principles, custom GPOs, and RBAC.
* **Security Awareness:** Ran internal GoPhish tests with tailored landing pages to show users what red flags look like in the wild.
* **Documentation & Audits:** Drafted Disaster Recovery Plans (DRP), Acceptable Use Policies (AUP), and incident response procedures built around HIPAA requirements.
* **Threat Hunting & Triage:** Used SentinelOne, Splunk, VirusTotal, and AlienVault OTX to investigate alerts and track down suspicious activity across the network.
* **Day-to-Day Operations:** Handled user onboarding/offboarding, racked servers, pulled and terminated network cabling, and handled Tier-2/3 tickets across multiple remote clinical offices.

#### Production Support
**Ibex Global** | Beckley, WV | *May 2019 – Oct 2023, Feb 2024 – Nov 2024*
* **Root-Cause Analysis:** Dug into repetitive system escalations to find the technical root cause, writing playbooks that cut down repeat tickets.
* **Escalations & Data Privacy:** Handled high-priority technical escalations involving provider dispute issues while strictly following HIPAA and PCI-DSS data standards.
* **Documentation:** Created standard operating procedures and internal guides to help onboard and train floor agents on troubleshooting steps.

---

### 🎓 Education
* **West Virginia Junior College** | A.A.S. in Cybersecurity (Honors) | *Graduated: 2025*

---

### 📬 Connect
* **Email:** [Michael.lannen93@gmail.com](mailto:Michael.lannen93@gmail.com)
* **LinkedIn:** [linkedin.com/in/michael-lannen-053588167](https://www.linkedin.com/in/michael-lannen-053588167)
* **Portfolio:** [michaelwlannen.github.io](https://michaelwlannen.github.io/)
* **Target:** I am actively looking for a cybersecurity role—SOC Analyst, Incident Responder, Threat Detection, or SecOps. Looking for a specific tool or stack not listed above? Don't worry, I’ve probably already looked up what you’re running and am already digging into it. I'm ready to step in, clear out alerts, protect infrastructure, and pull my weight from day one.
