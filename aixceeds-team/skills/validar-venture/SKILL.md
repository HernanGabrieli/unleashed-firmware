---
name: validar-venture
description: >
  This skill should be used when the user wants to evaluate a venture idea or
  an existing venture of the 4971 Ventures studio against stage gates —
  "validá esta idea", "¿seguimos con este venture?", "go o kill", "stage
  gate", "evaluá el venture", "validare l'idea", "nueva idea de negocio", or
  deciding where to put studio time and money.
metadata:
  version: "0.1.0"
---

# Validar venture (stage gates del studio)

Evaluate a venture with the 4971 Ventures stage-gate framework and return
GO / ITERAR / KILL with the next experiment.

## Steps

1. Load `contexto-aixceeds`. If the profile defines its own gate criteria, use
   those instead of the defaults below.
2. Identify the venture's current stage. Ask if unclear.
3. Gather evidence: user-provided data, Drive documents, and market research
   from `analista-mercado` when facts are missing.
4. Score each criterion of the current gate 0–3
   (0 = no evidence, 1 = weak, 2 = solid, 3 = strong) and justify each score
   with evidence, not opinion.
5. Ask `analista-inversiones` to check the economics, and
   `arquitecto-desarrollador` to check feasibility when the gate requires it.
6. Decide: **GO** if every must-have scores ≥2; **ITERAR** if a must-have is 1
   and a cheap experiment can fix it; **KILL** if a must-have is 0 after a
   fair test, or the economics cannot work.

## Default gates

| Gate | Stage | Must-haves | Typical budget / time |
|------|-------|-----------|------------------------|
| G0 | Idea → Validación | Painful, frequent problem; reachable buyer; studio fit | 0 € · 1 week |
| G1 | Validación → MVP | ≥10 problem interviews confirm the pain; willingness to pay signal (LOI, pre-sale, waitlist); market large enough | low · 2–4 weeks |
| G2 | MVP → Tracción | Users use it repeatedly; first paying customers; CAC hypothesis tested | moderate · 6–12 weeks |
| G3 | Tracción → Escala / spin-out | Repeatable acquisition; LTV/CAC ≥3 or a clear path; a CEO/operator identified; fundable story | per plan |

Studio-fit criteria (always scored): reuse of shared studio assets; fit with
the portfolio thesis; founder's unfair advantage; time to first revenue.

## Output

- **Veredicto**: GO / ITERAR / KILL (Blue Martini for GO, Red Martini only for KILL).
- Scorecard table: criterion, score, evidence, confidence.
- **Supuesto más riesgoso** and the cheapest experiment to test it
  (hypothesis, metric, threshold, deadline, cost).
- Next 3 actions with owner and date.

Write in the user's language.
