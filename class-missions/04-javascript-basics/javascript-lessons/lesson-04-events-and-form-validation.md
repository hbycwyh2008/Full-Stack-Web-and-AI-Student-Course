# Lesson 4: Events and Form Validation

## Lesson Goal

Handle user events and validate a simple form so required fields cannot be submitted empty, and clear success or error messages appear on the page.

By the end of this lesson, your page should include an interactive form — login, contact, student profile, or course registration — with client-side validation feedback.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on `addEventListener`, click and submit events, `event.preventDefault()`, reading input values, and showing validation messages. This prepares you for loading JSON data in Lesson 5.

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
2. Work through the **events and form handling** sections — event listeners, click handlers, and responding to user actions.
3. **Stop before Ajax/fetch sections.** Fetch is Lesson 5.
4. Focus on how JavaScript listens for events and reacts without reloading the page.

**Step B — map the course to this project:**

Choose **one** form type and add it to `web-basics-project/`:

| Form type | Required fields (minimum) |
|---|---|
| Login form | username/email, password |
| Contact form | name, email, message |
| Student profile form | name, grade level, interest |
| Course registration | name, course choice |

Use your existing CSS card/container styles. Show feedback in a `<p id="form-feedback">` element using Lesson 3 status classes.

**Individual notes:**

```text
addEventListener attaches...
submit event fires when...
preventDefault stops...
Empty field validation checks...
Success message shows when...
Error message shows when...
One thing I still do not understand is...
```

**Student output:** Form with validation messages visible on the page.

## Talk Robin

Each student speaks once before anyone speaks twice.

**Share:**

1. Which form type you chose
2. One event your script listens for
3. What `preventDefault()` does on submit
4. One confusion or question

**Student output:** Group list of validation patterns and unclear questions.

## Group Answer

As a group, prepare one shared answer:

```text
We use preventDefault on submit because...
An empty field check looks like...
A success message should...
Our group still needs help with...
```

**Student output:** One group answer.

## Teacher Clarification

The teacher checks what students already understand before explaining.

**Teacher checks:**

1. Do Lesson 3 DOM updates and status classes still work?
2. Can students pass a function to `addEventListener` without calling it immediately?
3. Do forms use `<label for="...">` matched to input `id`?
4. Are students validating before showing success?

**Teacher explanation rule:** Explain only the unclear parts. Do not run a full teacher-demo-first lesson.

The teacher explains only the common stuck points before the mission task.

## Mission Task

Students complete the main task.

**Task:**

1. Add a form to `index.html` — example contact form:

```html
<section id="contact-section" class="card">
  <h2>Contact</h2>
  <form id="contact-form">
    <label for="contact-name">Name</label>
    <input type="text" id="contact-name" name="name" required>

    <label for="contact-email">Email</label>
    <input type="email" id="contact-email" name="email" required>

    <label for="contact-message">Message</label>
    <textarea id="contact-message" name="message" rows="3" required></textarea>

    <button type="submit">Send</button>
  </form>
  <p id="form-feedback"></p>
</section>
```

2. Add validation to `script.js`:

```javascript
const contactForm = document.querySelector("#contact-form");
const feedbackEl = document.querySelector("#form-feedback");

function validateContactForm(name, email, message) {
  if (name.trim() === "") {
    return { ok: false, message: "Name is required." };
  }
  if (email.trim() === "") {
    return { ok: false, message: "Email is required." };
  }
  if (message.trim() === "") {
    return { ok: false, message: "Message is required." };
  }
  return { ok: true, message: "Form looks good — ready to submit (demo only)." };
}

contactForm.addEventListener("submit", function (event) {
  event.preventDefault();

  const name = document.querySelector("#contact-name").value;
  const email = document.querySelector("#contact-email").value;
  const message = document.querySelector("#contact-message").value;

  const result = validateContactForm(name, email, message);

  feedbackEl.textContent = result.message;

  if (result.ok) {
    feedbackEl.classList.remove("status-error");
    feedbackEl.classList.add("status-success");
  } else {
    feedbackEl.classList.remove("status-success");
    feedbackEl.classList.add("status-error");
  }
});
```

3. Adapt field names and messages to **your** form type.
4. Test: submit empty → error message; fill all fields → success message.
5. Confirm the page does **not** reload on submit.
6. Commit with message: `Add form validation with event listeners`.

**Mission output:**

- Interactive form with submit handler
- Empty-field validation with clear feedback
- One meaningful commit on GitHub

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block.

Students repeat the workflow independently **without looking at the tutorial**.

**Independent rebuild task:**

1. Add one extra validation rule — for example, message must be at least 10 characters.
2. Add a **Clear** button that resets the form and feedback message.
3. Test both buttons without reloading the page.
4. Commit: `Add message length check and clear button`.

**Exit prompts:**

```text
My form listens for...
preventDefault is needed because...
Empty field check returns...
Success feedback looks like...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Explain what happens when the user clicks Submit with an empty email field.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot showing error message after empty submit
2. Screenshot showing success message after valid submit
3. GitHub link to updated `script.js` with `addEventListener` and validation
4. One sentence: "Today I changed ___ by validating ___ on form submit."

## Success Criteria

You are successful if:

1. Your form uses `addEventListener("submit", ...)` with `preventDefault()`.
2. Empty required fields show a clear error message on the page.
3. Valid input shows a success message on the page.
4. The page does not reload when the form is submitted.
5. You made a meaningful commit on GitHub.

## Common Problems

| Problem | Try first |
|---|---|
| Page reloads on submit | Add `event.preventDefault()` inside submit handler. |
| Button does nothing | Check form `id` and selector match. |
| Validation always fails | Log each field value in Console; check `trim()`. |
| Feedback not visible | Confirm `#form-feedback` exists and status CSS classes are defined. |

## Fast Track / Support Track

Fast track:

If most students finish early, preview [Lesson 5](lesson-05-fetch-json-and-mini-project.md) local JSON structure only if evidence is complete.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
