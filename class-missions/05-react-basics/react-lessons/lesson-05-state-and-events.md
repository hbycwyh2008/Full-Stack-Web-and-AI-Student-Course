# Lesson 5: State and Events

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain props vs state in simple words.
2. Use `useState` to store and update UI state.
3. Attach click handlers that update state — not the DOM directly.
4. Build one controlled input field with `value` and `onChange`.
5. Add a second state-driven UI change during Exit Check.
6. Submit daily evidence listed below.

> **Prerequisite:** [Lesson 4](lesson-04-lists-map-and-keys.md) — project list renders from an array.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** **Do not open Coursera during Guided Practice or Exit Check.**

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** props vs state, `useState`, event handlers, toggling state, one controlled input. Full forms and conditional UI come in [Lesson 6](lesson-06-forms-and-conditional-ui.md). Do **not** use `document.querySelector` in new code.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra React tutorials during class.

**Required resource — two Coursera modules, selected items only:**

1. [Module 7](https://www.coursera.org/learn/learn-react/home/module/7) — **React State 01 — Introduction and Basics** (events only)
2. [Module 8](https://www.coursera.org/learn/learn-react/home/module/8) — **React State 02 — State Management and React Forms** (state basics only)

**Self-study cap:** watch only the items below during this block. Total **~28 minutes**. Do **not** open form scrims (Module 8 items 15+) in self-study — those are [Lesson 6](lesson-06-forms-and-conditional-ui.md).

Open the modules on Coursera. Use **only** these items:

| Item # | Title | Module | ~Time | When to use |
|---|---|---|---|---|
| 5 | Event Listeners | 7 | 6 min | **Core in class** |
| 1 | Props vs. State: Props | 8 | 4 min | **Core in class** |
| 2 | Props vs. State: State | 8 | 5 min | **Core in class** |
| 3 | `useState` | 8 | 5 min | **Core in class** |
| 5 | Changing state | 8 | 5 min | **Core in class** |
| 10 | Toggling state | 8 | 7 min | **Core in class** |

**Stop in-class viewing after item 10 (~28 min).** Module 7 items 1–4 and 6 (Chef Claude build) are **homework**. Module 8 item 4 (`useState` array destructuring) and items 6–9 are **homework**. Form topics continue in [Lesson 6](lesson-06-forms-and-conditional-ui.md).

Skip [Module 10](https://www.coursera.org/learn/learn-react/home/module/10) (API Integration / AI chef) — not core for CS1.

**Map the course to this project:**

| Course concept | What to build in `react-practice/` |
|---|---|
| Boolean state | Toggle visibility of ReactFacts details or an extra journal section |
| String state | Controlled `<input>` to filter journal entries by country or title |
| Handlers | Named functions or inline setters — be consistent |

**Individual notes:**

```text
Props vs state: props are... state is...
useState returns...
When the user clicks, React...
Controlled input needs value and onChange because...
One thing I still do not understand is...
```

**Student output:** Notes + Module 8 (partial) progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. "When the user clicks my button, React..."
2. One `useState` example from your plan
3. Why we do not use `document.querySelector` in React
4. One confusion or question

**Pair summary:** Agree on one props-vs-state sentence and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
We use useState instead of changing the DOM directly because...
Our group still needs help with...
```

**Teacher checks:**

1. Do students import `{ useState }` from `'react'`?
2. Can students explain props vs state with an example from their app?
3. Is anyone mutating state directly (for example, `state.push`)?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

> [!IMPORTANT]
> Close Coursera before this block. Build from the task list and your notes — no videos during hands-on practice.

**Task:**

1. Add state and a toggle button:

```jsx
import { useState } from "react";

const [showDetails, setShowDetails] = useState(false);

<button type="button" onClick={() => setShowDetails(!showDetails)}>
  {showDetails ? "Hide details" : "Show details"}
</button>
{showDetails && <p>Your extra project detail text here.</p>}
```

2. Add one controlled input:

```jsx
const [filterText, setFilterText] = useState("");

<input
  value={filterText}
  onChange={(e) => setFilterText(e.target.value)}
  placeholder="Filter projects..."
/>
<p>Current filter: {filterText}</p>
```

3. Test toggle and typing in the browser — no Console errors.
4. Commit with message: `Add useState toggle and controlled input`.

**Mission output:**

- UI changes on click via state
- One controlled input field
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add a second button that changes a text label via state (for example, greeting message).
2. Explain aloud: props vs state on your page.
3. Commit: `Add second state-driven label`.

**Exit prompts:**

```text
My boolean state controls...
My string state controls...
setState is called when...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** State is different from props because...

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot before and after toggle click
2. Screenshot showing controlled input with typed text
3. GitHub link showing `useState` and handlers in component
4. Coursera Module 7–8 progress screenshot (items listed above)
5. One sentence: "State is different from props because..."

## Success Criteria

You are successful if:

1. UI changes on click via state update.
2. One controlled input field works while typing.
3. No direct DOM manipulation in new code.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| State not updating | Use setter from `useState`; do not reassign state variable directly. |
| Input can't type | Missing `onChange` or `value` binding. |
| Toggle stuck | Check boolean negation `!showDetails`. |
| `useState is not defined` | Import from `'react'`. |

## Fast Track / Support Track

Fast track:

Watch Module 8 controlled-input items (15–17) as **homework** before [Lesson 6](lesson-06-forms-and-conditional-ui.md) if time allows.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
