# Lesson 10: Flexbox Layout Project

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain how Flexbox aligns child elements from a parent container.
2. Choose one final mini project — login page, profile card, or landing hero section.
3. Build the Flexbox layout in HTML and CSS using `display: flex`, `justify-content`, `align-items`, or `gap`.
4. Keep semantic HTML, external CSS, and container layout from earlier lessons.
5. Improve one alignment detail during Exit Check without reopening the tutorial.
6. Submit daily evidence listed below.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** `display: flex`, layout HTML, layout CSS, and choosing the final mini project direction. Final polish and submission happen in [Lesson 11](lesson-10-flexbox-layout-polish-and-submit.md). Do not add CSS Grid, animation libraries, or Bootstrap for this unit.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–25 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra layout tutorials during class.

**Required resource — [HTML & CSS Crash Course, Module 1](https://www.coursera.org/learn/html--css-crash-course/home/module/1)** (Kevin Powell / Scrimba).

**Class time target:** watch **items 27–29** during the 10–25 minute block. That is about 30 minutes — finish item 29 during Guided Practice or as homework if you run out of class time.

Items 30–31 are optional closing items in [Lesson 11](lesson-10-flexbox-layout-polish-and-submit.md), along with the **HTML and CSS Crash Course Quiz**.

Use **only** these Coursera/Scrimba items, **in this order**:

| Coursera item # | Title | ~Time | When to use |
|---|---|---|---|
| 27 | Creating columns with flexbox | 7 min | **Core in class** |
| 28 | Creating the layout from scratch - the HTML | 10 min | **Core in class** |
| 29 | Creating the Layout - The CSS | 13 min | **Core in class** |

**Stop here.** Do **not** open item 30 during this class.

Focus on how `display: flex` on a parent controls how child elements align. Watch for patterns you can reuse in a login page, profile card, or hero section.

**Choose your final project:**

Pick **one** project type and commit to it:

| Project type | What to build |
|---|---|
| **Simple login page** | Centered form with email/username, password, and submit button |
| **Profile card** | Avatar or image, name, short bio, and action links |
| **Landing hero section** | Headline, subtitle, and one or two call-to-action buttons |

Reuse colors and container styles from Lessons 2–3 where they still help. Update `index.html` and `style.css` — do not start a new folder.

**Individual notes:**

```text
My final project type is...
My main flex container is...
justify-content on my page is...
align-items on my page is...
gap helps because...
One thing I still do not understand is...
```

**Student output:** Notes ready for the final build and one chosen project type.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. Which project type you chose and why
2. Which element will be your flex container
3. One Flexbox property you plan to use
4. One confusion or question

**Pair summary:** Agree on one project idea and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
display: flex goes on...
justify-content controls...
align-items controls...
gap is useful because...
Our group still needs help with...
```

**Teacher checks:**

1. Did every student choose one project type?
2. Can students explain which element is the flex container?
3. Are earlier lesson files still in `web-basics-project/`?
4. Did anyone try to start a brand-new folder instead of extending the same project?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. Open `web-basics-project/index.html` and `style.css`.
2. Choose one mini project type: login page, profile card, or landing hero.
3. Identify one parent element that should become a flex container.
4. Build or update the HTML structure for that layout.
5. Add Flexbox CSS with `display: flex` and at least one of: `justify-content`, `align-items`, `flex-direction`, `gap`.
6. Keep external CSS in `style.css` — no inline styles.
7. Test in the browser and confirm the flex layout works.
8. Commit with message: `Build flexbox layout project`.

**Mission output:**

- One working flex layout in the browser
- Updated `index.html` and `style.css` in `web-basics-project/`
- Meaningful commits across the unit so far

Final project polish, README, and rubric self-check happen in [Lesson 11](lesson-10-flexbox-layout-polish-and-submit.md).

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Open your project page without the Coursera lesson.
2. Improve one alignment detail with Flexbox.
3. Be ready to explain which parent is the flex container and which children it controls.

**Exit prompts:**

```text
My final project type is...
My main flex container is...
justify-content is set to...
align-items is set to...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Explain why this course uses HTML for structure, CSS for style, and Flexbox for alignment — using your own page.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot or preview showing the first Flexbox alignment change
2. GitHub links to updated `index.html` and `style.css`
3. Screenshot or link showing today's commit
4. One sentence: "My flex container is ___; it controls ___."

## Success Criteria

You are successful if:

1. Your project page opens correctly in the browser.
2. You chose one final project direction.
3. You built a Flexbox layout in both HTML and CSS.
4. You can explain what the flex parent controls.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Items not centering | Put `display: flex` on the **parent**, not every child. |
| Items in a row when you wanted a column | Add `flex-direction: column`. |
| Uneven spacing | Use `gap` on the flex container. |
| Layout breaks on mobile | Add `flex-wrap: wrap`; avoid fixed widths on text containers. |
| Login labels not clickable | Match `for` on `<label>` to `id` on `<input>`. |

## Fast Track / Support Track

Fast track:

If this lesson is complete early, continue to [Lesson 11](lesson-10-flexbox-layout-polish-and-submit.md) only if your teacher approves.

Optional extra block (teacher-assigned):

Use one extra 90-minute session for debugging, DevTools practice, and adding the project to your Notion **Learning Projects** section.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

## After This Unit

Next: [JavaScript Basics](../../04-javascript-basics/) — extend the same `web-basics-project/` folder.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
