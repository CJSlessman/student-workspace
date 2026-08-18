---
description: Create a new assignment or project subfolder in the right class, file its materials, and log the due date
argument-hint: "[class] [short assignment name]"
---

Set up a new assignment in this workspace.

1. Determine which class it belongs to — from $ARGUMENTS if given, otherwise infer from context or ask. If ambiguous, ask; never guess.
2. Ask for (or infer) a short lowercase-hyphenated name, optionally prefixed `hw<N>-` (e.g., `hw2-linked-lists`).
3. Create `assignments/<short-name>/` inside that class folder — or `projects/<short-name>/` instead if it's programming work in a CS class.
4. If the user points at an assignment file (PDF, handout, starter code) anywhere in or outside the repo, move it into that subfolder and report where it went.
5. Ask for the due date (or read it from the assignment file if one was provided) and add a row to `SCHEDULE.md` with the class name, date, and assignment. Flag it if it's due within 7 days.
