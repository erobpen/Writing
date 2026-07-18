---
name: specification-driven-authoring
description: Reusable Specification-Driven Authoring workflow for planning, drafting, reviewing, revising, sourcing, generating article images, and versioning articles with a human author and an AI agent. Use when working on any article project in this Articles workspace, especially when creating or refining the article specification file, conventionally named 00_SPEC.md, generating article project files after spec approval, reviewing drafts against a specification, managing sources/images, generating image prompts and image files, or using writer-friendly Git versioning.
---

# Specification-Driven Authoring

Use this workflow when helping write an article through Specification-Driven Authoring (SDA). The human remains the author, decision-maker, and accountable editor. The AI acts as structured co-author, interviewer, editor, critic, researcher, and implementation agent.

## What SDA Means

Specification-Driven Authoring is a writing workflow in which the writer and AI first create an explicit specification for the article before generating the article itself. The specification records the writer's intent: purpose, audience, thesis, structure, tone, sources, constraints, visual plan, and approval status. The AI then uses that specification as the primary source of truth for outlining, drafting, reviewing, revising, and preparing the final article.

The basic SDA lifecycle is:

```text
idea -> specification -> approval -> outline -> draft -> review -> revision -> final article
```

The key discipline is that the writer approves the specification before the AI produces the full draft. This keeps the AI from improvising the article's purpose, structure, claims, or voice.

## Core Rule

Do not start by drafting the article. Start by creating or refining the specification.

The specification is the contract between the writer's intent and the AI's output. It should define what the article is trying to do before the AI produces the article itself.

## Quality Standard

When creating article files from an approved specification, optimize for quality above speed, token economy, or minimal model usage.

- Use the strongest available model unless the user explicitly chooses another model or imposes a cost, speed, or token constraint.
- Use as much context and output length as needed to follow the specification well.
- Do not compress reasoning, research, review, or revision steps merely to save tokens.
- Prefer careful staged work over a fast single-pass draft when quality would benefit.
- Treat the approved specification, source verification, publication requirements, and author voice as higher priorities than speed.

## Phase 1: Build the Specification

Work only on the article specification file, conventionally named `00_SPEC.md`, until the user explicitly approves it.

Use this loop:

1. Read the current article specification file.
2. Identify the single most important unresolved issue.
3. Ask one focused question.
4. After the user answers, propose the exact change to the article specification file.
5. Edit the article specification file only after approval, unless the user explicitly asks for direct editing.
6. Preserve accepted decisions.
7. Record unresolved matters clearly.
8. Avoid drafting article prose, except very small examples to clarify tone or structure.
9. When the spec is mature enough, explain why and ask whether to mark it approved.

The specification should eventually cover:

- working title and alternatives;
- purpose and thesis;
- target publication or publication type;
- audience and desired reader transformation;
- scope and exclusions;
- article length or length philosophy;
- tone, voice, and author perspective;
- key concepts and terminology;
- main claims and counterarguments;
- examples, cases, and evidence needs;
- research and citation requirements;
- ethical and practical concerns;
- structure, opening, and conclusion;
- image and figure plan;
- source verification rules;
- versioning and review rules;
- quality criteria;
- unresolved questions;
- approval status.

## Phase 2: Create the Article Project

Create additional article files only after the user approves the article specification file.

Before creating files, propose the project structure and get approval. A typical structure is:

```text
Article Folder/
├── 00_SPEC.md
├── 01_RESEARCH_PLAN.md
├── 02_SOURCES.md
├── 03_OUTLINE.md
├── 04_DRAFT.md
├── 05_IMAGE_PROMPTS.md
├── 06_EDITORIAL_REVIEW.md
├── 07_REVISION_PLAN.md
├── 08_FINAL.md
└── Images/
```

Adapt the file set to the approved specification. Do not create unnecessary files.

## Phase 3: Research and Sources

Treat facts, interpretations, assumptions, and creative choices differently.

- Factual and technical claims should be checked against external sources.
- If a credible source supports a claim, cite it.
- If no credible source is found after a reasonable search, present the claim only as the author's interpretation, hypothesis, original observation, or workflow experience.
- Never invent sources.
- Never imply consensus where none was found.
- Prefer direct links to original documents, official documentation, papers, guidelines, or primary sources.
- Keep references in a dedicated sources file when the project has moved beyond specification.

When writing for publications with citation rules, follow those rules. If the publication requests numerical references, use references such as `[1]`, `[2]`, and keep source details easy to verify.

## Phase 4: Outline, Draft, Review, Revise

Generate the outline from the approved specification, not from memory.

When drafting:

- Prioritize quality over speed or token count.
- Preserve the author's voice and decisions.
- Keep article sections aligned with the approved structure.
- Avoid adding unsupported claims.
- Flag missing evidence instead of filling gaps with invented certainty.
- Keep edits inspectable.

When reviewing:

- Review every draft against the article specification file.
- Identify mismatches between the draft and the specification.
- Separate structural issues, factual/source issues, tone issues, and publication-guideline issues.
- Propose a revision plan before large rewrites.

When revising:

- Prefer targeted edits over uncontrolled full rewrites.
- Preserve accepted material.
- Make significant changes easy to accept, reject, or revert.

## Images and Figures

Use images to explain the article, not to decorate it generically.

When the approved specification calls for images, create both:

- a reusable image prompt set, usually in `05_IMAGE_PROMPTS.md`;
- the actual image files, stored in the article's image folder.

For each planned image or figure, record:

- article location;
- purpose;
- suggested file name;
- prompt or creation instructions;
- caption/source line;
- alt text;
- usage rights or author-created status.

Store images in a separate image folder when the project moves beyond specification. Use one image per file. Name image files according to how they are referenced in the article.

If AI-generated images are used, identify them as author-created AI-assisted illustrations unless the publication requires different wording.

After creating image prompts, use those prompts to generate the images unless the user explicitly asks for prompts only. Choose the best production approach for the article rather than asking the user to decide every visual detail. For explanatory diagrams, prioritize clarity over decorative polish: generated visuals may use minimal or no embedded text, with precise labels, captions, source lines, and alt text kept in the article when that will produce a more reliable result.

Do not consider an article package complete while referenced image files are missing. Either generate the files, replace the references with prompt-only placeholders, or clearly mark the images as pending.

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
- Do not commit private setup files, full chat exports, credentials, or unrelated local notes unless the user explicitly requests it.

## Publication Safeguards

Before final submission:

- Check the article against the approved specification.
- Check the article against publication guidelines.
- Verify citations and links.
- Confirm image rights, captions, and alt text.
- Run a grammar and readability pass.
- Check for plagiarism risk.
- Confirm that no unsupported claim is presented as established fact.

## Useful Agent Behaviors

When the user asks to work on a specification, ask one question at a time.

When the user provides a decision, propose exact spec text before editing unless direct editing is requested.

When the user asks to create or revise article files, first read the article specification file, conventionally named `00_SPEC.md`.

When the user asks to save work, use the writer-facing versioning language and explain what was saved.

When unsure, preserve author control: ask before making irreversible or broad changes.

## Future Application Vision

The long-term goal is a purpose-built writing application that gives non-developers SDA, AI collaboration, source tracking, image handling, and version history out of the box.

Until such an application exists, a practical setup can combine:

- a text editor such as VS Code;
- an AI coding or writing agent such as Codex;
- Markdown files;
- Git/GitHub versioning hidden behind writer-friendly commands.
