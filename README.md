<h1 align="center">Tajamul Wani</h1>

<p align="center">
  <b>GTM Infrastructure Engineer</b> &nbsp;·&nbsp; Marketing Operations &nbsp;·&nbsp; API Integrations & Data Flow &nbsp;·&nbsp; Full-Stack Development with Claude Code
</p>

<p align="center">
  <sub>I build the systems and tools that power go-to-market operations.<br/>
  Data pipelines, API orchestration, debugging & monitoring infrastructure, and the software that makes marketing systems talk to each other.</sub>
</p>

<p align="center">
  <a href="https://tajamul-wani.netlify.app"><img src="https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=google-chrome&logoColor=white" /></a>
  &nbsp;
  <a href="https://linkedin.com/in/tajamul-wani"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" /></a>
  &nbsp;
  <a href="mailto:tajamul.270@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" /></a>
</p>

<br/>

---

## What I do right now

**GTM infrastructure** — I build the systems that power marketing operations. Not just configuring CRM pipelines, but designing data flows, building APIs that connect disparate systems, and creating the infrastructure that turns marketing intent into predictable pipeline.

**API orchestration & debugging** — I own the plumbing: REST APIs, webhooks, data transformations, and the monitoring that catches when systems fail silently. I build tools to inspect API responses, trace data flow, and debug why a lead didn't sync when it should have.

**Full-stack tooling with Claude Code** — I architect systems that Claude builds. I specify behaviour precisely, direct the development, review every component, and ship infrastructure that operates itself. No hand-written code — just tight specs and AI-directed builds.

**Operations & observability** — Linux servers, production deployment, log analysis, error tracking with Sentry, and the automation that keeps systems synchronized. I read logs, trace failures, and fix broken infrastructure.

<br/>

---

## How I build GTM infrastructure

I design systems that solve real problems in marketing operations: data moving between platforms without loss, APIs that behave predictably, and tools that let us see what's actually happening.

The constraint is intentional: I don't write code by hand. I architect, specify, direct Claude Code, review output, and operate it. This forces clarity — if I can't describe a system architecture clearly enough for an AI to build it, it's not ready to ship.

The payoff: infrastructure that's well-understood, maintainable, and built with the full complexity of the problem baked in from the start.

<br/>

| Layer | What I own |
|---|---|
| **Architecture** | Data model, system boundaries, API design, integration patterns, what belongs in code vs. no-code |
| **Specification** | Behaviour definition, error handling, edge cases, debugging hooks, logging strategy |
| **Direction** | Decomposing work, directing Claude Code, reviewing implementation, catching architectural issues early |
| **Operations** | Linux servers, deployment pipelines, environment management, production monitoring |
| **Debugging** | Log analysis, API tracing, data flow inspection, failure diagnosis and fix iteration |

<br/>

---

## Infrastructure projects built with Claude Code

<br/>

### 🔍 FormPing

**API monitoring & form validation infrastructure**

<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" />
</p>

A system that monitors the entire GTM funnel by crawling client sites with a headless browser, detecting forms, validating that submissions actually reach their destination, and tracking API responses. Integrated with Zapier workflows to alert when leads don't sync or forms break silently.

Solves the core GTM problem: campaigns run, traffic converts, leads disappear. FormPing catches this in minutes instead of at month-end when revenue is already lost.

Built end to end: Playwright crawlers, form detection, API validation, real-time dashboards, webhook integrations, and production infrastructure.

