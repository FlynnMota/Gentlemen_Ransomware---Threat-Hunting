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

**Note: additional configuration**
As this hunt is based on KQL queries for Sentinel/Defender it needs to be correctly connected to Sentinel or any other way to retrieve the data from the tables.
