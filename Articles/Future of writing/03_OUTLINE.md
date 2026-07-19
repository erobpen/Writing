# Outline

## Working Title

Future of Writing: From Writing Tools to Specification-Driven Authoring

## Subtitle

AI-assisted writing is not the end of authorship. It is the next interface problem, and writers need workflows that keep them in control.

## Article Shape

The article follows the approved 1/5, 2/5, 2/5 balance:

- Part 1: personal essay and legitimacy argument.
- Part 2: high-level SDA theory.
- Part 3: practical tutorial, split into setup and usage.

## Part 1: Writing Tools Did Not Start With LLMs

Purpose:

- Establish trust through the author's perspective.
- Argue that AI-assisted writing is part of a long evolution of writing tools.
- Avoid spending too long on the legitimacy debate.

Key beats:

1. Start with the discomfort around "AI writing" and "cheating."
2. Move backward through the tool lineage: pen and paper, typewriter, computer, text editor, spellchecker, grammar checker, AutoCorrect, autocomplete, language models, LLMs.
3. Explain that earlier language models existed before LLMs, but modern LLMs changed the interface by letting writers communicate through natural language.
4. Connect to Licklider's older idea of humans and computers cooperating, with humans setting goals and computers doing routinizable work.
5. Add the caution: the computer is still not human.
6. Mention Max Kotin's video as a reference candidate about judging text rather than suspected AI authorship.
7. Transition: if natural language is powerful but slippery, writers need a process. That process is SDA.

Suggested figure:

- Figure 1: From Writing Assistance to Agentic Writing.

## Part 2: What Specification-Driven Authoring Is

Purpose:

- Define SDA as a structured workflow.
- Explain why it is different from "ask AI to write an article."
- Show how human authorship is preserved.

Key concepts:

- Specification as the contract between intent and output.
- Human writer as author, decision-maker, and accountable editor.
- AI as interviewer, critic, researcher, editor, and implementation agent.
- Approval before drafting.
- Review against the specification.
- Source verification and image planning.
- Version history as safety.

Lifecycle:

```text
idea -> specification -> approval -> outline -> draft -> review -> revision -> final article
```

Important distinction:

- Prompting asks the AI for an answer.
- SDA builds the conditions under which an answer can be judged.

Suggested figures:

- Figure 2: The SDA Loop.
- Figure 3: Roles in Specification-Driven Authoring.
- Optional Figure 4: Specification as Contract.

## Part 3A: Setup

Purpose:

- Give readers a practical first setup, not every possible setup.
- Use VS Code + Codex + Git/GitHub.
- Translate developer tooling into writer language.

Setup steps:

1. Install VS Code.
2. Install Git.
3. Install or enable Codex in VS Code.
4. Create a writing project folder.
5. Create one subfolder per article.
6. Use a convention: each article begins with an article specification file, normally `00_SPEC.md`.
7. Create a Git repository for the writing folder.
8. Connect it to GitHub.
9. Keep private notes, full chat exports, and credentials out of public commits unless deliberately reviewed.

Suggested figures:

- Figure 5: Writer-Friendly Versioning.
- Figure 6: Setup and Usage Flow.

## Part 3B: Usage

Purpose:

- Show how the workflow feels in practice.
- Connect every practical action back to the SDA theory.

Usage loop:

1. Open the article folder.
2. Ask the agent to read the article specification.
3. Let the agent identify one unresolved issue.
4. Answer one focused question.
5. Approve exact spec changes.
6. Save Version.
7. Repeat until the spec is approved.
8. Generate article files from the approved spec.
9. Create research plan and source list.
10. Create outline.
11. Draft.
12. Review against spec.
13. Revise.
14. Publish Backup to GitHub.
15. Prepare final article after review.

Writer-facing commands:

- Save Version.
- Compare Versions.
- Restore Previous Version.
- Publish Backup to GitHub.

## Conclusion

Purpose:

- Reaffirm democratization of agentic AI.
- Acknowledge that the setup is not ideal yet.
- Point to the need for a purpose-built SDA writing application.
- Mention future articles about alternate setups and deeper human-computer communication issues.
- Link to the GitHub repository for readers who want the full process trail.
