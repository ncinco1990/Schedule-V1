# V13 Architecture Review

## Source reviewed
Base: VALBEN Project Dashboard V12.5 — 14-Day Field Lookahead.

## Existing application
- Single-file static web application (`index.html`)
- Supabase JS loaded from jsDelivr
- jsPDF loaded from jsDelivr
- Supabase email/password Auth
- `valben_projects` for project identity
- `valben_project_states.state` JSON for Schedule/Gantt, no-work calendar, horizon, Daily Reports and logo
- localStorage caches for resilience
- GitHub → Vercel static deployment

## V13 coordination architecture
Coordination records are normalized into dedicated Supabase tables rather than being duplicated inside the project JSON.
Schedule and Calendar views read the same `coordActivities` collection, so each coordination activity is one record.

### Tables
- `valben_coordination_activities`
- `valben_coordination_providers`
- `valben_coordination_email_log`
- `valben_coordination_shares`

### Security
Activities/providers/email logs are owner-protected with RLS.
Share snapshots are owner-managed; public readers can only retrieve a valid, unrevoked, non-expired token through one RPC that returns the saved snapshot payload.

## Compatibility
No existing Schedule, Gantt, Lookahead, Daily Field Report or project state row is deleted or rewritten.
The V13 database migration is additive.
