# Books

This repository contains a reusable Specification-Driven Authoring workflow for writing books with a human author and an AI collaborator.

The central file is `SDA_SKILL.md`. It adapts the article-focused SDA process from the Articles repository into a book-writing process with stronger support for premise, audience promise, book architecture, chapter planning, continuity, research, revision passes, and manuscript packaging.

`SDA_SKILL_SRB.md` is the Serbian translation of the book-writing skill.

## Recommended Layout

```text
Books/
├── README.md
├── CODEX_START_PROMPT.md
├── SDA_SKILL.md
├── SDA_SKILL_SRB.md
├── Templates/
│   └── 00_BOOK_SPEC_TEMPLATE.md
└── Book Projects/
```

Each book project should live in its own folder under `Book Projects/`. Start with a single `00_SPEC.md` file. Create chapter plans, research files, drafts, reviews, and final manuscript files only after the specification is approved.

## Writer-Facing Commands

- `Save Version`: create a local checkpoint.
- `Compare Versions`: show what changed between checkpoints.
- `Restore Previous Version`: recover earlier work after explicit confirmation.
- `Publish Backup to GitHub`: push saved work to the remote repository.

The point is to make version history feel like a writing safety system, not a software engineering ritual.
