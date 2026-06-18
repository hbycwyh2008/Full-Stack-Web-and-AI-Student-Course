# Lesson 6: Forms and Conditional UI

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Build a small React form with controlled inputs.
2. Use conditional rendering (`&&` or ternary) to show/hide UI.
3. Pass state or callbacks between parent and child components.
4. Explain when to lift state up to a parent.
5. Commit form + conditional UI with a meaningful message.
6. Submit Module 8–9 progress.

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

1. Finish [Learn React Module 8](https://www.coursera.org/learn/learn-react/home/module/8): forms and complex state (~2 hours total; complete remaining scrims from Lesson 5 + today).
2. Complete [Module 9](https://www.coursera.org/learn/learn-react/home/module/9): conditional rendering and state communication (~1 hour).

**Individual notes:**

```text
Conditional rendering with && means...
I lift state to the parent when...
My form submits or updates state by...
One thing I still do not understand is...
```

## Talk Robin

**Share:** one conditional UI pattern; one child-to-parent state pattern; one question.

## Group Answer

```text
Conditional UI helps our portfolio because...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Lesson 5 toggle still works; forms use controlled components.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Add a simple “Add project” form: fields for title + description; on submit, append to projects array in state.
2. Show “No projects yet” when array is empty; show list when not empty (conditional rendering).
3. Optional: extract form into child component; pass setter or handler from parent.
4. Commit: `Add project form with conditional list`.

## Independent Rebuild

Add validation message when title is empty (conditional text). Commit.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot: empty state and after adding one project
2. GitHub link showing form + conditional render + array state
3. Coursera Module 8–9 progress screenshot
4. One sentence: “Lifting state helps because...”

## Success Criteria

1. Form adds items to list in state.
2. Conditional empty vs list UI works.
3. Meaningful commit.
4. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Form reloads page | `e.preventDefault()` on submit handler. |
| List doesn't update | Use setter with new array `[...prev, newItem]`. |

## Fast Track / Support Track

Fast track:

Optional Module 11 quiz as homework for certificate.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
