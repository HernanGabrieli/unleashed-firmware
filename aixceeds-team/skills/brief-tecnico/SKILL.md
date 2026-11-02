---
name: brief-tecnico
description: >
  This skill should be used when the user needs technical design or
  development for AIXCEEDS or a 4971 Ventures venture — "diseñá la
  arquitectura", "necesito un MVP", "prototipo", "¿cuánto cuesta
  construirlo?", "build vs buy", "revisá este código", "due diligence
  técnica", "actualizá el Command Center", "architettura della soluzione".
metadata:
  version: "0.1.0"
---

# Brief técnico

Turn a business need into a buildable technical plan, then build it if asked,
through the `arquitecto-desarrollador` agent.

## Steps

1. Load `contexto-aixceeds`.
2. Write the brief (confirm with the user only if a field is unknown and changes the design):
   - Hypothesis or business goal the build serves.
   - Users and the one core flow.
   - Success metric and deadline.
   - Constraints: budget, data (personal data → GDPR), integrations, team.
3. Delegate to `arquitecto-desarrollador`:
   - Architecture, stack table, diagram, effort, monthly cost, risks.
   - Recommend the smallest version that tests the hypothesis.
4. If the user approves building:
   - In Claude Code: build in the project folder, test, and report what was verified.
   - In Cowork: produce the files (HTML, scripts, specs) in the outputs folder.
   - Web interfaces follow the AIXCEEDS template (Night mode by default).
5. For code review or technical due diligence: list findings by severity
   (crítico / importante / menor) with the concrete fix.

## Output

- **Recomendación** (2–3 lines).
- Brief, architecture, stack table, effort and cost.
- Risks and de-risking experiments.
- Build plan in milestones (week by week for MVPs).

Write in the user's language; code comments in English.
