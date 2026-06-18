# Lesson 9: Next.js Routing and Layouts

## Lesson Goal

By the end of this lesson, each student should be able to:

1. Create multiple routes with the App Router (`app/` folders).
2. Use a shared `layout.jsx` for header/footer across pages.
3. Link pages with `next/link` (not full page reload).
4. Port one idea from `react-practice/` (e.g. project list) into a Next page as static or props-based UI.
5. Commit routing + layout with meaningful message.
6. Submit [Learn Next.js Module 2](https://www.coursera.org/learn/learn-nextjs/home/module/2) evidence.

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

**Required resource — complete [Learn Next.js Module 2](https://www.coursera.org/learn/learn-nextjs/home/module/2):** Building Your First App with Routing (~1 hour).

Focus: PrintForge routing, layouts, navigation, media basics.

**Individual notes:**

```text
A route in App Router is created by...
layout.jsx wraps pages because...
next/link is better than <a> because...
One thing I still do not understand is...
```

## Talk Robin

**Share:** your planned routes (Home, About, Projects); one layout element; one question.

## Group Answer

```text
Shared layout helps our portfolio because...
Our group still needs help with...
```

## Teacher Clarification

**Teacher checks:** Lesson 8 app runs; students can draw a simple route map on paper.

The teacher explains only the common stuck points before the mission task.

## Mission Task

1. Add routes: `/` (home), `/projects` (list page), `/about` (short bio).
2. Add `app/layout.jsx` with site title and nav links using `Link`.
3. On `/projects`, show at least three project titles (hard-coded array or copied pattern from `react-practice/`).
4. Commit: `Add Next.js routes and shared layout`.

## Independent Rebuild

Add active nav styling or a footer line on all pages via layout. Commit.

Close full-solution references before this block. You may use your own short checklist, but do not copy a completed answer.

## Evidence to Submit

1. Screenshot of two different routes + shared nav
2. GitHub link showing `app/` structure and `Link` usage
3. Coursera Module 2 progress screenshot
4. One sentence: “Layouts in Next.js are like...”

## Success Criteria

1. At least three routes work via client navigation.
2. Shared layout visible on all pages.
3. Projects page shows list content.
4. All evidence submitted.

## Common Problems

| Problem | Try first |
|---|---|
| 404 on route | Folder name must match URL; file must be `page.jsx`. |
| Full page reload | Use `import Link from 'next/link'`. |

## Fast Track / Support Track

Fast track:

Preview Module 3 client vs server scrims before Lesson 10.

Support track:

- Complete the smallest working version first.
- Ask for a hint after you can show what you tried.
- Submit honest evidence of progress if the full mission is not finished.

Educational materials are copyright © 2026 Wang Morgan. All rights reserved. Students may use these materials for this course. Redistribution or commercial reuse requires permission.
