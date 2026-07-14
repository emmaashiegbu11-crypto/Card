## 2026-07-09 - [Bidirectional Focus Management for Undoable Actions]
**Learning:** For destructive actions with an "Undo" option, screen reader accessibility is significantly improved by managing focus bidirectionally. Moving focus to the "Undo" button upon deletion ensures the user is immediately aware of the reversal option, while returning focus to the original trigger upon restoration provides a seamless continuation of their workflow. Pairing this with `aria-live` announcements ensures multi-modal feedback.
**Action:** Always implement bidirectional focus management and `aria-live` announcements for interactions that temporarily remove elements from the UI.

## 2026-07-09 - [Loopable Empty State for Interactive Demos]
**Learning:** Providing a "loopable" experience in interactive demos via a clear empty state with a restoration action allows users to repeatedly explore interaction patterns (like deletion and undo) without refreshing the page. This increases engagement and provides a natural place for keyboard shortcut discovery.
**Action:** Always implement an accessible empty state with a primary "Restore" action in component-focused demonstration files.
