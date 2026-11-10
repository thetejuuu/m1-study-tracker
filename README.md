# M1 Hub

A responsive React + Vite study tracker for the Medicine (M1) posting.

## Features
- 42 teaching topics extracted from the supplied M1 lecture schedule.
- Independent **Taught**, **Read**, and **Revised** milestones.
- Search, specialty filtering, and progress filtering.
- Dark and light themes.
- Topic-specific personal notes and flagged topics.
- Revision queue with a simple 1, 3, 7, 14-day review rhythm.
- Study streak based on revision activity.
- JSON export/import for backup and transfer.
- Local-first storage: progress remains in the browser on the device where it was entered.

## Run locally
Requires Node.js 18+.

```bash
npm install
npm run dev
```

Open the local URL printed by Vite.

## Production build
```bash
npm run build
npm run preview
```

## Deploy to Vercel
1. Push this folder to a GitHub repository.
2. Import the repository in Vercel.
3. Framework preset: **Vite**.
4. Build command: `npm run build`.
5. Output directory: `dist`.

No environment variables are required.

## Important data note
The topic titles, lecturers and schedule dates are transcribed from the provided M1 lecture schedule as extracted for this tracker. Where a lecturer was not specified, that is stated. Review the list against your department's latest amended timetable before relying on dates. The app excludes seminars, PBLs, grand rounds, clinical activities and non-teaching periods, per the project brief.

## Data and privacy
Study data is stored in the browser's `localStorage`; it is not sent to a server. Export a JSON backup periodically. Clearing browser storage or using another browser/device will not carry progress across automatically.
