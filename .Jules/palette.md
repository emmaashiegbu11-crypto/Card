## 2026-07-09 - [Multi-modal Confirmation for Hidden Actions]
**Learning:** Copying to clipboard is an "invisible" action with no native DOM side effects, which can leave screen reader and keyboard users unsure of its success. Combining a tactile transition, a focus outline, immediate button label/color swap, and an aria-live announcement ensures a fully accessible, multi-modal confirmation.
**Action:** Pair clipboard copy actions with immediate color-shift feedback, an active state scale transition, and a polite aria-live announcement.
