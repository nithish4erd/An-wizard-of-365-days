# A Wizard Experience of 365 Days — V9

V9 is a story-depth and runtime-validation upgrade built from V7.

## Story depth
- 365 numbered episodes across 12 correctly ranged arcs.
- Every episode has a distinct opening, middle, and closing passage.
- Every day has two distinct, context-specific choices.
- Each choice records an outcome and an initiative/empathy story trait.
- Daily story choices remain gated behind completion of all 8 primary missions.

## Preserved systems
- Eight daily primary tasks, editable subtasks, XP, levels, attributes, streaks.
- Academy, houses, companion, games, Chronicle, Codex, spellbook and other V7 systems.
- Local save, JSON export/import, responsive UI and PWA files.

## V9 technical changes
- Save migration: reads V9 save first, then V7, then V6 if no V9 save exists.
- Service-worker cache updated to `wizard-experience-365-v8`.
- Reminder checker now tolerates a delayed timer tick by sending within a 3-minute window, with per-day/per-time duplicate protection.
- JavaScript syntax and story data consistency checks are included in the delivery report.

## Notification limitation
The reminder checker runs only while the app page is active. Browser timer throttling may delay a reminder. A static GitHub Pages PWA cannot guarantee notifications after the app is fully closed. Reliable closed-app delivery requires a push-notification backend/service or native Android scheduling.

## Deploy
Upload the contents of this folder to the root of the Wizard repository. Do not overwrite the separate A COLLEGE OF 1000 DAYS repository. Enable GitHub Pages from `main` / root.

## Save safety
V9 reads existing V7 and V6 saves and writes new progress to `wizardExperience365V9`. Export a JSON backup before changing deployed versions.


## V9 additions
- A dedicated Welcome Home gateway appears before the nine application navigation tabs.
- Welcome actions route into Command Center, Daily Story, Daily Missions and Academy.
- Aurelion daily event and magical field-note cards change with the in-app story day (365 day-indexed combinations).
- V8/V7/V6 local saves are migrated into the V9 save key.
