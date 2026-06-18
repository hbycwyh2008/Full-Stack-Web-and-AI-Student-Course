# Lesson 4: CORS and First Success

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Fix **CORS** so Next.js can read FastAPI responses (Udemy section + course pattern).
2. Demonstrate **end-to-end success**: user action → API → UI update.
3. Explain CORS in one sentence for oral check.
4. Add loading or error message when API fails.
5. Record **First Success** moment in README (timestamp + screenshot).
6. **Independent rebuild:** hand-type CORS fix + connected UI in `full-stack-practice/independent-rebuild/lesson-04/` — [independent-rebuild.md](../shared/independent-rebuild.md).

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

**Required resource — Udemy:**

Same course — sections on **CORS**, connecting frontend to backend, troubleshooting (teacher assigns exact lectures).

Review: Phase 9 full-stack integration pattern (concept only — your teacher will explain).

**Individual notes:**

```text
CORS error meant...
Fix applied on...
After fix, browser shows...
Loading state shows user...
One thing I still do not understand is...
```

## Talk Robin

**Share:** Before/after screenshot; why backend must allow frontend origin.

## Group Answer

```text
CORS protects...
We fixed it by...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Both servers running; students can name frontend and backend ports.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Apply Udemy CORS fix — verify data loads in browser.
2. Add simple loading text or spinner while fetching (course or your own).
3. Update README with **First Success** section:

   ```markdown
   ## First Success (Lesson 4)
   - Date:
   - What worked:
   - Screenshot: screenshots/first-success.png
   ```

4. Capture `screenshots/first-success.png` — full page with real data visible.
5. Commit: `Fix CORS and record first full-stack success`.

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close course videos, notes, AI tools, and follow-along code before this block.

**Required — no materials:** [independent-rebuild.md](../shared/independent-rebuild.md)

1. Close Udemy and follow-along projects — rebuild only in `independent-rebuild/lesson-04/`.
2. **Hand-type** minimal backend with `CORSMiddleware` allowing `http://localhost:3000`.
3. **Hand-type** minimal frontend with `fetch`, **loading** text, and **error** message.
4. Demo end-to-end from rebuild folders only; screenshot → `screenshots/rebuild-first-success.png`.
5. Add `REBUILD.md`; commit: `Independent rebuild lesson-04 (no materials)`.

**Oral check:** Explain CORS using only your rebuild code.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. `first-success.png` on GitHub (follow-along)
2. `independent-rebuild/lesson-04/` + `REBUILD.md` + rebuild screenshot
3. README First Success section filled
4. Commit history

## Success Criteria

1. Frontend displays live API data (follow-along).
2. Student can demo follow-along without Udemy video open.
3. CORS explained orally using **rebuild** code.
4. **Rebuild** mini full-stack works from memory-only folders.

## Common Problems

| Problem | Try first |
|---|---|
| Still blocked | Check `CORSMiddleware` origins include `http://localhost:3000`. |
| 404 on API | Verify path matches backend route exactly. |

## Fast Track / Support Track

Fast track:

Add basic error message if `fetch` fails (network or 500).

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
