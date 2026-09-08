VALBEN Project Dashboard V10.6 — Smart Excel Columns

BUILT FROM V10.5

WHY THIS VERSION
The Full Detail Schedule had too many fixed-width columns, making some fields hard to read.
V10.6 keeps the same Schedule/Gantt workflow but gives the table Excel-like column control.

NEW: MANUAL COLUMN RESIZE
- In Full Detail, drag the right edge of any column header.
- Works with mouse, trackpad and touch/pointer input.
- Width changes immediately while dragging.
- Column widths are saved locally in the browser/device.

NEW: DOUBLE-CLICK AUTO FIT
- Double-click a column separator.
- That individual column automatically sizes itself to its current content.
- Predecessor considers the available option text, not only the selected item.

NEW: AUTO FIT COLUMNS
- New Auto Fit Columns button.
- Automatically sizes all 14 Schedule columns from the current rows.
- Each column has safe minimum and maximum limits to prevent the table from becoming unusable.

NEW: RESET COLUMNS
- Restores the recommended professional widths.
- Hidden on narrow iPhone screens to reduce toolbar clutter.

NEW: SMART TASK NAME WIDTH
- As a longer activity name is typed, Task Name expands automatically.
- It only grows when needed.
- It is capped at a safe maximum so the Gantt remains accessible.

DEVICE-SPECIFIC PREFERENCE
- Widths are saved per browser/device instead of to the project cloud state.
- Windows can keep a wider detailed layout.
- iPad can keep a different touch-friendly layout.
- iPhone can use Auto Fit / 3-Week Fit without changing the Windows layout.

3-WEEK FIT
- The compact 3-Week Fit layout remains intentionally controlled.
- Manual column resizing applies to Full Detail.
- This prevents accidental resizing from damaging the compact 21-day mobile view.

ALL PRIOR FEATURES REMAIN
- Full Schedule Workspace / Full Screen
- Zoom
- Unified schedule scrolling
- 3-Week Fit
- Login / Forgot Password
- Multiple cloud projects
- Editable Project Name / Location
- Blockers
- Needs Attention
- Baseline vs Current
- Continuous Gantt
- FS / SS / FF
- No Work dates
- Calendar
- Three-Week Lookahead
- Print / PDF
- Themes / Dark Background
- Project logo upload

UPLOAD TO GITHUB
Replace these files in the ROOT of the same repository:
- index.html
- logo.jpg
- README.txt

Commit changes.
If the repository is connected to Vercel, it should redeploy automatically.

SUPABASE
No database migration is required for V10.6.
Column widths are a local interface preference and are intentionally not stored in the project database.
