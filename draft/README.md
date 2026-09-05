# 🗣️ draft

## The problem

Claude drafts in a competent, generic register that is not yours. Patching it word by word after the fact never quite fixes it, because the structure was wrong from the start.

## What it does

Loads your own style guide first, then drafts from it: your sentence rhythm, your phrasing rules, your spelling. It reads the actual thread for context rather than your summary of it, self-checks the draft against your rules, and shows you the draft rather than sending anything.

## Setup

Keep your writing rules in `~/.claude/STYLE.md`, or point the skill at wherever they live. Without one, the skill asks you for a few writing samples and works from those.

## Install

- **Claude Code:** copy `draft.md` to `~/.claude/commands/`, call `/draft <what to write>`.
- **Codex:** copy `draft.md` to `~/.codex/prompts/`, call `/draft <what to write>`.
