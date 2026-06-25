# Lesson 2: Next.js Routing and Layouts

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Create multiple routes with the App Router (`app/` folders).
2. Use a shared `layout.jsx` for header/footer across pages.
3. Link pages with `next/link` (not full page reload).
4. Port one idea from `react-practice/` into a Next page as static or props-based UI.
5. Add nav or footer polish during Exit Check without reopening Coursera.
6. Submit daily evidence listed below.

> **Prerequisite:** [Lesson 1](lesson-01-nextjs-getting-started.md) — `nextjs-practice/` runs with `npm run dev`.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** **Do not open Coursera during Guided Practice or Exit Check.**

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** nested routes, shared layouts, navigation — same skills as the Coursera **PrintForge** routing module. `Link` details and dynamic routes start in [Lesson 3](lesson-03-client-server-and-submission.md). Do **not** open Module 3 today.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra Next.js tutorials during class.

**Required resource — [Learn Next.js, Module 2](https://www.coursera.org/learn/learn-nextjs/home/module/2)** (Scrimba): **Building Your First App with Routing**.

**Self-study cap:** watch only the **Core in class** items below during this block. Total **~27 minutes**.

Open [Module 2](https://www.coursera.org/learn/learn-nextjs/home/module/2) on Coursera. Item numbers **restart at 1 inside each module**.

| Item # | Title | ~Time | When to use |
|---|---|---|---|
| 2 | Challenge — PrintForge Home Page | 5 min | **Core in class** |
| 3 | Challenge — PrintForge About Page | 4 min | **Core in class** |
| 4 | Nested Routes | 5 min | **Core in class** |
| 5 | Layouts part 1 | 5 min | **Core in class** |
| 6 | Layouts part 2 | 5 min | **Core in class** |
| 7 | Challenge — Add Header to PrintForge | 3 min | **Core in class** |
| 8 | Optimizing Fonts | 9 min | **Homework** |
| 9 | Optimizing Images | 10 min | **Homework** |

**Stop in-class viewing after item 7 (~27 min).** Item 1 (PrintForge Challenge Setup) is optional **homework** preview. Items 8–9 are **homework**.

Do **not** open [Module 3](https://www.coursera.org/learn/learn-nextjs/home/module/3) — that is [Lesson 3](lesson-03-client-server-and-submission.md).

**Map the course to this project:**

| Course concept | What to build in `nextjs-practice/` |
|---|---|
| `app/page.jsx` | Home route `/` |
| `app/about/page.jsx` | About route `/about` |
| `app/projects/page.jsx` | Projects list `/projects` |
| `app/layout.jsx` | Shared site title + nav with `Link` |
| From `react-practice/` | Reuse a list or card pattern on `/projects` |

**Individual notes:**

```text
A route in App Router is created by...
layout.jsx wraps pages because...
next/link is better than <a> because...
My planned routes are...
One thing I still do not understand is...
```

**Student output:** Notes + Module 2 progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../shared/talk-robin-rules.md).

**Share:**

1. Your planned routes (Home, About, Projects)
2. One element you will put in `layout.jsx`
3. One pattern from `react-practice/` you might reuse
4. One confusion or question

**Pair summary:** Agree on one shared layout pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
Shared layout helps our site because...
Our group still needs help with...
```

**Teacher checks:**

1. Does Lesson 1 app still run?
2. Can each student draw a simple route map on paper?
3. Do students know the folder → URL rule (`app/about/page.jsx` → `/about`)?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

> [!IMPORTANT]
> Close Coursera before this block. Use your notes and the task list below — no videos during hands-on practice.

**Task:**

1. Add routes:
   - `/` — home (existing `app/page.jsx`)
   - `/projects` — at least three project or journal titles (hard-coded array is fine; reuse data shape from `react-practice/` if helpful)
   - `/about` — short bio or course note
2. Add or update `app/layout.jsx` with site title and nav links using `Link` from `next/link`.
3. Confirm client-side navigation works — clicking nav should **not** full-reload the page.
4. Commit with message: `Add Next.js routes and shared layout`.

**Mission output:**

- At least three routes work via `Link` navigation
- Shared layout visible on all pages
- `/projects` shows list content
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../shared/independent-rebuild.md).

**Exit Check task:**

1. Add a footer line in `layout.jsx` that appears on all pages.
2. Optionally add simple active styling on the current nav link.
3. Commit: `Add footer to shared layout`.

**Exit prompts:**

```text
My three routes are...
layout.jsx is shared because...
Link prevents full reload because...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** Point to the folder that creates `/projects`.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot of two different routes showing shared nav
2. GitHub link showing `app/` structure and `Link` usage
3. Coursera Module 2 progress screenshot
4. One sentence: "Layouts in Next.js are like..."

## Success Criteria

You are successful if:

1. At least three routes work via client navigation.
2. Shared layout is visible on all pages.
3. Projects page shows list content.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| 404 on route | Folder name must match URL; file must be `page.jsx`. |
| Full page reload | Use `import Link from 'next/link'`, not plain `<a href>`. |
| Layout not wrapping page | `layout.jsx` must be in `app/` or the correct segment folder. |
| List empty | Hard-code at least three items in the projects page first. |

## Fast Track / Support Track

Fast track:

If Module 2 and mission evidence are complete early, preview [Lesson 3](lesson-03-client-server-and-submission.md) `'use client'` idea only.

Support track:

- Complete home + one extra route first; add about page if time runs short.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
