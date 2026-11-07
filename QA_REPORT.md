# V9 QA Report

- Built from V8; V8 source archive retained unchanged.
- Dedicated Welcome Home screen added before the application shell.
- Nine existing navigation tabs retained; welcome shortcuts route into them.
- 365 date-indexed daily event/fact combinations are generated from themed content pools and change with the calendar date.
- V8, V7 and V6 save keys are supported for migration to V9.
- Service worker cache and manifest labels updated to V9.

## Automated checks
- JavaScript syntax: run with `node --check js/app.js`.
- HTML structure: welcome screen and app shell IDs checked.
- Navigation IDs: all nine existing tabs retain matching view IDs.
- Daily world: 365 deterministic day indexes checked for distinct event/fact card combinations.
- ZIP integrity checked after packaging.

## Testing limitation
A full interactive browser/device test is not claimed here. Validate on Android Chrome after deploying to GitHub Pages. Browser reminders still require the page to remain active; closed-app delivery is not guaranteed by static hosting.
