# Codex Skills

Reusable skills for Codex workflows. Each skill is self-contained in its own
directory under `skills/` and is defined by a `SKILL.md` file.

## Available skills

| Skill | Purpose |
| --- | --- |
| [`dez-ticket-create`](skills/dez-ticket-create/SKILL.md) | Create structured tickets for features, bug fixes, and improvements. |
| [`dez-ticket-implement`](skills/dez-ticket-implement/SKILL.md) | Research, plan, implement, and verify ticket work. |

The ticket-creation skill includes a reusable template at
[`skills/dez-ticket-create/assets/ticket-template.md`](skills/dez-ticket-create/assets/ticket-template.md).

## Repository structure

```text
skills/
├── dez-ticket-create/
│   ├── SKILL.md
│   └── assets/
│       └── ticket-template.md
└── dez-ticket-implement/
    └── SKILL.md
```

## Adding a skill

1. Create a lowercase kebab-case directory under `skills/`.
2. Add a `SKILL.md` file with the skill name, description, goal, instructions,
   and any relevant guidelines or assets.
3. Keep templates, examples, and other supporting files inside the skill's
   directory.
4. Update this README with the new skill and its purpose.
5. Review the Markdown and run the validation checks below.

## Validation

There is no build system or automated test suite. Use these checks when making
changes:

```bash
rg --files
git diff --check
```

Also read each affected Markdown file end to end and verify that referenced
paths and instructions exist.

## License

This project is released under the [MIT License](LICENSE).
