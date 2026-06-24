# Lesson 3: CSS Basics and Selectors

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain basic CSS rule syntax: selector, property, and value.
2. Use simple element selectors to style a page.
3. Add one useful list to the existing page.
4. Change at least three visual properties beyond browser defaults.
5. Explain why CSS controls style while HTML controls structure.
6. Update styling during Exit Check without reopening the tutorial.
7. Submit daily evidence listed below.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** CSS introduction, basic rules, practice, recap, and HTML lists. Images and HTML practice come in [Lesson 4](lesson-06-css-files-and-selectors.md); external CSS linking comes in [Lesson 5](lesson-11-css-internal-external-stylesheets.md); classes and comments come in [Lesson 7](lesson-07-css-classes-ids-and-comments.md).

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–25 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra CSS tutorials during class.

**Required resource — [HTML & CSS Crash Course, Module 1](https://www.coursera.org/learn/html--css-crash-course/home/module/1)** (Kevin Powell / Scrimba).

**Class time target:** watch **items 9–13** during the 10–25 minute block. That is about 26 minutes — finish item 13 as homework only if you run out of class time.

Items 14–15 move to [Lesson 4](lesson-06-css-files-and-selectors.md). Items 16–17 move to [Lesson 5](lesson-11-css-internal-external-stylesheets.md). Items 18–20 move to Lessons 6–7. Do **not** open item 14 or later during this class.

Use **only** these Coursera/Scrimba items, **in this order**:

| Coursera item # | Title | ~Time | When to use |
|---|---|---|---|
| 9 | Intro to CSS | 7 min | **Core in class** |
| 10 | CSS Basics | 6 min | **Core in class** |
| 11 | Practice time! | 3 min | **Core in class** |
| 12 | Recap up until this point | 5 min | **Core in class** |
| 13 | Lists | 5 min | **Core in class** |

**Stop here.** Do **not** open item 14 (Images) or any later item during this class.

Focus on how CSS rules change the look of HTML elements, and how lists add structured HTML content.

**Map the course to this project:**

| Course concept | What to add to `web-basics-project/` |
|---|---|
| Element selectors | Style `body`, `h1`, `h2`, `p`, `a` |
| Lists | Add one `<ul>` or `<ol>` with at least three items |
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

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. One element selector and one class selector you used
2. One color or font choice you made
3. Why external CSS is better than inline styles for this project
4. One confusion or question

**Pair summary:** Agree on one useful CSS pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
HTML gives structure because...
CSS gives style because...
A class selector is different from an id selector because...
Our group still needs help with...
```

**Teacher checks:**

1. Is Lesson 1 `index.html` complete and opening in the browser?
2. Is `style.css` linked correctly from `<head>`?
3. Can students point to one element rule and one class rule in their code?
4. Did anyone use inline `style="..."`? (Avoid for this unit.)

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. Open `web-basics-project/index.html` from earlier lessons.
2. Create `style.css` in the same folder if it does not exist yet.
3. Link it in `<head>` if your teacher has not already provided the link.
4. Add one `<ul>` or `<ol>` with at least three items.
5. Style `body`, `h1`, `h2`, `p`, and `a` with element selectors.
6. Change at least **three** properties beyond browser defaults (colors, fonts, spacing, alignment).
7. Refresh the browser and confirm CSS is applied.
8. Commit with message: `Add CSS basics, list, and element styling`.

**Mission output:**

- `style.css` linked and working
- Visible styling with element selectors
- One list with at least three items
- No inline CSS on HTML elements
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Open your page without the Coursera lesson.
2. Change one color or font size using your own choice.
3. Point to two element selectors in your code.
4. Be ready to explain HTML vs CSS orally if called.

**Exit prompts:**

```text
My external CSS file is...
One element selector I used is...
One property/value pair I used is...
HTML structure lives in...
CSS style lives in...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Point to one HTML tag and the CSS rule that styles it.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot of your styled page in the browser
2. GitHub links to `web-basics-project/index.html` and `style.css`
3. Screenshot or link showing today's commit
4. One sentence: "Today I changed ___ by adding CSS rule ___."

## Success Criteria

You are successful if:

1. Your page looks clearly styled compared to Lesson 1.
2. Your CSS is in an external file, not inline.
3. You use at least three element selector rules.
4. You made a meaningful commit on GitHub.
5. You can explain the difference between HTML and CSS.
6. All evidence submitted.

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

If most students complete this lesson in about 45 minutes, continue directly into [Lesson 4](lesson-06-css-files-and-selectors.md) during the same 90-minute block.

Use this only if students have:

1. Working external CSS with visible changes.
2. No inline styles on HTML tags.
3. Completed Exit Check without reopening the tutorial.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
