# M1 Hub 2.0

A responsive React + Vite study tracker for the Medicine (M1) academic programme.

## Academic programme included
- **69 activities across Weeks 1–3**, transcribed from the schedule supplied in this conversation.
- Includes lectures, seminars, tutorials, PBL sessions, symposium, Medicine Grand Rounds, mini-project meetings, and free/missed lecture sessions.
- Week and activity-category filters, plus specialty, search, and progress filters.
- The clinical posting phase (Weeks 4–8) is intentionally not included in this version.

## Study tools
- Independent **Taught**, **Read**, and **Revised** milestones for each activity.
- Activity-specific personal notes and flags.
- Revision queue with a 1, 3, 7, 14-day review rhythm.
- Study streak based on revision activity.
- Dark and improved-contrast light themes.
- JSON export/import for backup and transfer.
- Confirmed reset-progress action clears progress markers, flags, and revision history while preserving notes, theme, and schedule.
- Local-first storage: data remains in the browser on the device where it was entered.

## Compatibility
The app retains the existing `m1hub-v1` localStorage key. On startup, saved records from the previous 42-topic version are matched to the new schedule by normalized activity title (and lecturer where possible), so matching progress and notes are carried forward. The new schedule metadata is applied to all activities. Export a backup before upgrading as a precaution.

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

## Data and privacy
Study data is stored in browser `localStorage`; it is not sent to a server. Export a JSON backup periodically. Clearing browser storage or using another browser/device will not carry progress across automatically.
