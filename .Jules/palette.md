## 2025-06-21 - [Empty Repository UX]
**Learning:** An empty repository is the ultimate "empty state." Providing a helpful entry point with clear call-to-actions and accessibility-first examples reduces friction for developers and sets the tone for the project's quality.
**Action:** When encountering an empty project, initialize it with a README that demonstrates core UX values and provides immediate value to the next person (or agent) who opens it.

## 2026-06-22 - [Living Documentation for Components]
**Learning:** For component-centric repositories, documentation that includes a "living demo" (like a simple `index.html`) is far more effective than static code snippets alone.
**Action:** Include a minimal, interactive demo for UI components to bridge the gap between documentation and implementation.

## 2026-06-23 - [Accessible Deletion Feedback]
**Learning:** Removing elements from the DOM without an announcement leaves screen reader users in a state of confusion.
**Action:** Use an `aria-live` region to announce the success of destructive actions like deletions.

## 2026-06-24 - [Undo vs Confirm Dialogs]
**Learning:** For most non-critical deletions, a non-blocking "Undo" pattern is superior to a disruptive "Confirm" dialog. It maintains user flow while still providing a safety net.
**Action:** Favor optimistic deletion with an "Undo" toast over `window.confirm()` for a smoother, more modern micro-interaction.
