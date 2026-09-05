# agent-skills

Single-purpose prompts for CLI coding agents. Each does one job: explain a concept, pressure-test a plan, draft in your voice, review a document, plan a day, write up a session.

Every skill is a plain Markdown file. It runs in **Claude Code** (`~/.claude/commands/`) or **Codex** (`~/.codex/prompts/`), invoked as `/name`. Each folder has its own README with the problem it solves, how it behaves, and how to install it on either agent.

## Skills

### 🧠 Think it through
- **[debate](debate/)** - a direct product leader interviews you about a plan, one question at a time, before you commit.
- **[learn](learn/)** - explains a technical concept at the 80/20, pitched at a non-engineer.

### 📓 Plan and record
- **[kickoff](kickoff/)** - starts a build project with the planning artefacts sized to the project: one-pager, scope, a single metric, repo set up.
- **[dayplan](dayplan/)** - builds today's plan from your calendar and backlog. Read only.
- **[capture](capture/)** - writes a finished session into the right notes.

### ✍️ Write and review
- **[draft](draft/)** - drafts in your voice by loading your style guide first, then self-checking against it.
- **[review-output](review-output/)** - reviews a document with a fresh, independent agent, so the reviewer is not the author.

## Getting started

Clone the repo, then for each skill you want, copy its prompt file into your agent's commands directory:

```bash
git clone https://github.com/amina-ghafor/agent-skills.git

cp agent-skills/learn/learn.md ~/.claude/commands/    # Claude Code
cp agent-skills/learn/learn.md ~/.codex/prompts/      # Codex
```

Then call it as `/learn <concept>`. `dayplan` and `capture` assume the [second-brain](https://github.com/amina-ghafor/second-brain) backlog format; the rest are self-contained.

## Adding a skill

One folder per skill: `name/name.md` for the prompt, `name/README.md` for the problem, behaviour and install notes. Keep the prompt body agent-neutral: plain instructions and `$ARGUMENTS`, no tool-specific syntax in the body itself.
