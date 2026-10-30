<div align="center">

# Hi, I'm Fernando

**I build and test detections, and I secure AI agents.**

Security engineer focused on detection engineering and AI agent security, with hands-on cloud security and incident response labs.

<img src="security-plus.png" alt="CompTIA Security+ Certified" height="110">
<img src="pentest-plus.png" alt="CompTIA PenTest+ Certified" height="110">

<br>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Fernando%20Cortez%20Jr-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/fernando-cortez-jr-a3529a313)

</div>

<br>

## What I work on

| AI agent security | Detection engineering |
|---|---|
| Attacking and defending LLM agents that use MCP tools: prompt injection, tool poisoning, default-deny policy, canary traps, and runtime detection | Writing, tuning, and testing detections in Sigma and Splunk, with false-positive analysis and MITRE ATT&CK mapping |
| [agent-tripwire](https://github.com/FCortezSecurity/agent-tripwire) · [mcp-security-lab](https://github.com/FCortezSecurity/mcp-security-lab) | [windows-endpoint-detection-ir](https://github.com/FCortezSecurity/windows-endpoint-detection-ir) · [cloud-security-detection-suite](https://github.com/FCortezSecurity/cloud-security-detection-suite) · [honeymap](https://github.com/FCortezSecurity/honeymap) |

## Featured projects

### [agent-tripwire](https://github.com/FCortezSecurity/agent-tripwire) &nbsp; ![release](https://img.shields.io/github/v/release/FCortezSecurity/agent-tripwire?style=flat)
A security gateway that sits between an AI agent and its MCP tools. It enforces a default-deny policy, pins tool definitions, traps misuse with decoys, and runs 12 detections (Sigma rules plus sequence rules).

In a scripted evaluation, **0 of 14 attacks succeed in enforce mode**, all 12 benign tasks still work, and the gateway adds about 10 ms per call. I also ran an evasion round against my own defenses first, and detection fell from 10 of 10 attacks to 10 of 13 before I fixed it. The README states what these results do and do not show.

### [mcp-security-lab](https://github.com/FCortezSecurity/mcp-security-lab)
A local lab for attacking and defending an LLM agent that uses MCP tools. It covers prompt injection and tool poisoning, then tests defenses with measured security and utility results.

### [windows-endpoint-detection-ir](https://github.com/FCortezSecurity/windows-endpoint-detection-ir)
A Windows endpoint detection and incident response lab using Sysmon and Splunk: 5 tuned detections with false-positive analysis, 2 full incident investigations, and MITRE ATT&CK mapping.

### [cloud-security-detection-suite](https://github.com/FCortezSecurity/cloud-security-detection-suite)
A consolidated AWS security toolkit: IAM configuration auditing, CloudTrail threat detection, and Splunk-based investigation workflows.

### [honeymap](https://github.com/FCortezSecurity/honeymap)
A honeypot threat-intelligence pipeline that parses attacker activity, enriches it, detects patterns, and maps the attacks.

Also: [aegis-fusion](https://github.com/FCortezSecurity/aegis-fusion), DevSecOps automation that runs Bandit, pip-audit, Gitleaks, Checkov, and Trivy, normalizes the findings, and enforces a policy gate in GitHub Actions.

## What I'm working on next

- Running the attacks from `mcp-security-lab` through `agent-tripwire` and publishing the hits and the misses
- Testing the gateway against a local model instead of a scripted agent

I learn by building in the open. Every repo is a real build with documented results, including its limitations.

<details>
<summary><b>Tools and technologies</b></summary>

<br>

**Languages and platforms**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)

**Detection, SIEM and IR**

![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat&logo=splunk&logoColor=white)
![Sigma](https://img.shields.io/badge/Sigma-5B5B5B?style=flat&logoColor=white)
![Sysmon](https://img.shields.io/badge/Sysmon-0078D4?style=flat&logoColor=white)
![CloudTrail](https://img.shields.io/badge/AWS%20CloudTrail-FF9900?style=flat&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE%20ATT%26CK-B22222?style=flat&logoColor=white)
![OpenCanary](https://img.shields.io/badge/OpenCanary-5B5B5B?style=flat&logoColor=white)

**DevSecOps**

![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
![Bandit](https://img.shields.io/badge/Bandit-F7B500?style=flat&logoColor=black)
![pip-audit](https://img.shields.io/badge/pip--audit-3776AB?style=flat&logoColor=white)
![Gitleaks](https://img.shields.io/badge/Gitleaks-D9381E?style=flat&logoColor=white)
![Checkov](https://img.shields.io/badge/Checkov-6C3FC5?style=flat&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=flat&logoColor=white)

**AI security**

![MCP](https://img.shields.io/badge/MCP-000000?style=flat&logoColor=white)
![OWASP LLM Top 10](https://img.shields.io/badge/OWASP%20LLM%20Top%2010-000000?style=flat&logoColor=white)
![Prompt Injection](https://img.shields.io/badge/Prompt%20Injection-8A2BE2?style=flat&logoColor=white)
![Red Teaming](https://img.shields.io/badge/Red%20Teaming-C0392B?style=flat&logoColor=white)

</details>

## Connect

I'm looking for security engineering, detection engineering, and AI security roles. The best way to reach me is [LinkedIn](https://www.linkedin.com/in/fernando-cortez-jr-a3529a313).
