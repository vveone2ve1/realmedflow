# MEDFLOW — Next.js foundation

This project converts the Library prototype into a real Next.js application and prepares the first live database connection to Supabase.

## Local setup
1. Install Node.js 20+.
2. Copy `.env.example` to `.env.local`.
3. Put the Supabase Project URL and anon/publishable key in `.env.local`.
4. In Supabase SQL Editor, run `supabase/schema.sql`.
5. Run `npm install` then `npm run dev`.
6. Open `/products` to verify that the page reads from the `products` table.

## Security
Never put the Supabase service-role/secret key in `.env.local` variables beginning with `NEXT_PUBLIC_` or in browser code. The anon/publishable key is intended for the client-side Supabase setup; RLS controls what it can read.
