# Lesson 2: Functions, Conditionals, and User Input

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Write a function with at least one parameter and a `return` value.
2. Use `if` / `else if` / `else` with comparison operators.
3. Test decision logic in the Console before connecting it to the page in [Lesson 3](lesson-03-dom-selection-and-page-updates.md).
4. Submit daily evidence listed below.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on functions, parameters, return values, and `if` / `else` logic. Keep output in the **Console** for now — DOM updates and input fields on the page come in [Lesson 3](lesson-03-dom-selection-and-page-updates.md).

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–25 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra JavaScript tutorials during class.

**Required resource — [Introduction to JavaScript and Ajax, Module 1](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu/home/module/1)** (JHU / Yaakov Chaikin).

**Class time target:** watch **items 6 and 7** during the 10–25 minute block. That is about 22 minutes.

Do **not** open Module 2 yet. DOM and events start in [Lesson 3](lesson-03-dom-selection-and-page-updates.md).

| Coursera item # | Title | ~Time | When to use |
|---|---|---|---|
| 6 | Lecture: Flow Control | 10 min | **Core in class** |
| 7 | Lecture: Functions Explained | 12 min | **Core in class** |
| 8 | Reading: Working with Functions | 5 min | Skim in class or homework |

**Stop here.** Do **not** open item 2 in Module 2 (DOM) until [Lesson 3](lesson-03-dom-selection-and-page-updates.md).

Focus on how functions take input, make a decision, and return a result.

**Map the course to this project:**

Add a simple decision tool to `script.js`. Choose **one** topic:

| Tool type | Example logic |
|---|---|
| Age checker | If age ≥ 13, show one message; else show another |
| Course recommendation | If score ≥ 80, recommend advanced track; else review track |
| Login message checker | If username length > 0, welcome message; else prompt to enter name |
| Quiz score feedback | If score ≥ 70, pass message; else retry message |

Test with `console.log(getFeedback("85"))` and other values — not on the page yet.

**Individual notes:**

```text
A function is...
A parameter is...
return sends back...
if checks whether...
One decision my tool makes is...
One thing I still do not understand is...
```

**Student output:** One working decision function tested in the Console.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. Which decision tool you chose
2. One parameter your function accepts
3. One condition your `if` statement checks
4. One confusion or question

**Pair summary:** Agree on one decision-tool pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
A function with a parameter is useful because...
An if/else statement helps when...
Our decision tool checks...
Our group still needs help with...
```

**Teacher checks:**

1. Does Lesson 1 `script.js` still run without errors?
2. Can students explain parameter vs argument?
3. Can students read function return values in the Console?
4. Are students comparing strings and numbers correctly? (`"5"` vs `5`)

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. Add a decision function to `script.js`:

```javascript
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

console.log("Empty test:", getFeedback(""));
console.log("Middle test:", getFeedback("65"));
console.log("High test:", getFeedback("90"));
```

2. Change the thresholds and messages to fit **your** decision tool topic.
3. Rename the function to match your topic (for example, `getScoreFeedback`).
4. Test at least three values in the Console: empty string, a middle value, a high value.
5. Commit with message: `Add decision tool with functions and conditionals`.

**Mission output:**

- Working decision function with `if` / `else if` / `else`
- Console logs showing at least three test results
- One meaningful commit on GitHub

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Add one more `else if` branch with your own message.
2. Log one test value that triggers your new branch.
3. Be ready to explain what happens when the input is empty.
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

## Evidence to Submit (85–90 min)

1. Screenshot of Console showing at least three logged decision results
2. GitHub link to updated `script.js`
3. One sentence: "Today I changed ___ by adding function ___ that checks ___."

## Success Criteria

You are successful if:

1. Your function uses at least one parameter and `return`.
2. Your code uses `if` / `else if` / `else` with comparison operators.
3. You tested at least three inputs in the Console with clear results.
4. You made a meaningful commit on GitHub.
5. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| Function returns `undefined` | Add `return` before the message string. |
| Condition never matches | Log the test value in Console; check `Number()` for numeric input. |
| Empty input crashes logic | Check `value.trim() === ""` first. |
| `value.trim is not a function` | Pass a string to the function, not a number literal without quotes. |

## Fast Track / Support Track

Fast track:

If most students finish early, preview [Lesson 3](lesson-03-dom-selection-and-page-updates.md) DOM selectors only if evidence is complete.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
