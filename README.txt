VALBEN Project Dashboard V10.8 — Gantt Alignment Engine

FIXED
- Gantt bars drifting vertically away from their activity rows.
- Bars appearing to disappear after several activities because the vertical drift accumulated.

WHAT CHANGED
- Schedule table header and Gantt header now use the same exact height.
- Each Gantt row is tagged with the same activity ID as its Schedule row.
- After rendering, V10.8 measures each actual table row and applies that exact height to the corresponding Gantt row.
- Bars are vertically centered in the synchronized row.
- The Gantt body height is recalculated from all activity rows.
- Dependency arrows now use measured row centers rather than a hard-coded 40 px row formula.
- A ResizeObserver re-aligns rows if geometry changes.
- Alignment is refreshed after column resizing, zoom, Full Detail / 3-Week Fit changes, and browser resizing.

DIAGNOSTICS
Guide → System Diagnostics now also checks:
- Expected activity rows vs rendered Gantt rows
- Expected working bar segments vs rendered segments
- Maximum row-height difference between table and Gantt

RESULT
The Gantt should remain aligned with 2, 5, 10, 20 or more activities.

UPLOAD
Replace in the same GitHub repository:
- index.html
- logo.jpg
- README.txt
- DEBUG_REPORT.txt (optional)

No Supabase migration is required.
