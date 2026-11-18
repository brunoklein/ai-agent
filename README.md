# Personal AI agent

A personal AI agent that lives on any computer and improves itself.

It remembers you, works on its own between conversations, and gets better at helping you every day. Give it a task, a project or a question; when you give it nothing, it picks up its own work and comes back with ideas.

- **Self-improving**: a short retro every day, its own playbook of lessons, and a scorecard to check the changes really help.
- **Proactive**: works on a timer, keeps the promises it made with a time, and writes to you with ideas, questions and a weekly note.
- **Does almost anything with you**: code, research, scripts, reminders, side projects, all on your machine.

## Quick start

1. On an always-on machine, clone this repo:

   ```bash
   git clone https://github.com/brunoklein/ai-agent.git ~/agent && cd ~/agent
   ```

2. Open your AI coding agent inside the folder (for example `claude` for Claude Code, or `codex`).
3. Send:

   ```
   Read AGENTS.md and run the bootstrap. Then introduce yourself and show me index.md.
   ```

4. Answer the questions in its hello message. It sets itself up to run in the background and start with your computer, and asks if you want to reach it through a chat app.

That's it: it now has a name, a memory and a home.

## Requirements

- **An always-on machine** with at least 1 GB of RAM and 32 GB of storage.
- **An AI coding agent**: Claude Code or Codex recommended.
- **Its own machine or user account**: the agent runs commands on its own.

## How it works

- **`AGENTS.md`** holds the agent's core rules. Only you edit it; the agent suggests changes in `proposals/`.
- **Memory is files.** Each session starts fresh, so the agent reads and writes markdown in its folder (`index.md`, `memory/`, `logs/`).
- **Two ways of running:**
  - *Live session*: you talk to it.
  - *Cycle*: a timer or a chat message starts it with nobody watching. It handles one request or one small task, then stops.
- **`inbox/` and `outbox/`**: leave requests as files in `inbox/`; answers, questions and ideas land in `outbox/`, or in your chat app.
- **Self-improvement**: a daily retro of yesterday, rules it writes for itself in `memory/playbook.md`, and a weekly note to you on what changed.
- **Git** records every change it makes, so you can review or roll back.

## Nice tools to connect

- **tmux**: keeps sessions running after you close the terminal.
- **Tailscale**: reach the machine from anywhere, without opening ports.
- **Claude Remote Control**: talk to the agent from the Claude app on your phone.
- **Slack, Telegram, Discord**: message the agent like a friend; it builds the bridge itself.
