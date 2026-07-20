# Image Prompts

Images should explain the SDA process rather than decorate the article generically. If generated images include unreliable text, generate the visual without labels and add labels manually afterward.

## Required Figure Set

### Figure 1: From Writing Assistance to Agentic Writing

- File name: `figure_01_tool_evolution.png`
- Location: Part 1.
- Caption draft: The path from physical writing tools to agentic writing assistants is an evolution of interfaces, not a single rupture.
- Alt text: Timeline showing writing tools evolving from pen and paper to typewriter, text editor, spellchecker, AutoCorrect, autocomplete, LLM chat assistant, and agentic writing assistant.
- Source note: Author-created AI-assisted illustration.
- Prompt:

```text
Create a clean editorial timeline diagram for a Medium article. Show the evolution of writing and computer-mediated writing assistance from pen and paper, typewriter, computer text editor, spellchecker, autocorrect, autocomplete, earlier language models, LLM chat assistant, to agentic writing assistant. The mood should be thoughtful and professional, not futuristic hype. Use a light background, simple icons, and clear horizontal progression. Leave generous space for labels if text will be added later. No brand logos.
```

### Figure 2: The SDA Loop

- File name: `figure_02_sda_loop.png`
- Location: Part 2.
- Caption draft: Specification-Driven Authoring turns AI writing into a reviewable loop: define intent first, draft second, revise against the specification.
- Alt text: Circular workflow with idea, questions, specification, approval, outline, draft, review, revision, and final article.
- Source note: Author-created AI-assisted illustration.
- Prompt:

```text
Create a clear process-loop diagram for Specification-Driven Authoring. Show these stages in a circular workflow: idea, writer-AI questions, specification, human approval, draft generation, review against specification, revision, final article. Emphasize that the human writer approves the specification and remains in control. Use an elegant editorial style, light background, restrained colors, and simple arrows. Make it understandable to non-developer writers. Avoid code imagery.
```

### Figure 3: Roles in Specification-Driven Authoring

- File name: `figure_03_roles_and_control.png`
- Location: Part 2.
- Caption draft: In SDA, the human remains author and decision-maker while the AI performs supporting roles.
- Alt text: Human writer at center, AI roles around the writer, with specification, sources, and version history as safeguards.
- Source note: Author-created AI-assisted illustration.
- Prompt:

```text
Create a simple role map for an AI-assisted writing workflow. Put the human writer at the center as author and decision-maker. Around the writer, show the AI agent as assistant, editor, critic, researcher, and implementation helper. Show the specification as a shared document that guides the AI. Show sources and version history as supporting safeguards. The style should be calm, clear, and educational, suitable for a technology essay on Medium.
```

### Figure 5: Writer-Friendly Versioning

- File name: `figure_05_writer_friendly_versioning.png`
- Location: Part 3A or Part 3B.
- Caption draft: Writers do not need to think in Git commands; they need safe writing actions.
- Alt text: Four writer-facing actions: Save Version, Compare Versions, Restore Previous Version, and Publish Backup to GitHub, with Git as an invisible safety layer.
- Source note: Author-created AI-assisted illustration.
- Prompt:

```text
Create an explanatory diagram that translates Git version control into writer-friendly actions. Show four actions: Save Version, Compare Versions, Restore Previous Version, and Publish Backup to GitHub. Present Git as an invisible safety layer behind the writing workflow, not as a developer tool the writer must master. Use a calm, trustworthy style, with document snapshots or stacked pages as visual metaphors.
```

### Figure 6: Setup and Usage Flow

- File name: `figure_06_setup_usage_flow.png`
- Location: Part 3.
- Caption draft: The setup is technical, but the daily workflow should feel editorial: specify, approve, draft, review, revise, and save.
- Alt text: Two-part flow: setup with VS Code, Codex, GitHub, and project folder; usage with specification, questions, approval, draft, source verification, revision, and publishing.
- Source note: Author-created AI-assisted illustration.
- Prompt:

```text
Create a two-part flow diagram for writers using Specification-Driven Authoring with VS Code, Codex, and Git. Part A is setup: install/open VS Code, connect Codex, prepare project folder, connect GitHub/versioning. Part B is usage: create specification, answer AI questions, approve spec changes, save version, generate draft, verify sources, revise, publish. Use simple icons and arrows, with a clean Medium-style editorial look. Make the flow approachable for non-developers.
```

## Additional Figures Used In Final Article

These figures were optional during planning but are now referenced in `08_FINAL.md`.

### Figure 4: Specification as Contract

