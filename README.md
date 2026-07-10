# EnhanceMove

A Next.js 14 + Supabase CRM starter for a single-user MVP.

## Stack
- Next.js 14 App Router
- TypeScript
- Tailwind CSS
- Supabase Auth + Postgres + RLS
- Lightweight custom UI primitives inspired by shadcn/ui

## Setup
1. Create a Supabase project.
2. Run `supabase/schema.sql` in the SQL editor.
3. Enable Email/Password and Magic Link auth in Supabase Auth.
4. Add these environment variables to `.env.local`:
   - `NEXT_PUBLIC_SUPABASE_URL`
   - `NEXT_PUBLIC_SUPABASE_ANON_KEY`
   - `SUPABASE_SERVICE_ROLE_KEY`
   - `NEXT_PUBLIC_SITE_URL`
5. Install dependencies:
   - `npm install`
6. Run the dev server:
   - `npm run dev`

## Deployment
- Deploy to Vercel.
- Add the same environment variables in Vercel.
- Point Supabase Auth redirect URLs at the deployed domain.
- Verify signup, login, onboarding, and CRUD flows.

## Branding
- Primary color is defined in `app/globals.css`.
- Change typography in `app/globals.css` if you want a different system stack.
- Keep the layout and spacing tokens intact for a clean CRM feel.
