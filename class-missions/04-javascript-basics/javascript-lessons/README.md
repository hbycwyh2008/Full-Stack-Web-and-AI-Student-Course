# JavaScript Basics Mini-Unit

Make a static webpage interactive with JavaScript — variables, functions, DOM updates, form validation, and local JSON data.

## Unit Goal

By the end of this unit, each student should be able to extend their HTML/CSS project with JavaScript so the page responds to user actions, validates input, and loads data from a local JSON file.

This is not a full computer science JavaScript theory unit. The focus is practical web development: build, test, debug, and submit evidence.

## Prerequisites

Complete the [HTML/CSS Web Basics mini-unit](../../03-html-css-basics/web-basics-lessons/) first. You should already have:

- `web-basics-project/index.html`
- `web-basics-project/style.css`

You will add `script.js` and later `data.json` to the **same folder**.

## Lesson Sequence

| Lesson | File | Focus |
|---|---|---|
| 1 | [lesson-01-javascript-basics.md](lesson-01-javascript-basics.md) | Link JS, console, variables, types, arrays, objects |
| 2 | [lesson-02-functions-conditionals-and-user-input.md](lesson-02-functions-conditionals-and-user-input.md) | Functions, conditionals, decision logic (console first) |
| 3 | [lesson-03-dom-selection-and-page-updates.md](lesson-03-dom-selection-and-page-updates.md) | DOM selection, `textContent`, `classList`, page feedback |
| 4 | [lesson-04-events-and-form-validation.md](lesson-04-events-and-form-validation.md) | Events, form validation, user feedback |
| 5 | [lesson-05-fetch-json-and-mini-project.md](lesson-05-fetch-json-and-mini-project.md) | HTTP/Ajax intro, local JSON, `fetch`, final mini project |

**Estimated time:** 5 lessons × 90 minutes each if every Coursera-aligned segment is taught in class. Teachers may combine adjacent lessons when students move quickly.

Each lesson follows the standard **seven-block** classroom flow with time labels:

Entry Point Check → Individual Learning → Talk Round 1 → Entry Points Check / Teacher Diagnosis → Guided Practice → Exit Check → Evidence to Submit.

See [classroom-flow.md](../../shared/classroom-flow.md) and [talk-robin-rules.md](../../shared/talk-robin-rules.md).

## CS1 Scope Limits

This unit is part of the front-end foundation. Keep it practical and small:

- Use selected sections of the Coursera [Introduction to JavaScript and Ajax: Building Web Apps (JHU)](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu) only.
- Do **not** require closures, IIFEs, prototypes, constructor functions, jQuery, or the full restaurant backend SPA as core tasks.
- Use **local `data.json`** with `fetch` — do not require a public API or live backend server for this unit.
- HTML, CSS, and JavaScript together stay within the broader CS1 front-end lesson budget. Teachers may assign some catch-up Coursera items as homework.

## Curriculum Reference

This unit is aligned with Coursera [Introduction to JavaScript and Ajax: Building Web Apps (JHU)](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu) (Yaakov Chaikin). The course has **Module 1 — Introduction to Javascript** and **Module 2 — Using Javascript to Build Web Applications**. Most lessons target about **25 minutes** of viewing; longer segments may continue into Guided Practice or homework.

| Class lesson | Coursera module | Coursera items | Approx. viewing time |
|---|---|---|---|
| [Lesson 1](lesson-01-javascript-basics.md) | [Module 1](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu/home/module/1) | 2–5, 10, 12 | ~28 min total; item 12 may finish as homework |
| [Lesson 2](lesson-02-functions-conditionals-and-user-input.md) | [Module 1](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu/home/module/1) | 6–7 | ~22 min |
| [Lesson 3](lesson-03-dom-selection-and-page-updates.md) | [Module 2](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu/home/module/2) | 2–3 | ~24 min |
| [Lesson 4](lesson-04-events-and-form-validation.md) | [Module 2](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu/home/module/2) | 4–5 | ~22 min |
| [Lesson 5](lesson-05-fetch-json-and-mini-project.md) | [Module 2](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu/home/module/2) | 6–9 | ~30 min total; HTTP reading may be skimmed in class |

Item 1 in each module is optional orientation. Items on closures, namespaces, OOP depth, and the full restaurant backend connection are **teacher reference or homework only** — not core CS1 mission requirements.

Item numbers and titles should match the Coursera sidebar. If a title differs slightly, match by **item number**.

Coursera materials are a reference only — mission tasks and evidence requirements are original to this class.

## Final Project

In Lesson 5, build a mini project that loads and displays data from local `data.json`. Choose one:

- Student course list viewer
- Simple product card list
- Quote generator using local JSON
- AI tool directory
- Restaurant menu viewer
- Book recommendation list

## Expected Evidence

Submit evidence after every lesson:

- Updated code committed to GitHub
- Screenshot or browser preview
- Items listed in **Evidence to Submit** in each lesson file

At the end of the unit, your folder should include:

```text
web-basics-project/
├── index.html
├── style.css
├── script.js
├── data.json
└── README.md
```

See [Evidence Levels](../../../evidence-levels.md).

## Optional Extra Lesson

If your teacher assigns it, use one extra 90-minute block for debugging, refactoring, and portfolio polish:

- Fix Console errors with DevTools
- Clean up function and selector names
- Add the project to your Notion **Learning Projects** section

## Optional Support Files

- [../student-handout-js-syntax-bridge.md](../student-handout-js-syntax-bridge.md) — Python ↔ JS comparison for students with prior coding experience (if your teacher provides it)
- [../optional-javascript-interactive-profile.md](../optional-javascript-interactive-profile.md) — extra practice (optional, if your teacher provides it)

## Advanced Ideas (Teacher Reference Only)

These are **not** core student tasks in CS1. Mention briefly if students ask; do not assign as mission requirements:

- prototypes, constructor functions, `this`
- IIFE, closures, namespaces

## Deprecated Materials

- [../lesson-01-javascript-in-the-browser.md](../lesson-01-javascript-in-the-browser.md)
- [../lesson-02-dom-selection-and-content.md](../lesson-02-dom-selection-and-content.md)
- [../lesson-03-events-and-functions.md](../lesson-03-events-and-functions.md)

Use this 5-lesson sequence instead.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
