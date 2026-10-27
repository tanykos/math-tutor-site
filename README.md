# Math Tutor Site

Conversion-focused marketing website for a private math tutor.

## Deployment

- Production URL: [deploy](https://math-tutor-site-gray.vercel.app/)

## Tech Stack

- Next.js 15 (App Router)
- React 19
- TypeScript
- CSS Modules
- ESLint

## Current Status

- ✅ Baseline platform is live on Vercel
- 🔄 Foundation phase: deployment, structure, and localization setup

## Getting Started

Install dependencies:

```bash
npm install
```

Run in development:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

Production build check:

```bash
npm run build
npm run start
```

## Environment Variables

- `.env.local` — local secrets, never committed
- `.env.example` — public template of required keys, no real secret values

## Architecture Decisions

### Why Next.js 15 (not 16)

The project currently runs on the latest Next.js 15 patch.  
This keeps delivery predictable while preserving modern App Router capabilities.

### Why App Router

The website is SEO-critical and expected to evolve with server-side integrations.  
App Router supports this with server-first rendering, scalable route structure, and clean boundaries between server and client logic.

### Why CSS Modules (not Tailwind or CSS-in-JS)

CSS Modules were selected for:

- predictable, component-level style scoping
- no runtime styling cost
- smooth compatibility with server components

This keeps styling maintainable and performant while preserving explicit visual control.

### Why real product context

Building for a real tutoring practice keeps decisions focused on practical outcomes: clarity, trust, lead quality, and conversion.

## Short Roadmap

- [X] Finalize deployment workflow for production and preview releases
- [ ] Establish scalable project structure for localization and server/client boundaries
- [ ] Launch RU/EN localization foundation
