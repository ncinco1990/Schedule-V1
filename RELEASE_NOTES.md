# V13.0 Release Notes — Field Coordination Center

## Added
- Deliveries, concrete, inspections and follow-ups
- One record rendered into Schedule + Day/Week/Month Calendar
- Project/provider/type/Level-Pour/date/status filters
- Today / Confirmations / Overdue indicators
- Editable provider/contact directory
- Concrete CY, mix, truck frequency, pump, hose and pre-inspection fields
- Separate concrete / pump / inspection follow-up activities
- Multiple reminders
- America/New_York timezone and DST wall-time validation
- Calendar drag-handle rescheduling with relative-reminder movement
- Offline cache + queued write fallback
- Share Week: selected activities, team/provider modes, PDF, mail-client draft
- Secure read-only snapshot links
- Public share reader via `?share=<token>`

## Preserved
V12.5 Schedule/Gantt, dependencies, Gantt alignment, Rolling Lookahead, 14-Day Field Lookahead, Calendar, Daily Field Report, project login/multi-project, baseline, blockers and existing PDFs remain.

## Not claimed as operational
- Direct server email: requires configured provider/secret
- Closed-app push notifications: requires Web Push backend/VAPID/service worker
