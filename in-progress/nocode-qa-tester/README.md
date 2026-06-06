# nocode-qa-tester

> Automated QA testing for Make / n8n AI workflows — no engineering required.

**⭐ Star this repo if you build AI automations for clients and want this tool.**

---

## The problem

You build AI automation workflows on Make or n8n. You ship them to clients.

Then: the chatbot hallucinates. The workflow breaks on edge cases. The client is unhappy.

You had no way to test it systematically before delivery — unless you did it by hand, query by query.

Tools like LangSmith or Galileo exist, but they're built for ML engineers. Not for no-code builders.

---

## What this does

Submit your Make / n8n webhook URL. Get back a PDF report with a score out of 10.

```
Your webhook URL
       │
       ▼
┌─────────────────────────────────────────────────┐
│  10 automated test cases sent to your webhook   │
│  • Rephrased inputs                             │
│  • Ambiguous questions                          │
│  • Off-topic queries                            │
│  • Basic jailbreak attempts                     │
└─────────────────────────────────────────────────┘
       │
       ▼
┌─────────────────────────────────────────────────┐
│  LLM judge evaluates each response              │
│  • Relevance                                    │
│  • Hallucination risk                           │
│  • Tone consistency                             │
│  • Safety                                       │
└─────────────────────────────────────────────────┘
       │
       ▼
  PDF report in your inbox
  Score: 7.4/10 — 3 issues found
```

No dashboard. No login. No complexity.  
Just: submit → test → report in your inbox.

---

## Who it's for

- Freelancers building AI chatbots / assistants on Make or n8n
- No-code agencies delivering automation workflows to clients
- Anyone who wants to QA an AI webhook before going live

---

## MVP scope

| Feature | Status |
|---------|--------|
| Accept webhook URL + email via form | 🔲 planned |
| Send 10 predefined test cases to webhook | 🔲 planned |
| LLM-judge evaluation (Claude API) | 🔲 planned |
| PDF report generation | 🔲 planned |
| Email delivery | 🔲 planned |
| Stripe payment (€29 one-shot) | 🔲 planned |

**Not in MVP:** user dashboard, login, history, subscription, custom test cases.

---

## Tech stack

- **Backend:** Node.js (or Python — TBD based on feedback)
- **LLM judge:** Anthropic Claude API
- **PDF generation:** Puppeteer or WeasyPrint
- **Email:** Resend or Postmark
- **Payment:** Stripe or Lemon Squeezy
- **Frontend:** Single HTML form (no framework)

---

## The 10 test cases

Each test targets a different failure mode of AI workflows:

| # | Type | What it tests |
|---|------|---------------|
| 1-2 | Rephrasing | Same question, different wording |
| 3-4 | Ambiguity | Vague or underspecified input |
| 5-6 | Off-topic | Completely unrelated request |
| 7-8 | Edge case | Unusual but valid input |
| 9 | Jailbreak attempt | Prompt injection, role override |
| 10 | Empty / nonsense | Robustness to garbage input |

---

## Roadmap

- [ ] v0.1 — Core pipeline (webhook → test → judge → PDF)
- [ ] v0.2 — Payment gate (€29 one-shot)
- [ ] v0.3 — Custom test case upload (JSON)
- [ ] v0.4 — Workflow type presets (support bot, lead gen, qualifier)
- [ ] v1.0 — Agency plan (batch testing, white-label reports)

---

## Contribute

This is being built in public. Feedback welcome via Issues.

Specifically looking for input on:
- **Which failure modes matter most** to you as a no-code builder
- **Pricing** — would you pay €29/report or prefer a monthly plan?
- **Stack preferences** — Node.js vs Python backend?

Open an issue or drop a comment — every bit of signal helps.

---

## Status

🔨 Pre-build. Validating demand before writing code.

If this solves a real problem you have: **star the repo**. That's the signal that moves this forward.

---

## Author

Built by [@adriencr81](https://github.com/adriencr81) — cybersecurity engineer turned no-code builder.
