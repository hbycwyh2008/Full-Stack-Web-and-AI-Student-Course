# Lesson 5: State and Events

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain props vs state in simple words.
2. Use `useState` to store and update UI state.
3. Attach click handlers that update state (not DOM directly).
4. Start a controlled form field with state.
5. Commit interactive behavior with a meaningful message.
6. Submit Module 7 progress + start Module 8 as homework if needed.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

## Entry Point Check

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra playlists during class.

**Required resource:**

1. Complete [Learn React Module 7](https://www.coursera.org/learn/learn-react/home/module/7): React State 01 (~40 min).
2. Start [Module 8](https://www.coursera.org/learn/learn-react/home/module/8): through `useState` and `Changing state` scrims if time allows.

**Individual notes:**

```text
Props vs state: props are... state is...
useState returns...
When the user clicks, React...
One thing I still do not understand is...
```

## Talk Robin

**Share:** “When the user clicks my button, React...”; one `useState` example; one question.

## Group Answer

```text
We use useState instead of changing the DOM directly because...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Students import `useState` from `'react'`; no direct `document.querySelector` in new code.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Add a button that toggles visibility of a paragraph or project detail (`useState` boolean).
2. Add one `<input>` whose value is controlled by state (`value` + `onChange`).
3. Commit: `Add useState toggle and controlled input`.

## Independent Rebuild

Add a second button that changes a text label via state. Explain aloud: props vs state.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot before and after toggle click
2. GitHub link showing `useState` and handler in component
3. Coursera Module 7 progress screenshot
4. One sentence: “State is different from props because...”

## Success Criteria

1. UI changes on click via state update.
2. One controlled input field.
3. Meaningful commit.
4. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| State not updating | Use setter from `useState`; don't mutate state directly. |
| Input can't type | Missing `onChange` or `value` binding. |

## Fast Track / Support Track

Fast track:

Finish Module 8 `useState` scrims before Lesson 6.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
