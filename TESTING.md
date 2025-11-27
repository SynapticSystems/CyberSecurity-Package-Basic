# Manual Test Log

## LoginSystem gating check (headless Playwright via browser container)
- Start `python -m http.server 8000` from project root.
- Navigated to `LoginSystem.html`.
- Verified vault title input and export button disabled before login: `locked_title_disabled=true`, `locked_export_disabled=true`.
- Submitted login with `genesis-admin` / `synaptics`, scope `DEFENSIVE-EDGE`, note `test-session`.
- Confirmed vault controls unlocked after login: `unlocked_title_disabled=false`, `unlocked_export_disabled=false`.
