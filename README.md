# GitKraken ADE

> **Private Preview** — GitKraken's ADE is currently in private preview with a limited number of testers.

This is the public issue tracker for **GitKraken's ADE**, currently developed under the codename **Kepler**.

## What is GitKraken's ADE?

GitKraken's ADE is an agentic development environment — a local and remotely accessible-application that puts AI-powered coding agents at the center of how you build software. It's where you plan, run, review, and ship work, with agents as a first-class part of your workflow.

### Tasks

The core unit in the ADE is a **Task** — a container for a piece of work. Each Task holds one or more **worktrees** (isolated, ready-to-commit branches), and each worktree can host one or more **agent sessions** (Claude, Codex, or any model via Open Code). Everything related to that work — context, branches, diffs, agent activity — lives inside the Task.

### Starting a Task

There are three ways to create a Task:

- **From scratch.** New worktree, new agent, blank slate. The fastest path when you know what you want to build.
- **From an issue.** Pick one or many issues from your connected tracker. The ADE spins up a Task per issue with the issue context already loaded — useful for working through a backlog in parallel.
- **From a pull request.** Pick one or many PRs and either start a review (optionally using GitKraken's PR review tool) or kick off agents to address feedback — each PR gets its own Task.

### Inside a Task

Inside a Task you can talk to your agent, watch the diff form in real time, inspect changes, and commit.

### Views

The ADE gives you three ways to view your tasks, worktrees, and agent sessions — toggle between them at the top of the screen:

- **List.** Tasks on the left, the active agent session in the middle, changes on the right. Best when you want to focus on one piece of work at a time.
- **Kanban.** Organizes worktrees and their agents into a workflow — Exploration, In Development, Review, Done. Filter the board and interact with agents directly from their cards. Best when you're thinking about work in terms of where it is in your process.
- **Console.** All active sessions at once in an exploded view with filters, so you can scan and interact with many agents in parallel. Best when you have a lot in flight and want to answer "what's everything doing right now?"

All three views offer similar functionality — they're different lenses on the same underlying work, so you can pick the one that matches how you like to think.

## Setup & configuration

### Repos directory and worktree paths

You can set your default repos directory and configure where new worktrees are created using relative paths in Settings. This is worth setting up early — it controls where all of your Task worktrees land on disk.

### Terminals

You can open embedded terminals directly from any worktree to run commands, debug, or interact with the file system outside of the agent.

### Custom commands

Create custom commands for each repo that run on demand or automatically when a new worktree is created. This is useful for bootstrapping worktrees — installing dependencies, running builds, starting test watchers, or anything else you'd normally do after checking out a fresh branch.

### Local and remote environments

By default the ADE works locally, but you can connect to remote environments via SSH. Look for the connection button in the top right corner of the app.

## Filing an issue

If you've found a bug or have a feature idea, open a new issue on the [Issues](../../issues) tab.

Before filing, please read [CONTRIBUTING.md](./CONTRIBUTING.md) — it covers what to include in a report and how to check for duplicates.

## License

See [LICENSE.md](./LICENSE.md).
