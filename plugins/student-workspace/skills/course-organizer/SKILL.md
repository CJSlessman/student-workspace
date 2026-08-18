---
name: course-organizer
description: Keeps a student's semester workspace organized and makes coursework help effective. Use whenever the user mentions classes, coursework, assignments, homework, projects, essays, problem sets, lectures, slides, syllabi, exams, quizzes, studying, grades, professors, or due dates — or drops any school file (PDF, slides, dataset, starter code) into the repo — even if they don't ask about organization. Also use when creating, moving, or filing anything in a workspace that has one folder per class.
---

# Course Organizer

This workspace organizes one semester of coursework: one top-level folder per class, plus a root `CLAUDE.md` and `SCHEDULE.md`. Your job is to help with the work itself AND keep the repo rigorously organized.

## Filing rules

- **One folder per class.** Everything related to a class lives inside that class's folder — no exceptions. Root contains only `CLAUDE.md`, `SCHEDULE.md`, and class folders.
- **Never leave files at the repo root.** When the user drops a new file into the repo (slides, assignment PDF, dataset, starter code), move it into the correct class folder and subfolder (`slides/`, `syllabus/`, `assignments/<name>/`, ...) and tell them exactly where you put it.
- **Ask when ambiguous.** If you can't tell which class a file or task belongs to, ask before creating or moving anything.
- **Naming:** lowercase, hyphenated, no spaces — folders and files alike.
- **One subfolder per assignment**, named `<short-name>` or `hw<N>-<short-name>` (e.g., `assignments/hw2-problem-set/`). Keep the prompt, the student's work, and drafts together in it.

## Schedule

- Keep `SCHEDULE.md` current: whenever a syllabus, assignment, or conversation reveals a due date or exam date, add it with the class name and date.
- At the start of a session, check `SCHEDULE.md` and flag anything due within 7 days.

## Coursework

- **Programming classes:** treat `projects/` subfolders as real codebases — proper structure, tests when appropriate, and a short README noting the assignment goal and how to run it. Follow the language/style requirements in that class's `CLAUDE.md`.
- **Non-programming classes:** help with essays, problem sets, readings, and study materials, following the citation style and formatting requirements in that class's `CLAUDE.md`.
- **Studying:** generate study guides, practice questions, or summaries from `slides/` and `notes/` — and save the results into that class's `notes/`.
- **Explain as you go.** When helping with graded work, walk through the reasoning so the student actually learns the material — they need to defend it on exams.

## Per-class rules

Each class folder has its own `CLAUDE.md` with course-specific rules (submission formats, citation style, language/version, professor quirks). Follow it whenever working in that folder. If the user corrects you twice about the same thing, offer to record it there.

## Scaffolding

When creating a new workspace, class, or schedule file, generate from the templates in this skill's `templates/` directory rather than improvising:

- `templates/root-claude-md.md` — root CLAUDE.md (substitute all placeholders)
- `templates/class-claude-md.md` — per-class CLAUDE.md stub
- `templates/schedule-md.md` — SCHEDULE.md starter

## Safety

- Before large reorganizations (moving many files), show the plan first.
- Never delete coursework — archive old material into an `archive/` subfolder inside the class instead.
