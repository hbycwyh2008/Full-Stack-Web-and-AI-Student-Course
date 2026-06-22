# Lesson 9: AsyncIO in FastAPI

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain sync vs async routes in plain language (waiting on I/O).
2. Convert at least one route to `async def`.
3. Use `await` with a simulated slow operation (e.g. `asyncio.sleep` or httpx call preview).
4. Connect async to future LLM API calls (course Phase 8).
5. Keep `/docs` working for async routes.
6. Submit Coursera Module 9 progress and repo evidence.

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

**Required resource — complete Coursera Module 9 (AsyncIO):**

[Module 9 — AsyncIO](https://www.coursera.org/learn/packt-introduction-to-fastapi-and-backend-development-fundamentals-7zg6w)

Focus: `async def`, `await`, concurrency for I/O-bound work, FastAPI async handlers.

**Individual notes:**

```text
Async helps when the server is waiting for...
await means...
LLM API calls are slow because...
I will make ___ route async because...
One thing I still do not understand is...
```

## Talk Robin

**Share:** Why blocking the server is bad during OpenAI calls; one async example from video.

## Group Answer

```text
POST /ask should be async when...
asyncio.sleep simulates...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Students know `async def` syntax; difference from regular `def`.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Change `POST /ask` to `async def`.
2. Add `await asyncio.sleep(1)` before stub answer (simulate LLM latency).
3. Add comment in code: `# Phase 8: replace sleep with real API call`.
4. Optional: add `GET /health/async` returning same as health with async handler.
5. Update README: one bullet on async and future AI integration.
6. Commit: `Make ask endpoint async with simulated delay`.

## Independent Rebuild

Call `/ask` in `/docs` — notice ~1s delay. Explain orally why real LLM calls need async.

**Oral check:** What is the server doing during `await`?

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. GitHub link to async route changes
2. Screenshot of `/ask` response after delay
3. Coursera Module 9 progress screenshot
4. README bullet on async + Phase 8
5. Commit history

## Success Criteria

1. At least one route uses `async def` and `await`.
2. `/docs` still executes route successfully.
3. README mentions Phase 8 LLM connection.
4. Student explains sync vs async simply.

## Common Problems

| Problem | Try first |
|---|---|
| Forgot await | Error on coroutine — add `await`. |
| Mixed sync DB in async route | For this lesson, stub `/ask` only; DB routes can stay sync. |
| import asyncio | Add at top of `main.py`. |

## Fast Track / Support Track

Fast track:

Read Module 10 video titles; do not install PostgreSQL until Lesson 10.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
