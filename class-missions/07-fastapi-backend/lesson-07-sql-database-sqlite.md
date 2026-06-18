# Lesson 7: SQL Database with SQLite

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain why persistent storage replaces in-memory lists.
2. Connect FastAPI to a SQLite database file.
3. Insert and retrieve rows with raw SQL or course-patterns from Module 7.
4. Keep projects data after server restart.
5. Add `sqlite` file pattern to `.gitignore` if using local dev DB (or commit empty seed — teacher choice).
6. Submit Coursera Module 7 progress and repo evidence.

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

**Required resource — complete Coursera Module 7 (SQL Database):**

[Module 7 — SQL Database](https://www.coursera.org/learn/packt-introduction-to-fastapi-and-backend-development-fundamentals-7zg6w)

Focus: SQLite connection, INSERT/SELECT, primary keys, integrating DB with routes.

**Individual notes:**

```text
In-memory data is lost when...
SQLite stores data in...
Primary key means...
My database file will be named...
One thing I still do not understand is...
```

## Talk Robin

**Share:** When AI handbook data needs a database vs files; one SQL concept from video.

## Group Answer

```text
We move from list to DB because...
SELECT is used when...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Lesson 6 complete; students understand SQL as structured tables.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Create `database.db` (or `app.db`) via init script or first route startup.
2. Create `projects` table: `id`, `title`, `description`.
3. Refactor `GET /projects` and `POST /projects` to read/write SQLite.
4. Restart server — confirm data persists.
5. Update README: how DB is created, file location.
6. Commit: `Persist projects in SQLite`.

## Independent Rebuild

Add two projects, restart uvicorn, verify list still has both.

**Oral check:** What is lost if we only use a Python list?

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. GitHub link to DB init / route changes
2. Screenshot: data survives server restart (before/after or terminal + `/docs`)
3. Coursera Module 7 progress screenshot
4. Commit history

## Success Criteria

1. SQLite stores projects across restarts.
2. GET/POST still work via `/docs`.
3. README documents database file.
4. No SQL credentials in repo (SQLite is local file).

## Common Problems

| Problem | Try first |
|---|---|
| Database locked | One connection at a time; close cursors. |
| Empty after restart | Writing to wrong file path; use absolute path from project root. |
| Table missing | Run CREATE TABLE on startup or migration script once. |

## Fast Track / Support Track

Fast track:

Add simple seed data script `seed.py` for demo projects.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
