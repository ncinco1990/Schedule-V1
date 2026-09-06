VALBEN Project Dashboard V10.1 — Mobile iPad/iPhone + Login Logo Fix

FIXED
- VALBEN Construction logo now appears directly on the Sign In screen.
- The Sign In logo remains the VALBEN company logo and is not replaced by a project's uploaded logo.
- Removed duplicate embedded default-logo images from index.html.
- logo.jpg is now the default asset, reducing initial page size and improving mobile loading.

IPAD / IPHONE OPTIMIZATION
- Touch-friendly bottom navigation for Dashboard, Schedule, Calendar, Lookahead, Print, Appearance and Guide.
- Compact responsive header.
- Header action buttons can be swiped horizontally.
- Schedule supports smooth horizontal and vertical touch scrolling.
- Desktop sticky task-pane behavior is disabled on smaller touch layouts for smoother Safari scrolling.
- iPhone inputs use 16px text to prevent Safari automatic zoom.
- Calendar stays readable with a swipeable seven-column layout on narrow screens.
- Lookahead and Print Preview support touch scrolling.
- Project, Account and Password Recovery dialogs adapt to mobile.
- iPhone safe-area spacing is included.
- Windows desktop layout remains unchanged above 1100px.

ALL V10.0 FEATURES REMAIN
- Supabase login.
- Forgot Password.
- Multiple cloud projects.
- Editable Project Name and Project Location.
- Gantt and FS/SS/FF dependencies.
- No Work dates.
- Calendar workload.
- Three-Week Lookahead.
- Print/PDF.
- Themes and Dark Background.
- Project logo upload.

DEPLOYMENT
Upload these three files to the ROOT of the same GitHub repository:
- index.html
- logo.jpg
- README.txt

Replace the old files and Commit changes. Vercel should redeploy automatically.

IMPORTANT
Keep logo.jpg in the same folder as index.html. The login screen uses it directly.
