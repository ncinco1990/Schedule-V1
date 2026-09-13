VALBEN Project Dashboard V11.4 — Launch Candidate

PURPOSE
This release is a stabilization and launch-readiness pass over V11.3.

FIXES
1. PLANNING HORIZON PROJECT SAVE
- Fixed an important V11.3 issue where the selected Rolling Lookahead week count was stored locally but was not included in the active project's Supabase JSON state.
- V11.4 includes horizonWeeks in currentProjectState().
- Switching devices/projects can now restore the saved 1–12 week horizon from project state.
- Older projects without horizonWeeks still default safely to 3 weeks.

2. SYSTEM DIAGNOSTICS
- Fixed a false Modal Layer failure when Schedule was not in Full Screen.
- Diagnostics now correctly treats the normal Schedule layer as 0 and Full Screen as the elevated workspace.
- Added checks for:
  - Planning horizon rendered vs configured
  - Project horizon included in save state
  - PDF engine availability

3. LAUNCH PREFLIGHT
Guide → System Diagnostics → Launch Preflight

Checks:
- Supabase browser library
- jsPDF library
- Core Schedule elements
- All 8 Blocker types
- Planning horizon range
- Gantt row / bar counts
- Project-state horizon persistence

4. PDF STABILITY
- Added a generation lock so double-clicking the watermark choice cannot launch two simultaneous PDF generations.

TESTED WORKFLOWS
- JavaScript syntax
- HTML ID uniqueness
- DOM reference integrity
- 12-activity Schedule render
- Gantt row count / bar count
- 1–12 week Rolling Lookahead controls
- Blocker type selection + save
- Smart Calendar with no task names in day cells
- Direct PDF generation path
- Activity reorder + dependency ID remapping
- Long Task Name wrapping
- System Diagnostics
- Desktop layout
- iPad-sized layout
- iPhone-sized layout

IMPORTANT
The browser app still depends on:
- Supabase service availability / valid project credentials
- jsDelivr access for Supabase JS and jsPDF libraries
- Vercel/GitHub deployment being correct

No Supabase database migration is required for V11.4.

UPLOAD TO GITHUB
Replace in the repository root:
- index.html
- logo.jpg
- README.txt
- DEBUG_REPORT.txt (optional)