- File name: `figure_04_spec_as_contract.png`
- Location: Part 2.
- Caption draft: The specification translates author intent into criteria the AI draft can be judged against.
- Alt text: Writer goals on the left, specification in the center, article outputs on the right.
- Source note: Author-created AI-assisted illustration.
- Prompt:

```text
Create a conceptual diagram showing a writing specification as the contract between human intent and AI-generated output. On the left, show the writer's goals, audience, tone, claims, sources, constraints, and structure. In the center, show the specification document as the organizing layer. On the right, show outline, draft, review, revision, and final article. Use a professional editorial diagram style with clean boxes and arrows. No software logos.
```

### Figure 7: Claim and Source Verification Flow

- File name: `figure_07_source_verification.png`
- Location: Part 3B or reference discussion.
- Caption draft: SDA separates sourced fact, author interpretation, and unsupported claims before publication.
- Alt text: Decision flow from claim to source search, citation if found, reframing or removal if not found, and final hallucination review.
- Source note: Author-created AI-assisted illustration.
- Prompt:

```text
Create a decision-flow diagram for source verification in AI-assisted writing. Start with a claim in the draft. Then show: search for external source, credible source found, cite with numerical reference, or no source found, reframe as author's interpretation or remove claim. Include a final review step for hallucination risk. Use a clear, minimal editorial style and avoid clutter.
```

## Tutorial Screenshot-Style Figures

These are article-facing instructional figures for Part 3A. They should look like clear screenshots a non-developer writer can follow, but they are author-created screenshot-style figures rather than official product screenshots.

### Figure 8: Install Codex Extension

- File name: `figure_08_install_codex_extension.png`
- Location: Part 3A, after the Codex extension installation steps.
- Caption draft: Install Codex from the VS Code Extensions view.
- Alt text: Screenshot-style guide showing the VS Code Extensions view, a search for Codex, the OpenAI Codex extension card, and the Install button.
- Source note: Author-created instructional screenshot-style figure.
- Prompt:

```text
Create a clear screenshot-style tutorial figure showing Visual Studio Code on Windows with the Extensions view open. Highlight the Extensions button, the search box containing "Codex", the result "Codex - OpenAI's coding agent" by OpenAI, and an Install button. Use clean readable interface text, simple callouts, and a Windows tutorial style. Avoid tiny text and avoid using unofficial logos beyond generic UI shapes.
```

### Figure 9: Create GitHub Account

- File name: `figure_09_create_github_account.png`
- Location: Part 3A, after the GitHub account setup step.
- Caption draft: Create a GitHub account first, then let Codex help connect the writing folder later.
- Alt text: Screenshot-style guide showing a browser on GitHub signup, with email, password, username, and email verification highlighted.
- Source note: Author-created instructional screenshot-style figure.
- Prompt:

```text
Create a clear screenshot-style tutorial figure showing a browser on a GitHub account creation page. Highlight fields for email, password, username, and email verification. Include a small note that GitHub will be used as backup later. Use clean readable interface text and generic browser chrome. Do not imitate a live official screenshot exactly; make it instructional and publication-ready.
```

### Figure 10: Create Writing Folders

- File name: `figure_10_create_writing_folders.png`
- Location: Part 3A, after the Windows File Explorer folder steps.
- Caption draft: Create the writing folders in Windows File Explorer before asking Codex to configure the project.
- Alt text: Screenshot-style guide showing Windows File Explorer with Documents, a Writing folder, a Name of your Article folder, and an Images folder.
- Source note: Author-created instructional screenshot-style figure.
- Prompt:

```text
Create a clear screenshot-style tutorial figure showing Windows File Explorer. Show Documents > Writing > Name of your Article > Images. Highlight the Writing folder, article folder, and Images folder. Use callouts that say create folders in File Explorer, not the terminal. Use a calm instructional style with large readable labels.
```

### Figure 11: Codex Setup Prompt

- File name: `figure_11_codex_setup_prompt.png`
- Location: Part 3A, after the setup prompt.
- Caption draft: After the folders and `SDA_SKILL.md` exist, paste the setup prompt into Codex and let the agent handle the Git side.
- Alt text: Screenshot-style guide showing VS Code with the Writing folder open, SDA_SKILL.md and 00_SPEC.md visible, and the Codex sidebar containing the setup prompt.
- Source note: Author-created instructional screenshot-style figure.
- Prompt:

```text
Create a clear screenshot-style tutorial figure showing VS Code with a Writing folder open. In the file explorer show SDA_SKILL.md, Name of your Article, 00_SPEC.md, and Images. On the right show a Codex sidebar with a setup prompt beginning "I am a writer, not a developer." Highlight that Codex will set up Git versioning and ask one focused specification question. Use readable text and a clean instructional layout.
```
