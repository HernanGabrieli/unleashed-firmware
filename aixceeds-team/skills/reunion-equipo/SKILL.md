---
name: reunion-equipo
description: >
  This skill should be used when the user wants the whole AIXCEEDS / 4971
  Ventures team to work on a question together — "reunión de equipo",
  "convocá al equipo", "board meeting", "qué opina el equipo", "riunione del
  team", "analicemos esto desde todos los ángulos", or any decision that
  crosses strategy, market, finance, technology and positioning.
metadata:
  version: "0.1.0"
---

# Reunión de equipo

Convene the AIXCEEDS consulting and development team on one question and
return a single, decided recommendation.

## Steps

1. **Load context**: load `contexto-aixceeds` and read the business profile.
2. **Frame the question**: restate the decision in one sentence. If the
   question is too vague to act on, ask one clarifying question, then proceed.
3. **Select participants**: choose only the agents whose expertise the
   question needs (usually 2–4):
   - `estratega-bizdev` — strategy, GTM, partnerships
   - `analista-mercado` — market evidence, competitors
   - `analista-inversiones` — numbers, risk, go/kill
   - `arquitecto-desarrollador` — feasibility, effort, cost
   - `rd-publicaciones` — positioning and narrative impact
4. **Run them in parallel**: launch the selected agents at the same time, each
   with the framed question, the relevant profile excerpts, and the instruction
   to answer from its own specialty in under 400 words with a clear position.
   If `analista-mercado` must supply facts the others need, run it first.
5. **Synthesize** as chair of the meeting:
   - Where the team agrees.
   - Where it disagrees, and which argument is stronger and why.
   - The decision.

## Output — "Acta de reunión"

```
# Acta · <tema> · <fecha>
Participantes: <agentes>

## Decisión
<2–3 líneas, en Blue Martini si es visual>

## Posiciones del equipo
- Estrategia: ...
- Mercado: ...
- Finanzas: ...
- Técnico: ...
- Posicionamiento: ...

## Desacuerdos y cómo se resolvieron

## Riesgo principal (Red Martini solo si es crítico)

## Próximos pasos
| # | Acción | Responsable | Fecha |
```

Offer to save the acta to Google Drive or turn it into a Gamma one-pager in
the AIXCEEDS template. Write in the user's language.
