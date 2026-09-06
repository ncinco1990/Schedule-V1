VALBEN Project Dashboard V9.9 — Login + Multi Project

Built from V9.8.

NEW:
- Email/password login using Supabase Auth.
- Projects button in the top toolbar.
- Create multiple independent projects.
- Each project has its own:
  - Schedule / Gantt
  - Activity dates and duration
  - Status and progress
  - FS / SS / FF dependencies
  - No Work dates
  - Calendar
  - Three-Week Lookahead
  - Uploaded project logo
- Project data saved directly to Supabase with Row Level Security.
- Each signed-in user can only read/write their own projects.
- Local browser cache remains available for resilience.
- First project can import the current local V9.8 schedule.

SUPABASE:
Project: yxqemwdekgovyiskmnyw
Tables:
- public.valben_projects
- public.valben_project_states

DEPLOYMENT:
Replace the files in your GitHub repository with this V9.9 package.
If the repository is already connected to Vercel, Vercel will redeploy automatically.

FIRST USE:
1. Open the Vercel website.
2. Create Account with email + password.
3. If Supabase asks for email confirmation, confirm the email and return to Sign In.
4. Create the first project.
5. For an existing V9.8 schedule, check “Use the current local schedule as the starting data”.
6. Sign in with the same account on another device to access the same projects.
