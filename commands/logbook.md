You are running the logbook skill manually via the /logbook command.

Read the full skill instructions from `.claude/skills/logbook/SKILL.md` before doing anything.

Then determine what the user wants based on what they typed after /logbook:

- `/logbook` alone → show the current log: read `docs/logbook/LOGBOOK.md` and return a summary of all entries
- `/logbook init` → run the initialization flow from SKILL.md
- `/logbook log [anything]` → log what follows as a decision or milestone entry
- `/logbook export` → run the case study seed export from SKILL.md
- `/logbook status` → show how many entries exist, the date of the last entry, and whether a case study seed exists
- `/logbook review [number or topic]` → pull up a specific past decision by entry number or keyword

If the user just types `/logbook` with no argument and logbook hasn't been initialized yet (no `docs/logbook/` folder), run the initialization flow automatically.

Always follow the behavior, tone, and file-writing rules defined in SKILL.md. Do not improvise outside of those rules.
