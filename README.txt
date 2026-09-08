VALBEN Project Dashboard V10.7 — Debug + Stability

BUILT FROM V10.6

PRIMARY BUG FIX: BLOCKER TYPE OPTIONS
Problem:
- The native Blocker Type dropdown could fail to display its options reliably, especially inside the Full Screen / mobile layout.

Fix:
- Replaced the native select dropdown with 8 visible touch-friendly option buttons:
  RFI
  Inspection
  Material
  Equipment
  Weather
  GC Decision
  Labor
  Other
- The selected type is highlighted.
- Works with mouse, touch and iPad/iPhone Safari-style layouts.
- Existing saved blocker types continue to load.

FULL SCREEN MODAL FIX
- The Blocker modal now uses a layer above the Schedule Full Screen workspace.
- Blocker editor remains visible while Schedule is in Full Screen.

PERFORMANCE / EVENT FIX
- V10.6 could add duplicate global pointer listeners each time Schedule re-rendered.
- V10.7 installs those global column resize listeners only once.
- This reduces the chance of duplicated resize behavior or gradual interface slowdown after many edits.

NEW: SYSTEM DIAGNOSTICS
Open:
Guide / Version Notes → System Diagnostics

Checks:
- Core UI elements
- Blocker option controls
- Blocker modal z-index vs Full Screen
- Schedule table
- Excel column resize handles
- Column resize listener initialization
- Project/task state
- Supabase client
- Current view / Full Screen / Zoom

The diagnostics are non-destructive and do not modify project data.

ALL PRIOR FEATURES REMAIN
- Full Schedule Workspace
- Full Screen / Escape exit
- Zoom
- Smart Excel-style columns
- Auto Fit / Reset Columns
- 3-Week Fit
- Unified Schedule scrolling
- Login / Forgot Password
- Multiple projects
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
- DEBUG_REPORT.txt (optional documentation only)

Commit changes.
If the repository is connected to Vercel, it should redeploy automatically.

SUPABASE
No database migration is required for V10.7.
