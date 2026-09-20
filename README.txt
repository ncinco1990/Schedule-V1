VALBEN Project Dashboard V12.0 - Daily Field Report

NEW SECTION
Daily Field Report has been integrated into the Project Dashboard under Reports.

SOURCE WORKFLOW
The section follows the VALBEN 3-page report structure:
01 Project & Shift
02 Average Manpower
03 Weather & Lost Time
04 Daily Activities
05 Safety, Site Conditions & Pending Information
06 Photo Record

V12 IMPROVEMENTS
- Structured delay category, responsible party and next action
- Automatic manpower total
- 10 default activity lines + up to 20
- Status per activity
- Weather evidence photo
- Four site photos with descriptions
- Browser-side photo compression for project sync
- Multiple saved reports per project
- Automatic/editable report number
- Daily summary generator + copy
- Direct jsPDF report output (not a screenshot)
- Optional By Norman Cinco watermark
- Responsive desktop / iPad / iPhone layout

PROJECT STORAGE
Daily reports are stored inside the existing valben_project_states.state JSON for the active project. No Supabase database migration is required. Photos are compressed before storage.

UPLOAD
Replace in the repository root:
- index.html
- logo.jpg
- README.txt
- TEST_REPORT.txt (optional)

TEST STATUS
V12 passed static JavaScript/DOM checks and Chromium smoke tests at Desktop (1440x1000), iPad (1024x768) and iPhone (390x844) layouts. See TEST_REPORT.txt for details. External Supabase/jsPDF services were stubbed during browser smoke tests to avoid modifying live production data.
