---
name: investigacion-mercado
description: >
  This skill should be used when the user asks for market research,
  competitor analysis, market sizing, trend scanning or a company/founder
  profile for AIXCEEDS or 4971 Ventures — "investigá el mercado",
  "competidores", "TAM SAM SOM", "tendencias de IA", "perfil de esta empresa",
  "ricerca di mercato", "quién más hace esto".
metadata:
  version: "0.1.0"
---

# Investigación de mercado

Run structured, cited market research through the `analista-mercado` agent.

## Steps

1. Load `contexto-aixceeds`.
2. Define the research brief in 4 lines: question, market (segment +
   geography), decision it informs, depth (rápida ≈ 1 page / profunda ≈ full report).
   Ask only if the question or geography is missing.
3. Delegate to `analista-mercado` with the brief. For a deep report on several
   geographies or segments, run one analyst per geography in parallel, then merge.
4. Check the result: every fact cited and dated, confidence marked, estimates
   labelled, no data older than 18 months without a flag.
5. Add a short "Implicaciones para 4971 Ventures" section: what this means for
   the portfolio and the recommended next step (often `validar-venture`).

## Output

- Hallazgos clave (3 bullets).
- Sizing (top-down and bottom-up) with assumptions.
- Competitive map and table.
- Espacio en blanco.
- Implicaciones y próximos pasos.
- Fuentes.

Offer to save the report to Google Drive in the AIXCEEDS template.
Write in the user's language.
