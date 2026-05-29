# Newborn Schedule Planner

Single-file HTML tool (index.html). Self-contained — embedded CSS and vanilla JS, no build step, no dependencies. Open directly in a browser to test.

## Conventions
- Stay self-contained: no external scripts or CSS.
- Every research-backed number stays cited in the sources panel.
- Match the Emily Oster style: honest evidence labels (Strong / Moderate / Practitioner consensus).

## Architecture
- Inputs at the top of <body> feed into update() in the bottom <script>.
- removalPlan() is the core physiological model; sexMultiplier() adjusts the daily milk volume.
- genSchedule() produces the three schedule variants, anchored on the baby's first morning meal (placeFeedTimes()).
- applyConstraints() / validGoalsFor() / validMethodsFor() keep the input segments from forming invalid combinations.
- saveSettings() / loadSettings() persist inputs in localStorage under SETTINGS_KEY.
- The export panel (openExporter(), renderExporter(), wireExporterTimeline()) lets the user customize events and generateICS() builds a downloadable .ics for Google Calendar — all client-side.
- ICON_PATHS and iconSvg() handle inline SVGs.
