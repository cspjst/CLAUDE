# Bootstrap templates

*Owned by synergy. Masters for starting a new project with Claude, per `operating-model` (the version in the synergy project wins). Copy them into a new project at bootstrap; from then on the copies belong to that project.*

## Placeholders
- `<PROJECT>` — the project's name in capitals; `<project>` — lower case where a path needs it.
- `<DEPT>` / `<dept>` — a department's name / its folder.
- `<HUMAN>` — the human's name (Jeremy).
- `<date>` — `YYYY-MM-DD`; `<time>` — `HH:MM`, UK local.
- `<…>` anything else — fill in or delete. Lines in *italics* starting "Guide:" are guidance; delete them once filled.

## The files, in bootstrap order
| Step | Template | Becomes, in the new project |
|---|---|---|
| 1 | `project-instructions.md` | pasted into the project's Instructions (Claude can't edit them) |
| 2 | `welfare/stakeholders.md` | `welfare/stakeholders.md` |
| 2 | `welfare/code-of-conduct.md` | `welfare/code-of-conduct.md` — signed by the human |
| 2 | `welfare/working-agreement.md` | `welfare/working-agreement.md` |
| 3 | `historiography.md` | `<project>-historiography.md` (owner: the main department) |
| 4 | `department-opening.md` | the first message of each department chat |
| 4 | `department-notes.md` | `<dept>/<dept>-notes.md` |
| any | `handover/handover.md` | `handover/<date>-<from>-to-<to>.md` |

## Rules that come with them
- Every project has a WELFARE department (operating model, principle 7).
- Rename each department chat by hand; auto-titles aren't reliable.
- One owner per document; the header of each says who.
- Claude doesn't write to a file the human has open, and verifies every write to the human's machine by reading it back.
