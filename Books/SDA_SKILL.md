---
name: specification-driven-book-authoring
description: Reusable Specification-Driven Authoring workflow for planning, drafting, reviewing, revising, sourcing, packaging, and versioning books with a human author and an AI agent. Use when working on any book project in this Books workspace, especially when creating or refining a book specification file, conventionally named 00_SPEC.md, generating project files after spec approval, planning chapters, managing research and sources, reviewing drafts against a specification, maintaining continuity, preparing manuscript assets, or using writer-friendly Git versioning.
---

# Specification-Driven Book Authoring

Use this workflow when helping write a book through Specification-Driven Authoring (SDA). The human remains the author, decision-maker, and accountable editor. The AI acts as structured co-author, interviewer, researcher, developmental editor, continuity assistant, critic, line editor, and implementation agent.

## What SDA Means for Books

Specification-Driven Authoring is a writing workflow in which the writer and AI first create an explicit specification for the book before generating the manuscript itself. The specification records the writer's intent: purpose, audience, promise, thesis or story premise, structure, tone, scope, research standards, chapter architecture, continuity rules, publishing constraints, and approval status. The AI then uses that specification as the primary source of truth for outlining, chapter planning, drafting, reviewing, revising, and preparing the final manuscript.

The basic SDA lifecycle for books is:

```text
idea -> book specification -> approval -> book architecture -> chapter plans -> chapter drafts -> developmental review -> revision passes -> final manuscript
```

The key discipline is that the writer approves the specification before the AI produces substantial manuscript prose. This keeps the AI from improvising the book's promise, argument, story, audience, structure, evidence, or voice.

## Core Rule

Do not start by drafting the book. Start by creating or refining the specification.

The specification is the contract between the writer's intent and the AI's output. For books, this contract matters even more than it does for articles because a book has long-range structure, recurring concepts, continuity, pacing, research debt, character or argument arcs, and many opportunities for drift.

## Quality Standard

When creating book files from an approved specification, optimize for quality above speed, token economy, or minimal model usage.

- Use the strongest available model unless the user explicitly chooses another model or imposes a cost, speed, or token constraint.
- Use as much context and output length as needed to follow the specification well.
- Do not compress reasoning, research, review, or revision steps merely to save tokens.
- Prefer careful staged work over a fast single-pass manuscript when quality would benefit.
- Treat the approved specification, source verification, author voice, reader promise, continuity, and publishing requirements as higher priorities than speed.
- Never allow volume to masquerade as progress: a weak chapter draft is not useful merely because it is long.

## Phase 1: Build the Book Specification

Work only on the book specification file, conventionally named `00_SPEC.md`, until the user explicitly approves it.

Use this loop:

1. Read the current book specification file.
2. Identify the single most important unresolved issue.
3. Ask one focused question.
4. After the user answers, propose the exact change to the book specification file.
5. Edit the book specification file only after approval, unless the user explicitly asks for direct editing.
6. Preserve accepted decisions.
7. Record unresolved matters clearly.
8. Avoid drafting manuscript prose, except very small examples to clarify tone, narrative distance, section style, or reader experience.
9. When the spec is mature enough, explain why and ask whether to mark it approved.

The specification should eventually cover:

- working title and alternatives;
- book category, genre, and comparable works;
- purpose, promise, and reader transformation;
- target reader and secondary readers;
- core thesis, argument, premise, or story question;
- author's perspective, authority, experience, and boundaries;
- scope, exclusions, and level of depth;
- book length, chapter count, and length philosophy;
- tone, voice, style, and reading experience;
- structure, parts, chapters, and progression;
- chapter pattern, recurring features, and reader exercises if any;
- key concepts, terminology, characters, settings, or frameworks;
- main claims, counterarguments, tensions, and open problems;
- examples, scenes, cases, interviews, data, and evidence needs;
- research and citation requirements;
- source verification rules;
- ethical, legal, privacy, and practical concerns;
- continuity rules for names, terms, dates, timeline, examples, claims, characters, and world details;
- images, figures, tables, worksheets, appendices, or supplemental materials;
- publication path, format, and submission constraints;
- manuscript package requirements;
- versioning and review rules;
- quality criteria;
- unresolved questions;
- approval status.

For fiction, memoir, narrative nonfiction, or essay collections, adapt these categories. A novel may need character arcs, setting rules, point of view, timeline, scene list, and continuity canon. A nonfiction guide may need reader outcomes, frameworks, exercises, research standards, examples, and implementation steps.

## Phase 2: Create the Book Project

