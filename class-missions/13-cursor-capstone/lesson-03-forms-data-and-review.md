# Lesson 8: Docker, PostgreSQL & Fetching Data

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Complete Udemy **§3 Backend: Setting Up Docker, DB & Fetching Data** (7 lectures · ~51 min).
2. Run **PostgreSQL** (Docker or local) and connect the Kanban app with **Drizzle ORM**.
3. Fetch board data server-side and show **loading** while data loads.
4. Show a clear **error state** when DB is down (stop Docker to demo).
5. Relate fetch/loading/error patterns to **FastAPI fetch** from Phase 01 (`full-stack-practice/`).
6. **Independent rebuild:** hand-type fetch + loading + error in `vibe-coding/independent-rebuild/lesson-08/` — [independent-rebuild.md](../shared/independent-rebuild.md).

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

**Required resource — Udemy §3:**

[Complete Cursor AI — §3 Backend: Docker, DB & Fetching Data](https://www.udemy.com/course/cursorai-nextjs/)

Complete all **7 lectures** in this section.

**Bridge reading (5 min):** Re-read your Phase 01 CORS/fetch notes in `full-stack-practice/FIRST_SUCCESS.md`.

**Individual notes:**

```text
Docker in this course...
Drizzle ORM is...
Server-side fetch happens in...
Loading UI shows when...
Error UI shows when DB...
Same pattern as FastAPI fetch because...
One thing I still do not understand is...
```

## Talk Robin

**Share:** Loading vs error when Postgres stops; how this mirrors FastAPI backend down.

## Group Answer

```text
Without loading users think...
Without error users think...
Capstone will use FastAPI instead of Server Actions for...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Docker/Postgres running; §2 UI complete; `npm run dev` shows board.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Complete §3 with Cursor — database schema + fetch wired to UI.
2. Verify **loading** state during slow fetch (throttle or refresh).
3. Stop DB — capture **error** UI screenshot.
4. Add to `vibe-coding/README.md` section **Phase 01 vs Phase 02 backend**:

   ```text
   Phase 01: Next.js → FastAPI → response
   Phase 02: Next.js → PostgreSQL (course) → capstone: Next.js → FastAPI → RAG
   ```

5. Commit: `Connect Kanban DB fetch with loading and error states`.

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close course videos, notes, AI tools, and follow-along code before this block.

**Required — no materials:** [independent-rebuild.md](../shared/independent-rebuild.md)

1. Close Udemy, Cursor, Docker notes, and `kanban-cursor/`.
2. In `vibe-coding/independent-rebuild/lesson-08/`, **hand-type**:
   - Page that `fetch`es data (real API, or `setTimeout` mock array from memory)
   - **`isLoading`** state + loading UI
   - **`error`** state + error UI (demo by wrong URL or stopped server)
3. Add `REBUILD.md`; commit: `Independent rebuild lesson-08 (no materials)`.

**Oral check:** Show loading → success → error without opening follow-along.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshots: loading + error + success (follow-along)
2. `independent-rebuild/lesson-08/` + `REBUILD.md` + rebuild screenshots
3. `vibe-coding/README.md` backend comparison notes
4. Udemy §3 progress screenshot
5. Commit history

## Success Criteria

1. Data from DB renders on follow-along board.
2. Loading/error visible in follow-along.
3. Student compares to Phase 01 FastAPI fetch.
4. **Rebuild** fetch pattern hand-typed without materials.

## Common Problems

| Problem | Try first |
|---|---|
| Docker permission denied | School IT policy; use local Postgres or teacher shared DB. |
| Connection string wrong | Check `.env`; never commit secrets. |
| Empty board after fetch | Verify migrations/seed data per course. |

## Fast Track / Support Track

Fast track:

Log one SQL query result in README to prove you understand what Drizzle fetched.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
