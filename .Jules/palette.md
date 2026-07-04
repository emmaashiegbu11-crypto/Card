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

## 2026-06-25 - [Progress Bars for Undo Toasts]
**Learning:** While "Undo" buttons provide a safety net, they can be stressful if the user doesn't know how long they have to react. A shrinking progress bar provides a calm, clear visual countdown that reduces anxiety and improves the predictability of the interface.
**Action:** Always pair timed "Undo" notifications with a visual indicator of the remaining time to improve the perceived control of the user.

## 2026-06-30 - [Spatial Cues for Keyboard Focus]
**Learning:** Keyboard users often miss out on spatial feedback (like card "lift" effects) that mouse users get on hover. Applying these transitions to `:focus-within` ensures all users receive consistent state-change cues.
**Action:** Always pair :hover spatial transitions with :focus-within to maintain visual parity between input methods.

## 2026-07-01 - [Loopable Demos and Restoration Feedback]
**Learning:** For interactive demos, providing a "loop" (an empty state with a reset) allows users to explore the interaction repeatedly without manual refreshes. Furthermore, adding specific "restoration" feedback (like a success highlight) makes the reversal of a destructive action feel as intentional and confirmed as the action itself.
**Action:** Implement empty states with reset capabilities for single-component demos and use visual highlights to confirm successful restoration of elements.

## 2026-07-04 - [Keyboard Shortcut Discoverability]
**Learning:** Keyboard shortcuts are powerful but often "invisible" to users. Providing explicit visual hints (like `(Esc)` or `(Delete)`) within ARIA labels, titles, and button text significantly lowers the barrier to entry for power users and improves overall accessibility.
**Action:** Always include keyboard shortcut hints in tooltips and ARIA labels for primary actions to bridge the gap between mouse and keyboard efficiency.
