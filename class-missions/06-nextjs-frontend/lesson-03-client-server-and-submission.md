# Lesson 10: Client vs Server Components and Phase 4 Submission

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Explain client vs server components in beginner terms.
2. Mark an interactive component with `'use client'` and use `useState` in Next.js.
3. Add one dynamic route or dynamic segment (Module 3 concept).
4. Complete Phase 4 evidence checklist in repo and Notion.
5. Orally explain the path from Phase 4 → course Phase 5 TypeScript → Phase 6 `nextjs-frontend/`.
6. Submit all Phase 4 evidence including both Coursera courses progress.

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

**Required resource — complete [Learn Next.js Module 3](https://www.coursera.org/learn/learn-nextjs/home/module/3):** Components, Links & Dynamic Pages (~1 hour).

Include: component types, **client vs server components**, dynamic routing (PrintForge / model-based pages).

Reference: [Client vs server aside](https://www.coursera.org/learn/learn-nextjs/ungradedWidget/cBgd0/aside-client-vs-server-components) in Module 3 if linked from course.

**Individual notes:**

```text
Server components run...
Client components need 'use client' when...
Dynamic routes use...
After Phase 4 I will learn TypeScript in...
The AI School Assistant frontend will live in...
One thing I still do not understand is...
```

## Talk Robin

**Share:** when you need `'use client'`; one dynamic route idea; one question about Phase 6.

## Group Answer

```text
Phase 4 prepared us for Next.js because...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Both `react-practice/` and `nextjs-practice/` run; students know folder names for Phase 6.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Create a client component (e.g. `app/components/ProjectToggle.jsx` with `'use client'`) that toggles detail text with `useState`.
2. Import it into a server page (default `page.jsx`).
3. Add one dynamic route, e.g. `app/projects/[id]/page.jsx`, showing project id from params (static array lookup is fine).
4. Update root `README.md` or add `phase-4-evidence.md` with links to both folders + Coursera screenshots list.
5. Commit: `Add client component and dynamic route for Phase 4`.

## Independent Rebuild

**Independent rebuild (oral if called):**

1. Without notes, explain: JSX → props → state → fetch → Next layout → client component.
2. Point to where FastAPI will connect in Phase 6–7.

Update Notion portfolio with Phase 4 block: links to GitHub folders + one screenshot.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. GitHub links: `react-practice/` and `nextjs-practice/`
2. Screenshot: client component interaction on Next page
3. Screenshot: dynamic route showing different `id`
4. Coursera progress: Learn React (modules completed in this track) + Learn Next.js (Modules 1–3)
5. Notion portfolio update with Phase 4 section
6. Written answer (5–8 sentences): “Phase 4 → Phase 5 TS → Phase 6 Next AI UI”
7. Commit history across Phase 4 (teacher may require **8+** meaningful commits total)

## Success Criteria

You are successful if:

1. Both projects run locally.
2. You used props, state, list map, and fetch in `react-practice/`.
3. You used routes, layout, `'use client'`, and one dynamic route in `nextjs-practice/`.
4. You can explain client vs server without reading slides.
5. Notion + GitHub evidence complete.

## Common Problems

| Problem | Try first |
|---|---|
| `useState` error in page | Move interactivity to `'use client'` file. |
| Dynamic route 404 | Folder `[id]` spelling; export default page component. |
| Missing Phase 3 skills | Review Phase 3 fetch lesson before demo. |

## Phase 4 Completion Checklist

```text
[ ] react-practice/ runs — components, props, map, state, fetch
[ ] nextjs-practice/ runs — routes, layout, client component, dynamic route
[ ] Coursera Learn React modules 1,2,4,5,7,8,9,12,13 (+ optional 10) done
[ ] Coursera Learn Next.js modules 1,2,3 done
[ ] Notion updated
[ ] Can explain path to nextjs-frontend/ (course Phase 6)
```

## Fast Track / Support Track

Fast track:

Students who finish early may ask your teacher for optional preview reading — do not start the full AI app until course Phase 6.

## After Phase 4

**Course track (not class missions folder numbering):** Phase 5 TypeScript → Phase 6 Next.js Frontend. Your teacher will share the formal overview.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
