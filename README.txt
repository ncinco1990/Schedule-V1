VALBEN Project Dashboard V10.2 — Project Control Essentials

Only three new functions were added to keep the app simple:

1. ACTIVITY BLOCKERS
- Blocker button on every Schedule activity.
- Types: RFI, Inspection, Material, Equipment, Weather, GC Decision, Labor, Other.
- Responsible, Required By and Note fields.
- Saving a blocker marks the activity Blocked.
- Resolve Blocker returns it to the appropriate normal status.
- Dashboard shows the number of open blockers.

2. NEEDS ATTENTION — TODAY + NEXT 7 DAYS
- Replaces the old generic Upcoming Activities panel.
- Prioritizes open blockers, delayed activities, today's starts/finishes and starts in the next 7 days.
- Uses existing schedule data automatically.

3. BASELINE VS CURRENT
- Set Baseline / Update Baseline button in Schedule.
- Stores approved Start and Finish dates for each activity.
- Variance display:
  0d = on baseline
  +Xd = late
  -Xd = ahead
- Baseline variance also appears in the Three-Week Lookahead.
- Baseline is saved per project in the existing Supabase project state.

ALL V10.1 FEATURES REMAIN
- Login and Forgot Password
- Multiple cloud projects
- Editable Project Name / Location
- iPad / iPhone optimization
- Windows desktop layout
- Continuous Gantt
- FS / SS / FF dependencies
- No Work dates
- Calendar
- Three-Week Lookahead
- Print / PDF
- Themes / Dark Background
- Project logo upload

UPLOAD TO GITHUB
Put these files in the ROOT of the same repository:
- index.html
- logo.jpg
- README.txt

Replace the V10.1 files and Commit changes.
If the repository is connected to Vercel, deployment should update automatically.

SUPABASE
No database migration is required for V10.2.
Blockers and Baseline values are stored in the existing project JSON state.
