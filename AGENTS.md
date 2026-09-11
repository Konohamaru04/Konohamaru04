# AGENTS.md

## Purpose

This repository is the source for a highly customized GitHub profile README.

The goal is to make the profile feel like a polished developer landing page rather than a collection of generic badges. The finished profile should communicate, within a few seconds:

- Amartya Deshmukh is a Lead Engineer.
- Primary strengths: full-stack engineering, AI/ML, GPU computing, developer tooling, and open source.
- Core technologies include C#, .NET, Python, TypeScript, Angular, React, PyTorch, CUDA, Docker, Azure, GitHub, and related tooling.
- The profile should prominently showcase technically interesting projects and open-source work.
- The visual identity should feel modern, technical, premium, and slightly futuristic.

The GitHub username is:

`Konohamaru04`

The GitHub profile repository is expected to be:

`Konohamaru04/Konohamaru04`

---

## Agent Working Style

Before making changes:

1. Inspect the existing repository.
2. Read the current `README.md`, `.github/workflows/`, and `assets/` if they exist.
3. Preserve any useful existing content unless replacing it clearly improves the result.
4. Make a short implementation plan before editing.
5. Prefer completing the requested work end-to-end rather than leaving placeholders.
6. Validate links, Markdown structure, asset paths, and GitHub Actions YAML after editing.
7. Summarize the files changed and any remaining manual setup.

Do not rewrite unrelated files.

Do not create unnecessary frameworks, package managers, or build systems for a profile README.

---

## Design Direction

Target aesthetic:

- dark developer dashboard
- terminal / engineering telemetry
- subtle cyberpunk or AI-lab influence
- premium rather than flashy
- clean spacing
- strong typography
- restrained animation
- consistent visual language

Suggested visual vocabulary:

- graphite / near-black backgrounds
- off-white text
- subtle green, cyan, blue, or violet accents
- monospace-inspired labels
- thin borders
- small telemetry-style labels
- grids, nodes, traces, waveform-like accents, or terminal elements

Avoid:

- excessive emojis
- dozens of unrelated shields
- huge walls of technology icons
- meme GIFs
- cluttered layouts
- neon overload
- overly childish visuals
- fake metrics
- fake experience
- fake projects
- fake contribution data
- huge blocks of biography text

The profile should look credible to engineers, recruiters, open-source users, and technical leaders.

---

## README Structure

Prefer a structure close to the following:

1. Hero
2. Short engineering identity / introduction
3. Current focus
4. Technology stack
5. Featured projects
6. GitHub / open-source telemetry
7. Contribution visualization
8. Optional activity or current-building section
9. Contact / links
10. Minimal footer

Do not mechanically add every section if it hurts the composition.

The first screen should be strong enough to work without scrolling.

---

## Hero Requirements

The hero should clearly communicate:

`AMARTYA DESHMUKH`

and a compact professional identity similar to:

`LEAD ENGINEER // FULL STACK // AI // GPU COMPUTING`

A short animated typing line may be used if it improves the page.

Possible copy direction:

- Building AI-powered developer tools.
- Full-stack engineering meets GPU computing.
- C# / Python / TypeScript / CUDA.
- Building things that probably use too much VRAM.

Keep humor subtle.

Do not make the hero feel like a résumé header.

---

## About / Identity

Keep the introduction concise.

Prefer 2-4 short lines over a long paragraph.

Emphasize:

- Lead Engineer
- Full-stack engineering
- AI / ML
- GPU computing
- developer tooling
- open source
- practical engineering and shipping products

Do not include private employer/client information unless it already exists in the repository or the user explicitly asks for it.

---

## Featured Projects

Projects are more important than generic profile statistics.

Prioritize strong technical projects such as:

### ComfyUI NVIDIA DLSS Frame Interpolation

Repository:
`Konohamaru04/ComfyUI-NVIDIA-DLSS-Frame-Interpolation`

Position it as a flagship project when appropriate.

Focus on:
- NVIDIA DLSS
- frame interpolation / frame generation
- ComfyUI integration
- GPU acceleration
- practical AI/video workflows

Do not hardcode star counts unless the value is dynamically sourced or explicitly provided for a snapshot.

### Tiny-LLM

Repository:
`Konohamaru04/Tiny-LLM`

Focus on:
- language-model engineering
- tokenizer / BPE
- transformer training
- PyTorch
- CUDA / GPU experimentation

### AutoComplete Engine

If a public repository exists, link it.

Focus on:
- ranking
- prefix search
- performance
- algorithms
- low-latency engineering

Do not invent URLs for repositories that cannot be found in the repo or provided context.

Featured project cards should explain why the project matters, not merely repeat the repository name.

---

## Technology Stack

Core stack may include:

### Languages
- C#
- Python
- TypeScript
- JavaScript
- SQL

### Application Development
- .NET
- ASP.NET
- Angular
- React
- Node.js
- Tauri
- Electron

### AI / ML / GPU
- PyTorch
- OpenCV
- ONNX Runtime
- CUDA
- FFmpeg
- ComfyUI
- local LLM tooling

### Data / Cloud / DevOps
- SQL Server
- SQLite
- Azure
- Docker
- GitHub Actions

