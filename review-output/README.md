# review-output

## The problem

Claude cannot reliably review its own output. In the same context that produced a document, it tends to agree with it.

## What it does

Spawns a separate agent with fresh context to review a document against a fixed checklist: accuracy, source integrity, stale claims, consistency, structure, voice, completeness, concision. It returns ranked findings with locations and one-line fixes, and does not touch the file.

## Use it

Copy `review-output.md` into `~/.claude/commands/` and call `/review-output <path or URL>`.
