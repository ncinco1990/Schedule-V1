VALBEN Project Dashboard V10.4 — Schedule Focus + Zoom

BUILT FROM V10.3

NEW: FULL SCREEN / FOCUS MODE
- Schedule has a new Full Screen button.
- When activated, the rest of the dashboard is hidden and Schedule uses the full browser viewport.
- A compact Focus toolbar stays available with:
  - Full Detail
  - 3-Week Fit
  - Zoom Out
  - Zoom percentage / Reset
  - Zoom In
  - Exit · Esc
- Pressing Escape exits Focus Mode.
- On browsers that support the native Fullscreen API, V10.4 also requests browser fullscreen.
- On iPhone/iPad Safari, CSS Focus Mode remains the reliable fallback even when native fullscreen is unavailable.

NEW: SCHEDULE ZOOM
- Zoom range: 65% to 125%.
- Zoom Out / Reset / Zoom In buttons are available in normal Schedule and Focus Mode.
- Zoom setting is saved in the browser.
- Keyboard shortcuts in Focus Mode:
  Ctrl/Cmd + Plus = zoom in
  Ctrl/Cmd + Minus = zoom out
  Ctrl/Cmd + 0 = reset
  Escape = exit Focus Mode

IPAD / IPHONE
- Focus Mode uses 100% of the available browser viewport.
- iPad/iPhone favor 3-Week Fit when entering Focus Mode.
- Default Focus zoom:
  iPad/tablet: 90% when no custom zoom has been selected.
  iPhone: 80% when no custom zoom has been selected.
- Safe-area spacing is included.
- The Focus toolbar can scroll horizontally on iPad.
- iPhone uses a compact Focus toolbar so the 21-day schedule keeps most of the screen.
- The unified Schedule horizontal scroll from V10.3 remains.

ALL PRIOR FEATURES REMAIN
- Login / Forgot Password
- Multiple projects
- Editable Project Name / Location
- Blockers
- Needs Attention
- Baseline vs Current
- Full Detail / 3-Week Fit
- Unified Schedule scrolling
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
If the repository is connected to Vercel, Vercel should redeploy automatically.

SUPABASE
No database migration is required for V10.4.
This release changes the Schedule interface and browser behavior only.
