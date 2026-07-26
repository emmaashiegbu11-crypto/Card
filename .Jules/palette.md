## 2026-07-09 - [Independent State Tracking for Toast Pauses]
**Learning:** When implementing hover-to-pause and focus-to-pause behaviors on auto-dismissing toast notifications, keeping track of both states independently (e.g., using 'isHovered' and active focus checks) ensures that triggering 'mouseleave' does not prematurely resume the timer while keyboard focus is still active within the toast.
**Action:** Always maintain distinct, non-overlapping checks for hover and keyboard focus before resuming any auto-hide progress bars or timers.
