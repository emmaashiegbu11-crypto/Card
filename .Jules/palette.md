## 2026-07-09 - [Bidirectional Focus Management for Undoable Actions]
**Learning:** For destructive actions with an "Undo" option, screen reader accessibility is significantly improved by managing focus bidirectionally. Moving focus to the "Undo" button upon deletion ensures the user is immediately aware of the reversal option, while returning focus to the original trigger upon restoration provides a seamless continuation of their workflow. Pairing this with `aria-live` announcements ensures multi-modal feedback.
**Action:** Always implement bidirectional focus management and `aria-live` announcements for interactions that temporarily remove elements from the UI.

## 2026-07-09 - [Graceful Focus Handover on Toast Expiration]
**Learning:** When a toast with an "Undo" option expires, focus can be left in a "dead" state if the user was focused on the Undo button. Programmatically shifting focus to the fallback restoration action (e.g., a "Restore" button in an empty state) prevents this and maintains a smooth keyboard navigation flow.
**Action:** Check `document.activeElement` before hiding a toast; if focus is on a transient action, move it to the next logical persistent action.
