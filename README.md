# LearnAI — Personalized AI Learning Assistant

A hackathon-ready full-stack starter implementing the core learning-gap loop with Next.js, TypeScript, Prisma, PostgreSQL, and a modular AI service.

## Included
- Premium landing page
- Student dashboard
- PostgreSQL + Prisma schema
- Demo seed data
- Diagnostic assessment with answer persistence
- Explainable learning gaps
- Mastery/gap engine foundation
- AI tutor endpoint with mock mode
- Adaptive-practice UI
- Personalized roadmap
- REST route handlers
- Responsive UI

## Run locally

1. Install Node.js 20+ and PostgreSQL.
2. Copy `.env.example` to `.env` and set `DATABASE_URL` + `NEXTAUTH_SECRET`.
3. Run:

```bash
npm install
npx prisma generate
npx prisma migrate dev --name init
npm run prisma:seed
npm run dev
```

Open http://localhost:3000

Demo data is pre-seeded. The current starter intentionally uses a fixed demo user in several API routes to make judging frictionless; replace that with `requireUser()` + session-based user IDs before production deployment.

## AI
Set `AI_PROVIDER=mock` for an API-key-free demo. When you wire OpenAI/Gemini, keep provider calls inside `lib/ai` and the `/api/ai/*` routes.
# py.learn
