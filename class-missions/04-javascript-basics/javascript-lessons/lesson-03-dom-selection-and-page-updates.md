# Lesson 3: DOM Selection and Page Updates

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain what the DOM is in one sentence.
2. Select elements with `document.querySelector` and `document.querySelectorAll`.
3. Change page text with `textContent` and status styling with `classList`.
4. Connect the [Lesson 2](lesson-02-functions-conditionals-and-user-input.md) decision tool to visible page feedback.
5. Submit daily evidence listed below.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on the DOM, `querySelector`, `textContent`, and `classList`. Change styles with CSS classes when possible — avoid inline styles unless necessary. Do **not** start Ajax/fetch yet — that is [Lesson 5](lesson-05-fetch-json-and-mini-project.md).

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–25 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra JavaScript tutorials during class.

**Required resource — [Introduction to JavaScript and Ajax, Module 2](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu/home/module/2)** (JHU / Yaakov Chaikin).

**Class time target:** watch **items 2 and 3** during the 10–25 minute block. That is about 24 minutes.

Item 1 is optional orientation. Items 4–5 move to [Lesson 4](lesson-04-events-and-form-validation.md). Ajax and JSON move to [Lesson 5](lesson-05-fetch-json-and-mini-project.md).

| Coursera item # | Title | ~Time | When to use |
|---|---|---|---|
| 2 | Lecture: The Document Object Model (DOM) Concept | 10 min | **Core in class** |
| 3 | Lecture: Traversing the DOM | 14 min | **Core in class** |

**Stop here.** Do **not** open item 4 (Handling Events) until [Lesson 4](lesson-04-events-and-form-validation.md).

**Map the course to this project:**

| Course concept | What to add to `web-basics-project/` |
|---|---|
| DOM | The live tree of page elements JavaScript can change |
| `querySelector("#id")` | Select one element by id |
| `querySelectorAll(".class")` | Select multiple elements |
| `textContent` | Change visible text safely |
| `classList.add/remove/toggle` | Switch CSS classes for status styling |
| HTML/CSS first | Keep structure in HTML, look in CSS, behavior in JS |

Add `id` attributes to HTML elements you want JavaScript to control. Add CSS classes like `.status-success` and `.status-error` in `style.css`.

**Individual notes:**

```text
The DOM is...
querySelector("#id") returns...
textContent changes...
classList.toggle helps because...
JavaScript should not replace good HTML/CSS because...
One element I will update is...
One thing I still do not understand is...
```

**Student output:** Page with at least two JavaScript-driven content or class updates.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. What the DOM is in one sentence
2. One selector you used (`#id` or `.class`)
3. One element you update with `textContent`
4. One confusion or question

**Pair summary:** Agree on one DOM update pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
To change text on a page, you first...
# in a selector means...
.class in a selector means...
Our group still needs help with...
```

**Teacher checks:**

1. Does the Lesson 2 decision function still work in the Console?
2. Do HTML elements have matching `id` values for selectors?
3. Can students explain `textContent` vs copying random `innerHTML` from the web?
4. Are students using CSS classes instead of many inline style changes?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. Add ids to key elements in `index.html` if missing — for example:

```html
<h1 id="page-heading">Your Title</h1>
<p id="status-message">Ready</p>
<div id="info-card" class="card">...</div>
```

2. Add a decision-tool section to `index.html`:

```html
<section id="decision-tool">
  <h2>Quick Check</h2>
  <label for="user-input">Enter a value:</label>
  <input type="text" id="user-input" placeholder="e.g. score or age">
  <button type="button" id="check-btn">Check</button>
  <p id="decision-result"></p>
</section>
```

3. Add to `style.css`:

```css
.status-success {
  color: #166534;
  background-color: #dcfce7;
  padding: 8px;
  border-radius: 6px;
}

.status-error {
  color: #991b1b;
  background-color: #fee2e2;
  padding: 8px;
  border-radius: 6px;
}
```

4. Add to `script.js`:

```javascript
const headingEl = document.querySelector("#page-heading");
const statusEl = document.querySelector("#status-message");
const inputEl = document.querySelector("#user-input");
const resultEl = document.querySelector("#decision-result");
const checkBtn = document.querySelector("#check-btn");

headingEl.textContent = "Updated by JavaScript";

function showSuccess(message) {
  statusEl.textContent = message;
  statusEl.classList.remove("status-error");
  statusEl.classList.add("status-success");
}

function showError(message) {
  statusEl.textContent = message;
  statusEl.classList.remove("status-success");
  statusEl.classList.add("status-error");
}

function runCheck() {
  const message = getFeedback(inputEl.value);
  resultEl.textContent = message;

  if (message.includes("Please enter")) {
    showError(message);
  } else {
    showSuccess(message);
  }
}

checkBtn.addEventListener("click", runCheck);
showSuccess("Page connected to JavaScript.");
```

5. Use your **Lesson 2** `getFeedback` function — do not rewrite the logic from scratch unless needed.
6. Refresh the browser — text and status class must update with **no red Console errors**.
7. Commit with message: `Add DOM selection and page updates`.

**Mission output:**

- At least two elements updated from JavaScript
- Lesson 2 decision tool shows feedback on the page
- Status message uses CSS classes, not inline styles
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add `<button type="button" id="toggle-status-btn">Toggle status</button>`.
2. Use `classList.toggle("status-success")` or swap messages when clicked.
3. Confirm the page still looks correct in your CSS layout.
4. Commit: `Add status toggle with classList`.

**Exit prompts:**

```text
My selector for the heading is...
textContent on my page changes...
classList helps because...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Point to one selector, one element, and explain what changes when your script runs.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot showing JavaScript-updated text and status styling on the page
2. GitHub links to updated `index.html`, `style.css`, and `script.js`
3. One sentence: "Today I changed ___ by selecting ___ and updating ___."

## Success Criteria

You are successful if:

1. You use `querySelector` to select at least two elements.
2. You change page text with `textContent`.
3. You use `classList` to apply at least one CSS class from JavaScript.
4. Your Lesson 2 decision tool shows feedback on the page, not only in Console.
5. You made a meaningful commit on GitHub.

## Common Problems

| Problem | Try first |
|---|---|
| `Cannot read properties of null` | Check `id` spelling in HTML and selector (`#` for id). |
| Nothing changes | Save all files; hard refresh (Cmd+Shift+R / Ctrl+Shift+R). |
| Class has no visual effect | Define the class in `style.css` first. |
| Layout breaks | JavaScript should change content/classes, not rebuild entire HTML structure. |

## Fast Track / Support Track

Fast track:

If most students finish early, preview [Lesson 4](lesson-04-events-and-form-validation.md) form submit handling only if evidence is complete.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
