# Lesson 8: Box Model, Spacing, and Borders

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain padding, margin, border, and content in the CSS box model.
2. Adjust padding and margin on existing page elements.
3. Use DevTools to inspect one spacing problem.
4. Explain why width and spacing affect readability.
5. Adjust spacing during Exit Check without reopening the tutorial.
6. Submit daily evidence listed below.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** box model, padding, margin, borders, and DevTools inspection. Box model wrap-up and page layout come in the next lessons.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–25 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra layout tutorials during class.

**Required resource — [HTML & CSS Crash Course, Module 1](https://www.coursera.org/learn/html--css-crash-course/home/module/1)** (Kevin Powell / Scrimba).

**Class time target:** watch **items 21–23** during the 10–25 minute block. That is about 26 minutes — finish item 23 as homework only if you run out of class time.

Items 24–26 move to [Lesson 9](lesson-08-box-model-borders-and-wrap-up.md).

Use **only** these Coursera/Scrimba items, **in this order**:

| Coursera item # | Title | ~Time | When to use |
|---|---|---|---|
| 21 | Intro to the box model | 6 min | **Core in class** |
| 22 | Margin and Padding | 12 min | **Core in class** |
| 23 | Borders | 8 min | **Core in class** |

**Stop here.** Do **not** open item 24 (Box model wrap up) or any later layout item during this class.

Focus on how each element is a box with layers: content → padding → border → margin.

**Map the course to this project:**

| Course concept | What to add to `web-basics-project/` |
|---|---|
| Box model | Explain content, padding, border, and margin |
| Spacing | Adjust padding and margin on body, headings, or sections |
| Borders | Add a visible border to a card or container |
| Width intro | Try one readable `max-width` value without finalizing layout |
| DevTools | Inspect one element and read its box model values |

**Individual notes:**

```text
Padding is...
Margin is...
The difference between padding and margin is...
max-width on a container helps because...
One spacing problem I saw in DevTools is...
One thing I still do not understand is...
```

**Student output:** Centered container/card layout with improved spacing.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. One spacing property you changed today (`padding`, `margin`, or `border`)
2. What your container or card looks like now
3. One thing you noticed in DevTools
4. One confusion or question

**Pair summary:** Agree on one layout fix and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
Padding controls space...
Margin controls space...
A centered container needs...
Our group still needs help with...
```

**Teacher checks:**

1. Is Lesson 2 CSS linked and working?
2. Can students explain padding vs margin?
3. Does the page use a centered container with `max-width`?
4. Do images stay inside the container on narrow screens?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. Open `web-basics-project/index.html` and `style.css`.
2. Pick one element that needs better spacing.
3. Adjust `padding` and `margin` in `style.css`.
4. Add `border` and optional `border-radius` to one card or container.
5. Open DevTools, inspect one element, and fix one spacing or border problem you find.
6. Save, refresh, and compare before/after spacing.
9. Commit with message: `Improve layout with box model and centered container`.

**Mission output:**

- Better spacing visible in the browser
- At least one spacing fix identified with DevTools
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Open your page without the Coursera lesson.
2. Adjust one padding or margin value until the layout looks more balanced.
3. Inspect the same element in DevTools and confirm the change.
4. Be ready to explain padding vs margin orally if called.

**Exit prompts:**

```text
My container class is...
Padding on my card is...
Margin between sections is...
One spacing problem I fixed is...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Explain content → padding → border → margin using one element on your page.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot of your improved spacing in the browser
2. GitHub link to updated `style.css` (and `index.html` if structure changed)
3. Screenshot or link showing today's commit
4. One sentence: "Today I changed ___ by adjusting padding/margin/border on ___."

## Success Criteria

You are successful if:

1. Your main content has more readable spacing.
2. You can explain padding vs margin.
3. You inspected at least one box model value in DevTools.
4. You used DevTools to inspect at least one spacing issue.
5. You made a meaningful commit on GitHub.
6. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Content stuck to the left | Add `max-width` and `margin: 0 auto` on the container. |
| Text touches the edge | Increase `padding` inside the container or card. |
| Huge gaps between sections | Check for double margins on both section and `.card`. |
| Image overflows | Add `max-width: 100%` to `img`. |
| Rounded corners not visible | Add a background color or border so radius shows. |

## Fast Track / Support Track

Fast track:

If most students complete this lesson in about 45 minutes, continue directly into [Lesson 9](lesson-08-box-model-borders-and-wrap-up.md) during the same 90-minute block.

Use this only if students have:

1. A centered container layout that works in the browser.
2. Fixed at least one spacing issue.
3. Completed Exit Check without reopening the tutorial.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
