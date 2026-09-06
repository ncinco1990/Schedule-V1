VALBEN Project Dashboard V10.3 — Unified Scroll + 3-Week Fit

BUILT FROM V10.2

SCHEDULE LAYOUT FIXES
- The task table is no longer sticky/frozen horizontally.
- Moving the bottom schedule scroll control moves the ENTIRE schedule:
  task table + Gantt timeline.
- Added a dedicated bottom horizontal navigator that stays easy to reach.
- Table and Gantt now behave as one continuous schedule canvas.

NEW VIEW MODES
1. FULL DETAIL
   - Shows every editable field:
     ID, Task, Duration, Start, Finish, Variance, %, Status, Blocker,
     Predecessor, Link, Move, Done, Delete.
   - Best for detailed editing.

2. 3-WEEK FIT
   - Keeps the most useful field controls beside the full 21-day timeline.
   - Desktop / iPad shows:
     ID, Task Name, Status, Blocker + complete 3-week Gantt.
   - iPhone uses a tighter timeline-focused layout so it remains readable.
   - All hidden fields are still available by tapping Full Detail.

BOTTOM SCHEDULE NAVIGATION
- Table button: returns to the left side of the schedule.
- 3 Weeks button: moves directly to the timeline.
- Slider: controls horizontal position of the whole schedule.

IPAD / IPHONE
- Screens 1100px and below open Schedule in 3-Week Fit automatically.
- iPad is designed to show the complete 3-week timeline beside a compact task list.
- iPhone keeps the task name visible with a compact, swipeable 21-day timeline.
- Full Detail remains available on both devices.
- Touch scrolling and Safari optimizations from V10.1 remain.

ALL V10.2 FEATURES REMAIN
- Supabase login / Forgot Password
- Multiple projects
- Editable Project Name / Location
- Blockers
- Needs Attention
- Baseline vs Current
- Continuous Gantt
- FS / SS / FF dependencies
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
No database migration is required for V10.3.
This version changes the interface/layout only.
