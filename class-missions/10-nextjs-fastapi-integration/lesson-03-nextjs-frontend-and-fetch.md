# Lesson 3: Next.js Frontend and Fetch

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Follow Udemy Project 1 **Next.js frontend** sections.
2. Run Next.js dev server (typically port 3000).
3. Call FastAPI from the browser or server component using `fetch` (course pattern).
4. Display API data on a page (even if CORS fails — fix in Lesson 4).
5. Submit frontend screenshot and commit.
6. **Independent rebuild:** hand-type minimal Next.js + `fetch` in `full-stack-practice/independent-rebuild/lesson-03/` — [independent-rebuild.md](../shared/independent-rebuild.md).

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

## Entry Point Check

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra playlists during class.

**Required resource — Udemy Project 1 (frontend sections):**

[Learn Next.js and FastAPI](https://www.udemy.com/course/learn-nextjs-and-fastapi-by-building-2-full-stack-apps/) — Next.js setup, pages/app router per course, fetch preview.

**Individual notes:**

```text
Frontend runs on port...
fetch URL is...
Data displays on page as...
If fetch fails, error looks like...
One thing I still do not understand is...
```

## Talk Robin

**Share:** Where `fetch` runs (client vs server in course); what you see if backend is off.

## Group Answer

```text
Frontend needs backend URL because...
JSON becomes UI when...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Both servers can run; students know both URLs.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Complete Udemy frontend steps through first data display attempt.
2. Update `full-stack-practice/README.md` **Frontend** section (install, `npm run dev`, env vars if any).
3. Screenshot page showing data OR clear error (CORS OK for Lesson 4) → `screenshots/frontend-fetch.png`.
4. Commit: `Add Next.js frontend fetch from Udemy project 1`.

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close course videos, notes, AI tools, and follow-along code before this block.

**Required — no materials:** [independent-rebuild.md](../shared/independent-rebuild.md)

1. Close Udemy and follow-along frontend — no copy-paste.
2. In `full-stack-practice/independent-rebuild/lesson-03/`, **hand-type**:
   - Minimal Next.js page (App Router or Pages — your choice from memory)
   - `fetch('http://localhost:8000/...')` to your **lesson-02 rebuild** backend (or mock if backend not running)
   - Display JSON or error text on page
3. Add `REBUILD.md`; commit: `Independent rebuild lesson-03 (no materials)`.

**Oral check:** Explain where `fetch` runs and what URL you used.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. GitHub link to frontend code (follow-along)
2. GitHub link to `independent-rebuild/lesson-03/` + `REBUILD.md`
3. Screenshot of page or DevTools Network tab
4. Commit history

## Success Criteria

1. Next.js dev server runs (follow-along).
2. Frontend attempts real API call (not mock-only) in follow-along.
3. README documents frontend startup.
4. **Rebuild** page hand-typed; `fetch` written from memory.

## Common Problems

| Problem | Try first |
|---|---|
| CORS error in console | Expected until Lesson 4 — capture screenshot as evidence. |
| Wrong API URL | Check `.env.local` or course config for backend base URL. |

## Fast Track / Support Track

Fast track:

Log fetch URL and response status in console for debugging practice.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
