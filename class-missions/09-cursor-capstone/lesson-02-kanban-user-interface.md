# Lesson 7: Building the Kanban User Interface

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Complete Udemy **§2 Building the Project User Interface** (5 lectures · ~49 min).
2. Build or prompt-build a **responsive Kanban UI** with **shadcn/ui** (dark/light theme per course).
3. Map UI columns/cards to your [Figma user flow](../optional-figma/) (handbook assistant screens).
4. Use Cursor to implement **one UI slice** only after writing a short plan.
5. Submit running UI screenshot and commit.
6. **Independent rebuild:** hand-type Kanban column UI in `vibe-coding/independent-rebuild/lesson-07/` — [independent-rebuild.md](../shared/independent-rebuild.md).

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

**Required resource — Udemy §2:**

[Complete Cursor AI — §2 Building the Project User Interface](https://www.udemy.com/course/cursorai-nextjs/)

Complete all **5 lectures** in this section (expand in Udemy sidebar).

Cross-check [Figma Phase 02](../optional-figma/) — layout, spacing, and loading placeholders.

**Individual notes:**

```text
shadcn/ui gives us...
Dark/light theme works by...
Kanban columns map to our capstone as...
I prompted Cursor to...
One thing I still do not understand is...
```

## Talk Robin

**Share:** One UI decision you made vs what Cursor suggested; how Figma informed your layout.

## Group Answer

```text
Good UI needs loading states because...
We still read AI diffs because...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** §1 homework done; Kanban repo runs (`npm run dev`); Lesson 6 README updated.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Finish §2 UI in `vibe-coding/kanban-cursor/` (follow Udemy prompts).
2. Add **loading skeleton or placeholder** on the main board view (course pattern or Figma-inspired).
3. Update `vibe-coding/README.md` — table: **Figma frame → Kanban component → future capstone route**.
4. Screenshot light **and** dark theme → `vibe-coding/kanban-cursor/screenshots/`.
5. Commit: `Build Kanban UI with Cursor — Lesson 7`.

## Independent Rebuild

> [!IMPORTANT]
> Independent work: close course videos, notes, AI tools, and follow-along code before this block.

**Required — no materials:** [independent-rebuild.md](../shared/independent-rebuild.md)

1. Close Udemy, Cursor, and `kanban-cursor/`.
2. In `vibe-coding/independent-rebuild/lesson-07/`, **hand-type**:
   - One Kanban **column** + 2–3 **static cards** (hard-coded array OK)
   - Basic styling (Tailwind or CSS) from memory
   - Loading placeholder component or skeleton (static demo OK)
3. Add `REBUILD.md`; commit: `Independent rebuild lesson-07 (no materials)`.

**Oral check:** Point to JSX you typed and explain structure.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshots (follow-along: light + dark or mobile + desktop)
2. `independent-rebuild/lesson-07/` + `REBUILD.md` + rebuild screenshot
3. Figma → UI mapping table in `vibe-coding/README.md`
4. Udemy §2 progress screenshot
5. Commit history

## Success Criteria

1. Kanban UI visible in follow-along (static OK if DB not wired).
2. Plan → Cursor → verify used once in follow-along.
3. Loading/placeholder in follow-along or **rebuild**.
4. **Rebuild** column UI hand-typed without materials.

## Common Problems

| Problem | Try first |
|---|---|
| shadcn install fails | Re-run course commands; check `components.json`. |
| Theme toggle broken | Compare with course repo diff; check `ThemeProvider`. |
| AI generated wrong layout | Narrow prompt: “only edit `app/page.tsx`”. |

## Fast Track / Support Track

Fast track:

Add a fourth column or custom card color — small scoped Cursor task with reflection note.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