Use technology icons selectively.

Prefer curated groups over a massive unstructured icon wall.

---

## GitHub Stats

Stats are supporting content, not the hero.

If using third-party generated cards:

- keep styling consistent with the profile
- hide unnecessary borders
- avoid excessive card count
- ensure cards degrade gracefully
- do not rely on them for essential information

Possible services include GitHub Readme Stats or similar established services, but avoid adding a dependency if a custom SVG or native GitHub content communicates the same information better.

Never fabricate:
- stars
- followers
- commits
- PR counts
- streaks
- repository metrics

---

## Contribution Animation

A contribution snake may be implemented using GitHub Actions.

Preferred output paths:

`dist/github-contribution-grid-snake.svg`

and/or:

`dist/github-contribution-grid-snake-dark.svg`

If adding the workflow:

- use minimal permissions
- use supported action versions
- schedule it reasonably
- allow manual dispatch
- write generated output to a dedicated branch if required by the chosen action
- reference the output correctly from `README.md`

Do not add an animation simply because it is popular. It must fit the visual design.

---

## Custom SVG Assets

Custom SVGs are encouraged when they materially improve the profile.

Good uses:

- hero banner
- terminal/status card
- project header
- engineering telemetry panel
- section separators
- compact stack visualization

Store authored assets under:

`assets/`

Use descriptive names, for example:

`assets/hero.svg`
`assets/system-card.svg`
`assets/stack.svg`

Requirements:

- SVG must be valid XML.
- Avoid scripts.
- Avoid external JavaScript.
- Avoid inaccessible tiny text.
- Keep text readable on desktop and mobile.
- Prefer responsive `viewBox`-based SVGs.
- Optimize file size where practical.
- Do not embed huge raster images into SVG.

If animations are used, keep them subtle and avoid distracting infinite motion.

---

## Dark / Light Theme

Where useful, use a `<picture>` element with `prefers-color-scheme` so GitHub can show different assets for dark and light themes.

Example pattern:

```html
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/hero-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/hero-light.svg">
  <img alt="Amartya Deshmukh — Lead Engineer" src="./assets/hero-dark.svg">
</picture>
```

Do not duplicate assets unless dark/light variants create a meaningful improvement.

---

## GitHub Markdown Constraints

This is a GitHub profile README, not a normal website.

Assume:

- JavaScript will not run.
- Arbitrary CSS should not be relied upon.
- Markdown and GitHub-supported HTML are the primary layout mechanisms.
- Remote images may fail or rate-limit.
- Relative repository assets are preferable for authored visuals.

Favor robust GitHub-compatible markup over browser tricks.

---

## Responsive Layout

The profile must remain readable on mobile.

Avoid:

- fixed-width layouts that require horizontal scrolling
- giant banners with tiny text
- overly wide tables
- too many side-by-side cards

When using HTML alignment or multiple images, verify that the result still degrades cleanly on narrow screens.

---

## Accessibility

Every meaningful image should have useful alt text.

Do not encode critical information only through color.

Maintain reasonable contrast.

Avoid flashing or aggressive animation.

---

## Repository Layout

Prefer a simple structure:

```text
.
├── AGENTS.md
├── README.md
├── assets/
│   ├── hero-dark.svg
│   ├── hero-light.svg
│   └── ...
└── .github/
    └── workflows/
        └── snake.yml
```

Only add directories when they are actually needed.

---

## Content Accuracy

Use only information supported by:

1. the repository,
2. linked public GitHub repositories,
3. explicit user instructions,
4. verifiable public information when research is requested.

Do not invent:
- job history
- project metrics
- awards
- company names
- follower counts
- star counts
- social links
- email addresses

If a value changes frequently, prefer a dynamic source or omit the number.

---

## External Links

For repository links, prefer canonical GitHub URLs.

Before adding social/contact links:
- reuse links already present in the repository, or
- add only links explicitly provided by the user.

Do not guess usernames on other platforms.

---

## Quality Bar

The final README should feel intentionally designed.

A good result should:

- communicate identity immediately
- make featured engineering work easy to discover
- have strong information hierarchy
- look cohesive in GitHub dark mode
- remain readable in light mode
- work on mobile
- contain no broken images
- contain no fake data
- avoid generic README-template vibes

When choosing between adding another widget and preserving whitespace, usually preserve whitespace.

---

## Validation

Before finishing, check:

1. `README.md` renders as valid GitHub-flavored Markdown.
2. Relative asset paths exist.
3. Repository URLs are valid.
4. SVG files are valid and have appropriate `viewBox` attributes.
5. Workflow YAML parses correctly.
6. Workflow permissions are no broader than necessary.
7. Generated-asset URLs match the workflow output.
8. No placeholder text remains unless explicitly marked for user input.
9. There is no fake dynamic data.
10. The page is not overloaded with third-party services.

If a tool for previewing Markdown is available, use it.

---

## Definition of Done

The task is complete when:

- the profile has a coherent visual identity
- the hero is polished
- the copy is concise
- the tech stack is curated
- flagship projects are prominent
- optional stats/animations visually match the design
- GitHub-specific limitations have been respected
- all changed files have been validated
- the final response explains exactly what was changed
