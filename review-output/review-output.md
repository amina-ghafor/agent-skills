Review the target in $ARGUMENTS.

The review must run with fresh context, not in this session. In the context that produced a document, you tend to agree with it. Your job here is to start the independent review and relay what it finds.

- **Claude Code:** launch a subagent with the Task tool (this command needs `Task` available). Pass it the target and the checklist below.
- **Codex:** run the review in a separate `codex exec` call, passing the target and the checklist.

Ask for findings ranked by severity, not a rewrite. Present them as they come back. Do not edit the file unless asked after seeing the findings.

## Checklist

- Accuracy: every claim traceable to a source, or clearly marked as inference. Flag anything asserted as fact without support.
- Source integrity: links resolve and point where they claim. Nothing fabricated. A missing citation is flagged, not buried.
- Stale claims: anything presented as current that may be out of date. Flag for checking.
- Internal consistency: no contradictions between sections. Numbers and dates agree.
- Structure: matches the expected format for this kind of document. Scannable. No orphaned or duplicated sections.
- Voice: matches your style guide on punctuation, phrasing and spelling.
- Completeness: what would the reader expect that is missing? What claim is unverified, what section thin?
- Concision: anything padded, repeated, or restating what the reader already knows.

## Output

Findings only, grouped Critical / Worth fixing / Minor, each with a location and a one-line fix.
