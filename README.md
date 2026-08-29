<h1 align="center">Tajamul Wani</h1>

<p align="center">
  <b>GTM Engineer</b> · Marketing Operations · AI-Directed Product Builder<br/>
  <sub>I design the systems that turn marketing intent into pipeline — and the software underneath them.</sub>
</p>

<p align="center">
  <a href="https://tajamul-wani.netlify.app"><img src="https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=google-chrome&logoColor=white" /></a>
  <a href="https://linkedin.com/in/tajamul-wani"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:tajamul.270@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" /></a>
</p>

---

## How I build

I read code. I don't write it by hand.

What I do instead is the part that decides whether software actually works: define the architecture, specify behaviour precisely enough that it can be implemented, direct Claude Code through the build, review what comes back, and own everything downstream of "the code exists" — deployment, servers, logs, test coverage, and the failures that only appear in production.

That constraint turns out to matter less than people expect and forces something useful: if I can't describe a system clearly, it doesn't get built. So I spend my time on data models, integration boundaries, failure modes, and what happens when the third-party API returns something unexpected. The implementation is the cheap part now. The architecture never was.

| Layer | What I own |
|---|---|
| **Architecture** | Data model, system boundaries, integration design, what belongs in code vs. no-code |
| **Direction** | Specifying behaviour, decomposing work, directing Claude Code, reviewing output |
| **Deploy** | Linux servers, SSH, Git-based deploy workflow, environments and secrets |
| **Verify** | Playwright suites, CI checks, Sentry monitoring, manual regression passes |
| **Operate** | Reading logs, tracing failures, fixing production, iterating on what actually broke |

---

## Marketing infrastructure

The GTM half of the job, and still the majority of it.

**CRM & pipeline architecture** — Pipelines, lifecycle stages, custom properties, and routing logic in GoHighLevel and HubSpot, designed so reporting reflects what actually happened rather than what someone hoped would.

**Funnels & landing pages** — Full builds across ClickFunnels, Unbounce, Kajabi, and LearnWorlds, with custom components dropped in wherever the builder hits its ceiling.

**Reusable component library** — Instead of rebuilding the same calculator, conditional form, or comparison table for every client, I maintain portable HTML/CSS/JS components that drop into Unbounce, ClickFunnels, GHL, Kajabi, and Elementor with minimal rework. Spec once, ship across accounts.

**Automation & outbound** — Prospecting through Apollo and Snov.io, sequence design, and the plumbing that keeps systems in sync: Zapier, Make, raw webhooks, REST APIs.

---

## Shipping & operations

The part I added most recently, and the part that changed how I think about everything else.

I provision and run my own Linux server rather than treating deployment as someone else's problem. The loop: SSH into the box, set up the project and its runtime, push local to GitHub, pull to the server, build, serve. Then the real work — reading logs when a service won't start, tracing a failed request back to a bad environment variable, telling a build failure apart from a runtime one, and fixing it on the machine instead of guessing from a dashboard.

```
local → GitHub → ssh → pull → build → serve → read logs → fix → repeat
```

Doing this by hand taught me more about how deployed applications behave than any managed platform would have. It also means that when infrastructure misbehaves, I can open a terminal instead of a support ticket.

`Linux` `SSH` `Git` `Docker` `Railway` `Supabase` `Firebase` `service management` `log analysis`

---

## Browser automation

I use Playwright for two very different jobs.

**As a data collection engine.** Driving a headless browser across client sites to detect page structure, capture screenshots, and extract the state of a page for comparison over time. This is the core of how FormPing knows a site changed.

**As a test harness.** End-to-end coverage for a live application — automating the flows I used to verify by hand every release: authentication, enrolment, module progression, quiz submission and scoring, dashboard state. Manual testing is fine until there's a deadline, at which point it quietly stops happening. The suite doesn't have that problem.

---

## Projects

### 🔍 FormPing
**Website monitoring platform** · `TypeScript` `Playwright` `Docker` `Railway` `Supabase` `Claude Code`

A monitoring service that crawls client sites with a headless browser, automatically detects contact forms, validates that submissions actually go through, and flags SEO and content changes — alerting to Slack.

