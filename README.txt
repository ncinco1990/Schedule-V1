VALBEN Project Dashboard V12.2 — Smart Photo Fit

PRIMARY UPDATE
Daily Field Report / Delay Report photo handling was optimized for both horizontal and vertical images.

SCREEN / FORM
- Weather / radar evidence photo uses Smart Fit.
- All 4 site photo slots use Smart Fit.
- Portrait photos remain portrait.
- Landscape photos remain landscape.
- Square photos remain square.
- Photos are centered automatically.
- The full image is shown with object-fit: contain.
- No automatic crop.
- No stretching.
- Orientation badge identifies PORTRAIT / LANDSCAPE / SQUARE.

PDF
- The PDF no longer stretches photos to fill a fixed rectangle.
- jsPDF reads the real image width/height.
- Each image is scaled proportionally to fit inside its PDF frame.
- Horizontal photos use the available width.
- Vertical photos use the available height.
- Empty space is centered with a neutral background rather than cropping evidence.

PHOTO QUALITY
- Compression max side increased from 720 px to 1200 px.
- JPEG quality increased from 0.58 to 0.72.
- High-quality canvas smoothing enabled.
- 20 MB original-file safety limit retained.

ALL V12.1 DAILY REPORT FEATURES REMAIN
- Operator manpower
- Warehouse / Bodega
- Carpenter Helper
- Crane manpower
- Crane Operator Time In / Out
- Delay fields
- Weather evidence
- Daily activities
- Safety / RFI
- Photo record
- Generated Daily Summary
- Direct PDF
- Optional By Norman Cinco watermark

No Supabase migration is required.
