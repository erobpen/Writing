# Future of Writing: From Writing Tools to Specification-Driven Authoring

AI-assisted writing is not the end of authorship. It is the next interface problem, and writers need workflows that keep them in control.

Draft note: citation [14] is author-provided and must be independently verified before final publication.

![Figure 1 placeholder: From Writing Assistance to Agentic Writing](Images/figure_01_tool_evolution.png)

## Writing Tools Did Not Start With LLMs

When people say that using AI for writing is cheating, I understand the concern. Writing is personal. It carries our judgment, our taste, our errors, our ambition, and sometimes our insecurity. If a machine is involved, it is easy to feel that something essential has been taken away.

But I do not think the question is as simple as "human or AI." Writers have always used tools. Pen and paper changed what could be recorded. Typewriters changed speed, legibility, and the physical labor of revision. Computers and text editors changed deletion, rearrangement, duplication, search, and storage. Spellcheckers and grammar checkers made correction part of the writing surface itself [3]. AutoCorrect made the machine intervene even earlier, replacing small mistakes while the writer was still composing [4].

Before large language models, there were language models. They were not chat assistants. They did not behave like collaborators. But the underlying idea that a system can model language, predict likely words, and assign probabilities to sequences is older than the current LLM wave. Jurafsky and Martin's textbook treats n-gram language models as a foundational part of natural language processing [2]. The difference now is scale, interface, and generality. GPT-3, for example, was presented as a large language model that could perform tasks from text instructions and examples without gradient updates for each task [5].

That is why I see LLMs less as an alien rupture and more as a major step in a long path. The path runs from writing tools to computer writing tools, from text editors to language models, and from language models to systems that can participate in a writing process through natural language.

This also connects to an older dream in computing: communicating with computers in a way that feels closer to human communication. In 1960, J. C. R. Licklider described "man-computer symbiosis" as a cooperative relationship in which humans would set goals and criteria while computers performed routinizable work needed to prepare for insight and decision [1]. That sounds surprisingly close to the best version of AI-assisted writing today. The writer sets the purpose, audience, thesis, constraints, and standard of quality. The machine helps organize, draft, compare, check, and revise.

But there is an important danger here. A computer that accepts natural language is still not human. It does not become a colleague in the moral sense just because we can talk to it in sentences. Engineers have long experience communicating with computers through formal languages, commands, APIs, and structured workflows. Natural language makes some of that power available to non-engineers, but it can also hide what is happening. It can make a system feel as if it understands, verifies, or intends more than it really does.

That is why I do not believe the real future of writing is simply "ask AI to write." That is too loose. It gives the model too much room to invent the article's purpose, structure, and evidence. Nor do I think the answer is to hunt for "AI writing" as if every suspicious sentence reveals guilt. Max Kotin recently argued that attempts to detect AI writing can be misleading or harmful, and that the better question is whether the text itself is good [14]. I agree with the direction of that argument: the human writer's judgment and responsibility matter more than whether AI was used as a tool.

The better question is this: how do we use AI in a way that preserves authorship?

My answer is Specification-Driven Authoring.

![Figure 2 placeholder: The SDA Loop](Images/figure_02_sda_loop.png)

## What Specification-Driven Authoring Means

Specification-Driven Authoring, or SDA, is a writing workflow in which the writer and the AI first create a specification for the article before generating the article itself.

That sounds simple, but it changes the relationship. Instead of asking the AI to write an article from a vague prompt, the writer and AI first define the article. The specification records the writer's intent: purpose, audience, thesis, structure, tone, claims, sources, exclusions, images, quality criteria, and unresolved questions.

Only after the specification is mature does the writer approve it. Then the AI uses it as the source of truth for the outline, draft, review, revision, and final article.

The lifecycle looks like this:

```text
idea -> specification -> approval -> outline -> draft -> review -> revision -> final article
```

The key word is approval. The writer does not hand the article to the machine and hope for the best. The writer builds a shared document that says what "good" means before the draft exists.

This is the difference between prompting and authoring with a process. A prompt asks for output. A specification defines the conditions under which the output can be judged.

In SDA, the AI can play several roles:

- interviewer, asking focused questions;
- editor, proposing clearer structure and language;
- critic, pointing out missing assumptions or weak claims;
- researcher, identifying claims that need sources;
- implementation agent, creating files, drafts, image prompts, reviews, and revisions.

But the writer remains the author. The writer decides what belongs in the specification. The writer approves changes. The writer judges the draft. The writer is accountable for the final text.

![Figure 3 placeholder: Roles in Specification-Driven Authoring](Images/figure_03_roles_and_control.png)

## Why the Specification Matters

The specification is the contract between the writer's intent and the AI's output.

Without a specification, the AI tends to optimize for plausible completeness. It may choose the audience, tone, examples, and structure without asking. It may make the article smoother while moving it away from what the writer actually meant.

With a specification, the writer can inspect the plan before the prose becomes seductive. The writer can say:

