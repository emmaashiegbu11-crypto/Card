## 2026-07-05 - [Keyboard Shortcut Discoverability]
**Learning:** Adding keyboard shortcuts (like Delete or R) significantly improves power-user efficiency, but they must be discoverable. Including the shortcut key in the `aria-label`, `title`, and as a subtle visible hint (e.g., "(R)") ensures all users, including those using screen readers, are aware of the capability.
**Action:** Always pair new keyboard shortcuts with visible and accessible hints in labels and titles to ensure they are discoverable.

## 2026-07-09 - [Undo Micro-Interaction Refinement]
**Learning:** Immediately halting progress bar animations and disabling the "Undo" button upon activation prevents confusing visual states and double submissions during the restoration transition.
**Action:** Stop timers and visual progress indicators instantly when an undo action is triggered.
