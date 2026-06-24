# Lesson 5: Fetch, JSON, and Mini Project

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain what JSON is and why data can live outside HTML.
2. Load local `data.json` with `fetch` and render items on the page.
3. Show a user-friendly message when loading fails.
4. Complete the Phase 3 mini project with README and rubric self-check.
5. Submit final unit evidence listed below.

## Required Resource

Open only the resource named in `Individual Learning`. If the resource is longer than 15 minutes, complete the assigned section in class and finish the rest as homework if your teacher assigns it.

## What to Focus On

Focus on JSON structure, HTTP/Ajax concepts, `fetch("data.json")`, `.then()`, basic error handling, and rendering data into the DOM. Use **local JSON first** — do not require a public API or restaurant backend for this unit.

## Entry Point Check (0–10 min)

Use the first 10 minutes to answer these before new instruction:

- What do I already know that connects to today?
- What file, tool, or concept should I open first?
- What is one question I need answered before the mission?

## Individual Learning (10–25 min)

> [!NOTE]
> **One required resource** for this block — see below. Do not browse extra JavaScript tutorials during class.

**Required resource — [Introduction to JavaScript and Ajax, Module 2](https://www.coursera.org/learn/introduction-to-javascript-and-ajax-building-web-apps-jhu/home/module/2)** (JHU / Yaakov Chaikin).

**Class time target:** watch **items 7, 8, and 9** during the 10–25 minute block. That is about 24 minutes. Skim **item 6** (HTTP reading) as homework if your teacher assigns it.

The restaurant backend SPA at the end of Module 2 is **reference only** — this class uses local `data.json` instead.

| Coursera item # | Title | ~Time | When to use |
|---|---|---|---|
| 6 | Reading: HTTP Basics | 8 min | Skim in class or homework |
| 7 | Lecture: Ajax — Part 1 | 10 min | **Core in class** |
| 8 | Lecture: Ajax — Part 2 | 8 min | **Core in class** |
| 9 | Lecture: JSON | 6 min | **Core in class** |

**Stop here for new course topics.** Later Module 2 items about the full restaurant backend are optional teacher reference.

Map Coursera examples to **local** `data.json` in your repo — same pattern, more reliable for beginners.

**Choose your final project:**

| Project | Example `data.json` content |
|---|---|
| Student course list viewer | course name, level, description |
| Simple product card list | name, price, tagline |
| Quote generator | quote, author |
| AI tool directory | tool name, purpose, link |
| Restaurant menu viewer | item, price, category |
| Book recommendation list | title, author, genre |

**Individual notes:**

```text
JSON is...
fetch("data.json") loads...
.then runs when...
Hardcoded HTML is different from loaded data because...
If fetch fails, I should...
My final project type is...
One thing I still do not understand is...
```

**Student output:** Draft `data.json` structure with at least three items.

## Talk Round 1 (25–40 min)

Each student speaks once before anyone speaks twice. See [talk-robin-rules.md](../../shared/talk-robin-rules.md).

**Share:**

1. Which final project you chose
2. One property each JSON object will have
3. Where loaded data will appear on the page
4. One confusion or question

**Pair summary:** Agree on one JSON field pattern and one question for the teacher.

## Entry Points Check / Teacher Diagnosis (40–55 min)

**Group answer:**

```text
JSON stores data as...
fetch is useful because...
If data.json is missing, we should...
Our group still needs help with...
```

**Teacher checks:**

1. Do Lessons 1–4 features still work on the same page?
2. Can students open `data.json` in the editor and validate array/object shape?
3. Do students know `fetch` must run from a served page or local server if `file://` blocks fetch? (Teacher may demo Live Server or similar.)
4. Are students using `.catch()` or basic error handling?

The teacher explains only the common stuck points before Guided Practice.

## Guided Practice (55–75 min)

**Task:**

1. Create `web-basics-project/data.json` — example course list:

```json
[
  {
    "id": 1,
    "name": "HTML Page Structure",
    "level": "Beginner",
    "summary": "Build semantic HTML pages."
  },
  {
    "id": 2,
    "name": "CSS Layout Basics",
    "level": "Beginner",
    "summary": "Style pages with external CSS."
  },
  {
    "id": 3,
    "name": "JavaScript Interactivity",
    "level": "Intermediate",
    "summary": "Make pages respond to users."
  }
]
```

2. Add a display area to `index.html`:

```html
<section id="data-section" class="card">
  <h2>Loaded Data</h2>
  <button type="button" id="load-data-btn">Load items</button>
  <p id="data-status">Click the button to load data.</p>
  <ul id="data-list"></ul>
</section>
```

3. Add fetch logic to `script.js`:

```javascript
const loadDataBtn = document.querySelector("#load-data-btn");
const dataStatusEl = document.querySelector("#data-status");
const dataListEl = document.querySelector("#data-list");

function renderItems(items) {
  dataListEl.innerHTML = "";

  items.forEach(function (item) {
    const li = document.createElement("li");
    li.textContent = item.name + " — " + item.summary;
    dataListEl.appendChild(li);
  });
}

function loadLocalData() {
  dataStatusEl.textContent = "Loading...";

  fetch("data.json")
    .then(function (response) {
      if (!response.ok) {
        throw new Error("Could not load data.json");
      }
      return response.json();
    })
    .then(function (data) {
      renderItems(data);
      dataStatusEl.textContent = "Loaded " + data.length + " items.";
      dataStatusEl.classList.remove("status-error");
      dataStatusEl.classList.add("status-success");
    })
    .catch(function (error) {
      console.error(error);
      dataStatusEl.textContent = "Could not load data. Check data.json path.";
      dataStatusEl.classList.remove("status-success");
      dataStatusEl.classList.add("status-error");
    });
}

loadDataBtn.addEventListener("click", loadLocalData);
```

4. Replace example fields with your project data structure.
5. Update `README.md` in `web-basics-project/`:

```md
# Web Basics + JavaScript Mini Project

## Project Type
(course list / products / quotes / etc.)

## What This Page Does
One sentence in your own words.

## Files
- index.html — structure
- style.css — styling
- script.js — interactivity
- data.json — local data

## What I Learned
Three bullet points from Lessons 1–5.
```

6. Test: click Load → items appear; temporarily rename `data.json` → error message appears.
7. Commit with message: `Complete fetch JSON mini project`.

**Mission output:**

- Local `data.json` loaded with `fetch`
- Data rendered into the page
- Error handling for failed load
- Updated README and meaningful commit history across the unit

## Exit Check (75–85 min)

> [!IMPORTANT]
> Independent work: close the Coursera lesson, notes, and AI tools before this block. See [independent-rebuild.md](../../shared/independent-rebuild.md).

**Exit Check task:**

1. Change list output to show one more JSON field (for example, `level` or `price`).
2. Add a filter button that shows only items matching one condition.
3. Confirm error handling still works.
4. Commit: `Improve JSON display and add filter`.

**Final project rubric — self-check before submission:**

| Criterion | Strong | Developing | Starting |
|---|---|---|---|
| HTML structure | Semantic tags, form, ids for JS hooks | Mostly valid; minor gaps | Broken or missing structure |
| CSS organization | External stylesheet; status/card classes | Works but messy | Inline styles dominate |
| JavaScript functionality | Variables, functions, conditionals work | Partial features | Script errors or missing logic |
| DOM updates | `textContent`, `classList`, dynamic list | Some updates only | Page never changes |
| Event handling | Click + submit with validation | One event type only | Events missing or broken |
| fetch / JSON usage | Local `data.json` loads and renders | Loads but incomplete render | fetch missing or broken |
| Error handling | User sees message if load fails | Console only | Crashes or silent fail |
| Code readability | Clear names, organized sections | Mostly readable | Hard to follow |
| GitHub evidence | Screenshots, commits, README | Most evidence present | Missing key evidence |
| Reflection quality | Specific about build and learning | General but honest | Vague or missing |

**Exit prompts:**

```text
My data.json contains...
fetch loads data when...
Loaded data appears in...
If fetch fails, the user sees...
One thing I can now do without the tutorial is...
One thing I still need help with is...
```

**Oral check if called:** Explain the difference between hardcoded HTML content and data loaded from JSON.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit (85–90 min)

1. Screenshot showing loaded data rendered on the page
2. Screenshot showing error message when load fails (teacher may guide test)
3. GitHub folder link to `web-basics-project/` with all files
4. Commit history showing work across Lessons 1–5 (five or more meaningful commits)
5. Completed final project rubric self-check
6. One sentence: "This unit taught me ___; my page demonstrates it by ___."

## Success Criteria

You are successful if:

1. Your page combines HTML/CSS from Phase 2 with JavaScript from Lessons 1–5.
2. Your form validates input and shows feedback.
3. Your page loads and displays local JSON with `fetch`.
4. Failed loads show a user-friendly message, not a silent error.
5. Your README and commit history show steady progress across the unit.

## Common Problems

| Problem | Try first |
|---|---|
| `Failed to fetch` | Confirm `data.json` is in same folder; use local server if `file://` blocks fetch. |
| Empty list after load | Log `data` in Console; confirm JSON is an array. |
| JSON parse error | Validate JSON syntax — no trailing commas; use double quotes. |
| Old content still showing | Clear list with `innerHTML = ""` before rendering. |
| CORS / network errors | Use local `data.json`, not an unstable public API. |

## Fast Track / Support Track

Fast track:

If Phase 3 evidence is complete early, preview [Phase 4: React Basics](../../05-react-basics/) only if your teacher approves.

Optional extra block (teacher-assigned):

Use one extra 90-minute session for debugging, refactoring, and adding the project to your Notion **Learning Projects** section.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

## After Phase 3

Next: [Phase 4: React Basics](../../05-react-basics/)

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
