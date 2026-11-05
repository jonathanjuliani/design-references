---
source: https://docs.stripe.com/terminal/payments/collect-card-payment
captured: 2026-10-27
surface: in-person card payment integration docs, failure and retry handling for a shipped reader
audience: builders of point-of-sale and kiosk apps that take cards in person
domains:
  - payments
  - developer-tools
principles:
  - trust-first
verify_after: 2027-04-27
---

## Taken

- An unknown outcome is its own state. When the response never arrives, look up the status of the original payment and retry that one. Never start a new charge, because that is how a customer pays twice.
- A declined card is retried against the same payment with a different card, so a retry cannot become a second charge.
- When the connection is lost, the app says so and blocks payment until it returns. Browsing can continue, paying cannot.
- The reader shows a processing state for several seconds before failing. The interface needs a deliberate "checking" screen, not an instant error.

## Rejected

- Offline mode that accepts cards without a connection. A declined offline payment is lost money for the operator, and an unattended kiosk has nobody to resolve it.

## Not applicable here

- Manual capture and the two-day authorisation window are backend concerns with no screen of their own.
