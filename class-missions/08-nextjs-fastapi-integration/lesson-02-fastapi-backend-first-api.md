# Lesson 2: FastAPI Backend and First API

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Follow Udemy Project 1 to run a **FastAPI** server locally.
2. Test at least one route in `/docs` or browser.
3. Explain JSON response shape the frontend will consume.
4. Store backend code under `full-stack-practice/` (course folder layout OK).
5. Submit `/docs` or API screenshot and commit.
6. **Independent rebuild:** hand-type minimal FastAPI in `full-stack-practice/independent-rebuild/lesson-02/` — [independent-rebuild.md](../shared/independent-rebuild.md).

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

**Required resource — Udemy Project 1 (backend sections):**

Same course: [Learn Next.js and FastAPI — Project 1 backend](https://www.udemy.com/course/learn-nextjs-and-fastapi-by-building-2-full-stack-apps/)

Teacher assigns: FastAPI project creation, routes, models, MongoDB connection intro (as far as class time allows).

**Individual notes:**

```text
My backend runs on port...
The main GET/POST route is...
Request body fields are...
/docs helps me because...
One thing I still do not understand is...
```

## Talk Robin

**Share:** One route you tested; difference from `fastapi-backend/` class missions; MongoDB vs in-memory.

## Group Answer

```text
Backend validates data with...
API returns JSON so frontend can...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Backend starts without crash; student can open `/docs`.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Complete Udemy backend steps through first working API (teacher checkpoint).
2. Add to `full-stack-practice/README.md` section **Backend**:
   - How to start server
   - Main endpoint list
3. Screenshot `/docs` or JSON response → `full-stack-practice/screenshots/backend-api.png` (create folder if needed).
4. Commit: `Add FastAPI backend from Udemy project 1`.

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close course videos, notes, AI tools, and follow-along code before this block.

**Required — no materials:** [independent-rebuild.md](../shared/independent-rebuild.md)

1. Close Udemy and your follow-along backend — do not copy-paste.
2. In `full-stack-practice/independent-rebuild/lesson-02/`, **hand-type** a minimal FastAPI app:
   - `main.py` with `GET /` or `GET /items` returning JSON
   - `requirements.txt` with `fastapi` and `uvicorn`
3. Run `uvicorn` and open `/docs` — screenshot → `screenshots/rebuild-api.png`.
4. Add `REBUILD.md`; commit: `Independent rebuild lesson-02 (no materials)`.

**Oral check:** Walk through your rebuild `main.py` line by line.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. GitHub link to backend files (follow-along)
2. GitHub link to `independent-rebuild/lesson-02/` + `REBUILD.md`
3. API or `/docs` screenshot (follow-along + rebuild)
4. Udemy progress screenshot
5. Commit history

## Success Criteria

1. FastAPI runs locally (follow-along).
2. At least one endpoint returns JSON (follow-along).
3. README documents how to run backend.
4. **Rebuild** FastAPI runs separately; code hand-typed without materials.

## Common Problems

| Problem | Try first |
|---|---|
| MongoDB connection fails | Follow Udemy env vars; teacher may provide shared DB URI for class. |
| Import errors | Activate venv; `pip install -r requirements.txt`. |

## Fast Track / Support Track

Fast track:

Add health route `GET /health` if not in course yet.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
