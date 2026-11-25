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

### Flagship AI platforms

| Project | What it does |
|---|---|
| [ai-paralegal](https://github.com/adamblansett/ai-paralegal) | Legal ops platform for OCR document ingestion, playbook contract review with Word Track Changes redlines, citation-backed research Q&A, PII/privilege guardrails, Bates stamping, and attorney review (FastAPI, pgvector, Celery, React) |
| [ai-finance-ops](https://github.com/adamblansett/ai-finance-ops) | Self-hosted AI finance operations platform implementing PDF/CSV/JSON ingestion with SHA-256 dedup, 3-way PO/GR/invoice reconciliation, AP/AR settlement matching, 13-week cash flow & scenario modeling, expense auditing, and SHA-256 SOX audit chains behind Controller approval gates (FastAPI, pgvector, Redis, React) |
| [ai-recruiter](https://github.com/adamblansett/ai-recruiter) | Job discovery, DNS-verified recruiter lookup, LLM fit evaluation, and Gmail outreach behind a human approval gate (FastAPI, Celery, React) |
| [ai-hr-platform](https://github.com/adamblansett/ai-hr-platform) | Standalone HR microservice for full employee lifecycle operations (integrates with `ai-recruiter`), RAG policy Q&A, leave/benefits/LMS, expense auditing, and performance reviews (FastAPI, pgvector, React) |
| [ai-customer-service](https://github.com/adamblansett/ai-customer-service) | Self-hosted AI contact center for inbound voice (Twilio/SIP/FreeSWITCH, sub-500ms barge-in) and web chat with human escalation (Next.js 16, Express) |
| [virtual-assistant](https://github.com/adamblansett/virtual-assistant) | Privacy-first autonomous executive assistant on local LLMs (Ollama/vLLM) with MCP tools and Telegram/Slack/WhatsApp approvals (Next.js) |

### Autonomous AI workforce platforms (Phase 1 & Phase 2 MVPs)

All 10 MIT-licensed enterprise operations MVPs below are implemented on a shared FastAPI / SQLAlchemy 2.0 / PostgreSQL (`pgvector`) / React 18 / TypeScript stack featuring local-first Ollama inference + offline mock modes, default cloud PII redaction (`LLM_REDACT_PII_FOR_CLOUD=true`), HITL approval gates, SHA-256 hash-chained audit trails, Docker Compose, and GitHub Actions CI (`ruff`, `mypy`, `pytest`, `vitest`, `npm audit`, Trivy):

| Phase | Platform | Implemented MVP Capabilities |
|---|---|---|
| Phase 1 | [ai-sdr](https://github.com/adamblansett/ai-sdr) | Outbound prospecting & verified buying signals with retroactive opt-out suppression, 5-dimension ICP (`A`–`D`) + BANT/MEDDIC scoring, manager-gated sequences, CRM hygiene & HITL dedup merges, and HMAC CRM webhooks |
| Phase 1 | [ai-it-admin](https://github.com/adamblansett/ai-it-admin) | Joiner/mover/leaver SCIM 2.0 dry-run provisioning diffs, service telemetry & TLS/quota incident triage, SaaS access/MFA audits, and `advisory_only` hybrid vector+keyword runbooks RAG behind IT approver RBAC |
| Phase 1 | [ai-insurance-ops](https://github.com/adamblansett/ai-insurance-ops) | ACORD/policy clause indexing & hybrid search, FNOL claims triage & weighted SIU scoring, citation-grounded coverage verification, 3/5-year loss-run underwriting risk analysis, and PII/PHI redaction sandbox |
| Phase 1 | [ai-logistics-coordinator](https://github.com/adamblansett/ai-logistics-coordinator) | HMAC carrier webhook & X12 EDI 214 freight tracking, multi-constraint carrier route optimization, `409`-enforced HITL carrier comms approval gate, and ASN/BOL warehouse shrinkage reconciliation |
| Phase 2 | [ai-admin-agent](https://github.com/adamblansett/ai-admin-agent) | IANA timezone-aware multi-party scheduling solver, corporate travel policy & disruption contingency planner, cited pre-meeting briefing dossiers, and `P0`–`P3` SLA correspondence triage with HITL draft approvals |
| Phase 2 | [ai-qa-release-engineer](https://github.com/adamblansett/ai-qa-release-engineer) | OpenAPI 3.x & user-flow Playwright TypeScript + `pytest`/`httpx` E2E test synthesis, CI failure root-cause triage + GitHub Actions security audits (`WF001`–`WF008`), LLM-eval regression checks, and SSRF-guarded Go/No-Go release gates |
| Phase 2 | [ai-compliance-auditor](https://github.com/adamblansett/ai-compliance-auditor) | 18-control SOC 2 TSC / HIPAA / GDPR registry, deterministic config/encryption/logging/RBAC/SOP policy scanners, tamper-evident evidence bundle verification, and 30-day DSAR workflows with `409` legal-hold blocks |
| Phase 2 | [ai-procurement-manager](https://github.com/adamblansett/ai-procurement-manager) | 8-family MSA/DPA/Order Form playbook contract diffing, P25/median/P75 SKU/SaaS pricing benchmarks, quote-to-PO budget validation with tiered approvals, and renewal deadline renegotiation workflows |
| Phase 2 | [ai-localization-manager](https://github.com/adamblansett/ai-localization-manager) | Round-trip JSON/PO/Flutter ARB/Markdown catalog sync, `pgvector` semantic translation memory & DNT termbases, ICU/placeholder/HTML/RTL BiDi/formality QA, pseudo-localization, and CI missing-key release gates |
| Phase 2 | [ai-data-governance](https://github.com/adamblansett/ai-data-governance) | Checksum-validated PII detection (`redact`/`mask`/`hash` + HKDF/Fernet vault `tokenize`/`detokenize`), Jaro-Winkler/Soundex undoable HITL record deduplication, E.164/USPS/ISO normalizers, and PostgreSQL schema hygiene audits |

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

Need help with a production problem, a new build, or private AI on your own infrastructure? [Book a free 30-minute call](https://adamblansett.com/book/) or try the [48-hour codebase audit portal](https://audit.adamblansett.com/).
