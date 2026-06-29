## 2024-06-29 - [Non-blocking Undo Pattern]
**Learning:** Favor non-blocking 'Undo' patterns (toast notifications) over disruptive 'window.confirm()' dialogs for non-critical user actions like deletions. This keeps the user in their flow while still providing a safety net.
**Action:** Replace 'window.confirm()' with a temporary toast notification containing an 'Undo' action.
