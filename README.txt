JF AGRO CLOUD APP - STARTER RELEASE

This release replaces the old device-only PIN login with Supabase Auth and reads live data from the Supabase project configured in www/index.html.

Included and connected:
- Supabase email/password sign-in
- Profile/role/active account check
- RLS-protected dealer directory
- Product list
- Sales and collection registers
- Admin-only dealer creation
- Team profile and dealer assignment count overview
- Responsive web/PWA layout

Important:
- Only the Supabase URL and publishable key are included. Never add a secret/service_role key to browser or Android code.
- This is the first cloud-connected release, not the finished full business system. Sales invoice entry, payment entry, stock posting, assignment editing UI, offline sync/conflict handling, and comprehensive bilingual translations still need implementation and testing before production use.
- The database RLS policies remain the security boundary. Do not disable RLS or expose secret keys.
- Open www/index.html through a local web server or deploy the www folder to HTTPS hosting. Supabase JS loads from jsDelivr CDN, so internet is required for sign-in.
- For Android, use Capacitor and build from this project; the zip does not contain a signed APK.

Copyright: © All Rights Reserved — Zahirryhan Shakib.
