# Robert L. Bogan Jr.

**AI Security Architect | Senior Cybersecurity Engineer | Agentic AI Security**

CISSP, CISM and CRISC certified cybersecurity professional working where enterprise security meets AI systems and automation.

My current work is securing AI agents, LLM applications, RAG architectures and autonomous workflows. That covers identity, authorization, prompt injection, adversarial testing, tool security, human approval, telemetry and controls whose effect can be measured.

## Current Focus

- Agentic AI security: MCP tool authorization and human approval for agent actions
- Prompt-injection and adversarial testing of agents and RAG systems
- LLM and agent evaluation with labeled datasets and reproducible measurement
- AI security controls on Microsoft 365, Azure and Google Cloud
- Detection engineering with Microsoft Sentinel and KQL

## Featured Projects

### [Nemotron Agent Evaluation & Security Benchmark Lab](https://github.com/sdballpark/nemotron-agent-eval-lab)
Evaluation harness for NVIDIA Nemotron 3.5 Lightning, qwen2.5 and Gemini 3.8 Flash on SOC alert triage and IT-operations agent tasks. Measures accuracy, prompt-injection effects against clean twins, and whether a trusted MCP authorization gateway holds when a model is steered.

**Measured result:** across 216 agent episodes, 96 of them carrying injected instructions, the payloads steered three of four models into requesting privileged actions and the gateway allowed none of them. Predictions for the key experiments were committed to git before any run.

### [GCP AI Security Lab](https://github.com/sdballpark/gcp-ai-security-lab)
A RAG assistant on Vertex AI and Cloud Run, attacked and then secured one control layer at a time across nine modules: IAM, Model Armor, VPC Service Controls, Sensitive Data Protection, Cloud Armor, CMEK, detections and identity-scoped retrieval.

**Measured result:** with no controls, 17 of 20 attack prompts and 8 of 10 harmless questions leaked synthetic SSNs and card numbers through a poisoned document. Model Armor alone stopped the leaks but blocked all 30 requests. Adding a DLP ingestion pipeline kept leaks at zero and let harmless questions through again. One finding: a Model Armor setting reported "Enabled" while only inspecting traffic, not blocking it.

### [Secure Microsoft 365 Copilot Agent Lab](https://github.com/sdballpark/secure-m365-copilot-agent-lab)
A declarative Microsoft 365 Copilot agent grounded in SharePoint, calling a controlled Security Actions API with Entra token validation, READ / WRITE / PRIVILEGED / DENIED actions, independent human approval and a tamper-evident audit chain.

**Measured result:** 6 of 6 deterministic control-plane cases and 7 of 7 live Microsoft 365 security checks passed. Indirect prompt injection, a document posing as an approval, and agent self-approval were all blocked.

### [IT Operations MCP Gateway](https://github.com/sdballpark/itops-mcp-gateway)
Secure MCP gateway for AI agents with four-tier authorization, human approval for privileged actions, prompt-injection defenses, append-only auditing, and ITSM and identity integration patterns.

**Measured result:** no privileged or denied action executed in 216 agent episodes run against it by the Nemotron lab, including every episode in which the model was steered.

### [Agentic SOC Triage](https://github.com/sdballpark/agentic-soc-triage)
LLM-driven SOC alert triage using ASIM-normalized alerts, a labeled evaluation corpus and a measured test harness.

**Measured result:** 90% accuracy with a 0% false-close rate on the project evaluation set, reproduced at 90.2% over 500 triages in the Nemotron lab.

### [Sentinel KQL Evaluation](https://github.com/sdballpark/sentinel-kql-eval)
Natural-language-to-KQL benchmark for security questions.

**Measured result:** schema grounding raised execution success from 9.1% to 68.2% on a local 14B model, measured against a real Kusto engine on the project test set.

### [Clinical RAG](https://github.com/sdballpark/clinical-rag)
Local clinical RAG over a medical reference manual, with hybrid retrieval, domain cross-encoder confidence, two-layer abstention, and an evaluation harness using human-validated judges.

**Measured result:** on 48 golden items, the abstention gate refused all 6 out-of-corpus questions while serving 98% of answerable ones, with 90% citation coverage and no invalid citations. A validation run that seemed to show both judges missing all 10 injected hallucinations turned out to be scoring stale verdicts; judged correctly, MiniCheck caught 10 of 10.

## Other Projects

- [AI Security Platform](https://github.com/sdballpark/ai-security-platform): a Rust prompt-injection detection engine and a Go security gateway sharing one detection core. A CI gate runs a labeled corpus on every commit: 25 of 26 attacks detected and 0 of 15 benign inputs flagged; the miss is character-spaced text.
- [Remediation Recommender](https://github.com/sdballpark/remediation-recsys): two-stage recommendation engine with collaborative filtering and LightGBM LambdaRank, a SQL feature pipeline, an evaluation gate and FastAPI serving.
- [AI Agent Automation](https://github.com/sdballpark/ai-agent-automation): multi-stage LLM workflow that generates, reviews and revises structured content.

## AI Security Architecture Themes

**Agent security**

Identity → Authorization → Tool permission → Human approval → Execution → Audit

**RAG security**

User → Retrieval → Untrusted content → LLM → Policy enforcement → Response

**Adversarial testing**

Prompt injection · Indirect prompt injection · Tool abuse · Privilege escalation · Data exfiltration · Unsafe agent actions

**AI governance**

NIST AI RMF · MITRE ATLAS · OWASP LLM Top 10 · Secure by design · Zero Trust · AI TRiSM

## Cybersecurity Background

Enterprise security architecture and engineering across EDR/XDR, endpoint security, vulnerability management, IAM, SIEM, security automation, cloud security, compliance and incident response.

Platforms and tools: Microsoft Azure · Google Cloud · Microsoft Sentinel · Microsoft Defender · Tanium · CrowdStrike Falcon · SentinelOne · ServiceNow · Splunk · Tenable · Python · PowerShell

## Earlier Machine Learning Work

These projects trace the path from applied machine learning into AI security engineering.

- [Predict House Prices](https://github.com/sdballpark/predict-house-prices): linear regression
- [Real-Time Fraud Detection](https://github.com/sdballpark/fraud-detection-spark): Apache Spark
- [Loan Default Prediction](https://github.com/sdballpark/loan-default-xgboost): XGBoost
- [Logistic Regression from Scratch](https://github.com/sdballpark/sgd-logistic-regression): SGD

## Connect

[LinkedIn](https://www.linkedin.com/in/robert-l-bogan-jr/)
