# Lesson 1: HTML Page Structure

## Lesson Goal

Build your first real webpage with correct HTML document structure so it opens in the browser and introduces you or a fictional product.

By the end of this lesson, you should have an unstyled but complete `index.html` saved in your repo with at least one commit.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on document structure, headings, paragraphs, links, images, and lists. Do not add CSS yet — styling comes in Lesson 2.

## Entry Point Check

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra HTML tutorials during class.

Students work individually first.

**Step A — Coursera reading and video:**

1. Open the Coursera course: https://www.coursera.org/learn/html--css-crash-course/home/module/1
2. Work through the **HTML fundamentals** sections only — document structure, headings, paragraphs, links, images, and lists.
3. **Stop before CSS sections.** CSS comes in Lesson 2.
4. Focus on how a valid HTML page is organized from `<!DOCTYPE html>` through `</html>`.

**Step B — map the course to this project:**

The Coursera course builds example pages step by step. Adapt that pattern for this course:

| Course concept | What to build in `web-basics-project/` |
|---|---|
| Document skeleton | `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`, `<title>` |
| Page title area | One `<h1>` plus a short intro paragraph |
| Content sections | At least two `<section>` blocks with `<h2>` headings |
| Links | At least one working `<a href="...">` |
| Images | At least one `<img>` with meaningful `alt` text |
| Lists | One `<ul>` or `<ol>` with three items |
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

## Talk Robin

Each student speaks once before anyone speaks twice.

**Share:**

1. What you chose to build — self intro or product
2. One HTML tag you used today and what it does
3. Where your `<h1>` and one `<h2>` appear
4. One confusion or question

**Student output:** Group list of useful structure patterns and unclear questions.

## Group Answer

As a group, prepare one shared answer:

```text
Every valid HTML page must include...
<head> is for...
<body> is for...
Our group still needs help with...
```

**Student output:** One group answer.

## Teacher Clarification

The teacher checks what students already understand before explaining.

**Teacher checks:**

1. Do students have a code editor and browser ready?
2. Can students explain the difference between `<head>` and `<body>`?
3. Does every page have one clear `<h1>`?
4. Did anyone put CSS in this lesson? (It should wait until Lesson 2.)

**Teacher explanation rule:** Explain only the unclear parts. Do not run a full teacher-demo-first lesson.

The teacher explains only the common stuck points before the mission task.

## Mission Task

Students complete the main task.

**Task:**

1. Create folder `web-basics-project/` in your course repo.
2. Create `index.html` with full HTML5 document structure.
3. Add `<header>`, `<main>`, and `<footer>`.
4. Include at least: one `<h1>`, two `<h2>`, three paragraphs or list items combined, one link, one list, one image.
5. Write real content — your own words, not copied tutorial text.
6. Open the file in your browser and test every link.
7. Commit with message: `Add HTML page structure for web basics project`.

**Mission output:**

- `web-basics-project/index.html` opens correctly in the browser
- Semantic structure with visible real content
- One meaningful commit on GitHub

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block.

Students repeat the workflow independently **without looking at the tutorial**.

This is not a delete-and-redo task. Stay on the same page and add one meaningful improvement.

**Independent rebuild task:**

1. Open `index.html` without the Coursera page.
2. Add one new list item or one new sentence in your own words.
3. Confirm every opening tag has a matching closing tag (or is self-closing like `<img>`).
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

## Evidence to Submit

1. Screenshot of your unstyled page open in the browser
2. GitHub link to `web-basics-project/index.html`
3. Screenshot or link showing today's commit in history
4. One sentence: "HTML gives structure because... CSS will give style because..."

## Success Criteria

You are successful if:

1. Your page opens in the browser with real content.
2. Your file includes valid document structure and semantic sections.
3. Your page has at least one link, one list, and one image with `alt` text.
4. You made a meaningful commit on GitHub.
5. You can explain the difference between HTML structure and CSS styling.

## Common Problems

| Problem | Try first |
|---|---|
| Blank page | Check that content is inside `<body>` and tags are spelled correctly. |
| Image does not show | Check `src` path; local images go in `images/` inside your project folder. |
| Link goes nowhere | Check `href` for typos or missing `https://`. |
| Page looks plain | Expected for Lesson 1 — CSS comes next lesson. |
| Weird characters | Add `<meta charset="UTF-8">` inside `<head>`. |

## Fast Track / Support Track

Fast track:

If most students complete this lesson in about 45 minutes, continue directly into [Lesson 2](lesson-02-css-basics-and-selectors.md) during the same 90-minute block.

Use this only if students have:

1. A working `index.html` in the browser.
2. Real content in their own words.
3. Completed the independent rebuild without reopening the tutorial.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
