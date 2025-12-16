# open-science-skills

Community-contributed domain skills for scientific discovery with Claude Code and other AI agents.

**Our goal:** Build a shared repository of scientific domain expertise that helps AI agents reason more effectively about specialized research domains. By capturing best practices, analysis strategies, and common pitfalls for each scientific domain, we enable AI-assisted discovery to benefit from community knowledge rather than starting from scratch every time.

## What are Skills?

Skills are modular capabilities that extend Claude's functionality with domain-specific expertise. Each skill packages instructions, workflows, and best practices that Claude uses automatically when relevant to your task.

## Available Domains

| Domain | Description |
|--------|-------------|
| [metabolomics](metabolomics/) | Metabolomics analysis: pathway analysis, flux calculations, metabolite interpretation |
| [genomics](genomics/) | Genomics and transcriptomics analysis strategies |
| [proteomics](proteomics/) | Proteomics data analysis (coming soon) |
| [structural-biology](structural-biology/) | Protein structure validation, AlphaFold interpretation, structural comparisons |
| [data-science](data-science/) | General statistical analysis and data exploration |

## Installation

### Option 1: Marketplace (Recommended)

Register this repository as a Claude Code plugin marketplace, then browse and install skills:

```bash
# Add the marketplace
/plugin marketplace add justaddcoffee/open-science-skills

# Browse available skills
/plugin marketplace browse open-science-skills

# Install individual skills
/plugin install open-science-skills:data-science
/plugin install open-science-skills:genomics
/plugin install open-science-skills:metabolomics
/plugin install open-science-skills:structural-biology
```

### Option 2: Manual Installation

Clone this repository into your Claude Code skills directory:

```bash
# Clone into project-level skills (recommended)
git clone https://github.com/justaddcoffee/open-science-skills.git .claude/skills/domains

# Or clone into personal skills
git clone https://github.com/justaddcoffee/open-science-skills.git ~/.claude/skills/domains
```

Then copy the domain folders you want to use:

```bash
# Example: install metabolomics skill
cp -r .claude/skills/domains/metabolomics .claude/skills/
```

## Skill Format

Each skill is a directory containing a `SKILL.md` file with YAML frontmatter:

```yaml
---
name: my-domain
description: What this skill does and when to use it
---

# My Domain

[Instructions for Claude...]
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for details on creating new skills.

## Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.
