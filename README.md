# Phoneme Activity Builder

Assessment 1 frontend tool for Speech Pathology teachers.

Create phoneme-based **Wordle** and **Word Search** classroom activities, preview them in the browser, then download standalone HTML files that open offline (no Next.js, React, npm, or server required for play).

## Requirements

- Node.js 18+ recommended
- npm

## Setup

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Scripts

| Command | Purpose |
|--------|---------|
| `npm run dev` | Development server (Turbopack) |
| `npm run build` | Production build |
| `npm run start` | Run production build |
| `npm run lint` | ESLint |
| `npm run test:wordle` | Phoneme-unit Wordle checks |
| `npm run test:html` | Standalone HTML generation checks |

## Student details

Before submission, replace placeholders in `src/data/student.js`:

- `STUDENT_NAME`
- `STUDENT_NUMBER`

## Project structure

```
src/
  app/           # Pages: Home, About, Wordle, Word Search, Settings
  components/    # Reusable UI
  data/          # HCE phonemes + word corpus
  lib/           # Wordle / Word Search logic + HTML generators
```

## Notes

- Frontend only — no database, authentication, or backend API
- Generated activities: `phoneme-wordle.html`, `phoneme-word-search.html`
- Theme (light/dark) and layout density preferences
