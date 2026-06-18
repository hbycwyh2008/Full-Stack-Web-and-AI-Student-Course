# Lesson 4: Lists, map, and Keys

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Store list data in a JavaScript array.
2. Render a list of components with `.map()`.
3. Assign a stable `key` prop on each list item.
4. Pass object props or spread object props into child components.
5. Commit list rendering with a meaningful message.
6. Submit Module 5 evidence.

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

**Required resource — complete [Learn React Module 5](https://www.coursera.org/learn/learn-react/home/module/5):** Data-Driven React 02 — Arrays and Advanced Props (~1 hour).

**Individual notes:**

```text
I map data to components using...
The key prop is needed because...
Spreading object props means...
One thing I still do not understand is...
```

## Talk Robin

**Share:** your array data shape; why keys matter; one question.

## Group Answer

```text
Data-driven UI beats copying many JSX blocks because...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Phase 3 array/loop skills still accessible; `key` not equal to array index when possible (teacher explains if needed).

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Create an array of at least **three** project objects (`id`, `title`, `description`).
2. Map to `<ProjectCard key={...} ... />` components.
3. Remove hard-coded duplicate cards from Lesson 3.
4. Commit: `Render project list from array with keys`.

## Independent Rebuild

Add one project to the array and confirm UI updates with one code change. Commit.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot of three+ cards from one array
2. GitHub link showing `.map()` and `key` in App or list component
3. Coursera Module 5 progress screenshot
4. One sentence: “Using map in React is like Phase 3 loops because...”

## Success Criteria

1. List rendered from array with `.map()`.
2. Each item has a `key`.
3. No duplicate hard-coded cards for the same data.
4. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Warning about keys | Add unique `key={item.id}`. |
| Empty list | Check array name and map return (return JSX). |

## Fast Track / Support Track

Fast track:

Optional: complete Module 6 quiz as homework for certificate.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
