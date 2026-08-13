# Phoneme Activity Builder

Assessment 1 frontend tool for Speech Pathology teachers.

Create phoneme-based **Wordle** and **Word Search** classroom activities, preview them in the browser, then download standalone HTML files that open offline (no Next.js, React, npm, or server required for play).

## Prerequisites (install first)

See `requirements.txt` for the full list. You need:

1. **Node.js 18+** — download from https://nodejs.org/
2. **npm** — included with Node.js

Check versions:

```bash
node -v
npm -v
```

## How to run this project

1. Open a terminal in the project folder.
2. Install dependencies (required once, or after `package.json` changes):

```bash
npm install
```

3. Start the development server:

```bash
npm run dev
```

4. Open the app in your browser:

[http://localhost:3000](http://localhost:3000)

5. Stop the server with `Ctrl + C` in the terminal.

### Production build (optional)

```bash
npm run build
npm run start
```

Then open [http://localhost:3000](http://localhost:3000).

## Scripts

| Command | Purpose |
|--------|---------|
| `npm install` | Install packages from `package.json` / `requirements.txt` |
| `npm run dev` | Development server (Turbopack) |
| `npm run build` | Production build |
| `npm run start` | Run production build |
| `npm run lint` | ESLint |
| `npm run test:wordle` | Phoneme-unit Wordle checks |
| `npm run test:html` | Standalone HTML generation checks |

## Student details

Configured in `src/data/student.js` (shown in the footer and About page).

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
- Package install uses **npm** (`npm install`), not `pip`
