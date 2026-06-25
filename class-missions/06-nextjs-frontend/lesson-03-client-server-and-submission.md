# Lesson 3: Client vs Server Components and Unit Submission

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain client vs server components in beginner terms.
2. Mark an interactive component with `'use client'` and use `useState` in Next.js.
3. Add one dynamic route segment (for example `app/projects/[id]/page.jsx`).
4. Complete front-end checkpoint evidence in repo and Notion.
5. Add one UI improvement during Exit Check without reopening Coursera.
6. Submit all unit evidence listed below.

> **Prerequisite:** [Lesson 2](lesson-02-nextjs-routing-and-layouts.md) — routes and shared layout work.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** **Do not open Coursera during Guided Practice or Exit Check.**

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** `Link` navigation, client vs server components, dynamic routes — same skills as Coursera **PrintForge** Module 3. This lesson is the **unit checkpoint** for React + Next.js practice folders.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra Next.js tutorials during class.

**Required resource — [Learn Next.js, Module 3](https://www.coursera.org/learn/learn-nextjs/home/module/3)** (Scrimba): **Components, Links & Dynamic Pages**.

**Self-study cap:** watch only the **Core in class** items below during this block. Total **~22 minutes**.

Open [Module 3](https://www.coursera.org/learn/learn-nextjs/home/module/3) on Coursera. Item numbers **restart at 1 inside each module**.

| Item # | Title | ~Time | When to use |
|---|---|---|---|
| 1 | Links in Next.js | 4 min | **Core in class** |
| 2 | Challenge — Add Links to Navbar | 3 min | **Core in class** |
| 4 | Aside: Client vs. Server Components | 6 min | **Core in class** |
| 6 | Dynamic Routes | 9 min | **Core in class** |
| 5 | Challenge — Create the Models List Page | 5 min | **Homework** |
| 7 | Model Detail Page | 5 min | **Homework** |
| 3 | Aside: TypeScript Organization in PrintForge | 4 min | **Homework** |
| 9 | Section 1 Recap | 3 min | **Homework** |

**Stop in-class viewing after item 6 (~22 min).** Items 5, 7, 3, and 9 are **homework**.

Optional reading: [Client vs server aside](https://www.coursera.org/learn/learn-nextjs/ungradedWidget/cBgd0/aside-client-vs-server-components) if linked from the course.

**Map the course to this project:**

| Course concept | What to build in `nextjs-practice/` |
|---|---|
| `'use client'` | Interactive toggle or button component |
| Server `page.jsx` | Imports client component; no `useState` in server file |
| `app/projects/[id]/page.jsx` | Shows project id from `params` |
| Checkpoint doc | Links to `react-practice/` + `nextjs-practice/` |

**Individual notes:**

```text
Server components run...
Client components need 'use client' when...
Dynamic routes use...
My dynamic route will show...
One thing I still do not understand is...
```

**Student output:** Notes + Module 3 progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../shared/talk-robin-rules.md).

**Share:**

1. When you need `'use client'`
2. One dynamic route idea (`/projects/1`, etc.)
3. One skill from `react-practice/` you reused in Next.js
4. One confusion or question

**Pair summary:** Agree on one client-vs-server rule and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
React practice prepared us for Next.js because...
Our group still needs help with...
```

**Teacher checks:**

1. Do both `react-practice/` and `nextjs-practice/` run?
2. Can students explain why `useState` belongs in a client file?
3. Can students name the folder pattern for a dynamic segment?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

> [!IMPORTANT]
> Close Coursera before this block. Use your notes and the task list below — no videos during hands-on practice.

**Task:**

1. Create a client component, for example `app/components/ProjectToggle.jsx`:

```jsx
"use client";

import { useState } from "react";

export default function ProjectToggle() {
  const [open, setOpen] = useState(false);
  return (
    <div>
      <button type="button" onClick={() => setOpen(!open)}>
        {open ? "Hide details" : "Show details"}
      </button>
      {open && <p>Extra project detail text here.</p>}
    </div>
  );
}
```

2. Import it into a server page (default `app/projects/page.jsx` or home page).
3. Add one dynamic route, for example `app/projects/[id]/page.jsx`, reading `params.id` and showing matching title from your hard-coded array.
4. Update root `README.md` or add `front-end-evidence.md` with links to both practice folders.
5. Commit with message: `Add client component and dynamic route`.

**Mission output:**

- Client component toggles UI with `useState`
- Dynamic route shows different content per `id`
- Checkpoint doc or README lists both projects
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../shared/independent-rebuild.md).

**Exit Check task:**

1. Without Coursera, add one more line of text to the dynamic route page template.
2. Be ready to explain orally: when a component must be a client component.
3. Update Notion portfolio with links to both GitHub folders + one screenshot.

**Exit prompts:**

```text
'use client' is needed when...
My dynamic route folder is...
Server page vs client component in my app...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** Trace JSX → props → state → fetch → Next layout → client component → dynamic route.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. GitHub links: `react-practice/` and `nextjs-practice/`
2. Screenshot: client component interaction on a Next page
3. Screenshot: dynamic route showing different `id`
4. Coursera progress: Learn React (modules your teacher assigned) + Learn Next.js Modules 1–3
5. Notion portfolio update with front-end practice section
6. One sentence: "Client components are needed when..."

## Success Criteria

You are successful if:

1. Both `react-practice/` and `nextjs-practice/` run locally.
2. `react-practice/` shows components, props, list map, state, and fetch (from Unit 05).
3. `nextjs-practice/` shows routes, layout, `'use client'`, and one dynamic route.
4. You can explain client vs server without reading slides.
5. Notion + GitHub evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| `useState` error in page | Move interactivity to a `'use client'` file; import into server page. |
| Dynamic route 404 | Folder must be `[id]`; export default page component. |
| `params` undefined | In App Router, read `params` from page props; check Next.js version docs if shape differs. |
| Missing React skills | Review [Unit 05](../05-react-basics/react-lessons/) before demo. |

## Unit Completion Checklist

```text
[ ] react-practice/ — components, props, map, state, fetch
[ ] nextjs-practice/ — routes, layout, client component, dynamic route
[ ] Coursera Learn React — modules assigned by teacher
[ ] Coursera Learn Next.js — Modules 1, 2, 3
[ ] Notion updated
[ ] Can explain how a future full-stack app connects frontend to FastAPI
```

## Fast Track / Support Track

Fast track:

Students who finish early may preview Unit 10 integration reading — do not start the full AI app until your teacher assigns it.

Support track:

- Complete client toggle + one static dynamic route first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full checkpoint is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
