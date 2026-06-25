# Lesson 6: Forms and Conditional UI

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Build a small React form with controlled inputs and submit handling.
2. Use conditional rendering (`&&` or ternary) to show empty vs list states.
3. Append new items to a projects array in state on form submit.
4. Explain when to lift state up to a parent component.
5. Add empty-field validation during Exit Check.
6. Submit daily evidence listed below.

> **Prerequisite:** [Lesson 5](lesson-05-state-and-events.md) — `useState` toggle and controlled input work.

## Required Resource

Open only the resource named in `Individual Learning`. **Self-study cap: 30 minutes maximum.** Items are split across Module 8 and Module 9 — do not watch the full modules.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** form submit, array state updates, conditional rendering (`&&` / ternary). `fetch` and `useEffect` come in [Lesson 7](lesson-07-useeffect-and-fetch.md). Skip Sound pads and AI chef scrims (Module 10).

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–40 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra React tutorials during class.

**Required resource — two Coursera modules, selected items only:**

1. [Module 8](https://www.coursera.org/learn/learn-react/home/module/8) — **React State 02 — State Management and React Forms**
2. [Module 9](https://www.coursera.org/learn/learn-react/home/module/9) — **React State 03 — Conditional Rendering and State Communication**

**Self-study cap:** watch only the items below during this block. Total **~30 minutes**.

| Item # | Title | Module | ~Time | When to use |
|---|---|---|---|---|
| 15 | React forms intro | 8 | 5 min | **Core in class** |
| 17 | Form submission | 8 | 7 min | **Core in class** |
| 19 | Chef Claude: Refactor form submission | 8 | 3 min | **Core in class** |
| 2 | Conditional rendering: `&&` | 9 | 7 min | **Core in class** |
| 5 | Conditional rendering: ternary | 9 | 5 min | **Core in class** |

**Stop here (~27 min).** Items 11–13 (lifting state) may continue in Guided Practice. Item 16 (Form basics) is optional homework if you need extra form review.

Skip [Module 10](https://www.coursera.org/learn/learn-react/home/module/10) (API Integration) and Sound pads challenges — optional teacher extension only.

Skip [Module 11](https://www.coursera.org/learn/learn-react/home/module/11) (quiz) unless assigned as homework.

**Map the course to this project:**

| Course concept | What to build in `react-practice/` |
|---|---|
| Add project form | Fields: title + description |
| Projects in state | Move array from Lesson 4 into `useState` |
| Empty state message | "No projects yet" when array is empty |
| List when not empty | Map cards when array has items |

**Individual notes:**

```text
Conditional rendering with && means...
I lift state to the parent when...
My form updates state by...
preventDefault on submit is needed because...
One thing I still do not understand is...
```

**Student output:** Notes + Module 8–9 progress started.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. One conditional UI pattern you will use
2. How your form adds to the projects array
3. One child-to-parent pattern (if using separate form component)
4. One confusion or question

**Pair summary:** Agree on one empty-state message and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
Conditional UI helps our portfolio because...
Our group still needs help with...
```

**Teacher checks:**

1. Does Lesson 5 toggle still work?
2. Do forms use controlled components (`value` + `onChange`)?
3. Are students creating a **new array** when adding items, not mutating in place?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. Move projects array into state:

```jsx
const [projects, setProjects] = useState([...initialProjects]);
```

2. Add a simple "Add project" form with title + description fields.
3. On submit:

```jsx
function handleSubmit(e) {
  e.preventDefault();
  const newProject = {
    id: Date.now(),
    title,
    description,
    status: "New"
  };
  setProjects((prev) => [...prev, newProject]);
  setTitle("");
  setDescription("");
}
```

4. Conditional UI:

```jsx
{projects.length === 0 && <p>No projects yet. Add one above.</p>}
{projects.length > 0 && (
  projects.map((p) => <ProjectCard key={p.id} {...p} />)
)}
```

5. Test: empty state → add one project → list appears.
6. Commit with message: `Add project form with conditional list`.

**Mission output:**

- Form adds items to list in state
- Empty vs list UI works
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close Coursera, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add validation: if title is empty, show error text under the form (conditional render).
2. Do not add the project when title is empty.
3. Commit: `Add empty title validation`.

**Exit prompts:**

```text
My form prevents default because...
Empty state shows when...
List shows when...
One thing I can now do without Coursera is...
One thing I still need help with is...
```

**Oral check if called:** Lifting state helps because...

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot: empty state and after adding one project
2. GitHub link showing form + conditional render + array state
3. Coursera Module 8–9 progress screenshot
4. One sentence: "Lifting state helps because..."

## Success Criteria

You are successful if:

1. Form adds items to the list in state.
2. Conditional empty vs list UI works.
3. Submit does not reload the page.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Form reloads page | `e.preventDefault()` in submit handler. |
| List doesn't update | Use setter with new array `[...prev, newItem]`. |
| Duplicate keys | Use unique `id` — `Date.now()` is OK for class demos. |
| Inputs stay filled after add | Reset title/description state after submit. |

## Fast Track / Support Track

Fast track:

If evidence is complete early, preview [Lesson 7](lesson-07-useeffect-and-fetch.md) fetch button pattern only.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
