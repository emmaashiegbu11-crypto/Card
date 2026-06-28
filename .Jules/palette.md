## 2024-06-28 - [Feedback for Invisible Actions]
**Learning:** Actions that don't have a visible DOM side-effect (like copying to clipboard) can be confusing for users if not paired with immediate feedback. Visual changes (icon swaps, tooltips) combined with ARIA live announcements bridge the gap between the user's action and their understanding of the result.
**Action:** Always provide both visual confirmation and screen reader announcements for "invisible" actions like clipboard copying or background saves.
