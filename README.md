# Gentlemen Ransomware

Jupyter notebook with KQL queries to hunt for Defense Evasion technique.

## 📋 Executive Summary


**Attack Summary:**
Gentlemen ransomware operates in 5 phases: (1) exploit internet-facing apps → (2) enumerate domain → (3) **disable security tools** → (4) move laterally → (5) encrypt & exfiltrate. This hunt focuses on **Phase 3 (Defense Evasion)** which is the most detectable and critical to interrupt.

**Target Audience:** SOC analysts, threat hunters, and security engineers using Microsoft Defender ATP

**What You'll see:**
- How Gentlemen ransomware (2025-2026) systematically disables defenses before encryption
- 7 practical KQL hunting queries to detect each attack stage in your environment
- Indicators of compromise mapped to MITRE ATT&CK framework
- Tuning guidance to reduce false positives specific to your organization


## **Note: additional configuration**
### 🔌 How to Connect This Notebook to Microsoft Sentinel / Defender

As this hunt is based on KQL queries for Sentinel/Defender and the purpose here is to share the knowledge how to hunt for those activities in that environment, **additional connection to Sentinel is needed**.<br>
To connect a Jupyter notebook to Microsoft Sentinel and run KQL hunting queries, you can either utilize the integrated Azure/Defender Portal Notebooks environment (which uses MSTICPy) or run queries locally/externally via the Kqlmagic library.
You may also need to insert some parameters to the hunting querie cells to make them retrieve the results appropriatelly.