Broken forms are the most expensive silent failure in marketing: the campaign runs, traffic converts, and nothing arrives. FormPing catches that in minutes instead of at the end of the month.

**My role:** product direction · architecture · AI-directed development · containerization and deployment · QA automation

[→ Repository](https://github.com/waseembashir/FormPing)

---

### 🎓 Learntopia
**Full-stack e-learning application** · `JavaScript` `Firebase` `Playwright` `Sentry` `Claude Code`

Students enrol in topic-specific course tracks, work through structured modules, and test themselves with randomized, timed quizzes. Progress, scores, and streaks persist in Firestore and surface on a personal dashboard and a public leaderboard.

Built end to end: data model, Google Auth, Firestore security rules, Captcha, Sentry error monitoring, and a Playwright E2E suite covering the full student journey.

**My role:** architecture · AI-directed development · security hardening · test automation · deployment

[→ Repository](https://github.com/TAJAMUL11/Learntopia)

---

### 🛡️ Secret Sentinel
**Local secret scanner for Git repositories** · `Python` `Git hooks` `GitHub Actions`

A CLI tool that catches hardcoded credentials before they reach a commit. Combines pattern matching for known key formats with entropy-based detection for everything else, installs as a Git pre-commit hook, and scores each finding by severity — AWS keys and API tokens as CRITICAL, JWTs and generic secret assignments as HIGH, high-entropy strings below that.

Deliberately offline by default: no cloud API, no environment variables, nothing leaves the machine. AI validation via a local Ollama or configured Gemini setup is available but strictly optional. Scan history is kept locally as JSONL so you can pull statistics across runs.

Built because "don't commit secrets" is advice, and a pre-commit hook is a control.

**My role:** concept · architecture · AI-directed development · packaging and CI

[→ Repository](https://github.com/tajamul-wani/secret-sentinel)

---

## Stack

**GTM & CRM**
---
<br/>
<img src="https://img.shields.io/badge/HubSpot-FF7A59?style=flat-square&logo=hubspot&logoColor=white" />
<img src="https://img.shields.io/badge/GoHighLevel-1C1C1C?style=flat-square" />
<img src="https://img.shields.io/badge/ClickFunnels-E74C3C?style=flat-square" />
<img src="https://img.shields.io/badge/Unbounce-4E6CFB?style=flat-square" />
<img src="https://img.shields.io/badge/Kajabi-14C38E?style=flat-square" />
<img src="https://img.shields.io/badge/LearnWorlds-5B5FC7?style=flat-square" />

**Automation & data movement**
---
<br/>
<img src="https://img.shields.io/badge/Zapier-FF4F00?style=flat-square&logo=zapier&logoColor=white" />
<img src="https://img.shields.io/badge/Make-6D5EF5?style=flat-square" />
<img src="https://img.shields.io/badge/REST_APIs-0052CC?style=flat-square" />
<img src="https://img.shields.io/badge/Webhooks-24292E?style=flat-square" />
<img src="https://img.shields.io/badge/Apollo-4F46E5?style=flat-square" />
<img src="https://img.shields.io/badge/Snov.io-6C63FF?style=flat-square" />

**Codebases I work in**
---
<br/>
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react" />
<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" />

**Ship & run**
---
<br/>
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white" />
<img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" />
<img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black" />
<img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
<img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white" />

**AI**
---
<br/>
<img src="https://img.shields.io/badge/Claude_Code-000000?style=flat-square&logo=anthropic&logoColor=white" />
<img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" />

---

## Currently learning

Going deeper on the systems layer rather than collecting more platforms.

- **AI Agents** — building tools that models can operate, not just prompt loops
- **Model Context Protocol (MCP)** — the plumbing that connects models to real systems
- **System Design** — vocabulary and patterns for decisions I've been making by instinct
- **RAG and LLM** — retrieval, context design, evaluation
- **Clay** — programmatic enrichment and outbound at scale
- **Python** — for the data and automation.
- **SQL** — querying the systems I've spent years filling with data

---

<p align="center">
  <sub>If it involves connecting a marketing system to something it wasn't designed to talk to, I'm interested.</sub>
</p>
