---
source: https://docs.clover.com/dev/docs/developer-quick-start-clover-kiosk-integration
captured: 2026-10-27
surface: developer guidance for third-party apps on a shipped self-ordering kiosk with a separate PIN pad
audience: unattended customers ordering and paying at a large-screen kiosk
domains:
  - payments
  - developer-tools
principles:
  - task-focused
  - trust-first
verify_after: 2027-04-27
---

## Taken

- An idle session gets a "Still there?" countdown before the order is cleared. The stated reason is privacy for the next customer as well as recovery for this one.
- Payment is a one-way hand-off. The big screen says to continue on the payment device and never asks the customer to come back for a secondary task such as a receipt email.
- Items are edited straight from the order summary, without repeated Back taps.
- Accessibility levels are a release gate, not advice. AA contrast, consistent action placement, an on-screen keyboard that can be reached, and plain error messages with handling instructions are the recommended floor.
- The attract or home screen keeps movement low and stays calm when nobody is using it.

## Rejected

- A progress bar across the top. A flow with four steps and a persistent order panel does not need one, and it competes with the total.

## Not applicable here

- The separate PIN-pad hardware and its screen. A single tablet carries payment in its own content area.
- Platform details such as customer mode and keeping the screen awake belong to the device, not the design.
