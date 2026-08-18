---
description: Interview the student and scaffold a personalized semester workspace (class folders, CLAUDE.md files, SCHEDULE.md)
argument-hint: "[optional semester name, e.g. Fall 2026]"
---

Set up a semester coursework workspace in the current directory.

## 1. Confirm location

Confirm with the user that the current directory is where they want their semester workspace. If the directory is non-empty (ignoring hidden files), warn them and list what's there before proceeding.

## 2. Interview

Ask the user (concisely, in one or two rounds — use $ARGUMENTS as the semester name if provided):

1. Semester name (e.g., "Fall 2026").
2. How many classes they're taking.
3. For each class: name and course code (e.g., "Operating Systems — CS 4348").
4. Which of those are programming/CS courses.

## 3. Scaffold

For each class, create one top-level folder named from the course in lowercase-hyphenated form (e.g., `cs4348-operating-systems/`) containing:

- `syllabus/`, `slides/`, `notes/`, `assignments/`, `exams/`
- `projects/` **only** for programming courses

## 4. Generate files

Read the templates in `${CLAUDE_PLUGIN_ROOT}/skills/course-organizer/templates/`:

- **Root `CLAUDE.md`** from `root-claude-md.md`: substitute the real semester name, class count, and the actual class list (marking which are programming courses). No placeholders may remain in the output.
- **Per-class `CLAUDE.md`** in each class folder from `class-claude-md.md`: fill in course name/code, semester, and whether it's a programming course; leave the remaining fields as prompts for the student to complete.
- **`SCHEDULE.md`** at the root from `schedule-md.md`, with the semester name filled in.

## 5. Wrap up

1. Show the created tree briefly.
2. Offer: "Drop your syllabi PDFs into each class's `syllabus/` folder and I'll read them to fill in SCHEDULE.md and your per-class CLAUDE.md files."
3. Offer to `git init` and make an initial commit (message: `Set up <semester> workspace`). Only do it if the user says yes and the directory isn't already a git repo.
