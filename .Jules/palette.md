## 2026-07-09 - Accessible Toast Notifications with Timer Controls and Focus Handover

**Learning:** Auto-dismissing toast notifications that contain interactive controls (like Undo) must pause their timer when hovered or focused (WCAG 2.2 Timing Adjustable) and include an immediate close/dismiss button. Additionally, if keyboard focus resides inside the toast when it expires or is dismissed, focus must be gracefully handed off to a logical action (such as the empty state Restore button) to prevent keyboard trap or focus loss.

**Action:** Attach hover (`mouseenter`/`mouseleave`) and focus (`focusin`/`focusout`) listeners to auto-dismissing toasts to pause/resume countdowns, and check `toast.contains(document.activeElement)` during dismissal/expiration to redirect focus smoothly.
