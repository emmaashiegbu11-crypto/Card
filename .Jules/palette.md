## 2026-07-09 - Accessible Card Deletion and Restoration Loop UX

**Learning:** When providing undoable destructive actions (like deleting a card) in a single-card or empty-state context, auto-dismissing toast notifications must gracefully yield keyboard focus to the empty state's primary restoration action when expired to prevent abrupt focus loss.

**Action:** Whenever a toast notification containing focus expires, check `document.activeElement` and shift focus to a logical next action (such as a restore/reset button) while maintaining live announcements.
