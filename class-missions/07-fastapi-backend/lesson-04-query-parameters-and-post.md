# Lesson 4: Query Parameters and POST

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Add optional query parameters to filter list endpoints.
2. Create a `POST` route that accepts a JSON request body.
3. Use HTTPException for bad requests (empty title, etc.).
4. Test GET with query strings and POST in `/docs`.
5. Explain GET vs POST in your own words.
6. Submit Coursera Module 4 progress and repo evidence.

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

**Required resource — complete Coursera Module 4 (Query Parameter):**

[Module 4 — Query Parameter](https://www.coursera.org/learn/packt-introduction-to-fastapi-and-backend-development-fundamentals-7zg6w)

Focus: query filters, POST bodies, request body models (intro), HTTP exceptions.

**Individual notes:**

```text
Query parameters appear in the URL like...
POST is used when...
HTTPException helps me...
My POST route will accept...
One thing I still do not understand is...
```

## Talk Robin

**Share:** GET vs POST; example query filter; why POST body is not in the URL.

## Group Answer

```text
We use query params to filter because...
POST /projects might...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Students can build `?limit=2` style URLs; know POST sends JSON body in `/docs`.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Extend `GET /projects` with optional query param `limit: int = 10`.
2. Add `POST /projects` accepting JSON `{"title": "...", "description": "..."}`.
3. Append new project to in-memory list; return created object with new `id`.
4. Raise `HTTPException(400)` if `title` is empty or whitespace.
5. Commit: `Add query filter and POST projects`.

## Independent Rebuild

In `/docs`, POST a new project, then GET list with `limit=1` — verify behavior.

**Oral check:** Why should secrets never go in query strings?

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. GitHub link to updated routes
2. Screenshot: POST success + GET with query param in `/docs`
3. Coursera Module 4 progress screenshot
4. Commit history

## Success Criteria

1. Query param limits list correctly.
2. POST adds item and validates empty title.
3. GET and POST both documented in `/docs`.
4. Student can explain GET vs POST orally.

## Common Problems

| Problem | Try first |
|---|---|
| POST body ignored | Use a Pydantic model or dict param — preview Lesson 6. |
| 422 Unprocessable | Match JSON field names to route parameter names. |
| List not updating | Mutate same in-memory list object, not a copy. |

## Fast Track / Support Track

Fast track:

Add `search` query param filtering titles by substring.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
