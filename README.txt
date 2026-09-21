VALBEN Project Dashboard V12.1 - Daily / Delay Report Optimized

DAILY / DELAY REPORT PDF
- Rebuilt to visually match the application form.
- Uses the same numbered sections, navy step badges, rounded white cards, light field boxes and section order.
- PDF remains data-driven, not a screenshot.

MANPOWER ADDED
- Operator
- Warehouse / Bodega
- Carpenter Helper
- Crane

CRANE OPERATOR SHIFT
- Operator Time In
- Operator Time Out
- Stored with each Daily Field Report and included in the PDF manpower section.

REMOVED
- Delay Next Action field
- Safety/Pending Next Action field
- PDF no longer prints either Next Action box.

COMPATIBILITY
- Existing V12.0 reports load normally.
- Older Next Action values may remain in legacy project JSON but are ignored by V12.1 UI/PDF.
- No Supabase schema migration is required because Daily Reports remain inside the existing project JSON state.

TESTS
See TEST_REPORT.txt.