[**→ Repository**](https://github.com/waseembashir/FormPing)

<br/>

### 🎓 Learntopia

**Full-stack education infrastructure with data persistence**

<p>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white" />
</p>

Infrastructure for a complete learning ecosystem: enrolment workflows, course progression tracking, assessment delivery, and score persistence in Firestore. Every interaction is captured, validated, and queryable.

Built with security and observability in mind: Google Auth, Firestore security rules, error tracking, automated end-to-end testing, and deployment pipelines.

The infrastructure that turns a course platform into a system we can trust and debug.

[**→ Repository**](https://github.com/TAJAMUL11/Learntopia) · [**→ Live**](https://learntopia.vercel.app)

<br/>

### 🛡️ Secret Sentinel

**Local secret detection infrastructure for Git**

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Git_Hooks-F05032?style=flat-square&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
</p>

Infrastructure that enforces secrets security at the Git layer. A CLI tool that catches hardcoded credentials before they commit, combining pattern matching with entropy-based detection. Installs as a pre-commit hook and surfaces findings in CI/CD pipelines.

Deliberately offline: no cloud API, no external dependencies, nothing leaves the machine. The philosophy: security controls live in code, not advice.

[**→ Repository**](https://github.com/tajamul-wani/secret-sentinel)

<br/>

---

## GTM operations infrastructure

The core of what I build.

**Data pipelines & synchronization** — Moving leads, accounts, and events between GoHighLevel, HubSpot, Zapier, Make, and dozens of third-party tools without data loss or duplication. Building the routing logic that ensures data goes where it belongs.

**API debugging & inspection tools** — Building infrastructure to see what's actually happening: log aggregation, API response inspection, webhook delivery verification, and the observability that catches silent failures.

**Integration architecture** — Designing how systems talk to each other: REST APIs, webhooks, data transformation layers, error handling strategies, and retry logic. Everything built so failures are visible and recoverable.

**Automation infrastructure** — Workflows that keep systems in sync automatically: data reconciliation, lead enrichment pipelines, sequence delivery, and the monitoring that alerts when something breaks.

<br/>

---

## Shipping & operations

I provision and operate Linux servers, manage deployments through Git, and run production systems myself.

```
local → GitHub → ssh → pull → build → serve → read logs → debug → fix → repeat
```

This isn't just deployment convenience. Operating systems myself taught me how real applications behave: how they fail, how to trace failures from logs, how to fix them without waiting for a vendor. It's the discipline that makes me better at designing infrastructure.

<p>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/SSH-24292E?style=flat-square" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Log_analysis-4B5563?style=flat-square" />
</p>

<br/>

---

## API & data inspection

I use specialized tools to understand what's actually happening in marketing systems.

**Webhook & API logging** — Capturing every inbound webhook, API call, and response so failures are visible. Building dashboards that show data flow in real time.

**Form & lead tracking** — Playwright-based crawlers that inspect forms, validate submissions, track API calls from client sites, and catch when leads go silent.

**Data validation** — Automated checks that ensure leads sync correctly, deduplication logic works, and data integrity is maintained across systems.

<br/>

---

## Stack

<br/>

#### GTM & Integration Platforms

<p>
  <img src="https://img.shields.io/badge/HubSpot-FF7A59?style=flat-square&logo=hubspot&logoColor=white" />
  <img src="https://img.shields.io/badge/GoHighLevel-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/Zapier-FF4F00?style=flat-square&logo=zapier&logoColor=white" />
  <img src="https://img.shields.io/badge/Make-6D5EF5?style=flat-square" />
  <img src="https://img.shields.io/badge/Apollo-4F46E5?style=flat-square" />
  <img src="https://img.shields.io/badge/Snov.io-6C63FF?style=flat-square" />
</p>

<br/>

#### API & Data Infrastructure

<p>
  <img src="https://img.shields.io/badge/REST_APIs-0052CC?style=flat-square" />
  <img src="https://img.shields.io/badge/Webhooks-24292E?style=flat-square" />
  <img src="https://img.shields.io/badge/Data_Pipelines-4B8BBE?style=flat-square" />
  <img src="https://img.shields.io/badge/Event_Streaming-FF6B6B?style=flat-square" />
  <img src="https://img.shields.io/badge/API_Debugging-4A4A4A?style=flat-square" />
</p>

<br/>

#### Development & Infrastructure

<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react" />
</p>

<br/>

#### Operations & Observability

<p>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black" />
  <img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
</p>

<br/>

#### AI-Directed Development

<p>
  <img src="https://img.shields.io/badge/Claude_Code-000000?style=flat-square&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" />
</p>

<br/>

---

## Currently learning

Going deeper on the systems layer rather than collecting more platforms.

- **AI Agents** — building tools that models can operate, not just prompt loops
- **Model Context Protocol (MCP)** — the plumbing that connects models to real systems
- **System Design** — vocabulary and patterns for decisions I've been making by instinct
- **RAG and LLM** — retrieval, context design, evaluation
- **Clay** — programmatic enrichment and outbound at scale
- **Python** — for the data and automation work
- **SQL** — querying the systems I've spent years filling with data

<br/>

---

<p align="center">
  <sub>If it involves building infrastructure that makes marketing systems reliable, observable, and connected — I'm interested.</sub>
</p>
