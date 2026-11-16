# Tajamul Wani

**GTM Engineer at LexHive** · GTM infrastructure · Marketing operations · Full-stack development with Claude Code

I build the systems behind customer acquisition: the funnel a prospect fills in, the tracking that proves they converted, and the pipelines that move the lead between platforms, with monitoring so nothing fails silently. Data pipelines, API orchestration, debugging and observability, and the software that makes marketing systems talk to each other.

I design the architecture, specify behaviour precisely, direct Claude Code to build it, review every component, then test, deploy and run it in production. I read the logs and fix what breaks.

[Portfolio](https://tajamul-wani.netlify.app) · [LinkedIn](https://linkedin.com/in/tajamul-wani) · [Email](mailto:tajamul.270@gmail.com)

---

## GTM and marketing operations

**Data pipelines and synchronisation**
Moving leads, accounts and events between GoHighLevel, HubSpot, Salesforce, Airtable, Zapier, Make, n8n and dozens of third-party tools without data loss or duplication. Routing, qualification and deduplication logic so data lands where it belongs.

**Integration architecture**
Designing how systems talk to each other: REST APIs, webhooks, data transformation layers, error handling and retry logic with backoff. Everything built so failures are visible and recoverable, with fallbacks and replay for anything that didn't make it through. I decide what belongs in code and what belongs in no-code.

**Automation**
Workflows that keep systems in sync on their own: data reconciliation, lead enrichment pipelines, sequence delivery, email systems, and alerting when something breaks.

**Outbound and enrichment**
Apollo and Snov.io for sourcing and enrichment, with sequences and delivery wired into the CRM. One campaign: 961 contacts sourced, 15.4% reply rate on the top segment.

**Tracking and attribution**
Meta Pixel and Conversions API sharing one event ID, so each conversion is counted once. Server-side events through GTM that still fire when the browser pixel is blocked. First-party attribution captured at landing and carried through to the CRM.

**CRM and pipeline architecture**
Data model, pipeline stages, system boundaries and integration patterns, set up for international clients across HubSpot, GoHighLevel and Salesforce.

**Funnels and product stores**
React, TypeScript and Vite on Vercel with Supabase behind them. Step logic defined as data, so a new variant is cheap to build and easy to measure. Accessibility tested.

---

## API debugging and observability

I build the tools to see what's actually happening in marketing systems, and I use them.

- **Webhook and API logging:** capturing every inbound webhook, API call and response, with dashboards showing data flow in real time
- **Delivery verification:** confirming webhooks actually arrived, inspecting API responses, and tracing a lead across service boundaries to find where it was lost and why
- **Form and lead tracking:** Playwright crawlers that inspect forms, validate submissions and catch leads going silent
- **Data validation:** automated checks that leads sync correctly, deduplication works, and integrity holds across systems
- **Production monitoring:** Sentry, log analysis and alerting

---

## How I work

| Layer | What I own |
|---|---|
| **Architecture** | Data model, system boundaries, API design, integration patterns, what belongs in code vs. no-code |
| **Specification** | Behaviour definition, error handling, edge cases, debugging hooks, logging strategy |
| **Direction** | Decomposing work, directing Claude Code, reviewing every component, catching architectural issues early |
| **Operations** | Linux servers, deployment pipelines, environment management, production monitoring |
| **Debugging** | Log analysis, API tracing, data flow inspection, failure diagnosis and fix iteration |

I don't write code by hand. I architect, specify, direct Claude Code, review and operate. That forces clarity: if I can't describe a system precisely enough for an AI to build it, it isn't ready to ship.

```
local → GitHub → ssh → pull → build → serve → read logs → debug → fix → repeat
```

I provision and operate Linux servers and run production systems myself. That taught me how real applications fail, how to trace failures from logs, and how to fix them without waiting for a vendor.

---

## Track record

- 2 years and 20+ end-to-end system builds for international clients: CRM and pipeline architecture, funnels and product stores, marketing attribution, automation and email systems
- 40+ campaign assets shipped
- One outbound campaign: 961 contacts sourced, 15.4% reply rate on the top segment

---

## Selected work

**[LeadRelay](https://github.com/tajamul-wani/leadrelay)** · [Live demo](https://leadrelay-funnel.vercel.app)
A lead capture pipeline built around what happens when things fail. One UUID serves as the database key, the Pixel event ID and the Conversions API event ID, so a retry can't create a duplicate and Meta can't count the same conversion twice. Delivery runs through either an n8n workflow or TypeScript in the repo, and undelivered leads are found and replayed through the live endpoint. 81 tests, CI, documented failure drills.

**[FormPing](https://github.com/waseembashir/FormPing)**
API monitoring and form validation for the whole GTM funnel. A form that silently stops submitting costs more than one that visibly breaks, so FormPing crawls client sites with a headless browser, detects forms, validates that submissions reach their destination, and tracks API responses. Integrated with Zapier workflows to alert when leads don't sync, so it's caught in minutes instead of at month-end. Playwright, TypeScript, Docker, Railway, Supabase. *[One line on exactly what you built.]*

**[Shumār](https://github.com/tajamul-wani/shumar)**
A Kashmiri-first calorie and macro tracker, built as an installable PWA that also opens offline. React 19, TypeScript, Vite and Tailwind v4, with Supabase and Google sign-in behind it. Food values live in a catalogue of Kashmiri and everyday foods, with pieces, cups and katoris converted to grams. Each person's daily target follows them across devices.
Built security-first: row-level security on every table, with tests proving one user can't see another's logs. Storage caps are enforced by database triggers under per-user locks, so concurrent requests can't slip past a limit. Unit, database and end-to-end tests run on phone, tablet and desktop in dark and light themes, with accessibility scans. CI runs lint, types, tests, `npm audit` and gitleaks over the full history, and every GitHub Action is pinned to an exact commit.

**[Learntopia](https://github.com/tajamul-wani/Learntopia)** · [Live](https://learntopia-react.web.app/)
A full-stack learning platform: enrolment, course progression, assessments, and score persistence in Firestore. Every interaction is captured, validated and queryable. Google Auth, Firestore security rules, Sentry, and automated end-to-end tests.

**[secret-sentinel](https://github.com/tajamul-wani/secret-sentinel)**
A pre-commit hook that catches hardcoded credentials before they reach a repo. Pattern matching plus entropy analysis, fully offline, written in Python, with CI integration.

---

## Stack

**GTM and CRM:** HubSpot · GoHighLevel · Salesforce · Airtable · Apollo · Snov.io
**Automation and integration:** n8n · Zapier · Make · REST APIs · Webhooks · Data pipelines
**Tracking:** Meta Pixel · Conversions API · Google Tag Manager (server-side)
**Development:** TypeScript · JavaScript · Python · React · Vite · Tailwind · Node.js
**Infrastructure:** Vercel · Supabase · Firebase · Railway · Docker · Linux · SSH · Git · GitHub Actions
**Quality and observability:** Playwright · Vitest · Sentry · log analysis · API debugging
**AI:** Claude Code · OpenAI · MCP (two Anthropic certifications)

---

## Currently learning

- **Clay:** programmatic enrichment and outbound at scale
- **SQL and Python:** deeper data and automation work
- **AI agents and RAG:** building tools that models can operate, and retrieval and evaluation for LLM systems

---

If it involves making marketing systems reliable, observable and connected, I'm interested.
