# Lesson 3: Props and Reusable Components

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Pass data into child components with props.
2. Destructure props in function components.
3. Build one reusable card component used twice with different props.
4. Use JavaScript expressions inside JSX where appropriate.
5. Commit props refactor with a meaningful message.
6. Submit Module 4 evidence.

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

**Required resource — complete [Learn React Module 4](https://www.coursera.org/learn/learn-react/home/module/4):** Data-Driven React 01 — Understanding Props (~1 hour).

**Individual notes:**

```text
Props are...
Destructuring props looks like...
I reused a component by passing...
One thing I still do not understand is...
```

## Talk Robin

**Share:** props vs hard-coded text; one non-string prop idea; one question.

## Group Answer

```text
Props make components reusable because...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Can students explain props direction (parent → child)?

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Create `ProjectCard.jsx` accepting props: `title`, `description`, `status`.
2. Render **two** `<ProjectCard />` instances with different prop values in `App.jsx`.
3. Commit: `Add reusable ProjectCard with props`.

## Independent Rebuild

Add a third card via props only — no copy-paste of JSX structure. Commit.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot showing three different cards (or two if fast track last lesson)
2. GitHub link to `ProjectCard.jsx` and usage in App
3. Coursera Module 4 progress screenshot
4. One sentence: “Props are like function parameters because...”

## Success Criteria

1. One component reused with different props.
2. Props destructured or accessed clearly.
3. Meaningful commit.
4. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| All cards show same text | Pass different prop values on each instance. |
| `props is undefined` | Check component parameter and spelling. |

## Fast Track / Support Track

Fast track:

Preview Module 5 mapping scrims if Module 4 is done early.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
