[README.md](https://github.com/user-attachments/files/26350289/README.md)
# 🎓 Flip AE Academy

Your onboarding hub for new Account Executives at Flip.

## Quick Start

```bash
# 1. Install dependencies
npm install

# 2. Start the dev server
npm run dev

# 3. Open http://localhost:3000
```

## Demo Login
The app runs in **demo mode** with mock users. Select any profile to explore:
- **AE view**: Alex Johnson, Sophie Williams, James Chen, Priya Patel
- **Manager view**: Sarah Mitchell, Tom Davies
- **Admin/Enablement view**: You (Enablement)

## Features
- ✅ Module overview with progress tracking
- ✅ Lesson content (text, video, images, Notion embeds)
- ✅ Mini quizzes with 80% pass rate, 3 attempts
- ✅ Force replay on failed attempts
- ✅ Module badges & certifications
- ✅ Manager view (progress, quiz scores, notes, workshop pass/fail)
- ✅ Admin panel (manage modules, lessons, content)
- ✅ Live workshop tracking (self-complete + manager verification)
- ✅ Progress persisted in localStorage

## Adding Content (Admin Panel)
1. Log in as **Enablement**
2. Go to **Manage Content** → select a module
3. Click **Edit** on any lesson
4. Paste your content (Markdown supported) and/or add video URLs

## Production Setup (Supabase)
1. Create a Supabase project at supabase.com
2. Run `supabase/schema.sql` in your SQL editor
3. Copy `.env.local.example` to `.env.local` and fill in your keys
4. Enable Google OAuth in Supabase Dashboard > Auth > Providers

## Brand Colours
Update the primary purple in `tailwind.config.ts`:
```ts
primary: '#7916ff', // ← replace with exact Flip hex
```

## Tech Stack
- **Next.js 14** (App Router)
- **Tailwind CSS** + shadcn-style components
- **localStorage** for data persistence (demo mode)
- **Supabase** ready (schema in `/supabase/schema.sql`)
