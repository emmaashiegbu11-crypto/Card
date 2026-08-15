## 2026-07-09 - Focus Management and Autohide Pause in Accessible Toasts

**Learning:** When implementing auto-dismissing toast notifications containing action buttons (such as "Undo"), auto-dismissal timers can trap or interrupt keyboard users if focus or hover events do not pause countdowns. Pausing the countdown independently on `mouseenter`/`focusin` and resuming on `mouseleave`/`focusout` ensures compliance with WCAG 2.2 Timing Adjustable guidelines while preventing focus loss. Additionally, when a toast action is dismissed or triggered, programmatically transferring focus back to the restore button or original trigger element maintains intuitive keyboard navigation flow.

**Action:** Always track `isHovered` and `isFocused` states independently when auto-dismissing interactive toasts. Manage focus explicitly upon deletion, undo, and expiration so screen reader and keyboard users maintain clear navigation context.
