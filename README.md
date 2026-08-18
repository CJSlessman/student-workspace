# student-workspace

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Organize an entire semester of college coursework in one repo — and get high-quality help from Claude Code across **both** programming and non-programming classes. One folder per class, a `CLAUDE.md` that teaches Claude your semester, a `SCHEDULE.md` that never lets a deadline sneak up on you, and commands that scaffold all of it in a two-minute interview.

## Quick start

**Path 1 — Claude Code plugin (recommended).** In Claude Code, run:

```
/plugin marketplace add CJSlessman/student-workspace
/plugin install student-workspace@student-workspace
```

Then open an empty folder for your semester and run:

```
/student-workspace:setup-semester
```

**Path 2 — Template repository.** Click **Use this template** at the top of this repo, clone your copy, and rename the `template/` example classes to your real ones (or just ask Claude to do it). You get the pre-built structure without installing anything.

## What `/setup-semester` does

1. Confirms the current directory is where you want your workspace (warns if non-empty).
2. Interviews you: semester name, number of classes, name/course code for each, and which are programming courses.
3. Scaffolds one folder per class and generates a root `CLAUDE.md` personalized with your real classes, a `CLAUDE.md` stub per class, and `SCHEDULE.md`.
4. Offers to read syllabi PDFs you drop into each class's `syllabus/` folder to fill in deadlines and course rules automatically.
5. Offers to `git init` and make the first commit.

Two more commands keep the workspace growing cleanly: `/student-workspace:new-class` adds a class mid-semester, and `/student-workspace:new-assignment` sets up an assignment subfolder, files your materials, and logs the due date.

## The structure it creates

```
your-semester/
├── CLAUDE.md                    # global rules, personalized to your classes
├── SCHEDULE.md                  # every deadline and exam, sorted by date
├── cs4348-operating-systems/    # example programming class
│   ├── CLAUDE.md                # course-specific rules (language, style, grading)
│   ├── syllabus/  slides/  notes/  assignments/  exams/
│   └── projects/                # treated as real codebases
└── hist1301-us-history/         # example non-programming class
    ├── CLAUDE.md                # citation style, submission formats
    └── syllabus/  slides/  notes/  assignments/  exams/
```

After setup, the bundled `course-organizer` skill keeps Claude on-convention: dropped files get filed into the right class automatically, due dates land in `SCHEDULE.md` (with a 7-day warning at session start), study materials get saved into `notes/`, and Claude explains its reasoning on graded work so you actually learn the material.

## Demo

<!-- TODO: demo GIF of /setup-semester -->
_Demo GIF coming soon._

## Contributing

Issues and PRs welcome — especially template improvements and conventions for class types not covered yet (labs, studios, seminars). Keep instruction files lean; plugin files over ~200 lines lose adherence.

## License

[MIT](LICENSE) © 2026 Charles Slessman
