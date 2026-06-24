# Lesson 4: Flexbox Mini Project

## Lesson Goal

Complete your web basics unit by building one polished mini project — a simple login page, profile card, or landing page hero section — using Flexbox for alignment.

By the end of this lesson, your `web-basics-project/` folder should be ready to submit as Phase 2 evidence on GitHub.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on `display: flex`, `justify-content`, `align-items`, `gap`, and finishing one complete mini project. Your HTML structure, external CSS, and container layout from Lessons 1–3 should still be in place.

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
2. Work through the **Flexbox** sections — flex containers, alignment, and simple row/column layouts.
3. Focus on how `display: flex` on a parent controls how child elements align.
4. Watch for patterns you can reuse in a login page, profile card, or hero section.

**Step B — choose your final project:**

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

## Talk Robin

Each student speaks once before anyone speaks twice.

**Share:**

1. Which project type you chose and why
2. Which element will be your flex container
3. One Flexbox property you plan to use
4. One confusion or question

**Student output:** Group list of project ideas and unclear questions.

## Group Answer

As a group, prepare one shared answer:

```text
display: flex goes on...
justify-content controls...
align-items controls...
gap is useful because...
Our group still needs help with...
```

**Student output:** One group answer.

## Teacher Clarification

The teacher checks what students already understand before explaining.

**Teacher checks:**

1. Did every student choose one project type?
2. Can students explain which element is the flex container?
3. Are Lessons 1–3 files still in `web-basics-project/`?
4. Did anyone try to start a brand-new folder instead of extending the same project?

**Teacher explanation rule:** Explain only the unclear parts. Do not run a full teacher-demo-first lesson.

The teacher explains only the common stuck points before the mission task.

## Mission Task

Students complete the main task.

**Task:**

1. Open `web-basics-project/index.html` and `style.css`.
2. Rebuild or refine the page into your chosen mini project.
3. Use Flexbox in at least **two** places (for example: center the page, align form fields, or space buttons).
4. Use `display: flex`, plus at least two of: `justify-content`, `align-items`, `flex-direction`, `gap`.
5. Keep external CSS in `style.css` — no inline styles.
6. Add `README.md` to the project folder:

```md
# Web Basics Mini Project

## Project Type
Login page / Profile card / Landing hero (circle one)

## What This Page Does
One sentence in your own words.

## What I Learned
Three bullet points from Lessons 1–4.
```

7. Test in the browser at desktop and narrow width.
8. Commit with message: `Complete flexbox mini project`.

**Mission output:**

- One finished mini project in the browser
- Flexbox used for intentional alignment
- `index.html`, `style.css`, and `README.md` in `web-basics-project/`
- At least four meaningful commits across Lessons 1–4

**Final project rubric — self-check before submission:**

| Criterion | Strong | Developing | Starting |
|---|---|---|---|
| HTML structure | Semantic tags, valid structure, working links and `alt` text | Mostly valid; minor gaps | Broken or missing structure |
| CSS organization | External stylesheet; clear selectors | Works but messy | Inline styles or disorganized |
| Visual layout | Centered, readable, Flexbox used intentionally | Works but uneven | Hard to read or broken |
| Code readability | Indented, logical class names | Mostly readable | Difficult to follow |
| GitHub evidence | Screenshots, commits, README submitted | Most evidence present | Missing key evidence |
| Reflection quality | Specific about build, learnings, and fixes | General but honest | Vague or missing |

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block.

Students repeat the workflow independently **without looking at the tutorial**.

**Independent rebuild task:**

1. Open your finished page without the Coursera lesson.
2. Improve one visual detail — spacing, button style, or text alignment.
3. Test both links if your project includes links (Notion, GitHub, or placeholder).
4. Be ready to explain your flex container and alignment choices orally if called.

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

## Evidence to Submit

1. Screenshot or preview of your finished mini project
2. GitHub folder link to `web-basics-project/` with `index.html`, `style.css`, and `README.md`
3. Commit history showing work from all four lessons (four or more meaningful commits)
4. Completed final project rubric self-check (note Strong / Developing / Starting for each row)
5. One sentence: "This unit taught me ___; my page demonstrates it by ___."

## Success Criteria

You are successful if:

1. Your mini project opens correctly in the browser.
2. Your page uses semantic HTML, external CSS, container layout, and Flexbox.
3. Your `README.md` is written in your own words.
4. Your GitHub repo shows meaningful commit history across the unit.
5. You can explain what you built and how Flexbox helped alignment.

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

If Phase 2 evidence is complete early, preview [Phase 3: JavaScript Basics](../../04-javascript-basics/) only if your teacher approves.

Optional extra block (teacher-assigned):

Use one extra 90-minute session for debugging, DevTools practice, and adding the project to your Notion **Learning Projects** section.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

## After Phase 2

Next: [Phase 3: JavaScript Basics](../../04-javascript-basics/)

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
