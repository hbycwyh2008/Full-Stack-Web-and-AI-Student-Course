# Lesson 7: useEffect and Fetch in React

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain why data fetching in React often uses `useEffect`.
2. Fetch JSON on button click with `async`/`await` inside a handler (Phase 3 skill).
3. Optionally preview `useEffect` for load-on-mount (Module 13).
4. Show loading and error states in the UI.
5. Document how this connects to a future FastAPI call in README.
6. Submit Module 12–13 progress (+ Module 10 API scrims if assigned).

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

**Required resource:**

1. Complete [Learn React Module 12](https://www.coursera.org/learn/learn-react/home/module/12): Side Effects 01 (~27 min).
2. Complete [Module 13](https://www.coursera.org/learn/learn-react/home/module/13): `useEffect` and fetch (~1 hour).

Optional if time: Module 10 API integration scrims (skip Sound pads challenges).

**Individual notes:**

```text
useEffect runs when...
fetch in React is similar to Phase 3 because...
Loading state matters because...
This will connect to our AI app when...
One thing I still do not understand is...
```

## Talk Robin

**Share:** sync vs async in UI; when to use button fetch vs `useEffect`; one question.

## Group Answer

```text
Our React app will call a backend later by...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Phase 3 `async/await` understood; CORS explained for public API vs local backend later.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Add button “Load quote” that `fetch`es `https://jsonplaceholder.typicode.com/todos/1` and displays `title` in state.
2. Show “Loading...” while fetching; show error message on failure.
3. Add to `react-practice/README.md` one bullet: “Next step: call FastAPI from Next.js in course Phase 6–7.”
4. Commit: `Add fetch demo with loading state in React`.

## Independent Rebuild

Change endpoint to `/users/1` and display `name`. Optional: one `useEffect` on mount — explain difference from button fetch.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot after successful fetch
2. GitHub link to fetch handler + loading UI
3. Coursera Module 12–13 progress screenshot
4. README bullet about FastAPI / Next.js next step

## Success Criteria

1. Fetch works with loading feedback.
2. Error handled without crashing app.
3. README mentions connection to full-stack course.
4. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| `Failed to fetch` | Check URL; school network; use jsonplaceholder. |
| Infinite re-fetch loop | Check `useEffect` dependency array (teacher help). |

## Fast Track / Support Track

Fast track:

Complete `react-practice/README.md` Phase 4 summary section before Lesson 8.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
