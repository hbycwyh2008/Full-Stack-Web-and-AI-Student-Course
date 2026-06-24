# Lesson 2: CSS Basics and Selectors

## Lesson Goal

Style the HTML page from Lesson 1 using an external CSS file so your page looks clearly designed — not like the browser default.

By the end of this lesson, you should have `style.css` linked from `index.html` and at least one new commit showing visible styling changes.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on linking external CSS, element/class/id selectors, colors, fonts, text alignment, and simple spacing. Do not use inline `style="..."` on HTML tags for this unit.

## Entry Point Check

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra CSS tutorials during class.

Students work individually first.

**Step A — Coursera reading and video:**

1. Open the Coursera course: https://www.coursera.org/learn/html--css-crash-course/home/module/1
2. Work through the **CSS fundamentals** sections — linking CSS, selectors, colors, fonts, and basic text styling.
3. **Stop before the box model and layout sections.** Those come in Lesson 3.
4. Focus on how rules in a separate `.css` file change the look of HTML elements.

**Step B — map the course to this project:**

| Course concept | What to add to `web-basics-project/` |
|---|---|
| External stylesheet | `<link rel="stylesheet" href="style.css">` in `<head>` |
| Element selectors | Style `body`, `h1`, `h2`, `p`, `a` |
| Class selectors | Add `class="card"` to sections; style with `.card` |
| ID selector | Add `id="tagline"` to one element; style with `#tagline` |
| Colors and fonts | Change at least three visual properties beyond browser defaults |
| Spacing intro | Use simple `margin` or `padding` on body or cards |

**Individual notes:**

```text
External CSS is linked with...
An element selector targets...
A class selector targets...
An id selector targets...
Inline CSS should be avoided here because...
One CSS rule I will write today is...
One thing I still do not understand is...
```

**Student output:** Lesson 1 page with visible styling from `style.css`.

## Talk Robin

Each student speaks once before anyone speaks twice.

**Share:**

1. One element selector and one class selector you used
2. One color or font choice you made
3. Why external CSS is better than inline styles for this project
4. One confusion or question

**Student output:** Group list of useful CSS patterns and unclear questions.

## Group Answer

As a group, prepare one shared answer:

```text
HTML gives structure because...
CSS gives style because...
A class selector is different from an id selector because...
Our group still needs help with...
```

**Student output:** One group answer.

## Teacher Clarification

The teacher checks what students already understand before explaining.

**Teacher checks:**

1. Is Lesson 1 `index.html` complete and opening in the browser?
2. Is `style.css` linked correctly from `<head>`?
3. Can students point to one element rule and one class rule in their code?
4. Did anyone use inline `style="..."`? (Avoid for this unit.)

**Teacher explanation rule:** Explain only the unclear parts. Do not run a full teacher-demo-first lesson.

The teacher explains only the common stuck points before the mission task.

## Mission Task

Students complete the main task.

**Task:**

1. Open `web-basics-project/index.html` from Lesson 1.
2. Create `style.css` in the same folder.
3. Link it in `<head>` with `<link rel="stylesheet" href="style.css">`.
4. Style `body`, `h1`, `h2`, `p`, and `a` with element selectors.
5. Add `class="card"` to at least two sections and style `.card`.
6. Add `id="tagline"` to one paragraph and style `#tagline`.
7. Change at least **three** properties beyond browser defaults (colors, fonts, spacing, alignment).
8. Refresh the browser and confirm CSS is applied.
9. Commit with message: `Add external CSS with selectors and basic styling`.

**Mission output:**

- `style.css` linked and working
- Visible styling with element, class, and id selectors
- No inline CSS on HTML elements
- One meaningful commit on GitHub

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block.

Students repeat the workflow independently **without looking at the tutorial**.

**Independent rebuild task:**

1. Open your page without the Coursera lesson.
2. Change one color or font size using your own choice.
3. Point to one element selector, one class selector, and one id selector in your code.
4. Be ready to explain HTML vs CSS orally if called.

**Exit prompts:**

```text
My external CSS file is...
One element selector I used is...
One class selector I used is...
One id selector I used is...
HTML structure lives in...
CSS style lives in...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Point to one HTML tag and the CSS rule that styles it.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot of your styled page in the browser
2. GitHub links to `web-basics-project/index.html` and `style.css`
3. Screenshot or link showing today's commit
4. One sentence: "Today I changed ___ by adding CSS rule ___."

## Success Criteria

You are successful if:

1. Your page looks clearly styled compared to Lesson 1.
2. Your CSS is in an external file, not inline.
3. You use at least one element selector, one class selector, and one id selector.
4. You made a meaningful commit on GitHub.
5. You can explain the difference between HTML and CSS.

## Common Problems

| Problem | Try first |
|---|---|
| CSS not applied | Check `<link href="style.css">` path and that both files are in the same folder. |
| Only some rules work | Check selector spelling; class names must match exactly. |
| ID style missing | Use only one `id="tagline"` on the page. |
| Colors look wrong | Hex colors need `#` (example: `#1a365d`). |
| Changes not visible | Hard refresh the browser (Cmd+Shift+R / Ctrl+Shift+R). |

## Fast Track / Support Track

Fast track:

If most students complete this lesson in about 45 minutes, continue directly into [Lesson 3](lesson-03-box-model-and-layout.md) during the same 90-minute block.

Use this only if students have:

1. Working external CSS with visible changes.
2. No inline styles on HTML tags.
3. Completed the independent rebuild without reopening the tutorial.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
