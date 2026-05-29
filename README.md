# Newborn Schedule Planner

A research-backed planner for newborn (0–3 months) feeding, pumping, and sleep schedules. Set your inputs and the tool generates three sample 24-hour schedules. Every milk-volume and sleep number is cited to a primary source or major guideline, with honest evidence-quality labels (Strong / Moderate / Practitioner consensus).

**Live demo:** https://chuxtina.github.io/newborn-schedule-planner/

## What it does

- Computes a daily milk target based on your baby's age, sex, and your breastmilk-vs-formula split
- Generates three sample 24-hour schedules, each anchored on the baby's first morning meal
- Models the physiology of milk removal — nursings + pumps with realistic spacing rules
- Flags supply trade-offs when the overnight gap is long enough to affect production
- Lets you customize a schedule and export it to Google Calendar as a downloadable .ics file
- Remembers your inputs between visits (saved locally in your browser)
- Cites every research-backed number in a side-panel sources view

## Run locally

It's a single self-contained HTML file — no build step, no dependencies, no tracking. Just open it.

```
open index.html
```

Or double-click the file in Finder/Explorer.

## Privacy

Everything runs in your browser. No analytics, no network requests, no data leaves the page.

## Disclaimer

For information, not medical advice. Talk to your pediatrician about your baby's individual needs.

Newborns don't actually follow schedules — they follow hunger and sleep pressure. The strongest evidence supports responsive (cue-based) feeding in the first months, not rigid clocks. Treat these schedules as a loose frame for your day, not a prescription. The most useful number on the page is the daily milk target; the times around it are just one plausible way to distribute it.
