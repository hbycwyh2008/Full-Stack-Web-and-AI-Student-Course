# Lesson 2: ReactFacts — Components and Styling

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Split the ReactFacts UI into at least three custom components (`Navbar`, `Main`, and one more).
2. Organize components in a `src/components/` folder and compose them in `App.jsx`.
3. Style React components with CSS classes (`className`) — not inline-only defaults.
4. Build the ReactFacts static page: navbar, main content with a facts list, and styled bullets.
5. Add one improvement during Exit Check without reopening Coursera.
6. Submit daily evidence listed below.

> **Prerequisite:** [Lesson 1](lesson-01-jsx-and-first-components.md) — `react-practice/` runs with `npm run dev`.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum** for in-class viewing. **Do not open Coursera during Guided Practice or Exit Check.**

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** ReactFacts markup, custom components, parent/child composition, fragments, and styling with CSS classes. Props and the Travel Journal project start in [Lesson 3](lesson-03-props-and-reusable-components.md). Do **not** open Module 4 (Props) today.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra React tutorials during class.

**Required resource — [Learn React, Module 2](https://www.coursera.org/learn/learn-react/home/module/2)** (Bob Ziroll / Scrimba): **Static pages in React 02 — Building with React**.

**Self-study cap:** watch only the **Core in class** items below during this block. Total **~30 minutes**.

Open [Module 2](https://www.coursera.org/learn/learn-react/home/module/2) on Coursera. Item numbers **restart at 1 inside each module**.

| Item # | Title | ~Time | When to use |
|---|---|---|---|
| 1 | ReactFacts Project — Markup | 4 min | **Core in class** |
| 3 | Custom Components | 6 min | **Core in class** |
| 4 | Custom Components Challenge Part 2 | 4 min | **Core in class** |
| 6 | Fragments | 2 min | **Core in class** |
| 7 | Custom Components — Parent/Child Components | 5 min | **Core in class** |
| 8 | Styling with Classes | 9 min | **Core in class** |
| 9 | Organizing Components | 5 min | **Homework** |
| 10 | Make Mental Outline of Project | 4 min | **Homework** |
| 11 | Initial Project Setup | 5 min | **Homework** |
| 12 | ReactFacts Project — Navbar & Styling | 8 min | **Homework** |
| 13 | ReactFacts Project — Main Content Section | 7 min | **Homework** |
| 14 | ReactFacts Project — Coloring the Bullets | 2 min | **Homework** |
| 15 | ReactFacts Project — Add Background Image | 5 min | **Homework** |

**Stop in-class viewing at item 8 (~30 min).** Items 9–15 are **homework** — watch after class or if your teacher assigned them before the next session. Guided Practice uses the written task list only.

Items 2 and 5 (quizzes) are optional homework. Do **not** open [Module 4](https://www.coursera.org/learn/learn-react/home/module/4) (Props) — that is [Lesson 3](lesson-03-props-and-reusable-components.md).

**Map the course to this project:**

| Course concept | What to build in `react-practice/` |
|---|---|
| ReactFacts markup | Navbar + main section with React facts list |
| `Navbar.jsx` | Logo/title area for the facts site |
| `Main.jsx` | Heading, intro text, `<ul>` of React facts |
| `src/components/` folder | One file per component |
| `App.css` or component CSS | Dark navbar, light main area, styled bullets |

Use the [ReactFacts Figma design](https://scrimba.com/links/figma-reactfacts) as a visual reference. Your facts text can be your own words — structure matters more than copying exact copy.

**Individual notes:**

```text
ReactFacts has these main sections...
A parent component passes structure by...
I styled my component using className...
Organizing components in folders helps because...
One thing I still do not understand is...
```

**Student output:** Notes + Module 2 concept items complete (items 1, 3–4, 6–8).

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. Your ReactFacts component tree (Navbar, Main, App)
2. One CSS class naming choice
3. One difference between `class` and `className`
4. One confusion or question

**Pair summary:** Agree on one good `components/` folder pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
Good ReactFacts structure includes...
Styling in React is different from HTML-only because...
Our group still needs help with...
```

**Teacher checks:**

1. Does Lesson 1 app still run?
2. Can each student name three components in their ReactFacts plan?
3. Are students using `className`, not `class`?
4. Did anyone put all JSX back into one file?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

> [!IMPORTANT]
> Close Coursera before this block. Build from the task list and your notes — no videos during hands-on practice.

**Task — build ReactFacts in `react-practice/`:**

1. Create `src/components/` with `Navbar.jsx` and `Main.jsx`.
2. Refactor Lesson 1 content into the ReactFacts layout — remove the placeholder "Phase 4" demo text unless it fits your facts list.
3. In `Main.jsx`, include a title, short intro, and a `<ul>` with at least **four** React facts.
4. Import a CSS file; style the navbar background, main text, and bullet list (item 14).
5. Add a background image or decorative background on the main section (item 15). Use a local file in `public/` or a simple CSS gradient if image setup is slow.
6. Compose `Navbar` + `Main` in `App.jsx`.
7. Confirm styling appears in the browser with no Console errors.
8. Commit with message: `Build ReactFacts Navbar and Main with CSS`.

**Mission output:**

- ReactFacts page with Navbar + Main visible in the browser
- Components live in `src/components/`
- CSS classes applied (not inline-only defaults)
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add a `Footer.jsx` component with one styled line (for example, your name or course phase).
2. Import and render it in `App.jsx` without reopening Coursera.
3. Commit: `Add Footer to ReactFacts`.

**Exit prompts:**

```text
My ReactFacts components are...
CSS is imported in...
className is used because...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** Point to parent and child components in your file tree.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot of styled ReactFacts page (navbar + facts list)
2. GitHub link showing `components/` folder + CSS
3. Coursera Module 2 progress screenshot
4. One sentence: "Components help my ReactFacts UI because..."

## Success Criteria

You are successful if:

1. ReactFacts has at least Navbar, Main, and Footer composed in App.
2. Visible CSS styling uses classes.
3. Main section shows a list of React facts.
4. App runs without Console errors.
5. You made a meaningful commit on GitHub.
6. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Styles not applied | Import CSS file; check `className` spelling matches CSS selector. |
| Component not showing | `export default` in component file; correct import path in App. |
| White screen after split | Check for missing closing tags in JSX; read Console. |
| Background image missing | Check path: files in `public/` use `/image.png`; imported assets use `import`. |

## Fast Track / Support Track

Fast track:

If Module 2 and mission evidence are complete early, preview [Lesson 3](lesson-03-props-and-reusable-components.md) props idea only.

Support track:

- Complete Navbar + Main first; add Footer and background image if time runs short.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
