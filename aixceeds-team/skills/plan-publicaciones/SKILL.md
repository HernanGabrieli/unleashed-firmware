---
name: plan-publicaciones
description: >
  This skill should be used when the user wants to build personal or brand
  positioning through publications — "plan editorial", "calendario de
  contenidos", "qué publico en LinkedIn", "quiero posicionarme como
  referente", "escribime un artículo / whitepaper / post", "thought
  leadership", "piano editoriale", or to research and draft any publication
  for Hernan Gabrieli, AIXCEEDS or 4971 Ventures.
metadata:
  version: "0.1.0"
---

# Plan de publicaciones (R&D de posicionamiento)

Design and produce publications that increase Hernan Gabrieli's authority,
through the `rd-publicaciones` agent.

## Mode A — Strategy and calendar (when no specific piece is requested)

1. Load `contexto-aixceeds`; read founder credentials and positioning topics.
2. Define with `rd-publicaciones`:
   - **Posicionamiento** in one sentence: "Hernan es la referencia en ___ para ___ porque ___".
   - 3–4 **pilares** de contenido, each with its distinctive point of view.
   - Audiences and channels (LinkedIn, newsletter, medios, conferencias, podcasts)
     per language market (ES / IT / EN).
3. Build a 90-day calendar: 1 deep "flagship" piece per month (whitepaper,
   research, long article) and its derivatives (posts, carousel, newsletter, talk).

Calendar table: semana · pilar · formato · título de trabajo · canal · idioma · estado.

4. Define authority metrics: qualified inbound, invitations to speak or write,
   quality of comments, follower growth in the target audience.

## Mode B — Produce a piece

1. Load `contexto-aixceeds`.
2. Confirm format, audience, language and length (use sensible defaults:
   LinkedIn post 150–250 words; article 1,000–1,500; whitepaper 2,500–4,000).
3. Research first: ask `analista-mercado` for data when the piece needs facts.
4. Draft with `rd-publicaciones`: one thesis, at least one original insight or
   named framework, cited sources, Hernan's voice, no AI-sounding filler.
5. Deliver: draft, 3 title options, 3 hook options, distribution and
   repurposing plan. For visual pieces (carousels, covers, whitepaper layout)
   apply the AIXCEEDS template and offer Gamma.

## Rules

- Never post or publish; drafts only, approved by the user.
- Never fabricate statistics, quotes or client cases. Portfolio cases only with approval.
- Write in the requested language; default to the user's language.
