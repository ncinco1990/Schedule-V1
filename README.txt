VALBEN Project Dashboard V12.3 — Delay Report Readability

PRIMARY FIX — SHIFT NOTES
The Shift Notes area was readable in the web form but was being squeezed into a small
PDF field beside Time Out. Long notes were therefore cut and difficult to read.

V12.3 changes the layout:

ON SCREEN
- Shift Notes is a larger 3-line field.
- It automatically grows while you type.
- It can continue growing up to a safe maximum height.
- A scrollbar appears only if the note becomes exceptionally long.
- Affected Work / Delay Details, Weather Notes, Safety Details, Summary, activity notes
  and photo descriptions also use automatic height adjustment.

PDF
- Shift Notes is no longer placed in the small right-side field.
- Prepared By, Time In and Time Out remain on their own row.
- Shift Notes now gets a FULL-WIDTH 544 pt field on the next row.
- The Project & Shift card was increased in height to match the form layout.
- Shift Notes can use multiple lines.

OTHER PDF READABILITY FIXES
- Added adaptive text fitting for report fields.
- The PDF first tries the normal font size.
- If a note is longer, the font is reduced slightly within safe limits.
- If content is still too long, the final visible line receives an ellipsis instead of
  being silently cut.
- Daily Activities use adaptive text fitting.
- Additional Daily Activities use adaptive text fitting.
- Daily Summary supports up to 6 fitted lines.
- Photo descriptions use adaptive fitting instead of raw 4-line clipping.

RETAINED
- Smart Photo Fit for portrait/landscape evidence
- Operator / Bodega / Carpenter Helper / Crane manpower
- Crane Operator Time In / Out
- Delay Category and Responsible Party
- No Next Action box
- Direct data-driven PDF
- Optional watermark
- Report history and project sync

No Supabase migration is required.
