THE UNDERGROUND — SUPABASE AUTH CONNECTION

FILES
- index.html
- style.css
- app.js
- supabase-config.js

SETUP
1. In Supabase, open Project Settings > API Keys.
2. Copy the Project URL.
3. Copy the Publishable key (not a Secret key and not service_role).
4. Open supabase-config.js in your project editor.
5. Replace PASTE_YOUR_PROJECT_URL_HERE and PASTE_YOUR_PUBLISHABLE_KEY_HERE.
6. Save all four files in the same website folder/repository.
7. Open/reload the site using its hosted HTTPS address.

EXPECTED RESULT
- The site restores an existing Supabase session or creates an anonymous guest session.
- The database trigger creates a pseudonymous profile.
- The guest pill and sidebar display the generated username.
- The browser keeps the guest session on that browser/device unless storage is cleared or the user signs out.

IMPORTANT
- Never put a Supabase Secret key or service_role key in browser code.
- This step connects authentication and reads the profile only.
- Posts, comments, votes, and bookmarks remain demo/local until the next integration step.
- For a production launch, configure CAPTCHA/rate limits and review RLS policies and moderation workflows.
