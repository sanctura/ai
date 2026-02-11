# People Inbox

Drop zone for raw information about people. Files placed here will be processed and routed to the correct location.

## How to Use

1. **Drop a file** in this folder with any raw information: meeting notes, observations, copy-pasted emails, feedback, flash report content, etc.
2. **Name it**: `YYYY-MM-DD-description.md` (e.g., `2026-02-11-amanda-london-meeting.md`)
3. **Content**: Freeform. No special format required. Just dump the information.
4. **Say "process inbox"** to Claude to have all files processed.

## What Happens During Processing

Claude will:
1. Read all files in `_inbox/`
2. Identify the person(s) and type of information in each file
3. Route content to the correct location:
   - Performance observations → `direct-reports/[name]/performance.md`
   - Meeting notes → `direct-reports/[name]/one-on-ones/` or `stakeholders/[name]/meetings/`
   - Flash report content → `direct-reports/[name]/flash-reports/`
   - Documents/contracts → note in profile or `direct-reports/[name]/documents/`
   - New person info → create stakeholder folder if needed
4. Move processed files to `_inbox/_processed/` with a note of what was done
5. Summarise all actions taken

## Tips

- Include the person's name in the filename or content so Claude can route it correctly
- Multiple people in one file is fine — Claude will split the content
- Raw is fine — notes don't need to be polished before dropping them here
- Date-stamp your files so processing order is clear

---

*Last Updated: 2026-02-11*
