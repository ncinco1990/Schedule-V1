VALBEN Project Dashboard V11.5 — Minimal Professional + Activity Fix

PRIMARY BUG FIX — ADD ACTIVITY
The most likely cause of "Add Activity does nothing" was an active Schedule filter.

Example:
- Search contains text
- Status = Completed
- Category filter is active
- A new blank Not Started / General activity is created
- The active filter immediately hides the new row

V11.5 FIX:
- + Add Activity clears Search
- Clears Status filter
- Clears Category filter
- Repairs stale/non-sequential IDs before adding
- Creates the next sequential ID
- Opens Schedule
- Focuses the new Task Name field
- Scrolls the new row into view
- Shows confirmation: Activity # added

DATA HARDENING
Legacy/project task rows now receive safe defaults for:
- Task Name
- Start
- Finish
- %
- Status
- Category
- Predecessor
- Link Type
- Blocker
- Baseline dates

MINIMAL PROFESSIONAL DESIGN
The interface was visually simplified without removing functionality:
- Lighter application background
- Cleaner white work panels
- Softer borders
- Reduced shadows
- More consistent button sizes
- More compact Schedule controls
- Cleaner inputs
- Quieter sidebar
- Better mobile toolbar scrolling
- Existing VALBEN/navy professional identity retained

FUNCTIONALITY RETAINED
- Multiple cloud projects
- Supabase login / Forgot Password
- Rolling Lookahead 1–12 weeks
- Gantt alignment
- Add/Delete/Drag activities
- Automatic ID renumbering
- FS / SS / FF dependencies
- Blockers
- Baseline / Variance
- Needs Attention
- Smart Calendar
- No Work dates
- Full Screen
- Zoom
- Excel-style column resizing
- Smart Task Name wrap
- Direct PDF + optional By Norman Cinco watermark
- System Diagnostics / Launch Preflight

NO SUPABASE DATABASE MIGRATION REQUIRED.

UPLOAD TO GITHUB
Replace:
- index.html
- logo.jpg
- README.txt
- TEST_REPORT.txt (optional)


MOBILE / IPAD FIX
- The large global header no longer stays sticky on iPad/iPhone.
- This prevents the header from covering the Schedule + Add Activity controls after the page scrolls to a newly created activity.
- The bottom mobile navigation remains available.
