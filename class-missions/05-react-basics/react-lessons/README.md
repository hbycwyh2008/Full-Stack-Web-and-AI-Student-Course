# React Basics Mini-Unit

Build one growing React + Vite app in `react-practice/` — from the **ReactFacts** static site through **Travel Journal** props and lists, then **state**, **forms**, and **`fetch`**.

## Unit Goal

By the end of this unit, each student should be able to build a React app in `react-practice/` that:

- Uses JSX, components, props, and state
- Includes a completed ReactFacts static page (Module 2)
- Renders a Travel Journal–style list from an array with `.map()` and `key`
- Handles form input and conditional UI
- Calls `fetch()` and shows loading or error feedback in the UI

Work in one folder — `react-practice/` — and grow the same project across all seven lessons.

## Prerequisites

Complete the [JavaScript mini-unit](../../04-javascript-basics/javascript-lessons/) first. You should understand:

- Variables, functions, arrays, objects
- DOM updates and form validation with vanilla JS
- `fetch()` with local JSON or a simple public endpoint

## Lesson Sequence

| Lesson | File | Coursera focus | Class mission |
|---|---|---|---|
| 1 | [lesson-01-jsx-and-first-components.md](lesson-01-jsx-and-first-components.md) | Module 1 — Getting Started | Vite setup, JSX, first component |
| 2 | [lesson-02-components-and-styling.md](lesson-02-components-and-styling.md) | Module 2 — Building with React | **ReactFacts** — components + CSS |
| 3 | [lesson-03-props-and-reusable-components.md](lesson-03-props-and-reusable-components.md) | Module 4 — Props | Travel Journal `Entry` with props |
| 4 | [lesson-04-lists-map-and-keys.md](lesson-04-lists-map-and-keys.md) | Module 5 — Arrays | Map journal entries from data |
| 5 | [lesson-05-state-and-events.md](lesson-05-state-and-events.md) | Module 7–8 (partial) | `useState`, events, toggle |
| 6 | [lesson-06-forms-and-conditional-ui.md](lesson-06-forms-and-conditional-ui.md) | Module 8–9 (partial) | Forms, conditional UI |
| 7 | [lesson-07-useeffect-and-fetch.md](lesson-07-useeffect-and-fetch.md) | Module 12–13 (partial) | `useEffect`, `fetch`, checkpoint |

**Estimated time:** 7 lessons × 90 minutes each.

Each lesson follows the standard **seven-block** classroom flow with time labels:

Entry Point Check → Individual Learning → Talk Round 1 → Entry Points Check / Teacher Diagnosis → Guided Practice → Exit Check → Evidence to Submit.

See [classroom-flow.md](../../shared/classroom-flow.md) and [talk-robin-rules.md](../../shared/talk-robin-rules.md).

## CS1 Scope Limits

Do **not** teach as core requirements in this unit:

- Next.js, React Router, Redux, Zustand
- Authentication, databases, server components
- Coursera capstone modules (Tenzies, Assembly: Endgame) as class missions
- Module 10 API Integration / AI chef challenges (optional teacher extension only)
- Full Coursera certificate completion in class time

## Curriculum Reference

