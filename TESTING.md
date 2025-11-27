# Manual Test Log

## LoginSystem gating check (headless Playwright via browser container)
- Start `python -m http.server 8000` from project root.
- Navigated to `LoginSystem.html`.
- Verified vault title input and export button disabled before login: `locked_title_disabled=true`, `locked_export_disabled=true`.
- Submitted login with `genesis-admin` / `synaptics`, scope `DEFENSIVE-EDGE`, note `test-session`.
- Confirmed vault controls unlocked after login: `unlocked_title_disabled=false`, `unlocked_export_disabled=false`.

## Integrated auth + admin + hub state (headless Playwright)
- With `python -m http.server 8000` running, navigated to `LoginSystem.html` and authenticated as `genesis-admin` / `synaptics` (scope `DEFENSIVE-EDGE`, note `integration-check`).
- Added a vault record (`integration secret`) and confirmed controls were unlocked post-login.
- Moved to `AdminControl.html` in the same session; save control auto-unlocked, configuration saved, and an audit log row was recorded.
- Visited `index.html` and verified the Interconnect Status card reflected linked auth session, seeded users, stored vault records, and updated admin configuration.
