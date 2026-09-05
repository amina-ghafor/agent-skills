# 📝 capture

## The problem

A working session produces decisions, facts you looked up, and loose ends. Most of it stays in the chat log and is gone by next week. Writing it up by hand is the step that gets skipped.

## What it does

Reads back over the session, pulls out the decisions, the facts worth keeping, and the open threads, and files each into the note it belongs in. It appends under today's date and shows you the diff before writing anything.

## How it behaves

- Matches an existing file before making a new one.
- Appends, never rewrites what is already there.
- Shows the diff first. Nothing is saved without a look.
- Leaves out anything already recorded and anything that led nowhere.

## Install

- **Claude Code:** copy `capture.md` to `~/.claude/commands/`, call `/capture`.
- **Codex:** copy `capture.md` to `~/.codex/prompts/`, call `/capture`.
