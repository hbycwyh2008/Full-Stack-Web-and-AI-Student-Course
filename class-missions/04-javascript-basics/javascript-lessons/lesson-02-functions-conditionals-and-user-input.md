# Lesson 2: Functions, Conditionals, and User Input

## Lesson Goal

Write simple functions and conditionals that respond to user input — for example, an age checker, course recommendation tool, login message checker, or quiz score feedback tool.

By the end of this lesson, your page should read a value from an input field and display a decision message in the Console or on the page.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on functions, parameters, return values, `if` / `else if` / `else`, comparison operators, and reading basic input from form fields. Keep DOM updates minimal — full page updates come in Lesson 3.

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
2. Work through the **functions and conditionals** sections — declaring functions, parameters, return values, and `if` / `else` logic.
3. **Stop before DOM manipulation sections.** DOM updates are Lesson 3.
4. Focus on how functions take input, make a decision, and return a result.

**Step B — map the course to this project:**

Add a simple decision tool to `web-basics-project/`. Choose **one**:

| Tool type | Example logic |
|---|---|
| Age checker | If age ≥ 13, show one message; else show another |
| Course recommendation | If score ≥ 80, recommend advanced track; else review track |
| Login message checker | If username length > 0, welcome message; else prompt to enter name |
| Quiz score feedback | If score ≥ 70, pass message; else retry message |

**Individual notes:**

```text
A function is...
A parameter is...
return sends back...
if checks whether...
Reading input.value gives...
One decision my tool makes is...
One thing I still do not understand is...
```

**Student output:** One working decision function connected to an input field.

## Talk Robin

Each student speaks once before anyone speaks twice.

**Share:**

1. Which decision tool you chose
2. One parameter your function accepts
3. One condition your `if` statement checks
4. One confusion or question

**Student output:** Group list of decision-tool ideas and unclear questions.

## Group Answer

As a group, prepare one shared answer:

```text
A function with a parameter is useful because...
An if/else statement helps when...
Our decision tool checks...
Our group still needs help with...
```

**Student output:** One group answer.

## Teacher Clarification

The teacher checks what students already understand before explaining.

**Teacher checks:**

1. Does Lesson 1 `script.js` still run without errors?
2. Can students explain parameter vs argument?
3. Can students read `document.querySelector("#my-input").value`?
4. Are students comparing strings and numbers correctly? (`"5"` vs `5`)

**Teacher explanation rule:** Explain only the unclear parts. Do not run a full teacher-demo-first lesson.

The teacher explains only the common stuck points before the mission task.

## Mission Task

Students complete the main task.

**Task:**

1. Add to `index.html` inside your main content area:

```html
<section id="decision-tool">
  <h2>Quick Check</h2>
  <label for="user-input">Enter a value:</label>
  <input type="text" id="user-input" placeholder="e.g. score or age">
  <button type="button" id="check-btn">Check</button>
  <p id="decision-result"></p>
</section>
```

2. Add to `script.js`:

```javascript
const inputEl = document.querySelector("#user-input");
const resultEl = document.querySelector("#decision-result");
const checkBtn = document.querySelector("#check-btn");

function getFeedback(value) {
  const number = Number(value);

  if (value.trim() === "") {
    return "Please enter a value first.";
  } else if (number >= 80) {
    return "Strong result — keep going!";
  } else if (number >= 50) {
    return "Good progress — review and retry.";
  } else {
    return "Needs more practice — ask for help.";
  }
}

function runCheck() {
  const message = getFeedback(inputEl.value);
  resultEl.textContent = message;
  console.log("Decision:", message);
}

checkBtn.addEventListener("click", runCheck);
```

3. Change the thresholds and messages to fit **your** decision tool topic.
4. Test at least three inputs: empty, a middle value, a high value.
5. Commit with message: `Add decision tool with functions and conditionals`.

**Mission output:**

- Working decision tool with function + conditionals
- Console log showing decision output
- One meaningful commit on GitHub

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block.

Students repeat the workflow independently **without looking at the tutorial**.

**Independent rebuild task:**

1. Add one more `else if` branch with your own message.
2. Rename your function to match your tool topic (for example, `getScoreFeedback`).
3. Test your new branch with a value that triggers it.
4. Commit: `Add extra conditional branch to decision tool`.

**Exit prompts:**

```text
My function is called...
It takes this parameter...
It returns...
One if condition checks...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Read your function aloud and explain what happens when the input is empty.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot showing your decision tool with a result message on the page
2. Screenshot of Console showing a logged decision
3. GitHub link to updated `script.js`
4. One sentence: "Today I changed ___ by adding function ___ that checks ___."

## Success Criteria

You are successful if:

1. Your function uses at least one parameter and `return`.
2. Your code uses `if` / `else if` / `else` with comparison operators.
3. Your tool reads input and shows a clear result message.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Function returns `undefined` | Add `return` before the message string. |
| Condition never matches | Log `inputEl.value` in Console; check `Number()` for numeric input. |
| Empty input crashes logic | Check `value.trim() === ""` first. |
| Button does nothing | Confirm `addEventListener("click", runCheck)` — pass function name without `()`. |

## Fast Track / Support Track

Fast track:

If most students finish early, preview [Lesson 3](lesson-03-dom-selection-and-page-updates.md) DOM selectors only if evidence is complete.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
