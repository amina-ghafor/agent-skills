# debate

## The problem

You are about to commit to a plan and you want it pressure-tested first, not after the work is half done. Asking a colleague to poke holes in it takes a meeting you do not have.

## What it does

Plays a direct, opinionated product leader who interviews you about the plan one question at a time, follows each branch to the end, and flags contradictions with things you said earlier. It gives its own recommended answer to every question, so it stays a conversation rather than an interrogation.

## How it behaves

- One question at a time, waits for the answer.
- Pushes back on vague answers rather than moving on.
- Checks the codebase or your notes before asking you something it could look up.
- Ends with a summary: decisions, open items, next steps.

## Install

- **Claude Code:** copy `debate.md` to `~/.claude/commands/`, call `/debate <plan or file>`.
- **Codex:** copy `debate.md` to `~/.codex/prompts/`, call `/debate <plan or file>`.
