# Lesson 3: DOM Selection and Page Updates

## Lesson Goal

Make your HTML/CSS page interactive by selecting elements with JavaScript and updating text, status messages, or CSS classes on the page.

By the end of this lesson, user actions or script logic should visibly change page content without reloading the browser.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on the DOM, `document.querySelector`, `document.querySelectorAll`, `textContent`, and `classList`. Change styles with CSS classes when possible — avoid inline styles unless necessary.

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
2. Work through the **DOM manipulation** sections — selecting elements, reading and changing content, and updating the page structure.
3. **Stop before Ajax/fetch sections.** Fetch is Lesson 5.
4. Focus on how JavaScript finds HTML elements and updates what the user sees.

**Step B — map the course to this project:**

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

## Talk Robin

Each student speaks once before anyone speaks twice.

**Share:**

1. What the DOM is in one sentence
2. One selector you used (`#id` or `.class`)
3. One element you update with `textContent`
4. One confusion or question

**Student output:** Group list of DOM patterns and unclear questions.

## Group Answer

As a group, prepare one shared answer:

```text
To change text on a page, you first...
# in a selector means...
.class in a selector means...
Our group still needs help with...
```

**Student output:** One group answer.

## Teacher Clarification

The teacher checks what students already understand before explaining.

**Teacher checks:**

1. Does Lesson 2 decision tool still work?
2. Do HTML elements have matching `id` values for selectors?
3. Can students explain `textContent` vs copying random `innerHTML` from the web?
4. Are students using CSS classes instead of many inline style changes?

**Teacher explanation rule:** Explain only the unclear parts. Do not run a full teacher-demo-first lesson.

The teacher explains only the common stuck points before the mission task.

## Mission Task

Students complete the main task.

**Task:**

1. Add ids to key elements in `index.html` if missing — for example:

```html
<h1 id="page-heading">Your Title</h1>
<p id="status-message">Ready</p>
<div id="info-card" class="card">...</div>
```

2. Add to `style.css`:

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

3. Add to `script.js`:

```javascript
const headingEl = document.querySelector("#page-heading");
const statusEl = document.querySelector("#status-message");
const cardEl = document.querySelector("#info-card");

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

// Demo: call one on load so you can see it work
showSuccess("Page connected to JavaScript.");
```

4. Connect your Lesson 2 decision tool: call `showSuccess` or `showError` based on the result instead of only logging to Console.
5. Refresh the browser — text and status class must update with **no red Console errors**.
6. Commit with message: `Add DOM selection and page updates`.

**Mission output:**

- At least two elements updated from JavaScript
- Status message uses CSS classes, not inline styles
- One meaningful commit on GitHub

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block.

Students repeat the workflow independently **without looking at the tutorial**.

**Independent rebuild task:**

1. Use test button: `<button type="button" id="toggle-status-btn">Toggle status</button>`.
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

## Evidence to Submit

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
