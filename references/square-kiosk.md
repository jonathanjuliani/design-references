---
source: https://squareup.com/help/us/en/article/8540-preview-diner-experience-on-square-kiosk
captured: 2026-10-27
surface: restaurant self-ordering kiosk on a mounted iPad, read from the vendor's documentation of the shipped flow
audience: diners ordering alone at a counter kiosk, mostly in a hurry
domains:
  - payments
principles:
  - task-focused
  - trust-first
verify_after: 2027-04-27
---

## Taken

- The order stays visible beside the menu while items are added. The vendor sells this persistent cart as a feature, and it means the total never needs a tap to check.
- Picture-led categories, large type, and large tap targets are named as the baseline, not as polish.
- Quantity is a +/- stepper on the item, and a line in the order reopens the same item to edit it. Remove is a per-line trash control, and clearing the whole order is a separate, confirmed action.
- The upsell confirm button carries the count and the price ("Add 2 items - $8.50"). A price on the action itself keeps the running total honest.
- Leaving mid-order asks for confirmation before the order is cancelled.

## Rejected

- The dining-option gate (dine in or to go) before the menu. One extra decision at the door, and a snack bar has no table service.
- Loyalty sign-in with a phone number in the top corner. It adds a second entry point before the customer has ordered anything.

## Not applicable here

- Tipping, signature, and receipt settings are merchant configuration, not customer flow.
