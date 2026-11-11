# Plugin marketplace

This repository contains marketplace manifests for my custom Claude Code and Codex plugins.

## Available plugins

| Plugin name | Version | Description | Repository |
| --- | --- | --- | --- |
| `context-manager` | v1.1.0 | Preserve engineering context across long-running tasks, sessions, and coding agents. | [duckysmacky/context-manager-skill](https://github.com/duckysmacky/context-manager-skill) |
| `guitar-setup` | v1.0.0 | Configure guitar and amplifier settings to play a certain song | [duckysmacky/guitar-setup-skill](https://github.com/duckysmacky/guitar-setup-skill) |
| `loom` | v1.3.0 | Drive your self-hosted Loom graph (projects, studies, ideas) from Claude | [duckysmacky/loom](https://github.com/duckysmacky/loom) |
| `lid-guard` | v1.0.0 | Keeps a Linux laptop awake with the lid closed while an AI coding agent works | [duckysmacky/lid-guard-plugin](https://github.com/duckysmacky/lid-guard-plugin) |

## Add the marketplace

### Claude

#### Claude Code

Add the marketplace in Claude Code:

```sh
claude plugin marketplace add duckysmacky/duckysmacky-plugin-marketplace
```

Then choose a skill from the table and install it by replacing `<skill-name>` with its name:

```sh
claude plugin install <skill-name>@duckysmacky
```

#### Claude app (desktop and web)

1. Open **Customize** in the left sidebar and go to the **Plugins** tab.
2. Click **Add**, then select **Add marketplace**.
3. Choose **Add from a repository** and enter `duckysmacky/duckysmacky-plugin-marketplace`.
4. Back in the **Plugins** tab, open **Discover**, select a plugin from the **Duckysmacky** marketplace, and click **Add**.

### ChatGPT and Codex

#### Codex

Add the marketplace from a terminal:

```sh
codex plugin marketplace add duckysmacky/duckysmacky-plugin-marketplace
```

Then choose a skill from the table and install it by replacing `<skill-name>` with its name:

```sh
codex plugin add <skill-name>@duckysmacky
```

#### ChatGPT app

1. Add the marketplace using the terminal command in the Codex section above.
2. Restart the ChatGPT desktop app.
3. Select **ChatGPT**, choose **Work**, and open **Plugins**.
4. Select the **Duckysmacky** marketplace, choose a plugin, and install it.
5. Start a new chat to use the plugin.

## Other agents

For agents supported by the [skills CLI](https://github.com/vercel-labs/skills), install the skills from each plugin's repository:

```sh
npx skills add duckysmacky/<skill-name>
```

Choose the skills and target agents when prompted. This installs skills only; plugin integrations such as custom MCP servers require separate configuration.

