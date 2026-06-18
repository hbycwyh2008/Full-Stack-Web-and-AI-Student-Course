# Lesson 3: Path Parameters

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Define path parameters with type hints in FastAPI routes.
2. Explain route order and why specific paths must come before generic ones.
3. Add `GET /items/{item_id}` (or `/projects/{project_id}`) returning JSON.
4. Test multiple path values in `/docs`.
5. Handle invalid input with appropriate HTTP errors (preview).
6. Submit Coursera Module 3 progress and repo evidence.

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

**Required resource — complete Coursera Module 3 (Path Parameter):**

[Module 3 — Path Parameter](https://www.coursera.org/learn/packt-introduction-to-fastapi-and-backend-development-fundamentals-7zg6w)

Focus: dynamic routes, type hints, decorators, simple data storage intro in course videos.

**Individual notes:**

```text
Path parameters look like...
Type hints help FastAPI because...
One example path I will build is...
Route order matters when...
One thing I still do not understand is...
```

## Talk Robin

**Share:** Path vs query parameter (preview); one typed path example; Coursera demo that helped.

## Group Answer

```text
We use {item_id} in the path when...
FastAPI validates types by...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Students can read `{param}` syntax; know difference from query string `?id=`.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Add in-memory list of 3 sample “projects” or “handbook sections” (dicts with `id` and `title`).
2. Add `GET /projects/{project_id}` returning one item or `404` if missing.
3. Add `GET /projects` listing all items.
4. Test in `/docs` with valid and invalid IDs.
5. Commit: `Add path parameter route for projects`.

## Independent Rebuild

Add a new project ID in code only (no Coursera), reload, verify in `/docs`.

**Oral check:** Where does FastAPI read `project_id` from?

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. GitHub link to updated `main.py`
2. Screenshot of `/docs` showing path route tests
3. Coursera Module 3 progress screenshot
4. Commit history

## Success Criteria

1. Path route returns correct JSON for valid IDs.
2. Missing ID returns clear error (404 or HTTPException).
3. List route still works.
4. Code uses type hints on path params.

## Common Problems

| Problem | Try first |
|---|---|
| Always 404 | Check ID type (int vs str) matches your data. |
| Route conflict | Put fixed paths like `/projects/active` before `/projects/{project_id}`. |
| Reload not picking changes | Save file; check terminal for reload message. |

## Fast Track / Support Track

Fast track:

Add optional path param with default using Query in Lesson 4 — preview only.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
