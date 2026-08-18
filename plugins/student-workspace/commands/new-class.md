---
description: Add one class to the workspace mid-semester (folder skeleton + CLAUDE.md stub)
argument-hint: "[class name / course code]"
---

Add a new class to this semester workspace.

1. Get the class name and course code (from $ARGUMENTS if given, otherwise ask), and ask whether it's a programming course (any class with coding projects).
2. Create a top-level folder named in lowercase-hyphenated form (e.g., `hist1301-us-history/`) with the standard skeleton: `syllabus/`, `slides/`, `notes/`, `assignments/`, `exams/`, plus `projects/` if it's a programming course.
3. Generate its `CLAUDE.md` stub from `${CLAUDE_PLUGIN_ROOT}/skills/course-organizer/templates/class-claude-md.md`, filling in course name/code, semester (read it from the root CLAUDE.md), and course type.
4. Add the class to the class list in the root `CLAUDE.md`.
5. Remind the user to add the class's deadlines to `SCHEDULE.md` — and offer to parse them automatically if they drop the syllabus into the new `syllabus/` folder.
