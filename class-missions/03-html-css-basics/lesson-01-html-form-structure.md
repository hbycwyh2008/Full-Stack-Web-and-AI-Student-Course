# Lesson 1: HTML Form Structure

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain what a web form is used for.
2. Build HTML form structure with `<form>`, `<label>`, `<input>`, `<textarea>`, and `<button>`.
3. Connect each `<label>` to its control with `for` and `id`.
4. Add `name` attributes for future form data submission.
5. Save work in `html-css-first-form/` with at least one commit.
6. Submit evidence of an unstyled working form in the browser.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on the pattern you need for today's mission. Do not collect extra tutorials during the first learning block.

## Entry Point Check

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra playlists during class.

**Step A — MDN reading:**

1. Open: https://developer.mozilla.org/en-US/docs/Learn_web_development/Extensions/Forms/Your_first_form
2. Read only:
   - What are web forms?
   - Designing your form
   - Implementing our form HTML (through `<button>`)
3. Do **not** read CSS sections yet.

**Individual notes:**

```text
A web form is for...
action and method on form mean...
Each label needs for because...
input vs textarea difference is...
One thing I still do not understand is...
```

## Talk Robin

**Share:**

1. Why forms matter for the AI School Assistant later
2. What `type="email"` does
3. What happens when you click a label
4. One question

## Group Answer

```text
A well-structured HTML form must include...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:**

1. Phase 1 Notion portfolio link still in your README?
2. Editor + browser ready?
3. Can students explain label/input connection?

The teacher explains only the common stuck points before the mission task.

## Mission Task

**Task:**

1. Create folder `html-css-first-form/`.
2. Build `index.html` with full document structure.
3. Add contact form:
   - Name — `<input type="text">`
   - Email — `<input type="email">`
   - Message — `<textarea>`
   - Submit — `<button type="submit">Send your message</button>`
4. Every label has `for`; every input has matching `id` and `name`.
5. Open in browser; click each label to test focus.
6. Commit: `Add HTML structure for contact form`.

## Independent Rebuild

**Independent rebuild:**

1. Add one more labeled text field without MDN.
2. Explain `action` on `<form>` in one sentence.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot of unstyled form in browser
2. GitHub link to `html-css-first-form/index.html`
3. Commit history screenshot or link
4. One sentence: “Each label needs a for attribute because...”

## Success Criteria

1. Form opens in browser with all fields.
2. Labels activate correct fields on click.
3. Meaningful commit on GitHub.
4. Student can explain HTML structure vs CSS (Lesson 2).
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Blank page | Check `<body>` and form inside it. |
| Label click fails | Match `for` on label to `id` on input. |

## Fast Track / Support Track

Fast track:

Continue into [Lesson 2](lesson-02-html-form-styling-and-github.md) in the same block if evidence is complete.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
