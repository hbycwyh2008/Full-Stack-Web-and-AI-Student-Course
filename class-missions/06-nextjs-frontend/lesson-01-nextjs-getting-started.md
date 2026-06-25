# Lesson 1: Getting Started with Next.js

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain how Next.js relates to React (framework on top of React).
2. Create `nextjs-practice/` with `create-next-app` and App Router.
3. Run `npm run dev` and open the default Next.js page.
4. Replace the home page with their name and a course heading.
5. Add one improvement during Exit Check without reopening Coursera.
6. Submit daily evidence listed below.

> **Prerequisite:** [Lesson 7](../05-react-basics/react-lessons/lesson-07-useeffect-and-fetch.md) — `react-practice/` complete. Keep `react-practice/`; start a **new** folder for Next.js.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** Watch only the listed Coursera items during that block. Optional homework items are listed there — **do not open Coursera during Guided Practice or Exit Check.**

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** Next.js intro, minimal setup, `create-next-app`, and `app/` folder basics. File-based routing and extra pages start in [Lesson 2](lesson-02-nextjs-routing-and-layouts.md). Do **not** open Module 2 today.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra Next.js tutorials during class.

**Required resource — [Learn Next.js, Module 1](https://www.coursera.org/learn/learn-nextjs/home/module/1)** (Scrimba): **Getting Started with Next.js**.

**Self-study cap:** watch only the **Core in class** items below during this block. Total **~29 minutes**.

Open [Module 1](https://www.coursera.org/learn/learn-nextjs/home/module/1) on Coursera. Item numbers **restart at 1 inside each module**.

| Item # | Title | ~Time | When to use |
|---|---|---|---|
| 2 | Next.js Intro | 3 min | **Core in class** |
| 3 | A Minimal Next.js Setup | 5 min | **Core in class** |
| 4 | Challenge: create a new Next.js app from scratch! | 4 min | **Core in class** |
| 5 | Adding a new page to our site | 3 min | **Core in class** |
| 6 | File-based routing in Next.js | 4 min | **Core in class** |
| 7 | Understanding create-next-app | 4 min | **Core in class** |
| 8 | Running create-next-app | 3 min | **Core in class** |
| 10 | create-next-app files walkthrough | 3 min | **Core in class** |

**Stop in-class viewing after item 10 (~29 min).** Item 9 (Scrimba Runner) is **homework**. Item 1 (Welcome) is optional homework.

Do **not** open [Module 2](https://www.coursera.org/learn/learn-nextjs/home/module/2) — that is [Lesson 2](lesson-02-nextjs-routing-and-layouts.md).

**Map the course to this project:**

| Course concept | What to build in `nextjs-practice/` |
|---|---|
| `create-next-app` | New folder in your course repo |
| `app/page.jsx` | Your name + heading for this unit |
| `README.md` | `npm install`, `npm run dev`, link to `react-practice/` |
| DevTools Console | Check for errors on load |

**Individual notes:**

```text
Next.js is different from Vite React because...
My nextjs-practice folder was created with...
The app/ directory is for...
page.jsx is the route for...
One thing I still do not understand is...
```

**Student output:** Notes + Module 1 progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../shared/talk-robin-rules.md).

**Share:**

1. React vs Next.js in one sentence
2. Where `page.jsx` lives in App Router
3. One Coursera item that helped today
4. One confusion or question

**Pair summary:** Agree on one difference between Vite and Next.js and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
We might use Next.js later in this course because...
Our group still needs help with...
```

**Teacher checks:**

1. Is Node.js working? Does `npm -v` run?
2. Can students name three folders: `react-practice/`, `nextjs-practice/`, future course frontend folder?
3. Can students point to `app/page.jsx` in a fresh `create-next-app` project?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

> [!IMPORTANT]
> Close Coursera before this block. Use your notes and the task list below — no videos during hands-on practice.

**Task:**

1. Create `nextjs-practice/` using `create-next-app` (JavaScript is OK; TypeScript may come in a later course phase):

```bash
npx create-next-app@latest nextjs-practice
```

Choose App Router when prompted. Accept defaults your teacher recommends.

2. Edit `app/page.jsx` (or `.js`): show your name and one heading, for example `Next.js Practice`.
3. Add `README.md`:

```md
# Next.js Practice

## Run
npm install
npm run dev

## Prior step
See ../react-practice/ for React + Vite work.
```

4. Open `http://localhost:3000` — confirm your text appears with **no red Console errors**.
5. Commit with message: `Initialize nextjs-practice with App Router`.

**Mission output:**

- Running Next.js app with custom home page
- `README.md` with run instructions
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../shared/independent-rebuild.md).

**Exit Check task:**

1. Add one `<p>` with your learning goal for this unit.
2. Refresh the browser and confirm it appears.
3. Commit: `Add learning goal to Next.js home page`.

**Exit prompts:**

```text
My home page file is...
Next.js builds on React by...
npm run dev starts...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** How is `app/page.jsx` different from Vite's `App.jsx`?

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot of localhost Next.js page
2. GitHub link to `nextjs-practice/`
3. Coursera Module 1 progress screenshot
4. One sentence: "Next.js builds on React by..."

## Success Criteria

You are successful if:

1. `npm run dev` works for `nextjs-practice/`.
2. Custom home page is visible in the browser.
3. README documents how to start the dev server.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Port in use | `npm run dev -- -p 3001` or close other servers. |
| Wrong folder | Run commands inside `nextjs-practice/`. |
| Blank page | Read terminal and browser Console errors. |
| Coursera scrim won't play | Desktop browser; log in if prompted. |

## Fast Track / Support Track

Fast track:

If Module 1 and mission evidence are complete early, preview [Lesson 2](lesson-02-nextjs-routing-and-layouts.md) route folder idea only — do not skip Lesson 1 evidence.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
