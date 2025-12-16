# Contributing to shandy-openskills

Thank you for your interest in contributing domain expertise to shandy-openskills!

## How to Contribute

### Adding a New Domain

1. Fork this repository
2. Create a new directory for your domain: `my-domain/`
3. Add a `SKILL.md` file with the required format (see below)
4. Submit a pull request

### Improving an Existing Domain

1. Fork this repository
2. Edit the relevant `SKILL.md` or reference files
3. Submit a pull request with a clear description of your changes

## Skill Format

Every skill must have a `SKILL.md` file with YAML frontmatter:

```yaml
---
name: my-domain-name
description: Brief description of what this skill does and when to use it (max 1024 chars)
---

# My Domain Name

## When to Use This Skill

- Bullet points describing when Claude should use this skill
- Be specific about data types, file formats, or research questions

## Core Concepts

[Explain key concepts in the domain...]

## Analysis Strategies

[Provide specific, actionable guidance...]

## Common Pitfalls

[Warn about common mistakes...]
```

### Naming Requirements

- `name`: lowercase letters, numbers, and hyphens only
- Maximum 64 characters
- Cannot contain "anthropic" or "claude"

### Content Guidelines

- Keep `SKILL.md` under 5,000 words
- Split large content into separate reference files
- Use concrete examples with code snippets where helpful
- Focus on actionable guidance, not general background

## Directory Structure

```
my-domain/
├── SKILL.md              # Required: main skill file
├── references/           # Optional: additional documentation
│   ├── topic-a.md
│   └── topic-b.md
└── scripts/              # Optional: helper scripts
    └── analysis.py
```

## Quality Standards

Before submitting, ensure your skill:

- [ ] Has valid YAML frontmatter with `name` and `description`
- [ ] Includes "When to Use This Skill" section
- [ ] Provides specific, actionable guidance
- [ ] Uses correct domain terminology
- [ ] Includes examples where appropriate
- [ ] Is under 5,000 words (or split into reference files)

## Review Process

1. Submit your PR
2. Maintainers will review for quality and accuracy
3. You may be asked to make revisions
4. Once approved, your skill will be merged

## Code of Conduct

Be respectful and constructive. We're building shared knowledge for the scientific community.

## Questions?

Open an issue if you have questions about contributing.
