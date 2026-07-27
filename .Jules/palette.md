## 2026-07-09 - [Fluid Notification Entry and Spring Motion]
**Learning:** For fluid entry/exit animations on notification components (like toasts), applying a slide-up transition using CSS translation combined with a custom 'cubic-bezier' easing function (e.g., 'cubic-bezier(0.34, 1.56, 0.64, 1)') achieves a smooth, professional spring effect.
**Action:** Combine CSS transform transitions with cubic-bezier functions on entry/exit states of temporary micro-feedback elements.

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

## 2026-07-09 - [Focus State Color Contrast on Dark Component Backgrounds]
**Learning:** For interactive controls embedded inside dark containers, standard medium-dark focus outline colors (such as `#2563eb` blue-600) can result in extremely low and non-WCAG-compliant contrast. Using lighter, high-contrast outlines (such as `#38bdf8` sky-400) specifically for elements inside dark-themed components ensures they remain fully visible to keyboard navigators.
**Action:** Always verify the contrast of focus indicators on dark container backgrounds and apply high-contrast focus styling like `.undo:focus-visible { outline: 2px solid #38bdf8; }` when appropriate.
