## 2026-07-09 - [Bidirectional Focus Management for Undoable Actions]
**Learning:** For destructive actions with an "Undo" option, screen reader accessibility is significantly improved by managing focus bidirectionally. Moving focus to the "Undo" button upon deletion ensures the user is immediately aware of the reversal option, while returning focus to the original trigger upon restoration provides a seamless continuation of their workflow. Pairing this with `aria-live` announcements ensures multi-modal feedback.
**Action:** Always implement bidirectional focus management and `aria-live` announcements for interactions that temporarily remove elements from the UI.

## 2026-07-09 - [Loopable Empty States and Focus Hand-off]
**Learning:** For interactive demos, providing a "loop" by implementing an empty state with a restoration capability allows users to explore interactions repeatedly without manual refreshes. When an interactive element (like an Undo button) expires, programmatically shifting focus to the new primary action in the empty state (like a Restore button) maintains a smooth keyboard navigation flow and prevents focus from being lost to the body.
**Action:** Implement loopable states for demos and manage focus hand-offs during state transitions, especially when elements are removed automatically due to timers.
