## Khaneil Campbell

**AI Solutions Engineer**

[khaneilcampbell.com](https://khaneilcampbell.com) · [LinkedIn](https://www.linkedin.com/in/khaneil-campbell) · contact@khaneilcampbell.com · [Benjaire](https://benjaire.com) 

### About

I have spent more than four years supporting the Columbia University community, with earlier IT roles at NYC Health + Hospitals, Montefiore and Buffalo State University. Resolving incidents and service requests for people who need to get back to work taught me to look past the first request to the real problem, and to earn trust with evidence rather than promises.

I bring that same discipline to AI. I build agents and integrations with Claude, MCP, CrewAI and n8n, with validation and human oversight designed in from the start. In Benjaire Flow, Claude drafts every reply but never sends one. In Atlas, nothing changes without my approval and an audit log entry. My approach is simple: solve problems with evidence, automate with intention and build systems people can trust.

*Fix it twice, document it. Ten times, automate it.*

### What I do

- **Discovery and scoping.** Turn a stakeholder's request into requirements I label verified, proposed or needs evidence, before writing code.
- **Agents and LLM integration.** Claude through the Anthropic API and MCP servers, CrewAI multi-agent pipelines and n8n workflows wired into real tools like Stripe, Canva, GitHub and email.
- **Shipping with guardrails.** Schema validation and citation checks on model output, spend caps, human approval gates, CI tests, secret scanning, CodeQL and strict Content Security Policies.
- **Adoption.** Runbooks, setup guides and knowledge articles written in the Knowledge-Centered Service style I used on the service desk.

### Selected work

| Project | Problem → what I built → how it's verified → outcome |
|---|---|
| [**Atlas**](https://github.com/khaneilcampbell/ai-ops-atlas) | I needed one place to see every agent, workflow and repository I run. Built a Tauri (Rust + React/TypeScript) Mac app and a Cloudflare Pages web build. Its Repository Intelligence agent sends one Claude request per run, validates the JSON against a schema, drops citations the model invented and enforces per-run and monthly spend caps. Write actions need Touch ID and are audit-logged. 139 test files, Playwright visual checks, a performance budget and CodeQL run in CI, and every merge ships a signed build. |
| [**Benjaire Flow**](https://benjaire.com/digital/flow) | Small service firms lose leads in their inbox. Built six importable n8n workflows: Claude sorts each website inquiry and drafts a reply for the owner to approve (it never sends to prospects), with reminders, a weekly digest and error alerts behind a Cloudflare Worker form with Turnstile. 17 test scenarios run before go-live, and an eval suite scores the sorting on 60 labeled inquiries: 100% spam and budget accuracy, 98% service match, 5 of 5 prompt-injection attempts resisted. Released as v1.0 with Stripe checkout. |
| [**Multi-Agent Commerce Pipeline**](https://github.com/khaneilcampbell/multi-agent-commerce-pipeline) | Take a digital product from idea to sale without manual handoffs. CrewAI agents on Claude plan the brand and listings, Canva's MCP server makes the designs, and Stripe sells them from a static storefront, run by systemd on a Linux VPS. New products stay drafts until I approve them, Stripe calls are idempotent, and 58 tests, gitleaks and pip-audit run in CI. |
| [**Splunk Brute Force Detection Lab**](https://github.com/khaneilcampbell/splunk-bruteforce-detection-lab) | Detection and observability from end to end. Simulated SMB brute force from Kali on Windows 11, caught it with a Splunk threshold alert (81 failed logons) and wrote triage notes automatically in Python through the Splunk REST API, with unit tests and step-by-step evidence |

### Latest on GitHub

<!-- This section is regenerated daily by .github/workflows/update-readme.yml. Edits between the markers are overwritten. -->
<!-- AUTO:REPOS:START -->
**5** public repositories · **6** stars · Top languages: Python, TypeScript, Astro, HTML

| Repository | About | Language | Updated |
|---|---|---|---|
| [**ai-ops-atlas**](https://github.com/khaneilcampbell/ai-ops-atlas) ★1 | Atlas is a secure, observable AI operations control plane that unifies enterprise infrastructure, repositories, business workflows, and autonomous agents into one intelligent operating platform. | TypeScript | 2026-11-08 |
| [**benjaire.com**](https://github.com/khaneilcampbell/benjaire.com) ★1 | Independent project: static website for Benjaire, a New York company, deployed on GitHub Pages and Cloudflare `accessibility` `cloudflare-pages` `github-pages` `html-css` | Astro | 2026-11-07 |
| [**multi-agent-commerce-pipeline**](https://github.com/khaneilcampbell/multi-agent-commerce-pipeline) ★2 | Multi-agent product pipeline: CrewAI agents on Claude, Canva MCP, and Shopify, deployed on a Linux VPS `ai-agents` `anthropic` `crewai` `mcp` | Python | 2026-11-04 |
| [**splunk-bruteforce-detection-lab**](https://github.com/khaneilcampbell/splunk-bruteforce-detection-lab) ★1 | Security operations lab simulating SMB brute-force attacks, with Splunk detection engineering and automated case triage in Python `blue-team` `cybersecurity` `detection-engineering` `python` | Python | 2026-11-02 |
| [**khaneilcampbell.com**](https://github.com/khaneilcampbell/khaneilcampbell.com) ★1 | AI-assisted portfolio site on GitHub Pages with Cloudflare DNS and automated security checks `accessibility` `cloudflare` `github-actions` `github-pages` | HTML | 2026-10-28 |
<!-- AUTO:REPOS:END -->

### Stack

| Area | Tools |
|---|---|
| **AI and agents** | Claude, Claude Code, Anthropic API, MCP servers and connectors, CrewAI, n8n |
| **Languages** | Python, TypeScript, Rust (Tauri), PowerShell, SQL, Splunk SPL |
| **Cloud, CI/CD and infrastructure** | GitHub Actions, Cloudflare Workers and Pages (D1, Access), Linux VPS with systemd, Docker, Git |
| **Security and observability** | Splunk Enterprise, CodeQL, gitleaks, pip-audit, Dependabot, CSP, MITRE ATT&CK, NIST incident response |
| **Enterprise IT** | ServiceNow, Confluence, Active Directory, Cisco Duo MFA, ITIL 4, Knowledge-Centered Service |

### Certifications

CompTIA Security+ · ITIL 4 Foundation · HDI KCS Foundation · HDI Customer Service Representative · AI Literacy: Advanced Course for Developers (Columbia University)
