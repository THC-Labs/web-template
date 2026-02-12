# Antigravity Context & Rules

## Tech Stack
- **Framework:** Next.js 15+ (App Router).
- **Styling:** Tailwind CSS.
- **Database:** Supabase (PostgreSQL).
- **Language:** TypeScript (Strict).

## Development Rules
1. **Supabase:**
   - Client Components: Import `createClient` from `@/utils/supabase/client`.
   - Server Components/Actions: Import `createClient` from `@/utils/supabase/server`.
   - Never create a client manually.
2. **Data Fetching:** Prefer Server Components. Use async/await.
3. **Styling:** Use Tailwind utility classes. Avoid custom CSS files.
4. **Security:** If modifying `transactions` or `balances`, use `@/utils/crypto` to encrypt payload before DB insertion.

## Project Structure
- `/app`: App Router pages.
- `/components`: Reusable UI.
- `/utils`: Helpers (Supabase, Crypto).
- `/types`: TypeScript interfaces (generated from DB).