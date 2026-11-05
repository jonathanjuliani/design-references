---
source: https://www.boothiq.com/docs/reference/timeouts
captured: 2026-10-27
surface: unattended paid photo booth, per-screen idle timeout reference from the vendor's docs
audience: walk-up customers using a paid machine with no attendant
domains:
  - payments
principles:
  - task-focused
verify_after: 2027-04-27
---

## Taken

- Timeouts are set per screen, not globally. The welcome screen never times out, choosing screens are short, and slow tasks get longer.
- Two-stage warning: "Are you still there?" well before the timeout, a short "Returning..." just before it, then the action.
- The payment screen times out by cancelling back one step, not by resetting the whole session.
- Timeouts never wipe money already paid. Paid state is protected even when the customer walks away.
- The thank-you screen returns to welcome after a few seconds so the next customer starts clean.

## Rejected

- Timeout values nobody can configure. A kiosk build should keep them as named constants in one place.

## Not applicable here

- The camera and print screens, and their capture-specific abandonment rules.
