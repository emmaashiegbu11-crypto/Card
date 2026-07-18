## 2026-07-09 - [Loopable Empty State and Focus Hand-off]
**Learning:** In interactive component demos, providing a "loop" via an empty state with a restoration action allows repeatable exploration. Programmatically shifting focus from an expiring toast's Undo button to the Restore button ensures keyboard users never lose their active focus state.
**Action:** Implement loopable states for interactive demos and manage focus hand-offs during transitions to avoid losing focus.

## 2026-07-09 - [Keyboard Shortcut Discoverability]
**Learning:** Icon-only buttons benefit from keyboard shortcut hints that are revealed on hover and focus. To ensure a clean UI, these hints can be hidden by default but smoothly transitioned into view on focus/hover, keeping them discoverable without cluttering the screen.
**Action:** Use CSS transition-based `.shortcut-hint` elements that expand on hover and focus-within to display shortcuts to keyboard and mouse users.
