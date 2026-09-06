VALBEN Project Dashboard V10.5 — Full Schedule Workspace

BUILT FROM V10.4

FIX: DELETE NO LONGER EXITS FULL SCREEN
- V10.5 no longer depends on the browser-native Fullscreen API.
- Full Screen is now a reliable full-viewport Schedule workspace.
- Browser confirmation dialogs, including Delete Activity, do not remove the Full Screen workspace.
- After deleting an activity, the Schedule keeps its Full Screen state and restores the previous horizontal/vertical scroll position.

FULL SCREEN NOW SHOWS THE COMPLETE SCHEDULE PAGE
The workspace includes:
- Schedule / Gantt title
- Full Detail / 3-Week Fit
- Zoom controls
- Baseline controls
- Add / Clear Activity controls
- Project Name
- Project Location
- Search
- Status filter
- Category filter
- Lookahead start
- Open Lookahead
- Calendar / No Work controls
- Dependency legend
- Task table
- 3-week Gantt
- Bottom unified horizontal navigator

EXITING FULL SCREEN
- The same Full Screen button changes to: Exit Full Screen.
- Press it again to exit.
- The keyboard Escape key also exits.
- The old separate Focus toolbar is no longer needed in the workspace.

IPAD / IPHONE
- Full Screen uses the complete available browser viewport.
- iPad keeps Project Name + Project Location visible and keeps the controls swipeable.
- iPhone keeps Project Name visible and hides Project Location only while in Full Screen to preserve working space.
- Search/filter/calendar controls remain horizontally swipeable.
- iPad/iPhone continue to favor 3-Week Fit.
- Existing zoom controls remain available.

ALL PRIOR FEATURES REMAIN
- Login / Forgot Password
- Multiple projects
- Editable Project Name / Location
- Blockers
- Needs Attention
- Baseline vs Current
- Full Detail / 3-Week Fit
- Unified Schedule scrolling
- Zoom
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
No database migration is required for V10.5.
This release changes the Schedule interface and browser behavior only.
