# Phoneme Activity Builder

A simple website for **Speech Pathology teachers**.

You can build two classroom games:

1. **Phoneme Wordle** — guess a word made of speech sounds (phonemes)
2. **Phoneme Word Search** — find phoneme words in a grid

After you build a game, you can **download an HTML file** and open it in any browser — even without internet, and without installing this project again.

---

## Student details

| Field | Value |
|--------|--------|
| **Name** | Ankan Das |
| **Student ID** | 22018897 |
| **Assessment** | Assessment 1 – Phoneme Activity Builder |

---

## What you need before starting

This project uses **Node.js** (not Python).

### Step A — Install Node.js

1. Go to: https://nodejs.org/
2. Download the **LTS** version
3. Install it (keep the default options)
4. Restart your computer if asked

### Step B — Check it worked

Open **Terminal** (Mac) or **Command Prompt / PowerShell** (Windows) and type:

```bash
node -v
npm -v
```

You should see version numbers (for example `v20.x.x` and `10.x.x`).

More detail is also in `requirements.txt`.

---

## How to run the project (easy steps)

### 1. Open the project folder in a terminal

Example (Windows):

```bash
cd "F:\My Assignments & Projects\phoneme-activity-builder"
```

Use your own folder path if it is different.

### 2. Install the project packages (first time only)

```bash
npm install
```

Wait until it finishes. This downloads everything listed in `package.json` / `requirements.txt`.

### 3. Start the website

```bash
npm run dev
```

### 4. Open it in your browser

Go to:

**http://localhost:3000**

You should see the Phoneme Activity Builder home page.

### 5. Stop the website

In the terminal, press:

**Ctrl + C**

---

## What each page does

| Page | What it is for |
|------|----------------|
| **Home** | Short introduction and links to the games |
| **Wordle** | Build and preview a phoneme Wordle game, then download HTML |
| **Word Search** | Build and preview a phoneme word search, then download HTML |
| **About** | Project info and student details |
| **Settings** | Light / dark mode and layout spacing |

---

## How to use Wordle (quick guide)

1. Open **Wordle**
2. Choose or build target phoneme words
3. Try the live preview on the right
4. Click **Generate HTML** to download `phoneme-wordle.html`
5. Open that file in Chrome/Edge/Firefox to play offline

---

## How to use Word Search (quick guide)

1. Open **Word Search**
2. Set rows/cols and randomize (or edit) the word list
3. Click **Generate Puzzle**
4. Play on the right side (drag to select words)
5. Click **Generate HTML** to download `phoneme-word-search.html`
6. Open that file in a browser to play offline

---

## Useful commands

| Command | Meaning |
|---------|---------|
| `npm install` | Install everything needed to run the app |
| `npm run dev` | Start the app for development |
| `npm run build` | Build a production version |
| `npm run start` | Run the production version |
| `npm run lint` | Check code style |
| `npm run test:wordle` | Run Wordle tests |
| `npm run test:html` | Test standalone HTML files |

---

## Project folders (simple map)

```
phoneme-activity-builder/
├── requirements.txt   ← what you need to install first
├── README.md          ← this guide
├── package.json       ← Node packages
└── src/
    ├── app/           ← website pages
    ├── components/    ← buttons, games, keyboard, etc.
    ├── data/          ← phonemes, words, student name/ID
    └── lib/           ← game logic + HTML download code
```

---

## Important notes

- This is a **frontend-only** project (no login, no database, no backend server for saving users).
- Downloaded game HTML files work **offline**.
- If something fails, usually the fix is:
  1. Make sure Node.js is installed
  2. Run `npm install` again
  3. Run `npm run dev` again
  4. Open http://localhost:3000

---

## Need help?

If the site does not open:

- Check that `npm run dev` is still running in the terminal
- Check you are using the correct address: `http://localhost:3000`
- Make sure no other app is already using port 3000
