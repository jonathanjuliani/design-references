---
source: https://support.toasttab.com/en/article/Kiosk-Placing-Orders-Making-Payments-and-Tipping
captured: 2026-10-27
surface: restaurant self-ordering kiosk ordering and payment flow, read from the vendor's documentation of the shipped flow
audience: guests ordering and paying alone at a restaurant kiosk
domains:
  - payments
principles:
  - task-focused
verify_after: 2027-04-27
---

## Taken

- While an item is customised, its total updates live in the bottom-right corner, the same corner as the next action.
- The order is reviewed and edited from one "View order" screen, then "Checkout now". Editing does not mean walking back through the menu.
- Card is the primary payment prompt, with the other methods as secondary buttons at the bottom of the same screen.
- Orders that time out or fail are voided with a named reason. An abandoned session ends on purpose instead of hanging.
- Declined-card guidance is to be discreet and suggest another method. The vendor cannot re-run a declined payment, so the screen has to offer a different card.

## Rejected

- Long modifier groups that need scrolling to reach the next group. A no-scroll kiosk cannot hide required choices below the fold.
- Pay with cash by printing a receipt for a cashier. There is no staff to take it.

## Not applicable here

- Promo codes, guest-information prompts, and the tipping screen are merchant options outside this order size.
