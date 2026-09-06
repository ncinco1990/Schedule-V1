VALBEN Project Dashboard V9.8 — Web Hosted + Supabase Sync

Architecture:
- FRONTEND: deploy index.html + logo.jpg to a static web host such as Vercel.
- BACKEND: Supabase Edge Function + Postgres cloud state.

Why:
Supabase Edge Functions intentionally rewrite HTML responses to text/plain.
They are designed for APIs, not for serving complete web pages.

V9.8 changes:
- Cloud Sync API points directly to the Supabase backend:
  https://yxqemwdekgovyiskmnyw.supabase.co/functions/v1/valben-dashboard?api=state
- The frontend can now be hosted on any normal static host without breaking sync.
- Guide / Version Notes updated to V9.8.
- All V9.7 scheduling, dependencies, Gantt colors, calendar, themes, Dark Mode,
  lookahead, print preview and cloud-sync UI remain.

Deployment target:
Upload index.html and logo.jpg to the frontend web host.
