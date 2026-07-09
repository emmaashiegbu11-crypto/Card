## 2026-07-09 - [Bidirectional Focus Management]
**Learning:** For undoable actions like deletion, managing focus bi-directionally is crucial for accessibility. Moving focus to the 'Undo' action in a toast upon deletion, and returning it to the original trigger upon restoration, ensures screen reader users never lose their place in the UI. Dynamically injecting the 'Undo' button into an `aria-live` region also ensures the status change is immediately announced.
**Action:** Always implement focus return logic and use dynamic `aria-live` content when providing an 'Undo' capability.
