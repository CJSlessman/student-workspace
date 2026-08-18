# student-workspace (plugin)

A Claude Code plugin that organizes an entire semester of coursework — programming and non-programming classes alike — into one clean repo, and teaches Claude the conventions to keep it that way.

## Install

```
/plugin marketplace add CJSlessman/student-workspace
/plugin install student-workspace@student-workspace
```

## Commands

| Command | What it does |
| ------- | ------------ |
| `/student-workspace:setup-semester` | Interviews you (semester, classes, which are programming courses) and scaffolds your personalized workspace: one folder per class, a tailored root `CLAUDE.md`, per-class `CLAUDE.md` stubs, and `SCHEDULE.md`. |
| `/student-workspace:new-class` | Adds one class mid-semester: folder skeleton, `CLAUDE.md` stub, schedule reminder. |
| `/student-workspace:new-assignment` | Creates `assignments/<name>/` (or `projects/<name>/` for programming work), files your assignment materials into it, and logs the due date in `SCHEDULE.md`. |

## Skill

The `course-organizer` skill runs in the background after setup. It keeps files filed in the right class folders, enforces lowercase-hyphenated naming, keeps `SCHEDULE.md` current (flagging anything due within 7 days), treats `projects/` folders as real codebases, follows each class's `CLAUDE.md` rules, saves generated study materials into `notes/`, and explains reasoning when helping with graded work.

## Structure it maintains

```
your-semester/
├── CLAUDE.md          # global rules, personalized to your classes
├── SCHEDULE.md        # every deadline and exam, sorted by date
└── <one folder per class>/
    ├── CLAUDE.md      # course-specific rules
    ├── syllabus/  slides/  notes/  assignments/  exams/
    └── projects/      # programming courses only
```

## License

MIT — see [LICENSE](LICENSE).
