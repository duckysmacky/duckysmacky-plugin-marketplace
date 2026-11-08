# Claude plugin marketplace

This repository contains the marketplace manifest for my custom Claude Code plugins & skills.

## Available skills

| Skill name | Version | Description | Repository |
| --- | --- | --- | --- |
| `context-manager` | v1.1.0 | Preserve engineering context across long-running tasks, sessions, and coding agents. | [duckysmacky/context-manager-skill](https://github.com/duckysmacky/context-manager-skill) |
| `guitar-setup` | v1.0.0 | Configure guitar and amplifier settings to play a certain song | [duckysmacky/guitar-setup-skill](https://github.com/duckysmacky/guitar-setup-skill) |
| `loom` | v1.3.0 | Drive your self-hosted Loom graph (projects, studies, ideas) from Claude | [duckysmacky/loom](https://github.com/duckysmacky/loom) |

## Installation

Add the marketplace in Claude Code:

```text
/plugin marketplace add duckysmacky/duckysmacky-plugin-marketplace
```

Then choose a skill from the table and install it by replacing `<skill-name>` with its name:

```text
/plugin install <skill-name>@duckysmacky
```
