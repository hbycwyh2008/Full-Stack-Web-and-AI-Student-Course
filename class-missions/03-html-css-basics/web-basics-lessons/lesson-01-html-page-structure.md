# Lesson 1: HTML Page Structure

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain the basic parts of a valid HTML5 document.
2. Build a real page with semantic structure — `header`, `main`, `footer`, headings, and paragraphs.
3. Save an unstyled `index.html` in `web-basics-project/` with meaningful content in their own words.
4. Test the page in the browser and confirm the content appears.
5. Add one improvement during Exit Check without reopening the tutorial.
6. Submit daily evidence listed below.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

**Today's pattern:** document structure, headings, and paragraphs. Links come in [Lesson 2](lesson-05-html-text-links-lists-images.md); lists and CSS come in [Lesson 3](lesson-02-css-basics-and-selectors.md); images come in [Lesson 4](lesson-06-css-files-and-selectors.md). Do not add CSS yet in this lesson.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–25 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra HTML tutorials during class.

**Required resource — [HTML & CSS Crash Course, Module 1](https://www.coursera.org/learn/html--css-crash-course/home/module/1)** (Kevin Powell / Scrimba).

**Class time target:** watch only **items 2, 4, and 5** during the 10–25 minute block. That is about 18 minutes.

Item 3 is optional career context. Items 6–8 move to [Lesson 2](lesson-05-html-text-links-lists-images.md). Do **not** try to finish every Coursera HTML item during this class.

Open Module 1 on Coursera. Each item is an interactive Scrimba lesson (video + code). Use **only** the items listed here, **in this order** (CSS and lists come in [Lesson 3](lesson-02-css-basics-and-selectors.md) — skip items 9–13 for now):

| Coursera item # | Title | ~Time | When to use |
|---|---|---|---|
| 2 | What are HTML and CSS? | 4 min | **Core in class** |
| 3 | Frontend Career Path | 2 min | Skip unless teacher assigns |
| 4 | Basic Terminology and Syntax | 5 min | **Core in class** |
| 5 | Let's write some HTML! | 9 min | **Core in class** |

**Stop here.** Do **not** open item 9 (Intro to CSS) or any later item — CSS starts in [Lesson 3](lesson-02-css-basics-and-selectors.md).

Focus on how a valid HTML page is organized from `<!DOCTYPE html>` through `</html>`.

**Map the course to this project:**

| Course concept | What to build in `web-basics-project/` |
|---|---|
| Document skeleton | `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`, `<title>` |
| Page title area | One `<h1>` plus a short intro paragraph |
| Content sections | At least two `<section>` blocks with `<h2>` headings |
| Semantic layout | Use `<header>`, `<main>`, and `<footer>` where appropriate |

Choose **one** topic for the whole page: a short self-introduction **or** a fictional product page. Do not switch mid-lesson.

**Individual notes:**

```text
<!DOCTYPE html> is needed because...
<head> vs <body> difference is...
<h1> should appear once because...
alt on img is for...
One semantic tag I used is...
One thing I still do not understand is...
```

**Student output:** A working unstyled `index.html` with real content, not placeholder lorem ipsum.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. What you chose to build — self intro or product
2. One HTML tag you used today and what it does
3. Where your `<h1>` and one `<h2>` appear
4. One confusion or question

**Pair summary:** Agree on one useful structure pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
Every valid HTML page must include...
<head> is for...
<body> is for...
Our group still needs help with...
```

**Teacher checks:**

1. Do students have a code editor and browser ready?
2. Can students explain the difference between `<head>` and `<body>`?
3. Does every page have one clear `<h1>`?
4. Did anyone add CSS in this lesson? (It should wait until Lesson 2.)

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. Create folder `web-basics-project/` in your course repo.
2. Create `index.html` with full HTML5 document structure.
3. Add `<header>`, `<main>`, and `<footer>`.
4. Include at least: one `<h1>`, two `<h2>`, and three short paragraphs.
5. Write real content — your own words, not copied tutorial text.
6. Open the file in your browser and confirm the content appears.
7. Commit with message: `Add HTML page structure for web basics project`.

**Mission output:**

- `web-basics-project/index.html` opens correctly in the browser
- Semantic structure with visible real content
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

This is not a delete-and-redo task. Stay on the same page and add one meaningful improvement.

**Exit Check task:**

1. Open `index.html` without the Coursera page.
2. Add one new list item or one new sentence in your own words.
3. Confirm every opening tag has a matching closing tag.
4. Be ready to explain your page structure orally if called.

**Exit prompts:**

```text
My page title is...
My <h1> says...
My main content sections are...
<head> holds...
<body> holds...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Explain `<!DOCTYPE html>` → `<head>` → `<body>` → `<main>` using your own file.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot of your unstyled page open in the browser
2. GitHub link to `web-basics-project/index.html`
3. Screenshot or link showing today's commit in history
4. One sentence: "HTML gives structure because... CSS will give style because..."

## Success Criteria

You are successful if:

1. Your page opens in the browser with real content.
2. Your file includes valid document structure and semantic sections.
3. Your page has one clear `<h1>`, at least two sections, and real paragraphs.
4. You made a meaningful commit on GitHub.
5. You can explain the difference between HTML structure and CSS styling.
6. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Blank page | Check that content is inside `<body>` and tags are spelled correctly. |
| Section heading missing | Check that each main section has an `<h2>`. |
| Page looks plain | Expected for Lesson 1 — CSS comes next lesson. |
| Weird characters | Add `<meta charset="UTF-8">` inside `<head>`. |

## Fast Track / Support Track

Fast track:

If most students complete this lesson in about 45 minutes, continue directly into [Lesson 2](lesson-05-html-text-links-lists-images.md) during the same 90-minute block.

Use this only if students have:

1. A working `index.html` in the browser.
2. Real content in their own words.
3. Completed Exit Check without reopening the tutorial.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
