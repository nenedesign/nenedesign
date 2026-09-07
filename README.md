# Neville Ko — AI Product Manager & Builder

I'm Neville Ko, Head of Product & Experience at [Distinct AI](https://www.distinctplugins.io/) and an [official n8n creator](https://n8n.io/creators/nene/) with published templates on the n8n marketplace. I have 20 years of experience shipping 0-to-1 products and I'm now building production-grade AI automation for regulated industries like financial services and healthcare.

I specialize in agentic RAG systems, multi-agent orchestration, and governance-aware AI mapped to real compliance frameworks: SEC/FINRA, OSFI E-23, SOC 2 Type II, PCI-DSS v4.0, and OWASP LLM Top 10. My work is production-ready, privacy-first, and built with audit trails, least-privilege tooling, and human-in-the-loop controls.

---

## Featured Work

### [AI Governance: OWASP LLM Top 10 Implementations](https://github.com/nenedesign/ai-governance-owasp10)

![OWASP LLM Top 10](https://img.shields.io/badge/OWASP_LLM_Top_10-000000?style=flat&logoColor=white)

Working implementations of all 10 OWASP LLM risks for financial services, insurance, and legal tech: n8n workflows, system prompt library, and governance checklists.

| Risk | Artifact | Coverage |
|------|----------|----------|
| [LLM01 Prompt Injection](https://github.com/nenedesign/ai-governance-owasp10/tree/main/workflows/llm01-prompt-injection-scanner) | Workflow + Prompt | 21-pattern scanner, risk-score gating |
| [LLM02 Sensitive Info Disclosure](https://github.com/nenedesign/ai-governance-owasp10/tree/main/workflows/llm02-pii-detector) | Workflow + Prompt | 7-category PII redaction |
| [LLM03 Supply Chain](https://github.com/nenedesign/ai-governance-owasp10/blob/main/governance/llm03-model-intake-assessment.md) | Governance doc | Model intake assessment checklist |
| [LLM04 Data Poisoning](https://github.com/nenedesign/ai-governance-owasp10/tree/main/workflows/llm04-llm08-rag-security-pipeline) | Workflow | RAG ingestion validation + allowlist |
| [LLM05 Improper Output Handling](https://github.com/nenedesign/ai-governance-owasp10/blob/main/prompt-library/llm05-output-sanitization.md) | Prompt | Output sanitization system prompt |
| [LLM06 Excessive Agency](https://github.com/nenedesign/ai-governance-owasp10/tree/main/workflows/llm06-hitl-approval-gate) | Workflow + Prompt | Human-in-the-loop approval gate |
| [LLM07 System Prompt Leakage](https://github.com/nenedesign/ai-governance-owasp10/blob/main/governance/llm07-system-prompt-audit.md) | Governance + Prompt | Audit framework + hardened prompt |
| [LLM08 Vector/Embedding Weaknesses](https://github.com/nenedesign/ai-governance-owasp10/tree/main/workflows/llm04-llm08-rag-security-pipeline) | Workflow | Sanitization + audit metadata on upsert |
| [LLM09 Misinformation](https://github.com/nenedesign/ai-governance-owasp10/blob/main/prompt-library/llm09-grounding-uncertainty.md) | Prompt | Grounding and uncertainty disclosure |
| [LLM10 Unbounded Consumption](https://github.com/nenedesign/ai-governance-owasp10/tree/main/workflows/llm10-rate-limiter) | Workflow | Sliding-window rate limiter |

---

### [AI Governance: PCI-DSS v4.0](https://github.com/nenedesign/ai-governance-pci-dss)

![PCI-DSS v4.0](https://img.shields.io/badge/PCI--DSS_v4.0-003087?style=flat&logoColor=white)

Practical guardrails for deploying AI in payment card environments, implementing PCI-DSS v4.0 at the inference layer.

| Artifact | Type | Coverage |
|----------|------|----------|
| [Cardholder Data Detector](https://github.com/nenedesign/ai-governance-pci-dss/blob/main/workflow.json) | n8n workflow | Pre-inference PAN/CVV/expiry masking across all 4 card networks |
| [PCI Scope Boundary System Prompt](https://github.com/nenedesign/ai-governance-pci-dss/blob/main/pci-scope-boundary-prompt.md) | System prompt | Hard prohibitions, redirect instructions, masked input handling |

---

### [AI Governance: SOC 2 Type II](https://github.com/nenedesign/ai-governance-soc2)

![SOC 2 Type II](https://img.shields.io/badge/SOC_2_Type_II-006CB8?style=flat&logoColor=white)

Audit infrastructure for LLM deployments in SOC 2 Type II environments: tamper-evident interaction logging, automated retention enforcement, and an AI system evidence template for auditors.

| Artifact | Type | Coverage |
|----------|------|----------|
| [Audit Log Pipeline](https://github.com/nenedesign/ai-governance-soc2/blob/main/audit-log-pipeline/workflow.json) | n8n workflow | Webhook-triggered, SHA-256 integrity hash, append-only Supabase insert |
| [Retention Enforcer](https://github.com/nenedesign/ai-governance-soc2/blob/main/retention-enforcer/workflow.json) | n8n workflow | Daily schedule, flags entries expired after 90 days |
| [SOC 2 AI Evidence Template](https://github.com/nenedesign/ai-governance-soc2/blob/main/soc2-ai-evidence-template.md) | Document template | Structured documentation for AI systems under SOC 2 audit |

---

### [n8n Workflow Templates](https://github.com/nenedesign/n8n-workflows)

![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat&logo=n8n&logoColor=white)

Production-ready automation workflows: agentic RAG, AI agents, and developer utilities; all importable directly into n8n.

| Workflow | Category | Level | Use Case |
|----------|----------|-------|----------|
| [Autonomous customer support agent](https://github.com/nenedesign/n8n-workflows/tree/main/ai-agents/autonomous-customer-support-agent) | AI Agents | Advanced | SaaS and enterprise customer support |
| [Multi-KB agentic RAG assistant](https://github.com/nenedesign/n8n-workflows/tree/main/rag/multi-kb-agentic-rag-assistant) | RAG | Advanced | Internal knowledge Q&A for teams |
| [Slack Gemini Agent](https://github.com/nenedesign/n8n-workflows/tree/main/ai-agents/slack-gemini-agent) | AI Agents | Intermediate | AI assistant for Slack workspaces |
| [Gmail AI Triage](https://github.com/nenedesign/n8n-workflows/tree/main/ai-agents/gmail-ai-triage) | AI Agents | Intermediate | High-volume inbox management |
| [Seed a Supabase AI knowledge base from Notion](https://github.com/nenedesign/n8n-workflows/tree/main/rag/seed-supabase-from-notion) | RAG | Intermediate | RAG pipeline ingestion from Notion |
| [AI Daily Briefing Bot](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/ai-daily-briefing-bot) | Utilities | Beginner | Daily news digest for teams |
| [Claude to Slack MCP Connection Test](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/claude-to-slack-mcp-test) | Utilities | Beginner | Developer MCP integration testing |
| [URL and Article Summarizer to Slack](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/url-article-summarizer-to-slack) | Utilities | Beginner | Content research and curation |
| [API Health Monitor](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/api-health-monitor) | Utilities | Beginner | DevOps uptime monitoring |
| [RSS Feed to Slack Alert](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/rss-feed-to-slack-alert) | Utilities | Beginner | Topic and brand monitoring |
| [GitHub PR to Slack Notifier](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/github-pr-to-slack-notifier) | Utilities | Beginner | Engineering team PR visibility |
| [AI Webhook Classifier](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/ai-webhook-classifier) | Utilities | Intermediate | Support triage and content routing |

---

## Research Focus

- **Multi-Agent Orchestration:** modality-agnostic, agent-to-agent workflows focused on security and privacy
- **Privacy-First Local AI:** on-device open-weight models for sensitive financial and healthcare data
- **Context and Memory Management:** hybrid memory retrieval for context-aware personalization
- **Hybrid Inference Routing:** optimizing token efficiency, latency, and cost across cloud and local

---

## Stack

**IDEs and Editors**  
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat&logo=visualstudiocode&logoColor=white) ![Cursor](https://img.shields.io/badge/Cursor-000000?style=flat&logoColor=white) ![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat&logo=anthropic&logoColor=white)

**Agents and Workflows**  
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat&logo=n8n&logoColor=white) ![MCP Servers](https://img.shields.io/badge/MCP_Servers-D97757?style=flat&logo=anthropic&logoColor=white) ![Google ADK](https://img.shields.io/badge/Google_ADK-4285F4?style=flat&logo=google&logoColor=white) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)

**Inference and APIs**  
![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=flat&logo=anthropic&logoColor=white) ![Gemini API](https://img.shields.io/badge/Gemini_API-8E75B2?style=flat&logo=googlegemini&logoColor=white) ![Perplexity API](https://img.shields.io/badge/Perplexity_API-20808D?style=flat&logoColor=white) ![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat&logo=ollama&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white) ![OpenRouter](https://img.shields.io/badge/OpenRouter-6467F2?style=flat&logoColor=white)

**AI Models**  
![Claude](https://img.shields.io/badge/Claude-D97757?style=flat&logo=anthropic&logoColor=white) ![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=flat&logo=googlegemini&logoColor=white) ![Gemma](https://img.shields.io/badge/Gemma-4285F4?style=flat&logo=google&logoColor=white) ![Cohere](https://img.shields.io/badge/Cohere-39594E?style=flat&logoColor=white)

**Prototyping**  
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat&logo=figma&logoColor=white) ![Lovable](https://img.shields.io/badge/Lovable-FF6B6B?style=flat&logoColor=white) ![Google AI Studio](https://img.shields.io/badge/Google_AI_Studio-4285F4?style=flat&logo=google&logoColor=white) ![Distinct AI](https://img.shields.io/badge/Distinct_AI-111111?style=flat&logoColor=white)

**Data and Knowledge**  
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat&logo=supabase&logoColor=white) ![Postgres](https://img.shields.io/badge/Postgres-4169E1?style=flat&logo=postgresql&logoColor=white) ![Notion](https://img.shields.io/badge/Notion-000000?style=flat&logo=notion&logoColor=white) ![Obsidian](https://img.shields.io/badge/Obsidian-7C3AED?style=flat&logo=obsidian&logoColor=white) ![Open WebUI](https://img.shields.io/badge/Open_WebUI-000000?style=flat&logoColor=white)

---

**Links:** [Portfolio](https://www.fromus.ca/ai-builds) · [LinkedIn](https://www.linkedin.com/in/nevilleko/) · [n8n Official Creator](https://n8n.io/creators/nene/)

---

Open to advisory, consulting, and collaboration on AI automation, agentic systems, and governance-aware AI for regulated industries. [Connect on LinkedIn](https://www.linkedin.com/in/nevilleko/)
