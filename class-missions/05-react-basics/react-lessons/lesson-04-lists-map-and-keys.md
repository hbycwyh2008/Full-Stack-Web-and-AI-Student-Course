# Lesson 4: Lists, map, and Keys

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Store journal entry data in a JavaScript array of objects.
2. Render a list of `Entry` components with `.map()`.
3. Assign a stable `key` prop on each list item.
4. Remove hard-coded duplicate `<Entry />` instances from Lesson 3.
5. Add one new entry to the array during Exit Check and confirm the UI updates.
6. Submit daily evidence listed below.

> **Prerequisite:** [Lesson 3](lesson-03-props-and-reusable-components.md) — `Entry` accepts props and renders correctly.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** **Do not open Coursera during Guided Practice or Exit Check.**

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** `.map()`, `key`, and data-driven lists — same as Coursera **Travel Journal: Map Entry components**. State and `useState` come in [Lesson 5](lesson-05-state-and-events.md). Do **not** open Module 8 today.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra React tutorials during class.

**Required resource — [Learn React, Module 5](https://www.coursera.org/learn/learn-react/home/module/5)** (Bob Ziroll / Scrimba): **Data-Driven React 02 — Working with Arrays and Advanced Props**.

**Self-study cap:** watch only the items below during this block. Total **~28 minutes**.

Open [Module 5](https://www.coursera.org/learn/learn-react/home/module/5) on Coursera. Use **only** these items:

| Item # | Title | ~Time | When to use |
|---|---|---|---|
| 3 | Review — array `.map()` | 7 min | **Core in class** |
| 5 | Mapping components | 6 min | **Core in class** |
| 6 | Map quiz! | 4 min | **Core in class** |
| 7 | Travel Journal: Map Entry components | 7 min | **Core in class** |
| 8 | Travel Journal: `key` prop | 4 min | **Core in class** |
| 9 | Travel Journal: Pass object as props | 6 min | **Homework** |

**Stop in-class viewing at item 8 (~28 min).** Item 9 is **homework**. Do **not** open [Module 8](https://www.coursera.org/learn/learn-react/home/module/8) (`useState`) — that is [Lesson 5](lesson-05-state-and-events.md).

**Map the course to this project:**

| Course concept | What to build in `react-practice/` |
|---|---|
| `journalData` array | At least 3 objects with `id`, `country`, `city`, `startDate`, `endDate`, `title`, `description` |
| `.map()` in App or list component | `<Entry key={entry.id} {...entry} />` or explicit props |
| Remove duplicates | Delete hard-coded `<Entry />` lines from Lesson 3 |

**Individual notes:**

```text
I map data to Entry components using...
The key prop is needed because...
Spreading object props means...
Data-driven UI beats copying JSX because...
One thing I still do not understand is...
```

**Student output:** Notes + Module 5 progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. Your array shape — one object example
2. Where `.map()` lives in your file tree
3. What happens if you omit `key`
4. One confusion or question

**Pair summary:** Agree on one `id` field strategy and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
We use .map() instead of copying Entry JSX because...
Our group still needs help with...
```

**Teacher checks:**

1. Does ReactFacts still render above the journal section?
2. Can students point to the array and the `.map()` call?
3. Is each mapped element given a unique `key`?
4. Did anyone delete Lesson 3 hard-coded entries yet?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

> [!IMPORTANT]
> Close Coursera before this block. Build from the task list and your notes — no videos during hands-on practice.

**Task:**

1. Create `journalData.js` (or define the array in `App.jsx`) with at least **three** entry objects. Each needs a unique `id`.
2. Replace hard-coded `<Entry />` instances with:

```jsx
{journalData.map((entry) => (
  <Entry
    key={entry.id}
    country={entry.country}
    city={entry.city}
    startDate={entry.startDate}
    endDate={entry.endDate}
    title={entry.title}
    description={entry.description}
  />
))}
```

Or spread props: `<Entry key={entry.id} {...entry} />` if you understand spreading from Module 5 item 9.

3. Confirm all entries render; ReactFacts section unchanged.
4. Commit with message: `Map journal entries from array with keys`.

**Mission output:**

- Journal list driven by array data
- Each item has a unique `key`
- ReactFacts section still visible
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add one more object to `journalData` and refresh — confirm a fourth entry appears.
2. Commit: `Add fourth journal entry to data array`.

**Exit prompts:**

```text
My array lives in...
.map() returns...
key is set to...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** Why does React need a `key` when mapping?

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot showing ReactFacts + mapped journal list
2. GitHub link showing array + `.map()` + `key`
3. Coursera Module 5 progress screenshot
4. One sentence: "`.map()` helps because..."

## Success Criteria

You are successful if:

1. Journal entries render from an array with `.map()`.
2. Each item has a stable `key`.
3. ReactFacts section still works.
4. No hard-coded duplicate `<Entry />` blocks remain.
5. You made a meaningful commit on GitHub.
6. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Warning about keys | Add `key={entry.id}` on the outermost element in map. |
| Blank list | Check array import/path; log array in Console. |
| Wrong props on cards | Match prop names in array objects to `Entry` destructuring. |
| Duplicate keys | Ensure each `id` is unique in the array. |

## Fast Track / Support Track

Fast track:

If evidence is complete early, preview [Lesson 5](lesson-05-state-and-events.md) `useState` idea only.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
