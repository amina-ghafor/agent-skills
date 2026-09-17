# 📅 dayplan

## The problem

Every morning is the same arithmetic: a calendar full of fixed points, a backlog full of candidates, and no quick way to see which tasks actually fit the gaps without doing the sums by hand.

## What it does

Reads the day's calendar and backlog, then returns one plan: the fixed points and the space between them, a task matched to each gap, a named starting task, and anything due this week that will not make it into today. Nothing gets written back.

## How it behaves

- Read only, always. The calendar and backlog are never edited.
- Returns one plan, not a menu of options.
- A full day is reported as full, with what gets cut named explicitly.

## Assumes

The [second-brain](https://github.com/amina-ghafor/second-brain) backlog format: `## `-headed sections, tasks carrying a `(1h)` or `(30m)` estimate.

## Install

- **Claude Code:** copy `dayplan.md` to `~/.claude/commands/`, call `/dayplan`.
- **Codex:** copy `dayplan.md` to `~/.codex/prompts/`, call `/dayplan`.
