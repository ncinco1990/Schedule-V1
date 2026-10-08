# VALBEN V13 Deployment

## Current hosting method
The application remains a static frontend intended for the same GitHub → Vercel deployment used by the current Schedule app.

Upload these files to the repository root:
- `index.html`
- `logo.jpg`
- `logo_field.jpg` (used by the Field Lookahead if present)

Vercel should redeploy automatically when the connected repository receives the commit.

## Data persistence
Existing Schedule/Gantt, Rolling Lookahead and Daily Field Report data remain in:
- `valben_projects`
- `valben_project_states.state`

V13 Field Coordination uses separate Supabase tables:
- `valben_coordination_activities`
- `valben_coordination_providers`
- `valben_coordination_email_log`
- `valben_coordination_shares`

This avoids rewriting or migrating the existing project JSON.

The final V13 security/share migration was applied to the current Supabase project. The SQL is included under `supabase/migrations/` for backup/redeployment.

## Read-only share links
Operational in V13 against the configured Supabase project.
A link contains a random token and reads only a saved snapshot through `valben_get_coordination_share`.
It does not expose editing or the rest of the project.

## Email
V13 does NOT claim direct email sending.
The built-in `Prepare Email` action opens the user's email client and logs `client_opened`.

To enable true server-side sending:
1. Deploy `supabase/functions/send-coordination-email/index.ts` as an authenticated Edge Function.
2. Configure Supabase secrets:
   - `RESEND_API_KEY`
   - `COORDINATION_FROM_EMAIL`
3. Verify the sender domain with the selected email provider.
4. Add the direct-send button only after a successful production send test.

Never put the email provider secret in `index.html`, GitHub public files, or browser JavaScript.

## Notifications
In-app reminders and browser Notification API alerts are implemented while the browser/app session is running.
Closed-app push is NOT active.

To support closed-app push you need:
- service worker push handling,
- VAPID keys stored server-side,
- a push-subscription table tied to the authenticated user/device,
- a scheduled backend/Edge Function that finds due reminders and sends Web Push messages.

Do not treat the current browser alert button as closed-app push.

## Timezone
Coordination uses `America/New_York`.
Local date/time is converted to UTC before storage and round-tripped through `Intl.DateTimeFormat`.
Invalid wall times during the daylight-saving spring transition are rejected instead of silently shifting.
