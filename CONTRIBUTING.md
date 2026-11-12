# Contributing

Thanks for helping improve **Kepler**. This repository is the public issue tracker — the best way to contribute right now is to report bugs and suggest features through GitHub issues so the team can triage and address them.

## Before you file

**Search existing issues first.** Bugs and ideas may have already been reported. Check both open and closed issues to see if yours already exists — if it does, please add a reaction or a comment with any additional details instead of opening a duplicate. This helps the team prioritize and keeps the tracker manageable.

## Opening an issue

Go to the [Issues](../../issues) tab, click **New issue**, and pick the template that fits:

- **Bug report** — something is broken, crashes, gives the wrong result, or no longer works the way it used to.
- **Feature request** — something Kepler doesn't do yet, or a change to how it currently works.

Each template walks you through the information the team needs. Blank issues are disabled, so please use one of the templates.

### Bug or feature request?

A simple rule of thumb:

- **If Kepler does something wrong, or stops doing something it used to do, it's a bug.** Crashes, errors, wrong results, and things that don't work the way the app says they should all count.
- **If you want Kepler to do something it doesn't do today, or to work differently than it was designed to, it's a feature request.**

Some cases that are easy to get wrong:

| Situation | Template |
| --- | --- |
| Something worked in an earlier version and doesn't any more | Bug report |
| A button, setting, or menu item does nothing, or does the wrong thing | Bug report |
| Something you expected to exist isn't there, like support for another issue tracker or a filter you'd find useful | Feature request |
| Something works as designed, but you think the design should change | Feature request |
| Something is confusing or slow | Bug report if it's broken or unusable, feature request if it works but could be better |

Don't worry about getting it exactly right: if you pick the wrong template, the team will relabel the issue during triage.

## Reporting a bug

The **Bug report** template asks for:

- **What happened** and **what you expected to happen**
- **Steps to reproduce** — as specific as you can make them
- **Your Kepler version and system details** — open **About Kepler** (macOS: **Kepler › About Kepler**; Windows/Linux: **Help › About**), click **Copy details**, and paste the result. This covers your Kepler version, release channel, and operating system in one go.
- **Where Kepler was running** — locally, in a remote environment (over SSH or in WSL), or through Remote Access in a browser or on your phone
- **Area and agent** (optional) — which part of Kepler is affected (e.g. Dashboard, task Changes, Terminal) and which agent you were using (e.g. Claude Code, Codex, GitHub Copilot), if relevant
- **Logs, screenshots, or screen recordings** if they help illustrate the problem. To get logs, go to **Settings › Help › Logs** and click **Save logs…** — this creates a `kepler-logs-YYYY-MM-DD.zip` you can attach. Logs can include file paths and repository names, so please review them and remove anything sensitive first.

The more reliably we can reproduce the issue, the faster we can fix it.

## Requesting a feature

The **Feature request** template asks for:

- **The problem** you're trying to solve or the workflow you'd like to improve
- **What you'd like to see** — your suggested solution, if you have one in mind
- **Why it matters** — context that helps us understand the value
- **Alternatives or workarounds** (optional) — anything you've tried or considered instead

We read every feature request and use them to shape the roadmap, even when we can't act on each one immediately.

## What happens next

The team triages incoming issues regularly. You may be asked for more details, linked to a related issue, or given an idea of what to expect next. Thanks for taking the time to file a thoughtful report — it makes a real difference.
