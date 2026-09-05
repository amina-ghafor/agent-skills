# dayplan

## The problem

You start the day with a calendar and a task list and have to work out, in your head, what actually fits between the meetings and what to touch first. It is the same puzzle every morning.

## What it does

Reads today's calendar and your backlog, then writes one plan to the terminal: the fixed points and the gaps, which tasks fit which gap, one task to start with, and anything due this week that will not fit today. It does not edit anything.

## How it behaves

- Read only. Never touches the backlog or the calendar.
- One plan, not a set of options.
- If the day is already full, says so and names what gets dropped.

## Assumes

The [second-brain](https://github.com/amina-ghafor/second-brain) backlog format: `## sections`, and task lines with a `(1h)` or `(30m)` estimate.

## Install

- **Claude Code:** copy `dayplan.md` to `~/.claude/commands/`, call `/dayplan`.
- **Codex:** copy `dayplan.md` to `~/.codex/prompts/`, call `/dayplan`.