- This is the audience.
- This is the central claim.
- This is the tone.
- These are the sources we trust.
- These are the claims that still need evidence.
- These are the things the article should not do.
- This is how we will know whether the draft succeeded.

The specification also protects against one of the most important risks of AI writing: unsupported confidence. If every substantive claim must be checked against an external source, the article becomes less vulnerable to hallucination. If no source is found, the claim can still exist, but only as the author's interpretation, hypothesis, or workflow experience.

That distinction matters. Some claims are facts. Some are interpretations. Some are original ideas. They should not be written in the same voice.

SDA also makes images part of the article plan rather than an afterthought. If the article needs diagrams, the specification can define what each figure should explain, where it belongs, what file name it should have, what caption it needs, and what alt text should accompany it. This matters for publications such as Towards AI, whose contributor guidelines ask writers to use numerical references, cite image sources, include alt text, avoid plagiarism, and submit unpublished Medium drafts with at least five minutes of reading time [6].

Finally, SDA makes versioning part of writing. Developers already benefit from Git and GitHub. Git records changes to files over time so earlier versions can be recalled later [11]. GitHub repositories store files and revision history, and can be public or private [12]. Writers need the same safety, but not necessarily the same vocabulary.

For writers, the useful concepts are simpler:

- Save Version.
- Compare Versions.
- Restore Previous Version.
- Publish Backup to GitHub.

That is enough to begin.

![Figure 5 placeholder: Writer-Friendly Versioning](Images/figure_05_writer_friendly_versioning.png)

## A Practical Setup: VS Code, Codex, Git, and GitHub

There should be a dedicated writing application that does all of this out of the box. A non-developer writer should not have to assemble a coding editor, an AI agent, Markdown files, Git, GitHub, image prompts, and citation tracking just to write an article with discipline.

But until that application exists, we can borrow the developer workflow and translate it into writer language.

The practical setup I am using is:

- VS Code as the editor;
- Codex as the AI agent beside the files;
- Markdown as the writing format;
- Git as the local version history;
- GitHub as the backup and transparency layer.

This is not the only possible setup. Future articles can explore variants. For now, this is a working path.

VS Code is useful because it can open a folder as a workspace, show multiple Markdown files, and work with Git through an integrated source-control interface. Its documentation says Git support is built in, while your machine still needs Git installed [7]. It also provides graphical operations such as staging, committing, viewing diffs, and reviewing commit history without forcing every action through the terminal [7].

Codex is useful because it can work with the context already open in the editor. OpenAI's Codex IDE documentation describes using Codex beside open files, reviewing changes in place, and starting a chat with editor context already available [9]. The Codex CLI documentation also emphasizes working in a local project directory and creating Git checkpoints before and after tasks [10].

Here is the setup in writer language.

### Part A: Set Up the Workspace

1. Install VS Code.

   On Windows, the user setup is recommended for most people because it does not require administrator permissions [8]. After installation, VS Code can open a folder from the command line with `code .`, but writers can also open folders through the graphical interface.

2. Install Git.

   Git is the versioning engine underneath the writer-friendly commands. You do not need to understand all of Git to benefit from it. The important idea is that it records changes over time and lets you return to earlier versions [11].

3. Install or enable Codex in VS Code.

   In VS Code, the practical goal is to have the article files on one side and Codex available beside them. The writer should be able to ask questions, approve changes, and inspect edits in context.

4. Create a writing repository.

   Make one main folder for writing projects. Inside it, create one subfolder per article.

   Example:

   ```text
   Writing/
   ├── SDA_SKILL.md
   ├── Future of writing/
   │   └── 00_SPEC.md
   └── Another article/
       └── 00_SPEC.md
   ```

5. Add the reusable SDA workflow.

   At the root of the writing folder, keep a reusable file such as `SDA_SKILL.md`. This tells the AI agent how the writing process should work across articles.

6. Create the first article specification.

   In each article folder, start with an article specification file, conventionally named `00_SPEC.md`. The `00_` prefix is not magic. It simply makes the specification sort first, where both writer and AI can see that it is the source of truth.

7. Connect to GitHub when ready.

   GitHub should be treated as backup and, when appropriate, as transparency. A public repository can let curious readers inspect the workflow. A private repository is safer for early drafts, sensitive notes, or client work.

![Figure 6 placeholder: Setup and Usage Flow](Images/figure_06_setup_usage_flow.png)

### Part B: Use the Workflow

Once the setup exists, the daily workflow is not technical. It is editorial.

Open the article folder in VS Code. Ask Codex to read the specification. Then follow a simple loop:

1. Codex reads the current specification.
2. Codex identifies the single most important unresolved issue.
3. Codex asks one focused question.
4. The writer answers.
5. Codex proposes the exact change to the specification.
6. The writer approves, rejects, or revises.
7. Codex edits the specification only after approval.
8. The writer runs Save Version.

Repeat this until the specification is good enough.