Create additional book files only after the user approves the book specification file.

Before creating files, propose the project structure and get approval. A typical structure is:

```text
Book Folder/
├── 00_SPEC.md
├── 01_RESEARCH_PLAN.md
├── 02_SOURCES.md
├── 03_BOOK_ARCHITECTURE.md
├── 04_CHAPTER_OUTLINES/
├── 05_DRAFTS/
├── 06_CONTINUITY_AND_STYLE.md
├── 07_EDITORIAL_REVIEW.md
├── 08_REVISION_PLAN.md
├── 09_FINAL_MANUSCRIPT.md
└── Assets/
```

Adapt the file set to the approved specification. Do not create unnecessary files. A short ebook may need fewer files. A researched nonfiction book, workbook, textbook, memoir, or novel may need more.

Useful optional files and folders include:

- `INTERVIEWS.md` for interview plans, transcripts, permissions, and follow-up questions;
- `CASE_STUDIES.md` for examples that recur across chapters;
- `CHARACTER_BIBLE.md` for fiction or narrative nonfiction;
- `WORLD_AND_TIMELINE.md` for setting, dates, sequence, and continuity;
- `GLOSSARY.md` for terms that must remain stable;
- `WORKSHEETS/` for exercises, templates, and reader tools;
- `APPENDICES/` for supporting material that should not interrupt the main manuscript;
- `MANUSCRIPT_NOTES.md` for unresolved craft, research, or publication issues.

## Phase 3: Research and Sources

Treat facts, interpretations, assumptions, memories, interviews, invented story material, and creative choices differently.

- Factual, historical, legal, medical, financial, scientific, technical, and biographical claims should be checked against credible sources.
- If a credible source supports a claim, cite it or record it in the sources file.
- If no credible source is found after a reasonable search, present the claim only as the author's interpretation, hypothesis, original observation, memory, or creative construction.
- Never invent sources.
- Never imply consensus where none was found.
- Prefer direct links to original documents, official documentation, papers, books, interviews, archives, guidelines, or primary sources.
- Keep references in a dedicated sources file when the project has moved beyond specification.
- Track research debt explicitly. Do not hide uncertain claims inside smooth prose.
- For interviews, record consent, attribution preferences, date, medium, and usable quotations.
- For memoir or personal narrative, mark memory-based material honestly and avoid presenting uncertain recollection as independently verified fact.

When writing for a publisher, agent, magazine excerpt, academic venue, or self-publishing platform with citation rules, follow those rules. If the publication requests numerical references, use references such as `[1]`, `[2]`, and keep source details easy to verify.

## Phase 4: Book Architecture and Chapter Planning

Generate the book architecture from the approved specification, not from memory.

The architecture should define:

- the book's promise and governing question;
- the part structure, if any;
- chapter sequence and escalation;
- the purpose of each chapter;
- reader transformation chapter by chapter;
- recurring sections, exercises, summaries, examples, or motifs;
- evidence and story beats needed by chapter;
- expected chapter lengths or relative weights;
- dependencies between chapters;
- optional appendices or supplemental materials.

Before drafting a chapter, create or verify that chapter's outline. The outline should explain what the chapter must accomplish, what it must not cover, which sources or examples it uses, how it connects to earlier and later chapters, and what open questions remain.

## Phase 5: Draft, Review, Revise

Draft from the approved specification, the book architecture, and the relevant chapter outline.

When drafting:

- Prioritize quality over speed or token count.
- Preserve the author's voice and decisions.
- Keep chapter content aligned with the approved structure.
- Avoid adding unsupported claims.
- Flag missing evidence instead of filling gaps with invented certainty.
- Maintain continuity with earlier chapters, established terminology, examples, character details, timeline, and tone.
- Record assumptions that need author confirmation.
- Keep edits inspectable.

When reviewing:

- Review every chapter draft against the book specification, book architecture, and chapter outline.
- Identify mismatches between the draft and the specification.
- Separate developmental issues, structural issues, continuity issues, factual/source issues, tone issues, line-level issues, and publication-guideline issues.
- Check whether the chapter earns its place in the book.
- Check whether the chapter advances the reader, argument, story, or emotional arc.
- Propose a revision plan before large rewrites.

When revising:

- Prefer targeted edits over uncontrolled full rewrites.
- Preserve accepted material.
- Make significant changes easy to accept, reject, or revert.
- Track unresolved research, continuity, or editorial decisions.
- Use revision passes intentionally: developmental pass, structure pass, evidence pass, continuity pass, line edit, copyedit, and proofread.

## Continuity and Style Control

