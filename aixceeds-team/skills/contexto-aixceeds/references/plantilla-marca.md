# Plantilla de marca AIXCEEDS

Apply this template to every visual or formatted deliverable. Values match the
AIXCEEDS Portfolio Command Center v7.

## Two modes

| Mode | Background | Text | Typography |
|------|-----------|------|-----------|
| **Night** (default) | Dark night blue `#0B1426` (layers `#0F1B33`, `#14233F`, `#1A2C4E`) | Silver `#E9ECF1` (secondary `#C9CFD9`, muted `#8D97A8`) | Book Antiqua |
| **Silver** | Shiny silver `#E9ECF1` (layers `#C9CFD9`) | Dark night blue `#0B1426` | Calibri |

Use Night for presentations, dashboards and hero pieces. Use Silver for
documents meant to be printed or read at length.

## Highlights

- **Blue Martini `#2E74E8`** — always the primary highlight: key numbers, links, active states, the one idea per slide.
- **Miami cyan `#00D4FF`** — optional secondary accent for data series, used sparingly.
- **Red Martini `#E23B4E`** — rarely: risks, kill decisions, critical alerts only.
- **White `#FFFFFF`** — rarely: maximum emphasis on Night backgrounds.

## Typography stacks (CSS)

```css
--serif: "Book Antiqua", "Palatino Linotype", Palatino, "URW Palladio L", Georgia, serif;
--sans: Calibri, Carlito, "Segoe UI", Candara, system-ui, sans-serif;
```

- Night mode: headings and body in `--serif`; small UI labels may use `--sans`.
- Silver mode: headings and body in `--sans`.

## CSS tokens

```css
:root{
  --navy:#0B1426; --navy-2:#0F1B33; --navy-3:#14233F; --navy-4:#1A2C4E;
  --silver:#E9ECF1; --silver-2:#C9CFD9; --silver-3:#8D97A8; --silver-4:#5E6A7E;
  --martini:#2E74E8; --miami:#00D4FF; --red:#E23B4E;
  --hair:rgba(201,207,217,.18);
}
```

## Style rules

- One highlight color per view. Red Martini never appears next to good news.
- Hairline dividers (`--hair`) instead of heavy boxes.
- Generous whitespace; numbers large, labels small and muted.
- Brand name always written **AIXCEEDS** in caps; **4971 Ventures** as written.
