<div align="center">

# Iliass Malki

**Software Engineer — AI & DevOps**
Casablanca, Morocco

I build LLM agents that survive contact with production — and the Azure infrastructure they run on.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Iliass_Malki-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/iliass-malki-0794a5302/)
[![Email](https://img.shields.io/badge/Email-iliassmalki@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:iliassmalki@gmail.com)
[![Oracle Certified](https://img.shields.io/badge/Oracle_Cloud-3×_Certified_2025-F80000?style=flat-square&logo=oracle&logoColor=white)](#credentials)

</div>

---

## What I actually do

Most "AI engineers" ship a chatbot. I ship the whole system around it: the retrieval layer that keeps
answers grounded, the tool interface the model calls, the identity boundary it can't cross, the
Terraform that stands it all up, and the pipeline that redeploys it on every merge.

Over the last year I've put **eight AI systems into production** at a BPO/CX group — email copilots,
multi-agent CRM assistants, RAG ordering agents, and autonomous French-speaking phone agents that
answer real customer calls end to end, with no human in the loop.

<table>
<tr>
<td width="33%" valign="top">

### 🤖 AI & agents
LangChain · LangGraph multi-agent · RAG over Azure AI Search & ChromaDB · MCP tool servers ·
Azure OpenAI / AI Foundry · Realtime API speech-to-speech · LangSmith tracing · PII anonymization ·
prompt-injection hardening

</td>
<td width="33%" valign="top">

### ☁️ DevOps & cloud
Terraform (Azure IaC) · GitHub Actions CI/CD · Docker & Compose · Kubernetes ·
Azure Container Apps, App Gateway WAF, Key Vault, ACR, managed identity ·
Keycloak zero-trust (OIDC/PKCE/JWKS) · OpenTelemetry + Grafana

</td>
<td width="33%" valign="top">

### 🧱 Full-stack
FastAPI · Spring Boot · Node/Express · React 19 + Vite · Next.js 16 · Angular ·
React Native (Expo) · PostgreSQL, MongoDB, Redis, Cosmos · hexagonal & layered architecture

</td>
</tr>
</table>

---

## Selected work

> Professional projects were built at **Outsourcia** (BPO/CX group) and live in private repos.
> End clients are under NDA — described by sector only.

| Project | What it is | The hard part |
| --- | --- | --- |
| **Agent Assist** | Multi-service AI support platform augmenting human agents across email, live calls and WhatsApp | **16 Terraform modules**, **5 CI/CD pipelines**, a 6-service stack behind Keycloak zero-trust, and real-time call insights (LiveKit → Silero VAD → Azure Speech → LLM) streamed over WebSocket |
| **LCI Agent Assist** | Multi-agent copilot inside the Dynamics 365 Smart Assist panel | LangGraph graph routing across ~10 institutions, PII stripped before the LLM ever sees it, and a 👍/👎 → OpenTelemetry → Grafana feedback loop. I owned the full Azure infra. |
| **Voice Agent (speech-to-speech)** | Autonomous French phone agent for a retail client — recognizes the caller, looks up orders, books appointments, files tickets | Azure Realtime API over WebSocket with **barge-in truncation**, per-call prompt injection from the caller's number, **9 model-callable tools**, and a **hand-rolled SIP↔WebRTC bridge** (Janus + aiortc) alongside the Twilio path |
| **OLPA** | B2B commercial-intelligence platform — crawls business signals, enriches companies, synthesizes sales briefs | Async Crawl4AI/Playwright ETL into MongoDB + an agentic Next.js 16 chat with 14 read/write DB tools |
| **Doctolib MCP Server** | MCP server exposing booking automation as LLM-callable tools | Wrapping Selenium as MCP without touching it, and squeezing every Docker layer **under the 200 MB registry limit** via 7 staged pip installs |
| **Kaoul Agent** | RAG conversational ordering assistant (mobile + back-office) | PDF → embeddings → ChromaDB ingestion behind a clean FastAPI service architecture |

---

## Public repos

| Repo | What | Stack |
| --- | --- | --- |
| [**self-hosted-whatsapp-ai-assistant**](https://github.com/Iliassmalki/self-hosted-whatsapp-ai-assistant) | AI that answers your WhatsApp — **no API key, no Meta subscription**. Shells out to a local Claude CLI instead. ~130 lines. Sandboxed subprocess, message fencing, and hard rules enforced in code after a prompt-only rule failed. | Node.js, puppeteer |
| [**medicalconsultationmanager**](https://github.com/Iliassmalki/medicalconsultationmanager) | Hospital appointment platform with AI-assisted scheduling and end-to-end RBAC | Spring Boot, Spring Security, Angular, langchain4j + Mistral |
| [**SmartTicketManagerwithkpis**](https://github.com/Iliassmalki/SmartTicketManagerwithkpis) | Event ticketing app with a real star-schema warehouse feeding Metabase KPI dashboards | React Native, Express/Sequelize, PostgreSQL, Metabase |
| [**androidquizz**](https://github.com/Iliassmalki/androidquizz) | Native Android quiz with **camera-based anti-cheat** and AI-generated questions | Java, Android |

---

## Credentials

- **Oracle Cloud Infrastructure 2025 — Certified DevOps Professional**
- **Oracle Cloud Infrastructure 2025 — AI Foundations Professional**
- **Oracle Cloud Infrastructure 2025 — AI Foundations Associate**

**Engineering degree in Software Engineering** — EMSI Casablanca, 2021–2026.

---

## How I work

- **Root cause over patch.** One guard in the shared function beats a guard in every caller.
- **Audit first, then fix.** I read the whole flow before touching it — the smallest diff in the wrong place is just a second bug.
- **Rules in code, not in prompts.** If an LLM must not do something, the guardrail lives outside the model.
- **Ship it, then document it.** Every system I build gets an architecture note and a living ops note.

---

<div align="center">

**Arabic** (native) · **French** (fluent) · **English** (fluent)

[iliassmalki@gmail.com](mailto:iliassmalki@gmail.com) · [LinkedIn](https://www.linkedin.com/in/iliass-malki-0794a5302/)

</div>
