# Hi, I'm Adam Blansett

**Senior Full-Stack & AI Engineer** · Cincinnati, OH area

I've spent 10+ years building and modernizing enterprise software in banking, healthcare, aviation, logistics, and market research. These days I build my own products and run AI systems on open-source models I host myself.

[Website](https://adamblansett.com) · [Blog](https://adamblansett.com/blog/) · [LinkedIn](https://linkedin.com/in/adamblansett) · [X](https://x.com/AdamBlansett) · [Email](mailto:Adam.Blansett@gmail.com)

---

## What I'm building

**Self-hosted AI systems.** I run open-source LLMs (Llama, Qwen, DeepSeek) on llama.cpp, Ollama, and Hugging Face and fine-tune them with LoRA. I'm also building a training pipeline where larger models generate and evaluate the training data used to fine-tune smaller self-hosted ones (synthetic data plus distillation). These models power my products below as well as my open-source AI platforms.

**Divinari.** A language-learning platform that brings together language study, cultural heritage, and faith-based learning. It pairs a Next.js web platform with Flutter mobile apps built with Riverpod and Clean Architecture on an offline-first data layer, with AI-assisted instruction from my self-hosted models plus Gemini.

**OmniScreener.** A crypto analysis and paper-trading research platform. It pulls Coinbase market data and technical indicators, runs ML-assisted analysis, and tracks experiments so I can check how its calls actually turned out.

## Open-source AI platforms

Self-hosted, privacy-first AI systems built around local open-weight models, PII/privilege guardrails, and human-in-the-loop approvals.

| Project | What it does |
|---|---|
| [ai-paralegal](https://github.com/adamblansett/ai-paralegal) | Legal ops platform for OCR document ingestion, playbook contract review with Word Track Changes redlines, citation-backed research Q&A, PII/privilege guardrails, Bates stamping, and attorney review (FastAPI, pgvector, Celery, React) |
| [ai-recruiter](https://github.com/adamblansett/ai-recruiter) | Job discovery, DNS-verified recruiter lookup, LLM fit evaluation, and Gmail outreach behind a human approval gate (FastAPI, Celery, React) |
| [ai-hr-platform](https://github.com/adamblansett/ai-hr-platform) | Standalone HR microservice for full employee lifecycle operations (integrates with `ai-recruiter`), RAG policy Q&A, leave/benefits/LMS, expense auditing, and performance reviews (FastAPI, pgvector, React) |
| [ai-customer-service](https://github.com/adamblansett/ai-customer-service) | Self-hosted AI contact center for inbound voice (Twilio/SIP/FreeSWITCH, sub-500ms barge-in) and web chat with human escalation (Next.js, Express) |
| [virtual-assistant](https://github.com/adamblansett/virtual-assistant) | Privacy-first autonomous executive assistant on local LLMs (Ollama/vLLM) with MCP tools and Telegram/Slack/WhatsApp approvals (Next.js) |

## Open-source developer tools

| Project | What it does |
|---|---|
| [llm-eval-toolkit](https://github.com/adamblansett/llm-eval-toolkit) | Local contract-based evaluation framework that tests AI outputs against expectations, catches regressions, and compares model or prompt changes |
| [ai-app-production-auditor](https://github.com/adamblansett/ai-app-production-auditor) | Offline CLI that audits web apps (especially AI-generated ones) for config issues, exposed secrets, missing quality checks, and deployment risks |
| [frontend-backend-diagnostic](https://github.com/adamblansett/frontend-backend-diagnostic) | Diagnostic CLI that traces frontend/backend integration failures, including URL mismatches, CORS, auth, and contract drift |
| [flutter-offline-first-starter](https://github.com/adamblansett/flutter-offline-first-starter) | Starter kit for Flutter apps (Drift/SQLite, Riverpod) that keep working offline and sync when the connection returns |
| [webhook-reliability-workbench](https://github.com/adamblansett/webhook-reliability-workbench) | Captures, inspects, and replays webhooks locally; verifies HMAC signatures and simulates delivery failures |
| [api-contract-tester](https://github.com/adamblansett/api-contract-tester) | CLI that validates HTTP APIs against explicit contracts, imports OpenAPI specs, and catches integration regressions |
| [release-readiness-action](https://github.com/adamblansett/release-readiness-action) | GitHub Action ([Marketplace](https://github.com/marketplace/actions/release-readiness-action)) and CLI that checks structure, docs, local secrets, and dependencies before a release deploys |

## Where I've worked

- **Fifth Third Bank:** Spring Boot microservices on the authorization team, part of the authentication infrastructure that handled the bank's logins
- **GE Aviation:** Node.js APIs for aviation maintenance and fleet data, with ~95% automated test coverage
- **CareStar:** Laravel and Angular applications used to determine eligibility for government services
- **Directions Research:** Technical lead across 20+ enterprise applications; ran RabbitMQ for about 3 years across thousands of queues; built Salesforce integrations

## Tech I work with

- **Languages:** Java · TypeScript · JavaScript · PHP · Python · Dart · SQL
- **Frameworks:** Spring Boot · Node.js/Express · FastAPI · Laravel · Angular · React · Next.js · Flutter
- **AI & ML:** Llama · Qwen · DeepSeek · llama.cpp · Ollama · Hugging Face · LoRA · RAG · MCP · Gemini API
- **Infrastructure & Data:** AWS · Docker · Kubernetes · Prometheus · RabbitMQ · Redis · Celery · PostgreSQL (pgvector) · MySQL · MongoDB · SQLite/Drift
- **Security:** OAuth 2.0 · OIDC · SSO · JWT · HashiCorp Vault · AES-256-GCM

---

Need help with a production problem, a new build, or private AI on your own infrastructure? [Book a free 30-minute call](https://adamblansett.com/book/) or see my [48-hour codebase audit](https://adamblansett.com/services/).
