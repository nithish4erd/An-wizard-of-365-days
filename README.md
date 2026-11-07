# A Wizard Experience of 365 Days — V6

V6 adds the Arcane Codex systems to the V5 visual redesign.

## Included
- Identity Stat Engine: each checked subtask casts a vote toward a Wizard Identity; 10 votes unlock a permanent profile badge.
- Spellbook: seven-day task streak unlocks the matching spell; task completion triggers a visual Arcane Burst, optional vibration, and a short generated tone.
- Ikigai Four Arcane Circles: four daily balance groups; completing all four grants a companion bond bonus and records a secret-page milestone.
- Shadow Boss Arena: weekly attack score based on completed primary missions; 80%+ earns a victory reward.
- Never Miss Twice Rune: records a missed-day return opportunity and preserves the streak when all eight primary missions are completed the next day.
- Tiny Habits Anchor Runes: create contextual prompts and display them on the dashboard.
- Mirror of Erised: save a 365-day vision and dated reflection checkpoints.
- Interactive Alchemy: craft a 2× XP elixir for the next primary mission reward.
- Aurelion Timekeeper: live clock and default reminder times of 07:00, 13:00 and 18:00, notification permission and test notification.

## Deploy
Upload the contents of this folder to the root of the NEW Wizard repository. Do not modify the old A COLLEGE OF 1000 DAYS repository. Enable GitHub Pages from `main` / root.

## Notification limitation
The reminder checker runs while the app page is open. A normal static GitHub Pages PWA cannot guarantee exact-time notifications after the app is fully closed. Reliable closed-app delivery requires a push-notification backend/service or native Android scheduling. The UI intentionally explains this limitation; the test notification does not prove scheduled background delivery.

## Data
Local browser storage only; no account or cloud sync. Export backups periodically. V6 uses a separate storage key and service-worker cache. This is a PWA prototype, not a native APK. Test on the live GitHub Pages URL and Android device before relying on reminders.
