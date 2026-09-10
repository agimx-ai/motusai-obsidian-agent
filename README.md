# MotusAI Agent

**Bring an AI agent into Obsidian to work with your notes, files, and voice.**

MotusAI Agent connects your Obsidian vault to the Agent Harness running in [MotusAI Seed](https://github.com/agimx-ai). It gives you an AI workspace inside Obsidian where you can ask questions, work with notes and attachments, organize knowledge, and carry out multi-step tasks.

> MotusAI Agent is a desktop-only companion for MotusAI Seed. MotusAI Seed must be installed and running, with its official **Agent Harness** plugin enabled.

## What you can do

- **Work with your vault through conversation** — ask questions about your notes, summarize material, rewrite content, and organize information.
- **Reference the exact context you need** — mention notes from the current vault and attach supported local files to a conversation.
- **Use agent tools and Skills** — let Agent Harness handle multi-step work, file operations, terminal tasks, and other enabled tools while showing their progress in the chat.
- **Transcribe voice into Obsidian** — record a conversation or meeting and save the ongoing transcript directly to a new or existing note.
- **Choose the right model for each conversation** — switch between model connections configured in MotusAI Seed and select a supported thinking level.
- **Keep separate, persistent conversations** — create, rename, switch, and resume conversations for different projects or topics.
- **Stay in control** — answer clarification questions and approve sensitive capabilities before the agent continues.

## Requirements

- Obsidian Desktop 1.8.7 or later
- MotusAI Seed installed and running
- The official **Agent Harness** plugin enabled in MotusAI Seed
- At least one conversation model configured in Agent Harness

## Getting started

1. Start MotusAI Seed.
2. Install and enable the official **Agent Harness** plugin in Seed.
3. Open Agent Harness in Seed and configure a model connection.
4. In Obsidian, open **Settings → Community plugins → Browse**.
5. Search for **MotusAI Agent**, install it, and enable it.
6. Select the sparkle icon in the Obsidian ribbon, or run **Open Agent chat** from the Command Palette.
7. Approve the local connection in MotusAI Seed if prompted, then start a conversation.

To give the agent context from your vault, reference the relevant note from the chat composer. If Seed asks you to choose a workspace folder, select the root of the current Obsidian vault.

## Models

Model connections are configured in MotusAI Seed rather than in Obsidian. Agent Harness supports OpenAI, Anthropic, Google Gemini, OpenRouter, DeepSeek, Xiaomi MiMo, OpenAI-compatible endpoints, and Alibaba Cloud Model Studio (DashScope). Availability depends on your Seed configuration.

## Privacy and data

- Model API keys are managed by MotusAI Seed and are not stored in the Obsidian vault.
- Agent conversations and session data are managed by Agent Harness in Seed, not written into the vault as plugin configuration.
- Notes are read or modified only when they are included in the task and the corresponding Agent Harness action is allowed.
- Requests sent to a configured model provider are subject to that provider's privacy policy.

## Manual installation

Download `main.js`, `manifest.json`, and `styles.css` from the [latest release](https://github.com/agimx-ai/motusai-obsidian-agent/releases/latest). Place them in:

```text
<your-vault>/.obsidian/plugins/motusai-vault-agent/
```

Reload Obsidian, then enable **MotusAI Agent** under **Settings → Community plugins**.

## Troubleshooting

### MotusAI Agent cannot connect

Make sure MotusAI Seed is running and the official Agent Harness plugin is enabled. If Seed displays an access request, approve it and return to Obsidian.

### No model is available

Open the Agent Harness plugin details in MotusAI Seed, add a model connection and API key, then save it. Return to Obsidian and reopen the Agent chat.

### The agent cannot access a note

Reference the note from the chat composer. If Seed asks for a workspace folder, choose the root of the current vault rather than an individual file or your Downloads folder.

## Support

Use the [issue tracker](https://github.com/agimx-ai/motusai-obsidian-agent/issues) for bug reports and feature requests. When reporting a problem, include your Obsidian version, MotusAI Agent version, MotusAI Seed version, and the steps needed to reproduce it. Do not include API keys or private note contents.
