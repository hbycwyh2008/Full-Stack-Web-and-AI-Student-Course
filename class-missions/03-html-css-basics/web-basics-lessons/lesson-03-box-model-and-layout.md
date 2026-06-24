# Lesson 3: Box Model and Layout

## Lesson Goal

Improve your page layout using the CSS box model so content sits in a centered container or card with readable spacing.

By the end of this lesson, your page should look organized on both wide and narrow browser windows, and you should know how to inspect spacing with DevTools.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on content, padding, border, margin, width, containers, background color, border radius, and DevTools inspection. Flexbox comes in Lesson 4.

## Entry Point Check

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra layout tutorials during class.

Students work individually first.

**Step A — Coursera reading and video:**

1. Open the Coursera course: https://www.coursera.org/learn/html--css-crash-course/home/module/1
2. Work through the **box model and layout** sections — padding, margin, border, width, and container-style layout.
3. **Stop before Flexbox sections.** Flexbox is Lesson 4.
4. Focus on how each element is a box with layers: content → padding → border → margin.

**Step B — map the course to this project:**

| Course concept | What to add to `web-basics-project/` |
|---|---|
| Box model | Set `padding`, `margin`, and `border` on container and cards |
| Centered container | Wrap main content in `.page-container` with `max-width` and `margin: 0 auto` |
| Card layout | Style `.card` sections with background, padding, and `border-radius` |
| Page background | Different background on `body` vs container |
| DevTools | Inspect one element and read its box model values |
| Image safety | `img { max-width: 100%; }` so images do not overflow |

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

## Talk Robin

Each student speaks once before anyone speaks twice.

**Share:**

1. One spacing property you changed today (`padding`, `margin`, or `border`)
2. What your container or card looks like now
3. One thing you noticed in DevTools
4. One confusion or question

**Student output:** Group list of layout fixes and unclear questions.

## Group Answer

As a group, prepare one shared answer:

```text
Padding controls space...
Margin controls space...
A centered container needs...
Our group still needs help with...
```

**Student output:** One group answer.

## Teacher Clarification

The teacher checks what students already understand before explaining.

**Teacher checks:**

1. Is Lesson 2 CSS linked and working?
2. Can students explain padding vs margin?
3. Does the page use a centered container with `max-width`?
4. Do images stay inside the container on narrow screens?

**Teacher explanation rule:** Explain only the unclear parts. Do not run a full teacher-demo-first lesson.

The teacher explains only the common stuck points before the mission task.

## Mission Task

Students complete the main task.

**Task:**

1. Open `web-basics-project/index.html` and `style.css`.
2. Add `class="page-container"` to `<main>` (or wrap sections in a container div).
3. Center the layout with `max-width: 720px` and `margin: 0 auto`.
4. Give the container a background, padding, border, and `border-radius`.
5. Update `.card` sections with consistent inner spacing.
6. Add `img { max-width: 100%; height: auto; }` if you use images.
7. Open DevTools, inspect one element, and fix one spacing problem you find.
8. Test in a wide window and a narrow window — no horizontal scroll.
9. Commit with message: `Improve layout with box model and centered container`.

**Mission output:**

- Centered container/card layout visible in the browser
- At least one spacing fix identified with DevTools
- One meaningful commit on GitHub

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block.

Students repeat the workflow independently **without looking at the tutorial**.

**Independent rebuild task:**

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

## Evidence to Submit

1. Screenshot of your centered container/card layout in the browser
2. GitHub link to updated `style.css` (and `index.html` if structure changed)
3. Screenshot or link showing today's commit
4. One sentence: "Today I changed ___ by adjusting padding/margin/border on ___."

## Success Criteria

You are successful if:

1. Your main content sits in a centered, readable container.
2. Your cards or sections have consistent spacing.
3. Your page does not overflow horizontally on narrow screens.
4. You used DevTools to inspect at least one spacing issue.
5. You made a meaningful commit on GitHub.

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

If most students complete this lesson in about 45 minutes, continue directly into [Lesson 4](lesson-04-flexbox-mini-project.md) during the same 90-minute block.

Use this only if students have:

1. A centered container layout that works in the browser.
2. Fixed at least one spacing issue.
3. Completed the independent rebuild without reopening the tutorial.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
