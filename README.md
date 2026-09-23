# AI Website Copy Generator for Local Businesses

**Prompt Engineering Task 1 — Future Interns (2026)**
**Author:** Harikalaxmi ([jharika43](https://github.com/jharika43))
**Tool used:** Claude (claude.ai)

---

## 🏢 Business Chosen

**Glow Studio** — a hair, skin & bridal styling salon in Hyderabad.

> Real-client framing: *"Website copy for Glow Studio, Hyderabad"*

Chosen because salons are a common local-business type with a clear customer pain point (generic, low-trust websites) that AI-generated conversion copy can directly fix.

## 🎯 Problem Being Solved

Glow Studio, like most local salons, had no strong online value proposition, no structured service descriptions, and no clear call-to-action — visitors couldn't tell why they should book there instead of a competitor. This task generates a complete, ready-to-publish copy set that fixes all three.

## 🧠 Prompt Logic

A single **reusable base prompt** (see `prompts/base-template.txt`) is used for every business type. It works by separating two kinds of input:

1. **Fixed structure instructions** — what sections to generate (hero, intro, 3 services, CTA), with word/sentence limits so output is scannable and website-ready, and a "no placeholders" rule so nothing needs manual cleanup.
2. **Swappable variables** — business type, name, location, description, target audience, tone, and desired CTA action.

Only the variables change between a salon, cafe, clinic, or agency — the instruction structure stays identical. This is what makes the prompt system repeatable across real clients rather than a one-off.

| Variable | Value used for Glow Studio |
|---|---|
| Business type | Salon |
| Business name | Glow Studio |
| Location | Hyderabad |
| Description | Hair, skin, and bridal styling salon |
| Target audience | Working women aged 20–45 seeking quality salon services |
| Tone | Warm, welcoming, slightly premium |
| Desired CTA action | Book an appointment |

## 📁 Repo Structure

```
ai-website-copy-generator/
├── README.md                     ← this file
├── prompts/
│   └── base-template.txt         ← reusable prompt (any business type)
└── outputs/
    ├── homepage-copy.md
    ├── services-copy.md
    └── cta-section.md
```

## ✅ Deliverable Checklist

- [x] Homepage copy with clear value proposition
- [x] Service page descriptions tailored to business type
- [x] Strong, urgency-aware CTA section
- [x] Tone adapted for a salon (friendly/warm, slightly premium)
- [x] Structured, reusable prompt documented separately from outputs
- [x] Content is publish-ready, no placeholders

## 🔁 Reusing This for Another Business

Swap only the variable table above (business type, name, tone, CTA action) and re-run `prompts/base-template.txt` — no structural changes needed. See the task's suggested tone mapping:

| Business | Tone | Desired Action |
|---|---|---|
| Cafe | Cozy, casual, sensory | Visit / Order online |
| Clinic | Calm, trustworthy, clear | Book a consultation |
| Agency | Bold, confident, outcome-driven | Get in touch / Request a quote |
