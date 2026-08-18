<!-- Template: root CLAUDE.md. Replace every {{PLACEHOLDER}}; the output must contain none. -->
# {{SEMESTER_NAME}} — Course Workspace

This repository organizes all coursework for my {{SEMESTER_NAME}} semester. I am taking {{CLASS_COUNT}} classes: {{CLASS_LIST_SENTENCE — e.g., "STAT 3355 Data Science is a programming course with coding projects; HIST 1301 and PSY 1301 are non-programming courses with essays, problem sets, and general assignments"}}. Your job is to help me with the work itself AND keep this repository rigorously organized.

## Directory Structure

Each class gets exactly one top-level folder. Everything related to a class lives inside that class's folder — no exceptions.

- Root contains only: `CLAUDE.md`, `SCHEDULE.md`, and one folder per class:
{{CLASS_FOLDER_BULLET_LIST — one bullet per class: `folder-name/` — Course Code, Course Name (programming course / non-programming course)}}
- Standard layout inside every class folder: `CLAUDE.md` (class-specific rules), `syllabus/`, `slides/`, `notes/`, `assignments/`, `exams/`, and `projects/` for programming classes.

## Organization Rules

- Never place a file at the repository root except `CLAUDE.md` and `SCHEDULE.md`. Every other file belongs inside a class folder.
- If it's ambiguous which class a file or task belongs to, ask me before creating or moving anything.
- Assignments get their own subfolder, named `<short-name>` or `hw<N>-<short-name>` (e.g., `assignments/hw2-problem-set/`). Keep the prompt/instructions, my work, and any drafts together in that subfolder.
- Use consistent, lowercase, hyphenated names for folders and files. No spaces.
- When I drop a new file into the repo (slides, assignment PDF, dataset), move it into the correct class folder and subfolder, and tell me where you put it.
- Keep `SCHEDULE.md` current. When a syllabus or assignment reveals a due date or exam date, add it to `SCHEDULE.md` with the class name and date. Flag anything due within 7 days when I start a session.

## Working on Coursework

- **Programming classes:** Treat `projects/` subfolders as real codebases — proper structure, tests when appropriate, follow any language/style requirements from that class's `CLAUDE.md`, and keep a short README in each project noting the assignment goal and how to run it.
- **Non-programming classes:** Help with essays, problem sets, readings, and study materials. Follow the citation style and formatting requirements listed in that class's `CLAUDE.md`.
- **Studying:** When asked, generate study guides, practice questions, or summaries from the materials in `slides/` and `notes/` — and save them into `notes/`.
- **Explain as you go.** When helping with graded work, walk me through the reasoning so I actually understand the material — I need to be able to defend this work on exams.

## Class-Specific CLAUDE.md Files

Each class folder has its own `CLAUDE.md` that loads automatically when you work in that folder. Keep global rules here and course-specific rules there. Per-class files should include: course name, professor, semester; submission format requirements (file types, naming, citation style); for programming classes the required language/version, allowed libraries, style guide, and how work is graded/tested; and any professor-specific quirks or repeated feedback.

## General Conduct

- Keep this file and per-class `CLAUDE.md` files short and current. If I correct you twice about the same thing, add the correction to the appropriate `CLAUDE.md`.
- Before large reorganizations (moving many files), show me the plan first.
- Don't delete anything without asking — archive old material into an `archive/` subfolder inside the class instead.
