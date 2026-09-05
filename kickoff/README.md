# 🚀 kickoff

## The problem

You start a personal build project and skip the thinking, or you overdo it and write a full PRD for a weekend job. Both go wrong. The first leaves you with no way to tell if it worked; the second reads as someone who cannot right-size their own work.

## What it does

Produces the planning artefacts for a build, sized to the build. Small projects get a one-pager and nothing else. Larger ones add a measurement plan and acceptance criteria. Then it sets up the repo with the one-pager committed and the next three actions written down.

## How it behaves

- Sizes the project first and confirms the size with you before producing anything.
- The one-pager has a mandatory, non-empty Non-goals row.
- Forces a "Cut for v1" list with at least one real item.
- Picks a single outcome metric, not a dashboard.
- Keeps published prose in your voice, loading your style guide the way the `draft` skill does.
- Quotes third-party concepts directly and briefly, with attribution, rather than rewording them as your own.

## Install

- **Claude Code:** copy `kickoff.md` to `~/.claude/commands/`, call `/kickoff <project idea>`.
- **Codex:** copy `kickoff.md` to `~/.codex/prompts/`, call `/kickoff <project idea>`.
