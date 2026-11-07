# V10 QA Report

- Navigation uses one delegated bubble-phase click handler.
- Removed capture-phase `stopImmediatePropagation()` interception and duplicate direct tab handlers.
- `tab()` explicitly reveals the app shell and selected view, updates active state, and scrolls to the selected view.
- Service-worker cache bumped to `wizard-experience-365-v10`.
- JavaScript syntax check and navigation target audit are performed during packaging.
- Full Android Chrome testing remains outstanding.
