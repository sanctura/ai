# People Inbox

Drop zone for raw information about people. Files placed here will be processed and routed to the correct location by the **inbox-processor** agent.

## How to Use

1. **Drop a file** in this folder with any raw information: meeting notes, observations, copy-pasted emails, feedback, flash report content, etc.
2. **Name it**: `YYYY-MM-DD-description.md` (e.g., `2026-02-11-amanda-london-meeting.md`)
3. **Content**: Freeform. No special format required. Just dump the information.
4. **Say "process inbox"** to Claude to have all files processed.

## What Happens During Processing

The **inbox-processor** agent (`.claude/agents/inbox-processor.md`) handles the full workflow:

1. Scan all files in `_inbox/` (skips README.md and `_processed/`)
2. Classify each file by person(s) and content type (observation, achievement, concern, feedback, meeting notes, flash report, task, decision, etc.)
3. Route content to the correct destinations:
   - Performance observations/feedback → `direct-reports/[name]/performance.md` (with appropriate tags)
   - Meeting notes → `direct-reports/[name]/one-on-ones/` or `stakeholders/[name]/meetings/`
   - Flash report content → `direct-reports/[name]/flash-reports/`
   - Documents/contracts → `direct-reports/[name]/documents/`
   - Tasks/decisions/context → `direct-reports/[name]/info-base.md`
   - New person → create folder from appropriate template
4. Update each person's **information base** (`info-base.md`) with structured, compiled data
5. Move processed files to `_inbox/_processed/` with a routing comment
6. Output a structured summary of all actions taken

## Tips

- Include the person's name in the filename or content so the agent can route it correctly
- Multiple people in one file is fine — the agent will split the content by person
- Raw is fine — notes don't need to be polished before dropping them here
- Date-stamp your files so processing order is clear

---

*Last Updated: 2026-02-15*