This unit is aligned with the Coursera course [Learn React](https://www.coursera.org/learn/learn-react) (Bob Ziroll / Scrimba). The course has **20 modules** on Coursera; CS1 uses **7 class lessons** mapped to **9 content modules** below. Test/quiz modules (3, 6, 11, 14, 15–20) are optional homework only.

**Self-study rule:** Watch Coursera **only** during **Individual Learning** (or as assigned homework). Maximum **~30 minutes** of in-class viewing per lesson. **Do not open Coursera during Guided Practice, Exit Check, or independent rebuild** — those blocks are hands-on coding only.

Item titles and numbers below were verified against the Coursera course API (June 2026). **Item numbers restart at 1 inside each module.**

| Class lesson | Coursera module | Module title | Assigned items |
|---|---|---|---|
| [Lesson 1](lesson-01-jsx-and-first-components.md) | [Module 1](https://www.coursera.org/learn/learn-react/home/module/1) | Static pages in React 01 — Getting Started | IL: 3–6, 9–10 (~26 min) |
| [Lesson 2](lesson-02-components-and-styling.md) | [Module 2](https://www.coursera.org/learn/learn-react/home/module/2) | Static pages in React 02 — Building with React | IL: 1, 3–4, 6–8 (~30 min); HW: 9–15 (~36 min) |
| [Lesson 3](lesson-03-props-and-reusable-components.md) | [Module 4](https://www.coursera.org/learn/learn-react/home/module/4) | Data-Driven React 01 — Understanding Props | 5–6, 9–10, 12 (~26 min) |
| [Lesson 4](lesson-04-lists-map-and-keys.md) | [Module 5](https://www.coursera.org/learn/learn-react/home/module/5) | Data-Driven React 02 — Arrays and Advanced Props | 3, 5–8 (~28 min) |
| [Lesson 5](lesson-05-state-and-events.md) | [Module 7](https://www.coursera.org/learn/learn-react/home/module/7) + [Module 8](https://www.coursera.org/learn/learn-react/home/module/8) | Events + State basics | M7: 5; M8: 1–3, 5, 10 (~28 min) |
| [Lesson 6](lesson-06-forms-and-conditional-ui.md) | [Module 8](https://www.coursera.org/learn/learn-react/home/module/8) + [Module 9](https://www.coursera.org/learn/learn-react/home/module/9) | Forms + Conditional Rendering | M8: 15, 17, 19; M9: 2, 5 (~27 min) |
| [Lesson 7](lesson-07-useeffect-and-fetch.md) | [Module 12](https://www.coursera.org/learn/learn-react/home/module/12) + [Module 13](https://www.coursera.org/learn/learn-react/home/module/13) | Side Effects — Meme Generator + fetch/useEffect | M12: 4–5; M13: 1–3 (~25 min) |

### Module 2 — what students learn

[Module 2](https://www.coursera.org/learn/learn-react/home/module/2) is the **ReactFacts** project. Students should **not** build a separate portfolio layout in this lesson. The Coursera module covers:

1. ReactFacts markup preview
2. Custom components and parent/child composition
3. Fragments and styling with CSS classes
4. Organizing files and completing the ReactFacts navbar, main content, bullets, and background

Lessons 3–4 follow the **Travel Journal** arc (Modules 4–5) by adding journal `Entry` components below the ReactFacts section in the same app.

Coursera materials are a reference only — mission tasks and evidence are original to this class.

## Final Project (Lesson 7)

Submit a working `react-practice/` app that includes:

- ReactFacts static page (Navbar, Main, styled facts list)
- Travel Journal entries with props and `.map()`
- Interactive state (toggle or form)
- `fetch()` with loading and error UI
- Updated `README.md` with run instructions and what you learned

## Expected Evidence

Submit evidence after every lesson:

- Screenshot of running app in browser
- GitHub link to changed files
- Items listed in **Evidence to Submit** in each lesson file

At the end of the unit:

```text
react-practice/
├── src/
│   ├── App.jsx
│   ├── main.jsx
│   ├── App.css
│   └── components/
│       ├── Navbar.jsx
│       ├── Main.jsx
│       ├── Footer.jsx
│       ├── Entry.jsx
│       └── ...
├── public/
├── README.md
└── package.json
```

See [Evidence Levels](../../../evidence-levels.md).

## Optional Extra Lesson

If your teacher assigns it, use one extra 90-minute block for debugging, refactoring, and portfolio polish:

- Fix Console errors in DevTools
- Improve component and CSS organization
- Add the project to your Notion **Learning Projects** section

## Optional Support

- [../optional-react-component-portfolio.md](../optional-react-component-portfolio.md) — extra component practice

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
