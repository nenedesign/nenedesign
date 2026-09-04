# Neville Ko — AI Product Manager & Builder



> AI Product Manager, Builder & Strategist — 20 years shipping 0-to-1 products

I'm Neville Ko, currently Head of Product & Experience at [Distinct AI](https://www.distinctplugins.io/) and an [official n8n creator](https://n8n.io/workflows/18427-seed-a-supabase-ai-knowledge-base-from-notion-with-ollama-embeddings/) with a published template on the n8n marketplace (more templates pending n8n approval). This repo contains production-ready AI automation workflow templates I've built for agentic RAG pipelines, AI agents, multi-agent orchestration, privacy-first local inference, and developer utilities. All workflows are designed to be imported directly into n8n and adapted for real use cases.

I'm currently focused on governance-aware AI for regulated industries (financial services, healthcare).

---

## Featured Work

### [n8n Workflow Templates](https://github.com/nenedesign/n8n-workflows)
Production-ready automation workflows: agentic RAG, AI agents, and developer utilities; all importable directly into n8n.

| Workflow | Category | Level | Canvas |
|----------|----------|-------|--------|
| [Autonomous customer support agent](https://github.com/nenedesign/n8n-workflows/tree/main/ai-agents/autonomous-customer-support-agent) | AI Agents | Advanced | [View](https://github.com/nenedesign/n8n-workflows/blob/main/ai-agents/autonomous-customer-support-agent/preview.png) |
| [Multi-KB agentic RAG assistant](https://github.com/nenedesign/n8n-workflows/tree/main/rag/multi-kb-agentic-rag-assistant) | RAG | Advanced | [View](https://github.com/nenedesign/n8n-workflows/blob/main/rag/multi-kb-agentic-rag-assistant/preview.png) |
| [Slack Gemini Agent](https://github.com/nenedesign/n8n-workflows/tree/main/ai-agents/slack-gemini-agent) | AI Agents | Intermediate | [View](https://github.com/nenedesign/n8n-workflows/blob/main/ai-agents/slack-gemini-agent/preview.png) |
| [Gmail AI Triage](https://github.com/nenedesign/n8n-workflows/tree/main/ai-agents/gmail-ai-triage) | AI Agents | Intermediate | [View](https://github.com/nenedesign/n8n-workflows/blob/main/ai-agents/gmail-ai-triage/preview.png) |
| [Seed Supabase from Notion](https://github.com/nenedesign/n8n-workflows/tree/main/rag/seed-supabase-from-notion) | RAG | Intermediate | [View](https://github.com/nenedesign/n8n-workflows/blob/main/rag/seed-supabase-from-notion/preview.png) |
| [AI Daily Briefing Bot](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/ai-daily-briefing-bot) | Utilities | Beginner | [View](https://github.com/nenedesign/n8n-workflows/blob/main/utilities/ai-daily-briefing-bot/preview.png) |
| [Claude to Slack MCP Test](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/claude-to-slack-mcp-test) | Utilities | Beginner | [View](https://github.com/nenedesign/n8n-workflows/blob/main/utilities/claude-to-slack-mcp-test/preview.png) |
| [URL & Article Summarizer to Slack](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/url-article-summarizer-to-slack) | Utilities | Beginner | [View](https://github.com/nenedesign/n8n-workflows/blob/main/utilities/url-article-summarizer-to-slack/preview.png) |
| [API Health Monitor](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/api-health-monitor) | Utilities | Beginner | [View](https://github.com/nenedesign/n8n-workflows/blob/main/utilities/api-health-monitor/preview.png) |
| [RSS Feed to Slack Alert](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/rss-feed-to-slack-alert) | Utilities | Beginner | [View](https://github.com/nenedesign/n8n-workflows/blob/main/utilities/rss-feed-to-slack-alert/preview.png) |
| [GitHub PR to Slack Notifier](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/github-pr-to-slack-notifier) | Utilities | Beginner | [View](https://github.com/nenedesign/n8n-workflows/blob/main/utilities/github-pr-to-slack-notifier/preview.png) |
| [AI Webhook Classifier](https://github.com/nenedesign/n8n-workflows/tree/main/utilities/ai-webhook-classifier) | Utilities | Intermediate | [View](https://github.com/nenedesign/n8n-workflows/blob/main/utilities/ai-webhook-classifier/preview.png) |

---

## System Architecture

Production customer support agent with 50 nodes, async webhook intake, multi-KB RAG with web search fallback, confidence-gated routing, and full audit trail.

```mermaid
flowchart LR
    A["Inbound Request\nWebhook · Slack · Email"] --> B["Auth · Rate Limit · PII Scrub"]
    B --> C["202 Accepted"]
    B --> D["AI Support Agent"]
    D --> E[("Primary KB")]
    D --> F[("Reference KB")]
    D --> G["Web Search Fallback"]
    E & F & G --> H{"Confidence\nScore"}
    H -- High --> I["Auto-Reply\nSlack · Email · Webhook"]
    H -- Low --> J["Human Escalation\n+ Audit Log"]
```

---

## Research Focus

- **Multi-Agent Orchestration** — modality-agnostic, agent-to-agent workflows focused on security and privacy
- **Privacy-First Local AI** — on-device open-weight models for sensitive financial and healthcare data
- **Context & Memory Management** — hybrid memory retrieval for context-aware personalization
- **Hybrid Inference Routing** — optimizing token efficiency, latency, and cost across cloud and local

---

## Stack

**Automation & Agents:** `n8n` · `Claude Code` · `MCP Servers` · `LangChain` · `Google ADK`  
**Inference & Models:** `Ollama` · `Docker` · `OpenRouter` · `Claude API` · `Gemini API` · `Perplexity API`  
**Data & Storage:** `Supabase` · `Postgres` · `Notion` · `Obsidian` · `Open WebUI`

---

**Links:** [Portfolio](https://www.fromus.ca/ai-builds) · [LinkedIn](https://www.linkedin.com/in/nevilleko/) · [n8n Official Creator](https://n8n.io/workflows/18427-seed-a-supabase-ai-knowledge-base-from-notion-with-ollama-embeddings/) · [n8n Marketplace](https://n8n.io/creators/)

---

Open to advisory, consulting, and collaboration on AI automation, agentic systems, and governance-aware AI for regulated industries — [connect on LinkedIn](https://www.linkedin.com/in/nevilleko/)
