# Robert L. Bogan Jr.

**AI Security Architect | Senior Cybersecurity Engineer | Agentic AI Security**

CISSP, CISM and CRISC certified cybersecurity professional working where enterprise security meets AI systems and automation.

My current work is securing AI agents, LLM applications, RAG architectures and autonomous workflows. That covers identity, authorization, prompt injection, adversarial testing, tool security, human approval, telemetry and controls whose effect can be measured.

## Current Focus

- AI and LLM security
- Agentic AI security
- MCP and agent tool authorization
- Prompt injection and adversarial testing
- RAG security
- Microsoft Sentinel and KQL
- Microsoft 365 Copilot and Copilot agents
- Azure AI and Azure OpenAI
- Human-in-the-loop security controls
- AI security governance
- Security automation
- EDR and XDR

## Featured Projects

### [Nemotron Agent Evaluation & Security Benchmark Lab](https://github.com/sdballpark/nemotron-agent-eval-lab)
Evaluation harness for NVIDIA Nemotron 3.5 Lightning, qwen2.5 and Gemini 3.8 Flash on SOC alert triage and IT-operations agent tasks. Measures accuracy, prompt-injection effects against clean twins, and whether a trusted MCP authorization gateway holds when a model is steered.

**Measured result:** across 216 agent episodes, 96 of them carrying injected instructions, the payloads steered three of four models into requesting privileged actions and the gateway allowed none of them. Predictions for the key experiments were committed to git before any run.

### [IT Operations MCP Gateway](https://github.com/sdballpark/itops-mcp-gateway)
Secure MCP gateway for AI agents with four-tier authorization, human approval for privileged actions, prompt-injection defenses, append-only auditing, and ITSM and identity integration patterns.

**Measured result:** no privileged or denied action executed in 216 agent episodes run against it by the Nemotron lab, including every episode in which the model was steered.

### [Agentic SOC Triage](https://github.com/sdballpark/agentic-soc-triage)
LLM-driven SOC alert triage using ASIM-normalized alerts, a labeled evaluation corpus and a measured test harness.

**Measured result:** 90% accuracy with a 0% false-close rate on the project evaluation set, reproduced at 90.2% over 500 triages in the Nemotron lab.

### [AI Security Platform](https://github.com/sdballpark/ai-security-platform)
Defense-in-depth controls for LLM applications: a Rust prompt-injection detection engine and a Go security gateway sharing one detection core, mapped to the OWASP LLM Top 10 and MITRE ATLAS.

### [Sentinel KQL Evaluation](https://github.com/sdballpark/sentinel-kql-eval)
Natural-language-to-KQL benchmark for security questions.

**Measured result:** schema grounding raised execution success from 9.1% to 68.2% on a local 14B model, measured against a real Kusto engine on the project test set.

### [AI Agent Automation](https://github.com/sdballpark/ai-agent-automation)
Python-based multi-stage AI workflow that generates, reviews, revises and automates structured content using LLMs and microservices.

### [Go Resume Matcher CLI](https://github.com/sdballpark/go_resume_matcher_cli)
Lightweight Go CLI for resume-to-job matching, designed for secure enterprise deployment.

## AI Security Architecture Themes

**Agent security**

Identity → Authorization → Tool permission → Human approval → Execution → Audit

**RAG security**

User → Retrieval → Untrusted content → LLM → Policy enforcement → Response

**Adversarial testing**

Prompt injection · Indirect prompt injection · Tool abuse · Privilege escalation · Data exfiltration · Unsafe agent actions

**AI governance**

NIST AI RMF · MITRE ATLAS · Secure by design · Zero Trust · AI TRiSM

## Cybersecurity Background

Enterprise security architecture and engineering across EDR/XDR, endpoint security, vulnerability management, IAM, SIEM, security automation, cloud security, compliance and incident response.

Platforms and tools: Microsoft Azure · Microsoft Sentinel · Microsoft Defender · Tanium · CrowdStrike Falcon · SentinelOne · ServiceNow · Splunk · Tenable · Python · PowerShell

## Earlier Machine Learning Work

These projects trace the path from applied machine learning into AI security engineering.

- Predict House Prices: linear regression
- Real-Time Fraud Detection: Apache Spark
- Resume Matching: NLP and cosine similarity
- Logistic Regression from Scratch: SGD

## Connect

[LinkedIn](LINKEDIN_URL)
