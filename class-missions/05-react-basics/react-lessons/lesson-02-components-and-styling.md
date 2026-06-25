# Lesson 2: Components and Styling

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Split UI into at least two custom components (parent + child).
2. Style React components with CSS classes imported into components.
3. Compose components in `App.jsx` with a clear file structure.
4. Explain why components beat one giant JSX block.
5. Add one improvement during Exit Check without reopening Coursera.
6. Submit daily evidence listed below.

> **Prerequisite:** [Lesson 1](lesson-01-jsx-and-first-components.md) — `react-practice/` runs with `npm run dev`.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** Watch only the listed Coursera items; finish ReactFacts build scrims during Guided Practice.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** custom components, parent/child composition, fragments, and styling with CSS classes. Props come in [Lesson 3](lesson-03-props-and-reusable-components.md). Do **not** open Module 4 (Props) today.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra React tutorials during class.

**Required resource — [Learn React, Module 2](https://www.coursera.org/learn/learn-react/home/module/2)** (Bob Ziroll / Scrimba): **Static pages in React 02 — Building with React**.

**Self-study cap:** watch only the items below during this block. Total **~26 minutes**. ReactFacts project scrims (Module 2 items 9–15) continue in Guided Practice.

Open [Module 2](https://www.coursera.org/learn/learn-react/home/module/2) on Coursera. Use **only** these items, **in this order**:

| Item # | Title | ~Time | When to use |
|---|---|---|---|
| 3 | Custom Components | 6 min | **Core in class** |
| 4 | Custom Components Challenge Part 2 | 4 min | **Core in class** |
| 6 | Fragments | 2 min | **Core in class** |
| 7 | Custom Components — Parent/Child Components | 5 min | **Core in class** |
| 8 | Styling with Classes | 9 min | **Core in class** |

**Stop here (~26 min).** Items 9–15 (ReactFacts build) continue in Guided Practice — not in the 30-minute viewing block.

Do **not** open [Module 4](https://www.coursera.org/learn/learn-react/home/module/4) (Props) — that is [Lesson 3](lesson-03-props-and-reusable-components.md).

**Map the course to this project:**

| Course concept | What to build in `react-practice/` |
|---|---|
| `Header.jsx` | Title + subtitle for your portfolio-style page |
| `MainContent.jsx` | Short intro paragraph |
| `App.css` or component CSS | Header background + main text color |
| `App.jsx` | Compose Header + MainContent |

**Individual notes:**

```text
A parent component passes structure by...
I styled my component using className...
Organizing components in folders helps because...
One thing I still do not understand is...
```

**Student output:** Notes + Module 2 progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. Your component tree (which two components you plan)
2. One CSS class naming choice
3. One difference between `class` and `className`
4. One confusion or question

**Pair summary:** Agree on one good folder/file pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
Good component structure for a portfolio page includes...
Styling in React is different from HTML-only because...
Our group still needs help with...
```

**Teacher checks:**

1. Does Lesson 1 app still run?
2. Can each student name two components in their plan?
3. Are students using `className`, not `class`?
4. Did anyone put all JSX back into one file?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. In `react-practice/src/`, create at least **two components** — for example `Header.jsx` and `MainContent.jsx`.
2. Create a CSS file; style header background and main text color (match your Notion/portfolio colors if you have them).
3. Import CSS in the component or `App.jsx`.
4. Compose both components in `App.jsx`.
5. Confirm styling appears in the browser with no Console errors.
6. Commit with message: `Add Header and MainContent with CSS classes`.

**Mission output:**

- At least two custom components visible in the browser
- CSS classes applied (not inline-only defaults)
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add a `Footer.jsx` component with one styled line in your own words.
2. Import and render it in `App.jsx` without reopening Coursera.
3. Commit: `Add Footer component`.

**Exit prompts:**

```text
My two main components are...
CSS is imported in...
className is used because...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** Point to parent and child components in your file tree.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot of styled multi-component page
2. GitHub link showing component files + CSS
3. Coursera Module 2 progress screenshot
4. One sentence: "Components help my UI because..."

## Success Criteria

You are successful if:

1. At least two custom components are composed in App.
2. Visible CSS styling uses classes.
3. App runs without Console errors.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Styles not applied | Import CSS file; check `className` spelling matches CSS selector. |
| Component not showing | `export default` in component file; correct import path in App. |
| White screen after split | Check for missing closing tags in JSX; read Console. |

## Fast Track / Support Track

Fast track:

If Module 2 and mission evidence are complete early, preview [Lesson 3](lesson-03-props-and-reusable-components.md) props idea only.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
