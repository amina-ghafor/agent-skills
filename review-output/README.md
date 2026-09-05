# review-output

## The problem

Claude cannot reliably review its own output. In the same context that produced a document, it tends to agree with it.

## What it does

Runs the review in fresh context, against a fixed checklist: accuracy, source integrity, stale claims, consistency, structure, voice, completeness, concision. It returns ranked findings with locations and one-line fixes, and does not touch the file.

## Install

- **Claude Code:** copy `review-output.md` to `~/.claude/commands/`, call `/review-output <path or URL>`. The command launches a subagent with the Task tool, so `Task` must be available to it.
- **Codex:** copy `review-output.md` to `~/.codex/prompts/`, call `/review-output <path or URL>`. The review runs as a separate `codex exec` call.
