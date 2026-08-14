## 2026-07-09 - [Consolidated Single-File Accessible Interactions]
**Learning:** For isolated interactive component demos, packing high-fidelity features (such as focus/hover-paused undo timers, keyboard shortcuts, and visual restoration feedback) into extremely compact consolidated scripts guarantees high performance, zero external dependencies, and absolute structural simplicity.
**Action:** Consolidate CSS state selectors and leverage multi-event listeners to keep micro-interaction prototype implementations clean, self-contained, and readable under tight space constraints.

## 2026-07-09 - [Toast Dismissibility and Graceful Focus Hand-off]
**Learning:** Automatically expiring notification toasts with interactive controls (like Undo) require an immediate close/dismiss button to satisfy WCAG 2.2 dismissibility. If a user dismisses a toast while keyboard focus is inside it, gracefully redirecting focus to a logical next action (such as the empty state restore button) prevents keyboard trap or focus loss.
**Action:** Always map focus states before destroying/hiding active notification toasts, and gracefully hand off focus to prevent accessibility and keyboard navigation defects.