Maintain a dedicated continuity and style file when the project moves beyond specification.

Track:

- approved title, subtitle, terminology, spelling, capitalization, and naming conventions;
- recurring metaphors, frameworks, examples, and definitions;
- timeline, dates, ages, locations, organizations, and sequence;
- character names, traits, relationships, voice, and arcs when relevant;
- source usage and citation style;
- voice rules and phrases to prefer or avoid;
- formatting rules for headings, lists, notes, exercises, callouts, tables, figures, and appendices;
- unresolved continuity questions.

Before editing later chapters, check continuity against earlier accepted decisions. Do not silently change names, terms, dates, claims, or character facts.

## Images, Figures, Tables, and Assets

Use visuals and assets to serve the book, not to decorate it generically.

When the approved specification calls for images, figures, tables, worksheets, diagrams, maps, or other assets, create a reusable asset plan and store actual files in the book's asset folder.

For each planned asset, record:

- book location;
- purpose;
- suggested file name;
- prompt or creation instructions if generated;
- caption/source line;
- alt text where relevant;
- usage rights or author-created status;
- status: planned, drafted, approved, final, replaced, or removed.

Store assets in a separate folder when the project moves beyond specification. Use one asset per file where practical. Name files according to how they are referenced in the manuscript.

If AI-generated images are used, identify them as author-created AI-assisted illustrations unless the publisher or platform requires different wording.

Do not consider a book package complete while referenced assets are missing. Either generate or create the files, replace the references with prompt-only placeholders, or clearly mark the assets as pending.

## Manuscript Assembly and Publication Package

Before calling a book final, assemble and check the whole manuscript.

The final package may include:

- final manuscript;
- title page;
- subtitle and metadata;
- dedication;
- epigraph permissions if any;
- table of contents;
- introduction and conclusion;
- acknowledgments;
- notes, bibliography, references, or works cited;
- appendices;
- author bio;
- book description, back-cover copy, or sales copy;
- asset folder;
- permissions log;
- style sheet;
- proofreading checklist.

Adapt the package to the publishing path. A proposal, query package, self-published ebook, print book, workbook, textbook, and serialized online book have different requirements.

## Writer-Friendly Versioning

Use Git/GitHub as the safety layer, but present it to writers with ordinary writing language.

Preferred commands:

- `Save Version`: create a local checkpoint.
- `Compare Versions`: show what changed between checkpoints.
- `Restore Previous Version`: recover an earlier checkpoint after explicit confirmation.
- `Publish Backup to GitHub`: push saved work to the remote repository.

Avoid requiring writers to understand Git internals during normal use. Explain Git only as much as needed for trust, safety, and recovery.

Before committing:

- Check what changed.
- Stage only files relevant to the current save.
- Use a clear commit message.
- Do not commit private setup files, full chat exports, credentials, interview material without permission, sensitive notes, or unrelated local files unless the user explicitly requests it.

## Publication Safeguards

Before final submission or publication:

- Check the manuscript against the approved specification.
- Check the manuscript against publisher, agent, platform, or format guidelines.
- Verify citations, permissions, links, quotations, and bibliography entries.
- Confirm image and asset rights, captions, and alt text where relevant.
- Run grammar, readability, copyediting, and proofreading passes.
- Check for plagiarism risk.
- Confirm that no unsupported claim is presented as established fact.
- Confirm that interview, memoir, private, or sensitive material has appropriate permission and framing.
- Confirm consistency of title, subtitle, author name, chapter titles, terminology, and formatting.

## Useful Agent Behaviors

When the user asks to work on a specification, ask one question at a time.

When the user provides a decision, propose exact spec text before editing unless direct editing is requested.

When the user asks to create or revise book files, first read the book specification file, conventionally named `00_SPEC.md`.

When the user asks to draft a chapter, also read the book architecture, chapter outline, continuity and style file, and sources relevant to that chapter.

When the user asks to save work, use the writer-facing versioning language and explain what was saved.

When unsure, preserve author control: ask before making irreversible or broad changes.

Do not treat a book as a pile of chapters. Treat it as a designed reader experience with memory, sequence, promise, rhythm, evidence, and revision history.

## Future Application Vision

The long-term goal is a purpose-built writing application that gives non-developers SDA, AI collaboration, source tracking, continuity management, asset handling, manuscript packaging, and version history out of the box.

Until such an application exists, a practical setup can combine:

- a text editor such as VS Code;
- an AI coding or writing agent such as Codex;
- Markdown files;
- Git/GitHub versioning hidden behind writer-friendly commands.
