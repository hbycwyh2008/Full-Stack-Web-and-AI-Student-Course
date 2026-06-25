# Lesson 4: Lists, map, and Keys

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Store list data in a JavaScript array of objects.
2. Render a list of components with `.map()`.
3. Assign a stable `key` prop on each list item.
4. Remove hard-coded duplicate cards from Lesson 3.
5. Add one new item to the array during Exit Check and confirm the UI updates.
6. Submit daily evidence listed below.

> **Prerequisite:** [Lesson 3](lesson-03-props-and-reusable-components.md) — `ProjectCard` accepts props.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** Skip Module 6 (quiz) unless assigned as homework.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** `.map()`, `key`, and data-driven lists. State and `useState` come in [Lesson 5](lesson-05-state-and-events.md). Do **not** open Module 8 today.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra React tutorials during class.

**Required resource — [Learn React, Module 5](https://www.coursera.org/learn/learn-react/home/module/5)** (Bob Ziroll / Scrimba): **Data-Driven React 02 — Working with Arrays and Advanced Props**.

**Self-study cap:** watch only the items below during this block. Total **~30 minutes**.

Open [Module 5](https://www.coursera.org/learn/learn-react/home/module/5) on Coursera. Use **only** these items:

| Item # | Title | ~Time | When to use |
|---|---|---|---|
| 3 | Review — array `.map()` | 7 min | **Core in class** |
| 5 | Mapping components | 6 min | **Core in class** |
| 6 | Map quiz! | 4 min | **Core in class** |
| 7 | Travel Journal: Map Entry components | 7 min | **Core in class** |
| 8 | Travel Journal: `key` prop | 4 min | **Core in class** |

**Stop here (~28 min).** Item 9 (Pass object as props) may continue in Guided Practice. Do **not** open [Module 8](https://www.coursera.org/learn/learn-react/home/module/8) (`useState`) — that is [Lesson 5](lesson-05-state-and-events.md).

**Map the course to this project:**

| Course concept | What to build in `react-practice/` |
|---|---|
| `projects` array | At least 3 objects with `id`, `title`, `description`, `status` |
| `.map()` in App or list component | `<ProjectCard key={p.id} ... />` |
| Remove duplicates | Delete hard-coded cards from Lesson 3 |

**Individual notes:**

```text
I map data to components using...
The key prop is needed because...
Spreading object props means...
Data-driven UI beats copying JSX because...
One thing I still do not understand is...
```

**Student output:** Notes + Module 5 progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. Your array data shape (what fields each object has)
2. Why React warns about missing keys
3. One connection to Phase 3 JavaScript arrays
4. One confusion or question

**Pair summary:** Agree on one array field naming pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
Data-driven UI beats copying many JSX blocks because...
Our group still needs help with...
```

**Teacher checks:**

1. Can students still explain props from Lesson 3?
2. Does each project object have a unique `id` for `key`?
3. Can students return JSX from `.map()` (parentheses or return)?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. Create an array of at least **three** project objects:

```javascript
const projects = [
  { id: 1, title: "...", description: "...", status: "In progress" },
  { id: 2, title: "...", description: "...", status: "Done" },
  { id: 3, title: "...", description: "...", status: "Planned" }
];
```

2. Map to `<ProjectCard key={project.id} title={...} ... />` components.
3. Remove hard-coded duplicate cards from Lesson 3.
4. Confirm three cards render from one array change.
5. Commit with message: `Render project list from array with keys`.

**Mission output:**

- List rendered from array with `.map()`
- Each item has a unique `key`
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add one new project object to the array only.
2. Confirm the UI shows a fourth card without duplicating JSX blocks.
3. Commit: `Add fourth project to array`.

**Exit prompts:**

```text
My array is called...
map returns...
key is set to...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** Explain why `.map()` in React is like a loop in Phase 3 JavaScript.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot of three or more cards from one array
2. GitHub link showing `.map()` and `key` in App or list component
3. Coursera Module 5 progress screenshot
4. One sentence: "Using map in React is like Phase 3 loops because..."

## Success Criteria

You are successful if:

1. List is rendered from an array with `.map()`.
2. Each item has a stable `key`.
3. No duplicate hard-coded cards for the same data.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Warning about keys | Add `key={item.id}` on the outermost element in map. |
| Empty list | Check array name; ensure map **returns** JSX. |
| Same card repeated | Spread or pass different fields from each object. |

## Fast Track / Support Track

Fast track:

If Module 5 is done early, preview [Lesson 5](lesson-05-state-and-events.md) `useState` idea only.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
