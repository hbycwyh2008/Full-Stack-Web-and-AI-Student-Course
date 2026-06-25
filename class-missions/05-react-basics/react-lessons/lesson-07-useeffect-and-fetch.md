# Lesson 7: useEffect and Fetch in React

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain why data fetching in React often uses `useEffect` or an async handler.
2. Fetch JSON on button click with `async`/`await` and show result in state.
3. Display loading and error states in the UI.
4. Optionally preview `useEffect` for load-on-mount (Module 13).
5. Complete Phase 4 checkpoint README and rubric self-check.
6. Submit Phase 4 evidence listed below.

> **Prerequisite:** [Lesson 6](lesson-06-forms-and-conditional-ui.md) — form and conditional list work.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** **Do not open Coursera during Guided Practice or Exit Check.**

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** controlled components, fetching data, `useEffect` intro. This is the Phase 4 checkpoint. Skip capstone modules 15–20 (Tenzies, Assembly: Endgame).

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra React tutorials during class.

**Required resource — two Coursera modules, selected items only:**

1. [Module 12](https://www.coursera.org/learn/learn-react/home/module/12) — **React Side Effects 01 — Building the Meme Generator & Managing State**
2. [Module 13](https://www.coursera.org/learn/learn-react/home/module/13) — **React Side Effects 02 — Data Fetching & useEffect in React**

**Self-study cap:** watch only the items below during this block. Total **~30 minutes**.

| Item # | Title | Module | ~Time | When to use |
|---|---|---|---|---|
| 4 | Meme Generator — Controlled Components — part 1 | 12 | 6 min | **Core in class** |
| 5 | Meme Generator — Controlled Components — part 2 | 12 | 6 min | **Core in class** |
| 1 | Fetching data in React | 13 | 6 min | **Core in class** |
| 2 | Intro to `useEffect` | 13 | 3 min | **Core in class** |
| 3 | `useEffect()` syntax and default behavior | 13 | 4 min | **Core in class** |
| 4 | `useEffect()` Dependencies array | 13 | 7 min | **Homework** |
| 5 | `useEffect` empty dependencies array | 13 | 3 min | **Homework** |
| 6 | `useEffect` quiz! | 13 | 5 min | **Homework** |
| 7 | `useEffect` practice! | 13 | 5 min | **Homework** |
| 8 | Meme Generator — Fetch Memes | 13 | 8 min | **Homework** |

**Stop in-class viewing after item 3 (~25 min).** Module 13 items 4–14 are **homework** (dependencies, Meme fetch, cleanup, refs).

Skip [Module 14](https://www.coursera.org/learn/learn-react/home/module/14) (quiz) and modules 15–20 (Tenzies, Assembly: Endgame capstones) unless your teacher assigns optional extension.

Button-triggered `fetch` with `async`/`await` (Phase 3 skill) is the class mission pattern in Guided Practice; `useEffect` is introduced in the core items above.

**Map the course to this project:**

| Course concept | What to build in `react-practice/` |
|---|---|
| Load button | Fetch on click first (Phase 3 skill) |
| Result in state | Display JSON field in UI |
| Loading text | "Loading..." while waiting |
| Error message | User-friendly text if fetch fails |
| README | Next step: FastAPI + Next.js in later phases |

**Individual notes:**

```text
useEffect runs when...
fetch in React is similar to Phase 3 because...
Loading state matters because...
This will connect to our AI app when...
One thing I still do not understand is...
```

**Student output:** Notes + Module 12–13 progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. Sync vs async in the UI — one example from your app
2. Button fetch vs `useEffect` on mount — when each helps
3. What the user should see while data loads
4. One confusion or question

**Pair summary:** Agree on one loading-message pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
Our React app will call a backend later by...
If fetch fails, we should show...
Our group still needs help with...
```

**Teacher checks:**

1. Does Phase 3 `async`/`await` still make sense to students?
2. Can students explain CORS at a high level (public API vs local backend later)?
3. Are loading and error states planned in UI, not only `console.log`?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

> [!IMPORTANT]
> Close Coursera before this block. Build from the task list and your notes — no videos during hands-on practice.

**Task:**

1. Add UI:

```jsx
<button type="button" onClick={loadQuote}>Load quote</button>
<p>{quoteText}</p>
```

2. Add fetch handler with loading and error state:

```jsx
const [quoteText, setQuoteText] = useState("Click the button to load a quote.");
const [loading, setLoading] = useState(false);

async function loadQuote() {
  setLoading(true);
  setQuoteText("Loading...");

  try {
    const response = await fetch("https://jsonplaceholder.typicode.com/todos/1");
    if (!response.ok) throw new Error("Bad response");
    const data = await response.json();
    setQuoteText("Loaded: " + data.title);
  } catch (error) {
    console.error(error);
    setQuoteText("Could not load data. Check Console or network.");
  } finally {
    setLoading(false);
  }
}
```

3. Test successful load and broken URL (teacher-guided) for error message.
4. Update `react-practice/README.md`:

```md
## Phase 4 Checkpoint
- Components, props, list, state, form, fetch demo complete.

## Next Step
Call FastAPI from Next.js in course Phases 6–7.
```

5. Commit with message: `Add fetch demo with loading state in React`.

**Optional extension:** one `useEffect` on mount — explain difference from button fetch orally.

**Mission output:**

- Fetch works with loading feedback
- Error handled without crashing app
- Updated README with next-step note

**Phase 4 rubric — self-check before submission:**

| Criterion | Strong | Developing | Starting |
|---|---|---|---|
| JSX and components | Multiple components composed clearly | Mostly clear | Broken structure |
| Props and lists | Reusable card + `.map()` + `key` | Partial | Missing |
| State and events | `useState` + handlers work | Partial | Missing or broken |
| Forms and conditional UI | Add form + empty/list states | Partial | Missing |
| fetch and loading UI | Load + loading/error feedback | Loads only | Broken or missing |
| Code readability | Clear names, organized files | Mostly readable | Hard to follow |
| GitHub evidence | Screenshots, commits, README | Most present | Missing key items |
| Reflection quality | Specific about learning | General | Vague |

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Change endpoint to `https://jsonplaceholder.typicode.com/users/1` and display `data.name`.
2. Explain aloud: "`fetch` returns a Promise because..." and "loading state helps because..."
3. Commit: `Fetch user name with async await`.

**Exit prompts:**

```text
My fetch function is called...
While fetch runs, the user sees...
If fetch fails, the user sees...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** How will this React app connect to a Python backend later?

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot after successful fetch
2. Screenshot or note showing error message when load fails (teacher may guide test)
3. GitHub link to fetch handler + loading UI in `script` / component files
4. Updated `README.md` with Phase 4 checkpoint and next-step bullet
5. Completed Phase 4 rubric self-check
6. Commit history showing work across Lessons 1–7
7. One sentence: "Phase 4 taught me ___; my app demonstrates it by ___."

## Success Criteria

You are successful if:

1. Button triggers fetch — page updates from state, not direct DOM edits.
2. Loading text or disabled button shows while waiting.
3. Failed fetch shows user-friendly message without crashing the app.
4. README documents run steps and connection to later full-stack phases.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| `Failed to fetch` | Check URL; school network; use jsonplaceholder URL exactly. |
| Infinite re-fetch loop | Check `useEffect` dependency array — ask teacher. |
| Stuck on "Loading..." | Use `finally` to reset loading state. |
| CORS on random API | Use jsonplaceholder or local backend later with teacher setup. |

## Fast Track / Support Track

Fast track:

If Phase 4 evidence is complete early, preview [Phase 5: Next.js Frontend](../../06-nextjs-frontend/) only if your teacher approves.

Optional extra block (teacher-assigned):

Debugging, refactoring components, and Notion portfolio update.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

## After Phase 4

Next: [Phase 5: Next.js Frontend](../../06-nextjs-frontend/)

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
