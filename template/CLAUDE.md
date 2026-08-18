# Course Workspace

This repository organizes all my coursework for the current semester. I am taking five classes: some may be programming courses with coding projects, others are courses with essays, problem sets, labs, and general assignments. Your job is to help me with the work itself AND keep this repository rigorously organized.

> **Template note:** rename the `class-1/` … `class-5/` folders to your real classes (lowercase-hyphenated, e.g. `bio301-genetics/`), update the list below, and delete this note. `class-1/` and `class-2/` include a `projects/` folder as programming-course examples — add `projects/` to any class with coding work, and remove it where it isn't needed. Or skip all of this and let Claude do it: ask it to "set up my semester" and answer its questions.

## Directory Structure

Each class gets exactly one top-level folder. Everything related to a class lives inside that class's folder — no exceptions.

- Root contains only: `CLAUDE.md`, `SCHEDULE.md`, and one folder per class:
  - `class-1/` — (programming-course example — rename me)
  - `class-2/` — (programming-course example — rename me)
  - `class-3/` — (rename me)
  - `class-4/` — (rename me)
  - `class-5/` — (rename me)
- Standard layout inside every class folder: `CLAUDE.md` (class-specific rules), `syllabus/`, `slides/`, `notes/`, `assignments/`, `exams/`, and `projects/` for programming courses.

## Organization Rules

- Never place a file at the repository root except `CLAUDE.md` and `SCHEDULE.md`. Every other file belongs inside a class folder.
- If it's ambiguous which class a file or task belongs to, ask me before creating or moving anything.
- Assignments get their own subfolder, named `<short-name>` or `hw<N>-<short-name>` (e.g., `assignments/hw2-essay-outline/`). Keep the prompt/instructions, my work, and any drafts together in that subfolder.
- Use consistent, lowercase, hyphenated names for folders and files. No spaces.
- When I drop a new file into the repo (slides, assignment PDF, dataset), move it into the correct class folder and subfolder, and tell me where you put it.
- Keep `SCHEDULE.md` current. When a syllabus or assignment reveals a due date or exam date, add it to `SCHEDULE.md` with the class name and date. Flag anything due within 7 days when I start a session.

## Working on Coursework

- **Programming courses:** Treat `projects/` subfolders as real codebases — proper structure, tests when appropriate, follow any language/style requirements from that class's `CLAUDE.md`, and keep a short README in each project noting the assignment goal and how to run it.
- **Non-programming courses:** Help with essays, problem sets, readings, labs, and study materials. Follow the citation style and formatting requirements listed in that class's `CLAUDE.md`.
- **Studying:** When asked, generate study guides, practice questions, or summaries from the materials in `slides/` and `notes/` — and save them into `notes/`.
- **Explain as you go.** When helping with graded work, walk me through the reasoning so I actually understand the material — I need to be able to defend this work on exams.

## Class-Specific CLAUDE.md Files

Each class folder has its own `CLAUDE.md` that loads automatically when you work in that folder. Keep global rules here and course-specific rules there. Per-class files should include: course name, professor, semester; submission format requirements (file types, naming, citation style); for programming courses the required language/version, allowed libraries, style guide, and how work is graded/tested; and any professor-specific quirks or repeated feedback.

## General Conduct

- Keep this file and per-class `CLAUDE.md` files short and current. If I correct you twice about the same thing, add the correction to the appropriate `CLAUDE.md`.
- Before large reorganizations (moving many files), show me the plan first.
- Don't delete anything without asking — archive old material into an `archive/` subfolder inside the class instead.
