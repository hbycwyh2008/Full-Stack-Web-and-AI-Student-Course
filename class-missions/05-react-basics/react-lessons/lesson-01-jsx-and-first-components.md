# Lesson 1: JSX and First React Components

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain why React uses components and JSX.
2. Create a Vite + React project in `react-practice/`.
3. Write and render a first React component with their name and course phase.
4. Run the dev server and confirm the app opens in the browser.
5. Add one improvement during Exit Check without reopening Coursera.
6. Submit daily evidence listed below.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** Watch only the listed Coursera items; finish any extra scrims during Guided Practice or as homework.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** first React code, JSX, composable ideas, and Vite setup. Custom components and CSS classes come in [Lesson 2](lesson-02-components-and-styling.md). Do **not** open Module 2 today.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra React tutorials during class.

**Required resource — [Learn React, Module 1](https://www.coursera.org/learn/learn-react/home/module/1)** (Bob Ziroll / Scrimba): **Static pages in React 01 — Getting Started with React**.

**Self-study cap:** watch only the items below during this block. Total **~27 minutes**. Item 1 (Course Introduction) is optional.

Open [Module 1](https://www.coursera.org/learn/learn-react/home/module/1) on Coursera. Item numbers **restart at 1 in each module**. Use **only** these items, **in this order**:

| Item # | Title | ~Time | When to use |
|---|---|---|---|
| 3 | What we'll learn | 2 min | **Core in class** |
| 4 | First React Code 🎉 | 7 min | **Core in class** |
| 5 | First React Challenge | 3 min | **Core in class** |
| 6 | Local Setup w/ Vite | 6 min | **Core in class** |
| 9 | Using JSX | 2 min | **Core in class** |
| 10 | Why React? It's Composable! | 7 min | **Core in class** |

**Stop here (~27 min).** Do **not** open item 11 or Module 2 — those start [Lesson 2](lesson-02-components-and-styling.md).

Items 1–2 (intro/welcome) and 7–8 (Libraries, React.createElement) are optional homework.

**Map the course to this project:**

| Course concept | What to build in `react-practice/` |
|---|---|
| Vite + React project | New folder in your course repo |
| `App.jsx` | Show your name + `Phase 4 React` |
| `README.md` | How to run `npm install` and `npm run dev` |
| DevTools Console | Check for red errors on load |

**Individual notes:**

```text
JSX is...
A React component is...
Why React is composable means...
Why React is declarative means...
My Vite project folder is...
One thing I still do not understand is...
```

**Student output:** Notes + Module 1 progress started (screenshot or teacher sign-off).

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. JSX vs plain HTML — one difference
2. What a component is in your own words
3. One Coursera scrim that helped today
4. One confusion or question

**Pair summary:** Agree on one useful JSX rule and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
We use components because...
JSX helps us because...
Our group still needs help with...
```

**Teacher checks:**

1. Is Node.js installed? Does `npm -v` work in terminal?
2. Can students open `react-practice/` in the editor?
3. Can students explain HTML/CSS (Phase 2) vs React (Phase 4) at a high level?
4. Did anyone skip the README step?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. In your course repo, create `react-practice/` with Vite + React (follow Module 1 or teacher command):

```bash
npm create vite@latest react-practice -- --template react
cd react-practice
npm install
npm run dev
```

2. Replace the default `App.jsx` content with a component that shows:
   - Your name
   - One line: `Phase 4 React Basics`
3. Add `README.md`:

```md
# React Practice

## Run
npm install
npm run dev

## Goal
First React component for CS1 Phase 4.
```

4. Open the local URL in the browser — confirm your text appears with **no red Console errors**.
5. Commit with message: `Start react-practice with first component`.

**Mission output:**

- Running Vite app with custom JSX
- `README.md` with run instructions
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add a second line in JSX — for example, your learning goal for Phase 4.
2. Refresh the browser and confirm both lines appear.
3. Be ready to explain what JSX is orally if called.
4. Commit: `Add learning goal to first component`.

**Exit prompts:**

```text
My component file is...
JSX is different from HTML because...
npm run dev starts...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** What is JSX?

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot of running app in browser
2. GitHub link to `react-practice/`
3. Screenshot or link showing today's commit
4. Coursera Module 1 progress screenshot (partial OK with teacher sign-off)
5. One sentence: "Today I changed ___ by creating my first React component in ___."

## Success Criteria

You are successful if:

1. Vite app runs with your custom component visible.
2. README explains how to start the dev server.
3. No red errors in the browser Console on load.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| `npm` not found | Install Node.js LTS; restart terminal. |
| Blank page | Check `main.jsx` imports `App`; read Console errors. |
| Port already in use | Stop other dev servers or use the port Vite suggests. |
| Coursera scrim won't play | Desktop browser; log in if prompted; try later. |

## Fast Track / Support Track

Fast track:

If most students finish in about 45 minutes, preview [Lesson 2](lesson-02-components-and-styling.md) component split only — do not skip Lesson 1 evidence.

Use this only if the app runs and Exit Check is complete.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
