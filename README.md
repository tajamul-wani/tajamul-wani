<h1 align="center">Tajamul Wani</h1>

<p align="center">
  <b>GTM Engineer at LexHive</b> &nbsp;·&nbsp; GTM Infrastructure &nbsp;·&nbsp; Marketing Operations &nbsp;·&nbsp; Full-Stack with Claude Code
</p>

<p align="center">
  I build the systems behind customer acquisition: funnels, conversion tracking,<br/>
  lead pipelines and the monitoring that catches failures before revenue is lost.
</p>

<p align="center">
  <a href="https://tajamul-wani.netlify.app"><img src="https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=google-chrome&logoColor=white" /></a>
  &nbsp;
  <a href="https://linkedin.com/in/tajamul-wani"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" /></a>
  &nbsp;
  <a href="mailto:tajamul.270@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" /></a>
</p>

---

## What I do

| | |
|---|---|
| **Data pipelines** | Sync leads, accounts and events between HubSpot, GoHighLevel, Salesforce, Airtable, Zapier, Make and n8n with no loss or duplication |
| **Integration architecture** | REST APIs, webhooks, transformations, retries with backoff, fallbacks and replay, so failures are visible and recoverable |
| **Tracking & attribution** | Meta Pixel + Conversions API on one event ID, server-side GTM events, first-party attribution carried into the CRM |
| **Outbound & enrichment** | Apollo and Snov.io sourcing, enrichment pipelines and sequence delivery wired into the CRM |
| **Funnels & stores** | React, TypeScript and Vite on Vercel with Supabase, accessibility tested |
| **Monitoring & debugging** | Webhook and API logging, delivery verification, Sentry, log analysis, tracing a lost lead end to end |
| **Operations** | Linux servers, Docker, Git-based deployment, CI, production support |

<br/>

**How I work:** I don't write code by hand. I architect, specify, direct Claude Code, review every component, then deploy and run it myself.

```
local → GitHub → ssh → pull → build → serve → read logs → debug → fix → repeat
```

---

## Track record

**2 years** · **20+ end-to-end builds** for international clients · **40+ campaign assets** · **961 contacts** sourced in one outbound campaign with a **15.4% reply rate** on the top segment

---

## Projects

### LeadRelay
<p>
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" />
  <img src="https://img.shields.io/badge/Meta_CAPI-0467DF?style=flat-square&logo=meta&logoColor=white" />
</p>

Lead capture pipeline built around failure. One UUID is the database key, the Pixel event ID and the Conversions API event ID, so retries can't duplicate a lead and Meta can't count a conversion twice. Undelivered leads are found and replayed. 81 tests, CI, documented failure drills.

[**→ Repository**](https://github.com/tajamul-wani/leadrelay) · [**→ Live demo**](https://leadrelay-funnel.vercel.app)

<br/>

### FormPing
<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" />
</p>

Monitors the GTM funnel by crawling sites with a headless browser, finding forms and checking that submissions actually arrive. Zapier alerts fire when leads don't sync, so breakage is caught in minutes instead of at month-end.

[**→ Repository**](https://github.com/waseembashir/FormPing)

<br/>

### Shumār
<p>
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
</p>

Kashmiri-first calorie and macro tracker, installable as a PWA and usable offline. Google sign-in, row-level security on every table with tests proving users can't see each other's data, database-enforced storage limits, and CI with security scans.

[**→ Repository**](https://github.com/tajamul-wani/shumar)

<br/>

### Learntopia
<p>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white" />
</p>

Full-stack learning platform with enrolment, course progression, assessments and score persistence in Firestore. Google Auth, security rules, error tracking and automated end-to-end tests.

[**→ Repository**](https://github.com/tajamul-wani/Learntopia) · [**→ Live**](https://learntopia-react.web.app/)

<br/>

### Secret Sentinel
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Git_Hooks-F05032?style=flat-square&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
</p>

Pre-commit hook that catches hardcoded credentials before they reach a repo, using pattern matching and entropy detection. Fully offline.

[**→ Repository**](https://github.com/tajamul-wani/secret-sentinel)

---

## Stack

<p>
  <img src="https://img.shields.io/badge/HubSpot-FF7A59?style=flat-square&logo=hubspot&logoColor=white" />
  <img src="https://img.shields.io/badge/GoHighLevel-1C1C1C?style=flat-square" />
  <img src="https://img.shields.io/badge/Salesforce-00A1E0?style=flat-square&logo=salesforce&logoColor=white" />
  <img src="https://img.shields.io/badge/Airtable-18BFFF?style=flat-square&logo=airtable&logoColor=white" />
  <img src="https://img.shields.io/badge/Apollo-4F46E5?style=flat-square" />
  <img src="https://img.shields.io/badge/Snov.io-6C63FF?style=flat-square" />
</p>

<p>
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white" />
  <img src="https://img.shields.io/badge/Zapier-FF4F00?style=flat-square&logo=zapier&logoColor=white" />
  <img src="https://img.shields.io/badge/Make-6D5EF5?style=flat-square" />
  <img src="https://img.shields.io/badge/Meta_Pixel_%26_CAPI-0467DF?style=flat-square&logo=meta&logoColor=white" />
  <img src="https://img.shields.io/badge/Google_Tag_Manager-246FDB?style=flat-square&logo=googletagmanager&logoColor=white" />
  <img src="https://img.shields.io/badge/REST_APIs-0052CC?style=flat-square" />
  <img src="https://img.shields.io/badge/Webhooks-24292E?style=flat-square" />
</p>

<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" />
</p>

<p>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" />
  <img src="https://img.shields.io/badge/Railway-0B0D0E?style=flat-square&logo=railway&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white" />
</p>

<p>
  <img src="https://img.shields.io/badge/Claude_Code-000000?style=flat-square&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/MCP_Certified-D97757?style=flat-square&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" />
</p>

---

## Currently learning

**Clay** for programmatic enrichment · **SQL and Python** for data work · **AI agents and RAG**

<br/>

<p align="center">
  <sub>If it involves making marketing systems reliable, observable and connected, I'm interested.</sub>
</p>
