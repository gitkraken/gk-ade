# Kepler

> **Public Preview** — Kepler is currently in public preview.

This is the public issue tracker for **Kepler**, GitKraken's agentic development environment (ADE).

## What is Kepler?

Kepler is an agentic development environment (ADE) from GitKraken — a desktop app you can also reach remotely from a browser or your phone, that puts AI-powered coding agents at the center of how you build software. It's where you plan, run, review, and ship work, with agents as a first-class part of your workflow.

Kepler is available for macOS, Windows, and Linux.

### Tasks

The core unit in Kepler is a **Task** — a container for a piece of work. A task usually gets its own **worktree** (an isolated, ready-to-commit branch), and can hold one or more **agent sessions**, terminals, notes, and **resources** such as repositories, issues, pull requests, files, and links. Everything related to that work — context, branches, diffs, agent activity — lives inside the task.

A task doesn't need a repository: you can also start one in a plain folder.

### Starting a Task

Press **New task** and start with the prompt. Then attach whatever the work needs:

- **Repositories and folders.** Kepler creates a worktree for each repository, on a branch named from the task.
- **Issues and pull requests.** Browse and search your connected providers, then attach one or more issues or PRs as context, to plan or implement an issue, review a PR, or address feedback.
- **Files.** Upload files from your computer, or attach them by path.

You can also start tasks from the command palette, from an issue or PR on the Dashboard's **Todo** view, or with **Automations**, which start tasks for you (see below).

Already using another tool? **Import from another app** brings in your workspaces from Conductor, Orca, herdr, and Vibe Kanban as tasks, with their chats resumed. You'll find it in the File menu, and on the Tasks view while you have no tasks. Kepler also finds agent sessions you started in your own terminal, so you can continue them or adopt them into a task.

### Agents

Kepler works with **Claude Code**, **Codex**, **GitHub Copilot**, **Cursor**, **Antigravity**, **OpenCode**, **Pi**, **Auggie**, and **Grok Build**, and you can add your own as a **custom agent**. You choose the agent per task and per session. Most agents can run as a rich **Chat** or in a real **Terminal** inside Kepler.

You can save an agent, model, mode, and effort as a **preset**, and manage MCP servers in **Settings › Agents**.

### Inside a Task

The task page is where the work happens. You open its parts as tabs, which you can drag into groups and splits:

- **Chat** — talk to your agents, review their plans, and answer permission requests.
- **Changes** — watch the diff form, review and comment on lines, stage, commit, update your branch, and open pull requests.
- **Files**, **Notes**, and **Resources** — browse the worktree, keep task notes, and manage the issues, PRs, repos, files, and links attached to the task.
- **Terminal** — embedded terminals for running commands, debugging, or working outside the agent.

### Dashboard

The **Dashboard** is your overview of all your work. It runs on saved **views** that you name, reorder, and customize, each with its own layout, grouping, sort, filters, and search:

- **Tasks** — everything in flight, grouped by what needs your attention, progress stage, repository, activity, or your own task groups.
- **Todo** — the pull requests and issues waiting on you across your connected providers, ready to turn into tasks.
- **Agent Graph** — a live graph of what your agents are doing.

Each view can be shown as a **List**, a **Board**, or a **Graph**. You can open tasks as preview panels next to the list, so you can watch and talk to many agents at once.

### Automations and Actions

- **Actions** are reusable prompts. Each one can use its own agent, and you can run it from anywhere in Kepler.
- **Automations** watch GitHub or Jira for new activity that matches a query, or run on a schedule. Each run starts a task that runs an Action or your own prompt. Templates cover common jobs like reviewing pull requests that are waiting on you, or triaging new bugs.

### Ask Kepler and the command palette

**Ask Kepler** (Mod+L) is a side panel with a chat that knows what's on your screen. It can also change Dashboard views and settings, or draft an automation for you.

The **command palette** (F1 or Cmd/Ctrl+Shift+P) finds tasks, files, commands, and Todo items.

## Setup & configuration

### Integrations

Connect your code hosts and issue trackers in **Settings › Integrations**: GitHub, GitLab, Bitbucket, Azure DevOps (including their self-hosted editions), Jira, Linear, Trello, and Asana.

### Repositories and worktree folders

Set your **Repositories folder** in **Settings › Repositories** and your **Worktrees folder** in **Settings › Tasks**. The worktrees folder controls where every task's worktree lands on disk, so it's worth setting up early. Repositories Kepler finds by scanning your repositories folder stay untrusted until you trust them.

### Repository commands

Each repository can have its own **commands**, set up in its settings page under **Settings › Repositories**. Run them on demand from the **Run** menu, or have them run automatically when Kepler creates a new worktree. That's useful for bootstrapping worktrees: installing dependencies, running builds, starting test watchers, or anything else you'd normally do after checking out a fresh branch.

To copy ignored files such as `.env` into new worktrees, list them in a `.worktreeinclude` file.

### Remote environments and Remote Access

By default Kepler runs agents on your own machine, but there are two ways to work remotely:

- **Remote environments** (**Settings › Remote environments**) — run your agents on another machine, like a dev server or cloud VM, while you work from your own computer. Kepler installs itself on the remote machine over SSH. On Windows you can also use WSL.
- **Remote Access** (**Settings › Remote Access**) — reach this machine from any browser or your phone, through a secure GitKraken relay.

## Filing an issue

If you've found a bug or have a feature idea, open a new issue on the [Issues](../../issues) tab.

Before filing, please read [CONTRIBUTING.md](./CONTRIBUTING.md) — it covers what to include in a report and how to check for duplicates.

## License

See [LICENSE.md](./LICENSE.md).
