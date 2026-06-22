# Lesson 8: SQLModel and Dependency Injection

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Define a SQLModel class matching the `projects` table.
2. Use FastAPI dependency injection for database sessions.
3. Replace raw SQL with SQLModel CRUD on at least two routes.
4. Explain how models link database rows to API responses.
5. Update `requirements.txt` with `sqlmodel`.
6. Submit Coursera Module 8 progress and repo evidence.

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

**Required resource — complete Coursera Module 8 (SQLModel):**

[Module 8 — SQLModel](https://www.coursera.org/learn/packt-introduction-to-fastapi-and-backend-development-fundamentals-7zg6w)

Focus: SQLModel models, engine, session, `Depends()` pattern.

**Individual notes:**

```text
SQLModel combines...
Dependency injection means...
Depends(get_session) gives me...
My Project model fields are...
One thing I still do not understand is...
```

## Talk Robin

**Share:** Why ORM beats long SQL strings for small apps; what `Depends` does.

## Group Answer

```text
We inject session so routes...
SQLModel table=True means...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Lesson 7 SQLite working; `pip install sqlmodel` planned.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Add `models.py` with SQLModel `Project` (id, title, description).
2. Add `database.py` with engine, `get_session()` dependency.
3. Refactor `GET /projects` and `POST /projects` to use SQLModel session.
4. Keep Pydantic response models or use SQLModel read schema.
5. Commit: `Refactor projects to SQLModel with Depends`.

## Independent Rebuild

Create project via `/docs`, verify in DB using teacher-provided viewer or print in route (dev only).

**Oral check:** What does `Depends` save you from writing in every route?

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. GitHub link to `models.py`, `database.py`, updated routes
2. Screenshot of `/docs` CRUD still working
3. Coursera Module 8 progress screenshot
4. Commit history

## Success Criteria

1. SQLModel used with dependency injection.
2. Data still persists after restart.
3. requirements.txt includes `sqlmodel`.
4. Code structure is readable (split files).

## Common Problems

| Problem | Try first |
|---|---|
| Session not closing | Use `yield` pattern from course; context manager. |
| Model/table mismatch | Run migration or recreate dev DB with teacher approval. |
| Circular imports | Put models in separate module; import order matters. |

## Fast Track / Support Track

Fast track:

Convert PUT/DELETE from Lesson 5 to SQLModel if not done yet.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
