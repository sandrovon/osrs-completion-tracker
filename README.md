# OSRS Adventure Log

A personal Old School RuneScape progression tracker, designed for steady daily progress towards quest, diary, combat achievement and skill goals.

## Features
- Responsive dashboard with daily task suggestions based on incomplete goals and your time budget
- Checklists for a **starter catalogue** of quests, miniquests, achievement diary milestones and combat achievements
- Links to relevant OSRS Wiki guides
- All 23 current skills, editable manually; optional Wise Old Man player snapshot import
- Local automatic saving, JSON export/import
- No streaks or penalties for skipping days

**Data scope:** This is a working MVP, not yet the complete OSRS task catalogue. Add the remaining content to `src/data.ts` before treating the overall progress percentage as total-game completion. The planner uses simple prerequisites and estimates, not a proven globally optimal route.

## Run locally
```bash
npm install
npm run dev
```

## Deploy
Repository Settings → Pages → Build and deployment → Source: **GitHub Actions**. Push to main to deploy at https://sandrovon.github.io/osrs-completion-tracker/.

## Persistence
Progress is saved to this browser's localStorage. Use Export Backup to save it elsewhere. Cross-device sync / Supabase is not configured yet. Hiscores/Wise Old Man import depends on third-party API browser access and may fail; manual skill editing always works.
