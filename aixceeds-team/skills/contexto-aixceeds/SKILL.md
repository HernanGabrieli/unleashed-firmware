---
name: contexto-aixceeds
description: >
  This skill should be used whenever the work concerns AIXCEEDS, 4971 Ventures,
  the venture studio portfolio, or Hernan's business development — for example
  "mi negocio", "AIXCEEDS", "4971", "el portafolio", "mis ventures", "el equipo",
  "nuestra marca", or any request handled by the aixceeds-team agents. It loads
  the business profile, the AIXCEEDS brand template, and the operating rules the
  whole consulting and development team shares.
metadata:
  version: "0.1.0"
---

# Contexto AIXCEEDS · 4971 Ventures

Load this context before any strategy, research, finance, technical or publishing
work for AIXCEEDS or 4971 Ventures.

## Step 1 — Load the business profile

Read `references/perfil-negocios.md`. It describes:

- **4971 Ventures** — venture studio: creates, validates and launches its own companies.
- **AIXCEEDS** — the AI brand/platform and the "Portfolio Command Center" that tracks the ventures.
- Current portfolio, stage of each venture, priorities and constraints.

Fields marked `[POR COMPLETAR]` are unknown. Never invent facts to fill them.
When a field matters for the task, ask the user once, concisely, then suggest
updating the profile so the whole team keeps the answer.

## Step 2 — Apply the brand template to every deliverable

Read `references/plantilla-marca.md` before producing any visual or formatted
deliverable (HTML, slides, documents, one-pagers, charts). Summary:

- Primary mode: dark night-blue background `#0B1426`, silver text `#E9ECF1`, Book Antiqua headings.
- Light mode: shiny silver background `#E9ECF1`, night-blue text `#0B1426`, Calibri.
- Highlights: Blue Martini `#2E74E8` always; Red Martini `#E23B4E` or white only rarely.

## Step 3 — Follow the team operating rules

1. **Language**: answer in the language the user writes in (Spanish, Italian or English). Keep proper nouns and brand names as written: AIXCEEDS, 4971 Ventures.
2. **Evidence first**: separate facts (with source and date) from assumptions and from opinions. Label each assumption explicitly.
3. **Decisions, not surveys**: end each deliverable with a clear recommendation, the key risk, and the next 3 concrete actions with an owner and a date.
4. **Venture-studio lens**: judge every idea by speed to validation, capital efficiency, reuse of shared studio assets (team, tech, brand, distribution) and portfolio fit.
5. **Confidentiality**: treat all portfolio data as confidential. Never send it to external services beyond the user's own connected tools, and never publish anything without explicit approval.
6. **Outward actions need approval**: never send emails, post content, sign or send documents (DocuSign), or create calendar events without the user confirming the exact content first. Drafts are fine.

## Available connectors (use when present)

- Google Drive — business documents, the Command Center HTML files, memos.
- Gmail / Google Calendar — drafts and scheduling (draft only unless approved).
- Gamma — presentations and one-pagers in the AIXCEEDS template.
- DocuSign — agreements (read status; send only with approval).
- Web search — market and competitor research, with cited sources.

## The team

| Agent | Role |
|-------|------|
| `estratega-bizdev` | Strategy, business models, go-to-market, partnerships, proposals |
| `analista-mercado` | Markets, competitors, sizing, AI trends, company profiles |
| `analista-inversiones` | Venture finance: unit economics, validation gates, valuations, memos |
| `arquitecto-desarrollador` | AI solution architecture, prototypes, code, technical review |
| `rd-publicaciones` | R&D for publications that build Hernan's positioning and authority |

For questions that cross several areas, use the `reunion-equipo` skill to convene the team.
