---
name: memo-inversion
description: >
  This skill should be used when the user asks for an investment memo, a
  spin-out or fundraising memo, a due-diligence summary, or a capital
  allocation recommendation for a 4971 Ventures venture or an external
  opportunity — "memo de inversión", "investment memo", "due diligence",
  "preparame la pre-seed", "memo per gli investitori".
metadata:
  version: "0.1.0"
---

# Memo de inversión

Produce a decision-grade investment memo. Delegate the numbers to
`analista-inversiones` and the market section to `analista-mercado`.

## Steps

1. Load `contexto-aixceeds`.
2. Clarify the purpose: internal capital allocation, external fundraise
   (pre-seed / seed), or due diligence of a third-party company.
3. Collect inputs: metrics, deck, financials, cap table (from the user or Drive).
   List missing data instead of inventing it.
4. Draft the memo with the structure below. Keep it to 2–4 pages.
5. Run a red-team pass: write the three strongest reasons NOT to invest and
   answer each one honestly.

## Structure

1. **Recomendación** — invest / don't, amount, instrument, valuation range.
2. **Tesis en 3 puntos**.
3. **Problema y solución**.
4. **Mercado** — sizing, timing ("why now"), competition.
5. **Tracción y métricas** — with benchmark comparison.
6. **Modelo de negocio y unit economics**.
7. **Equipo** — and the studio's role.
8. **Ronda** — use of funds, milestones it buys, runway, cap table impact.
9. **Riesgos y mitigaciones** (red-team result).
10. **Qué tendría que ser cierto** for a 10x outcome.

## Rules

- Every number has a source or is labelled as an assumption.
- Flag where legal, tax or accounting advice is needed.
- Format in the AIXCEEDS template (Silver mode for documents) and offer to
  export to Google Drive, Word or a Gamma presentation.

Write in the user's language.
