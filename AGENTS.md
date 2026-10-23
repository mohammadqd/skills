# Repository Guidelines

## Project Structure & Module Organization

This repository contains reusable Codex skills. Each skill lives in its own
directory under `skills/` and is primarily defined by a `SKILL.md` file. Keep
skill-specific templates, examples, or other supporting files in that skill's
directory, such as `skills/dez-create-ticket/assets/`. There is no application
source tree or generated build output.

## Build, Test, and Development Commands

No build system or automated test suite is configured. Use these lightweight
checks while developing:

- `rg --files` — list tracked-style files and confirm the expected layout.
- `sed -n '1,240p' skills/<name>/SKILL.md` — inspect a skill and its instructions.
- `git diff --check` — catch whitespace errors before committing.

Validate changes by reading the affected Markdown files end to end and
checking that referenced paths and instructions exist.

## Coding Style & Naming Conventions

Write Markdown with clear headings, short paragraphs, and actionable numbered
steps. Use repository-relative paths in examples. Name skill directories with
lowercase kebab-case (for example, `dez-create-ticket`) and keep the required
entry file named `SKILL.md`. Use concise YAML front matter with `name` and
`description` when a skill needs metadata. Avoid adding dependencies or code
when a documented workflow is sufficient.

## Testing Guidelines

There are no language-level tests or coverage requirements. For documentation
changes, perform a manual review: verify Markdown structure, command examples,
links, referenced assets, and consistency with neighboring skills.

## Commit & Pull Request Guidelines

Existing commits use short, plain-language summaries (for example,
`adding two skills to create and implement tickets`). Follow the same style:
use a concise imperative or action-oriented subject, and keep unrelated edits
out of the commit.

Pull requests should explain the user-facing workflow change, list affected
skills or assets, and include validation performed (normally `git diff --check`
plus a manual Markdown review). Add screenshots only when rendered layout is
important; otherwise, link relevant files and examples directly.
