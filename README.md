## Khaneil Campbell

**AI Solutions Engineer · Forward Deployed Engineer**

[khaneilcampbell.com](https://khaneilcampbell.com) · [LinkedIn](https://www.linkedin.com/in/khaneil-campbell) · contact@khaneilcampbell.com · [Benjaire](https://benjaire.com) 

### About

I have spent more than four years supporting the Columbia University community, with earlier IT roles at NYC Health + Hospitals, Montefiore and Buffalo State University. Resolving incidents and service requests for people who need to get back to work taught me to look past the first request to the real problem, and to earn trust with evidence rather than promises.

I bring that same discipline to AI. I build agents and integrations with Claude, MCP, CrewAI and n8n, with validation and human oversight designed in from the start. In Benjaire Flow, Claude drafts every reply but never sends one. In Atlas, nothing changes without my approval and an audit log entry. My approach is simple: solve problems with evidence, automate with intention and build systems people can trust.

*Fix it twice, document it. Ten times, automate it.*

### What I do

- **Discovery and scoping.** Turn a stakeholder's request into requirements I label verified, proposed or needs evidence, before writing code.
- **Agents and LLM integration.** Claude through the Anthropic API and MCP servers, CrewAI multi-agent pipelines and n8n workflows wired into real tools like Stripe, Canva, GitHub and email.
- **Integrations and data.** Policy-scoped data APIs over PostgreSQL for n8n and agents, signed workflow-start paths, and durable storage for agent outputs.
- **Shipping with guardrails.** Schema validation and citation checks on model output, spend caps, human approval gates, CI tests, secret scanning, CodeQL and strict Content Security Policies.
- **Adoption.** Runbooks, setup guides and knowledge articles written in the Knowledge-Centered Service style I used on the service desk.

### Selected work

| Project | Problem → what I built → how it's verified → outcome |
|---|---|
| [**Atlas**](https://github.com/khaneilcampbell/ai-ops-atlas) | I needed one place to see and run every agent, workflow and repository I operate. Built a Tauri (Rust + React/TypeScript) Mac app and a Cloudflare Pages web build, with a Mission Control surface where I plan, approve and delegate goals to agents, and Phase 9 autonomous operations that correlate incidents and run read-only recovery playbooks under per-playbook policy, with an emergency stop and a redacted audit trail. The Repository Intelligence agent sends one Claude request per run, validates the JSON against a schema, drops citations the model invented and enforces per-run and monthly spend caps. Earlier additions: a PostgreSQL data foundation with a policy-scoped data API for n8n and agents, where agent changes to records become approvals rather than overwrites; a Task Center path that starts two n8n workflows through signed, allow-listed requests with input checks, daily caps, idempotency keys and Touch ID on the Mac; and an Output Library that stores agent reports in D1 metadata and a private R2 bucket. Most recently, a searchable Projects directory lists every Atlas project with its status, linked repositories and assigned agents, and Intel is reorganised into Intelligence, Activity, API and Repositories tabs. Newest: an Atlas Executive control plane (Phase 1) orchestrates goals on the Postgres database with bounded lifecycles, action-bound approvals, template plans, n8n dispatch with idempotency keys and authenticated result callbacks; its catalog entry stays paused until the two n8n drafts are published. Persistent agent memory and task memory let agents check existing work before acting (create, update, skip, wait, retry or escalate), and agent-written memory stays unverified until I verify it. Agent-occupancy markers on the map show which agents are inside each building. Also, the Mac app reads the Output Library and the database overview through new read-only website sync routes, authenticated with a sync key kept in the Keychain, so no database or agent credentials reach the app; a Team Residence Towers view lets you visit each agent's apartment workspace; and the Atlas Start webhook for a published n8n agent is live and refuses unsigned requests. Write actions are audit-logged. 139 test files, Playwright visual checks, a performance budget and CodeQL run in CI, and every merge ships a signed build. |
| [**Benjaire Flow**](https://benjaire.com/digital/flow) | Small service firms lose leads in their inbox. Built six importable n8n workflows: Claude sorts each website inquiry and drafts a reply for the owner to approve (it never sends to prospects), with reminders, a weekly digest and error alerts behind a Cloudflare Worker form with Turnstile. 17 test scenarios run before go-live, and an eval suite scores the sorting on 60 labeled inquiries: 100% spam and budget accuracy, 98% service match, 5 of 5 prompt-injection attempts resisted. Released as v1.0 with Stripe checkout. |
| [**Multi-Agent Commerce Pipeline**](https://github.com/khaneilcampbell/multi-agent-commerce-pipeline) | Take a digital product from idea to sale without manual handoffs. CrewAI agents on Claude plan the brand and listings, Canva's MCP server makes the designs, and Stripe sells them from a static storefront, run by systemd on a Linux VPS. New products stay drafts until I approve them, Stripe calls are idempotent, and 58 tests, gitleaks and pip-audit run in CI. |
| [**Splunk Brute Force Detection Lab**](https://github.com/khaneilcampbell/splunk-bruteforce-detection-lab) | Detection and observability from end to end. Simulated SMB brute force from Kali on Windows 11, caught it with a Splunk threshold alert (81 failed logons) and wrote triage notes automatically in Python through the Splunk REST API, with unit tests and step-by-step evidence |

### Recent activity

- **2026-11-23** — Atlas: agent-occupancy markers on the map show which agents are inside each building, with hover, keyboard and touch support and a click-through to the building's Inside view.
- **2026-11-22** — Atlas: persistent agent memory and task memory in the Atlas database, with a pre-run check that tells each agent whether to create, update, skip, wait, retry or escalate.
- **2026-11-22** — Atlas: Atlas Executive control plane (Phase 1) for server-side goal orchestration, with action-bound approvals, idempotency keys and authenticated result callbacks.
- **2026-11-22** — Atlas: review references shown in plain words, and the merge and signing kill switches documented.

### Latest on GitHub

<!-- This section is regenerated daily by .github/workflows/update-readme.yml. Edits between the markers are overwritten. -->
<!-- AUTO:REPOS:START -->
**5** public repositories · **4** stars · Top languages: Python, TypeScript, Astro, HTML

| Repository | About | Language | Updated |
|---|---|---|---|
| [**splunk-bruteforce-detection-lab**](https://github.com/khaneilcampbell/splunk-bruteforce-detection-lab) | Security operations lab simulating SMB brute-force attacks, with Splunk detection engineering and automated case triage in Python `blue-team` `cybersecurity` `detection-engineering` `python` | Python | 2026-11-23 |
| [**ai-ops-atlas**](https://github.com/khaneilcampbell/ai-ops-atlas) ★1 | Atlas is a secure, observable AI operations control plane that unifies enterprise infrastructure, repositories, business workflows, and autonomous agents into one intelligent operating platform. | TypeScript | 2026-11-23 |
| [**benjaire.com**](https://github.com/khaneilcampbell/benjaire.com) ★1 | Independent project: static website for Benjaire, a New York company, deployed on GitHub Pages and Cloudflare `accessibility` `cloudflare-pages` `github-pages` `html-css` | Astro | 2026-11-17 |
| [**khaneilcampbell.com**](https://github.com/khaneilcampbell/khaneilcampbell.com) | AI-assisted portfolio site on GitHub Pages with Cloudflare DNS and automated security checks `accessibility` `cloudflare` `github-actions` `github-pages` | HTML | 2026-11-16 |
| [**multi-agent-commerce-pipeline**](https://github.com/khaneilcampbell/multi-agent-commerce-pipeline) ★2 | Multi-agent product pipeline: CrewAI agents on Claude, Canva MCP, and Shopify, deployed on a Linux VPS `ai-agents` `anthropic` `crewai` `mcp` | Python | 2026-11-11 |
<!-- AUTO:REPOS:END -->

### Stack

| Area | Tools |
|---|---|
| **AI and agents** | Claude, Claude Code, Anthropic API, MCP servers and connectors, CrewAI, n8n |
| **Languages** | Python, TypeScript, Rust (Tauri), PowerShell, SQL, Splunk SPL |
| **Frontend and testing** | React, Playwright visual checks, performance budgets |
| **Data and storage** | PostgreSQL (Supabase), Cloudflare D1 and R2 |
| **Cloud, CI/CD and infrastructure** | GitHub Actions, Cloudflare Workers, Pages and Access, Linux VPS with systemd, Docker, Git |
| **Security and observability** | Splunk Enterprise, CodeQL, gitleaks, pip-audit, Dependabot, CSP, MITRE ATT&CK, NIST incident response |
| **Enterprise IT** | ServiceNow, Confluence, Active Directory, Cisco Duo MFA, ITIL 4, Knowledge-Centered Service |

### Certifications

CompTIA Security+ · ITIL 4 Foundation · HDI KCS Foundation · HDI Customer Service Representative · AI Literacy: Advanced Course for Developers (Columbia University)
