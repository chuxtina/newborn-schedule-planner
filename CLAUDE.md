# Newborn Schedule Planner

Single-file HTML tool (index.html). Self-contained — embedded CSS and vanilla JS, no build step, no dependencies. Open directly in a browser to test.

## Conventions
- Stay self-contained: no external scripts or CSS.
- Every research-backed number stays cited in the sources panel.
- Match the Emily Oster style: honest evidence labels (Strong / Moderate / Practitioner consensus).

## Architecture
- Inputs at the top of <body> feed into update() in the bottom <script>.
- removalPlan() is the core physiological model.
- genSchedule() produces the three schedule variants.
- ICON_PATHS and iconSvg() handle inline SVGs.
