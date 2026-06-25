# Lesson 3: Props and Reusable Components

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Pass data into child components with props.
2. Destructure props in a function component.
3. Build one reusable `Entry` component (Travel Journal pattern) used at least twice with different props.
4. Use JavaScript expressions inside JSX where appropriate.
5. Add a third journal entry during Exit Check without copy-pasting JSX structure.
6. Submit daily evidence listed below.

> **Prerequisite:** [Lesson 2](lesson-02-components-and-styling.md) — ReactFacts page runs with Navbar, Main, and styled components.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** **Do not open Coursera during Guided Practice or Exit Check.**

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** props, passing data parent → child, destructuring — same skills as the Coursera **Travel Journal** project. Lists with `.map()` come in [Lesson 4](lesson-04-lists-map-and-keys.md). Hard-code two `<Entry />` instances below your ReactFacts section — do **not** use `.map()` yet.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra React tutorials during class.

**Required resource — [Learn React, Module 4](https://www.coursera.org/learn/learn-react/home/module/4)** (Bob Ziroll / Scrimba): **Data-Driven React 01 — Understanding Props in React**.

**Self-study cap:** watch only the items below during this block. Total **~26 minutes**. Skip [Module 3](https://www.coursera.org/learn/learn-react/home/module/3) (Test Your Knowledge) unless assigned as homework.

Open [Module 4](https://www.coursera.org/learn/learn-react/home/module/4) on Coursera. Skip [Module 3](https://www.coursera.org/learn/learn-react/home/module/3) (quiz) unless assigned as homework. Use **only** these items:

| Item # | Title | ~Time | When to use |
|---|---|---|---|
| 5 | Props Part 1: Understanding the Concept | 3 min | **Core in class** |
| 6 | Props Part 2: Reusable Components | 2 min | **Core in class** |
| 9 | Props part 4: Passing data into a component | 8 min | **Core in class** |
| 10 | Props part 5: Receiving props in a component | 8 min | **Core in class** |
| 12 | Destructuring props | 5 min | **Core in class** |

**Stop here (~26 min).** Do **not** open [Module 5](https://www.coursera.org/learn/learn-react/home/module/5) item 3 (array `.map()`) — that starts [Lesson 4](lesson-04-lists-map-and-keys.md).

Items 1–4 (Travel Journal setup) and 13–14 are **homework** — optional preview of the `Entry` pattern you build today in Guided Practice.

**Map the course to this project:**

| Course concept | What to build in `react-practice/` |
|---|---|
| `Entry.jsx` | Accepts `country`, `city`, `startDate`, `endDate`, `title`, `description` |
| Two instances below ReactFacts | Different prop values on each entry |
| Destructuring | Clean parameter list in component |

Keep your ReactFacts section from Lesson 2. Add a **Travel Journal** section underneath with two hard-coded entries.

**Individual notes:**

```text
Props are...
Destructuring props looks like...
I reused Entry by passing...
Props flow from parent to child because...
One thing I still do not understand is...
```

**Student output:** Notes + Module 4 progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. Props vs hard-coded text — one example from your journal entry plan
2. One prop that is not a string (for example, dates)
3. Why props only flow parent → child
4. One confusion or question

**Pair summary:** Agree on one prop naming pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
Props make Entry reusable because...
Our group still needs help with...
```

**Teacher checks:**

1. Does the ReactFacts page from Lesson 2 still render?
2. Can students explain props direction (parent → child only)?
3. Can students show destructuring vs `props.title`?
4. Are both entry instances planned with **different** prop values?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

> [!IMPORTANT]
> Close Coursera before this block. Build from the task list and your notes — no videos during hands-on practice.

**Task:**

1. Create `Entry.jsx` accepting props: `country`, `city`, `startDate`, `endDate`, `title`, `description`.
2. Destructure props in the function parameter.
3. Below your ReactFacts section in `App.jsx`, render **two** `<Entry />` instances with different travel data.
4. Confirm both entries look different in the browser.
5. Commit with message: `Add reusable Entry component with props`.

**Mission output:**

- ReactFacts section still visible
- One `Entry` component reused with different props
- Props destructured or accessed clearly
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add a **third** `<Entry />` with new prop values only — no copy-paste of the component's internal JSX.
2. Commit: `Add third Entry via props`.

**Exit prompts:**

```text
My reusable component is...
Props I pass into Entry are...
Props are like function parameters because...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** Read one prop value from parent JSX and explain where it appears in the child.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot showing ReactFacts + two or three different journal entries
2. GitHub link to `Entry.jsx` and usage in App
3. Coursera Module 4 progress screenshot
4. One sentence: "Props are like function parameters because..."

## Success Criteria

You are successful if:

1. ReactFacts section still works.
2. One `Entry` component is reused with different props at least twice.
3. Props are destructured or accessed clearly.
4. Entries show different content from different prop values.
5. You made a meaningful commit on GitHub.
6. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| All entries show same text | Pass different prop values on each instance. |
| `props is undefined` | Check component parameter spelling; use destructuring `{ title }`. |
| Expression error in JSX | Wrap JavaScript in `{ curly braces }`. |
| ReactFacts disappeared | Keep Navbar/Main above the new journal section in App. |

## Fast Track / Support Track

Fast track:

If Module 4 is done early, preview [Lesson 4](lesson-04-lists-map-and-keys.md) journal data array shape only.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
