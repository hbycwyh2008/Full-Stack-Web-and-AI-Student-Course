# Lesson 1: JavaScript Basics

## Lesson Goal

Connect JavaScript to your existing HTML/CSS page and use variables to store profile or product information, then confirm your code runs in the browser Console.

By the end of this lesson, you should have `script.js` linked from `web-basics-project/index.html` with meaningful `console.log` output and no red errors.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on what JavaScript does on a webpage, linking `script.js`, the browser Console, `console.log`, and basic data types with `let` and `const`. Do not update the DOM yet — that comes in Lesson 3.

## Entry Point Check

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra JavaScript tutorials during class.

Students work individually first.

**Step A — Coursera reading and video:**

1. Open the Coursera course: https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu/home/module/2
2. Work through the **JavaScript fundamentals** sections — what JavaScript does in the browser, variables, strings, numbers, booleans, arrays, and objects.
3. **Stop before functions and DOM sections.** Those come in Lessons 2 and 3.
4. Practice opening DevTools → Console and reading `console.log` output.

**Step B — map the course to this project:**

Extend your [HTML/CSS project](../../03-html-css-basics/web-basics-lessons/lesson-04-flexbox-mini-project.md) in `web-basics-project/`:

| Course concept | What to add |
|---|---|
| Script link | `<script src="script.js"></script>` before `</body>` |
| Console check | `console.log("JavaScript is connected.")` |
| Strings | `const name = "..."` |
| Numbers | `let score = 0` or similar |
| Booleans | `const isStudent = true` |
| Arrays | `const skills = ["HTML", "CSS", "JavaScript"]` |
| Objects | `const profile = { name: "...", role: "..." }` |

Store information about a user profile, product, or course card — match the topic of your HTML/CSS page.

**Individual notes:**

```text
JavaScript on my page is for...
HTML is for structure because...
CSS is for style because...
let vs const difference is...
One array I created is...
One object property I used is...
One thing I still do not understand is...
```

**Student output:** Working `script.js` with variables and meaningful Console messages.

## Talk Robin

Each student speaks once before anyone speaks twice.

**Share:**

1. Where your `<script>` tag is placed in HTML
2. One variable you declared and its data type
3. What `console.log` helps you do
4. One confusion or question

**Student output:** Group list of clear ideas and unclear questions.

## Group Answer

As a group, prepare one shared answer:

```text
On one web page, HTML...
On one web page, CSS...
On one web page, JavaScript...
let is for...
const is for...
Our group still needs help with...
```

**Student output:** One group answer.

## Teacher Clarification

The teacher checks what students already understand before explaining.

**Teacher checks:**

1. Does `web-basics-project/index.html` from Phase 2 still open correctly?
2. Can students open DevTools Console (F12 or right-click → Inspect)?
3. Can students explain the three layers: HTML, CSS, JavaScript?
4. Did anyone put `<script>` in `<head>` without understanding load order? (Before `</body>` is fine for this unit.)

**Teacher explanation rule:** Explain only the unclear parts. Do not run a full teacher-demo-first lesson.

The teacher explains only the common stuck points before the mission task.

## Mission Task

Students complete the main task.

**Task:**

1. Open `web-basics-project/` from your HTML/CSS unit.
2. Create `script.js` in the same folder.
3. Link it in `index.html` before `</body>`:

```html
<script src="script.js"></script>
```

4. In `script.js`, include all of the following with **your own values**:

```javascript
console.log("JavaScript is connected to my page.");

const pageTitle = "Your Page Title";
const visitCount = 1;
const isPublished = true;

console.log("Title:", pageTitle, "| Visits:", visitCount, "| Live:", isPublished);

const tags = ["html", "css", "javascript"];
console.log("Tags:", tags);

const card = {
  name: "Your Name or Product",
  role: "Student Developer",
  level: 1
};
console.log("Card object:", card);

let message = "Building my interactive page.";
console.log(message);
```

5. Open the page in the browser → DevTools → Console. Confirm messages appear with **no red errors**.
6. Commit with message: `Add JavaScript basics and console logging`.

**Mission output:**

- `script.js` linked and running
- Console screenshot with variable output visible
- One meaningful commit on GitHub

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block.

Students repeat the workflow independently **without looking at the tutorial**.

**Independent rebuild task:**

1. Add one new property to your `card` object and log it.
2. Add one new item to your `tags` array and log the full array.
3. Fix one typo if the Console shows a syntax error — read the line number carefully.
4. Commit: `Update card object and tags array`.

**Exit prompts:**

```text
My script tag is placed...
One string variable I used is...
One number variable I used is...
One object property I added is...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Explain HTML vs CSS vs JavaScript using your own page.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot of DevTools Console showing your log messages
2. GitHub link to `web-basics-project/script.js`
3. Screenshot or link showing today's commit
4. One sentence: "Today I changed ___ by adding JavaScript variables for ___."

## Success Criteria

You are successful if:

1. `script.js` is linked and runs without Console errors.
2. Your code uses strings, numbers, booleans, an array, and an object.
3. You can explain what each layer — HTML, CSS, JavaScript — does on your page.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Console is empty | Check `<script src="script.js">` path; both files in same folder. |
| Red syntax error | Read line number; check missing quotes, commas, or braces. |
| `Uncaught ReferenceError` | Variable used before declared; check spelling. |
| Page HTML broken | Make sure `<script>` is **before** `</body>`, not inside a tag. |

## Fast Track / Support Track

Fast track:

If most students complete this lesson in about 45 minutes, continue directly into [Lesson 2](lesson-02-functions-conditionals-and-user-input.md) during the same 90-minute block.

Use this only if students have working Console output and completed the independent rebuild.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
