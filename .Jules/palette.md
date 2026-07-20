## 2026-07-09 - [Loopable Empty State and Focus Hand-off]
**Learning:** In interactive component demos, providing a "loop" via an empty state with a restoration action allows repeatable exploration. Programmatically shifting focus from an expiring toast's Undo button to the Restore button ensures keyboard users never lose their active focus state.
**Action:** Implement loopable states for interactive demos and manage focus hand-offs during transitions to avoid losing focus.

## 2026-07-09 - [Keyboard Shortcut Discoverability]
**Learning:** Icon-only buttons benefit from keyboard shortcut hints that are revealed on hover and focus. To ensure a clean UI, these hints can be hidden by default but smoothly transitioned into view on focus/hover, keeping them discoverable without cluttering the screen.
**Action:** Use CSS transition-based `.shortcut-hint` elements that expand on hover and focus-within to display shortcuts to keyboard and mouse users.

## 2026-07-09 - [Adjustable Toast Timing via Hover and Focus]
**Learning:** For dynamic content that auto-dismisses (such as toast notifications), users need a way to pause the timer to prevent accidental dismissal before they can read or interact with it. Halting and resuming the timer based on mouse hover and keyboard focus events provides an elegant, WCAG-compliant solution.
**Action:** Always bind `mouseenter`/`mouseleave` and `focusin`/`focusout` handlers to auto-dismissing notifications to pause and resume the remaining duration of the action.

## 2026-07-09 - [Dismissible Action Toasts and Focus Recovery]
**Learning:** Toasts featuring automated timers and interactive controls should include an explicit manual dismissal button. If a keyboard user manually dismisses the toast while focus is inside it, the focus must be programmatically recovered and gracefully handed off to a logical alternative (like the empty state's Restore button) to avoid a focus loss/keyboard trap.
**Action:** Always include a keyboard-accessible Close/Dismiss button in action toasts and implement bidirectional focus management for manual dismissal.
