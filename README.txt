FOUR CORNERS FOOD RECOVERY — PRODUCTION FRONTEND

This version replaces the browser-only demo/localStorage system with Supabase authentication
and the database/RLS structure already created for the project.

SETUP
1. Open config.js.
2. Replace YOUR_SUPABASE_PROJECT_URL with your Supabase Project URL.
3. Replace YOUR_SUPABASE_ANON_KEY with the project's public anon/publishable key.
4. Publish the folder to GitHub Pages.

IMPORTANT
- Never put a Supabase service_role/secret key in this frontend.
- RLS must remain enabled.
- The existing organization UUID is already configured:
  f308345c-a4cb-4375-b825-79c17557aae5
- The current admin profile must exist in Supabase Auth with a matching public.profiles row.

CURRENT LIVE WORKFLOWS
- Supabase email/password authentication
- Profile loading
- Live dashboard metrics
- Donation creation
- Donation listing/filtering
- Organization-level food requests
- Volunteer records
- Organization listing
- Admin pickup scheduling
- Live impact metrics
- Impact report export

SCHEMA NOTES
The existing donations table uses the column name "doner_id" (spelling preserved intentionally).
The app uses the existing schema rather than changing it.

BEFORE PILOT LAUNCH
- Create/verify Supabase Auth email settings.
- Confirm your admin user/profile.
- Test each RLS policy using separate test accounts.
- Add production domain/site URL and redirect URL in Supabase Auth settings.
- Add volunteer onboarding/training process.
- Add photo upload, notifications, maps/GPS, and automated donor/driver notifications as the next feature phase.
