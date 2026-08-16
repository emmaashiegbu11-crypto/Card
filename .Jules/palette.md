## 2026-07-09 - Accessible Toast Timer Control and Graceful Focus Transitions

**Learning:** When auto-dismissing notification toasts feature action controls (like Undo), pausing countdown timers on hover (`mouseenter`/`mouseleave`) and keyboard focus (`focusin`/`focusout`) satisfies WCAG 2.2 Timing Adjustable requirements and prevents unexpected focus loss while a keyboard user interacts with the toast. Additionally, when a toast expires or is dismissed while focused, gracefully handing focus off to the next logical action (such as the empty state restore button) maintains keyboard navigation context.

**Action:** Independently track hover and focus states when managing autohide timers on interactive toasts, and ensure focus transitions gracefully upon expiration or dismissal.