Then the writer approves the specification for article production. Only then does the AI create the research plan, sources file, outline, draft, image prompts, editorial review, revision plan, and final article.

This is exactly what happened in this article project. The repository for this experiment is available on GitHub for readers who want to inspect the evolving specification and workflow materials [13].

The four versioning commands are the most important part of making this safe for non-developers:

**Save Version** means create a local checkpoint. Use it after an important decision, a good specification update, or a draft milestone.

**Compare Versions** means inspect what changed. This is how the writer sees whether the AI changed only what was approved.

**Restore Previous Version** means recover an earlier checkpoint. This should require explicit confirmation because it can replace current work.

**Publish Backup to GitHub** means push saved work to the remote repository. It is the difference between "saved on this machine" and "backed up outside this machine."

In developer language, these are Git operations. In writer language, they are safety actions.

The same translation should happen across the workflow. "Commit" becomes "Save Version." "Diff" becomes "Compare Versions." "Remote" becomes "GitHub backup." "Repository" becomes "project folder with history."

This translation matters because the goal is not to turn every writer into a developer. The goal is to democratize the part of agentic AI that developers already benefit from: structured files, iterative changes, reviewable edits, source control, and recoverable versions.

## What This Changes

The usual fear is that AI will replace the writer. SDA points in another direction. It treats AI as a powerful assistant, but it also gives the writer structure:

- a specification before the draft;
- approval before major changes;
- sources before factual confidence;
- images planned with purpose;
- review against the original intent;
- version history for safety.

That structure is especially important for non-engineers. Engineers are used to communicating with computers through rigid forms: commands, APIs, compilers, schemas, tests, and version control. Natural language makes the computer easier to approach, but it can also make the workflow feel less bounded than it really should be.

SDA adds the boundary back.

It says: yes, talk to the AI in natural language. But do not let the conversation dissolve the author's responsibility. Put the decisions in a specification. Make the AI propose changes. Approve them. Save versions. Check sources. Review the draft against the intent.

That is not cheating. That is a writing process.

## Conclusion

The future of writing is not just better autocomplete. It is not just chatbots in the margin. It is the gradual transformation of writing into a collaboration between human intention and machine assistance.

But that collaboration needs discipline. If writers simply ask for drafts, they risk getting fluent prose without enough authorship. If they reject all AI assistance, they may miss a tool that can help them think, organize, verify, and revise. Specification-Driven Authoring is one attempt to find the middle path.

This article presents my current practical version: VS Code, Codex, Git, GitHub, Markdown, and a specification-first workflow. It is not the final answer. Future articles can explore different setups, different tools, and the deeper question of what it means to communicate with computers in natural language.

The long-term need is clear: writers should have an application built for this. It should include SDA, AI collaboration, source tracking, image handling, version history, review, and publishing support out of the box.

Until then, we can borrow the developer workflow and make it humane for writers.

## References

[1] J. C. R. Licklider, "Man-Computer Symbiosis," IRE Transactions on Human Factors in Electronics, vol. HFE-1, pp. 4-11, March 1960. https://groups.csail.mit.edu/medg/people/psz/Licklider

[2] D. Jurafsky and J. H. Martin, Speech and Language Processing, 3rd ed. draft, online manuscript released Jan. 6, 2026. https://web.stanford.edu/~jurafsky/slp3/

[3] Microsoft Support, "Check spelling and grammar in Office." https://support.microsoft.com/en-us/office/check-spelling-and-grammar-in-office

[4] Microsoft Support, "Add or remove AutoCorrect entries in Word." https://support.microsoft.com/en-US/Word/add-or-remove-autocorrect-entries-in-word

[5] T. B. Brown et al., "Language Models are Few-Shot Learners," arXiv:2005.14165, 2020. https://arxiv.org/abs/2005.14165

[6] Roberto Iriondo, "Contribute To AI With Towards AI," Towards AI, last updated Sept. 4, 2024. https://pub.towardsai.net/submit-your-medium-story-to-towards-ai-a4fa7e8b141d

[7] Microsoft, "Source Control in VS Code." https://code.visualstudio.com/docs/sourcecontrol/overview

[8] Microsoft, "Installing Visual Studio Code on Windows." https://code.visualstudio.com/docs/setup/windows

[9] OpenAI, "Codex IDE extension," ChatGPT Learn. https://learn.chatgpt.com/docs/codex/ide

[10] OpenAI, "Codex CLI," ChatGPT Learn. https://learn.chatgpt.com/docs/codex/cli

[11] S. Chacon and B. Straub, Pro Git, "About Version Control." https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control

[12] GitHub Docs, "About repositories." https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories

[13] R. Penco, "Writing" project repository. https://github.com/erobpen/Writing

[14] M. Kotin, "Nobody Can Spot AI in Writing, Actually," YouTube, published July 17, 2026. https://youtu.be/tze93ItrA9k?is=_uXCf1vGT5lslqgR
