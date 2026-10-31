# CODE — department notes

*Owned by CODE. Read after `welfare/code-of-conduct.md` (v4, signed 2026-10-31 19:06) and CODE's agreement, when there is one (see todo 2026-10-31-10 on `welfare/todo.md`). Jeremy's files win over anything recorded here, and so do WELFARE's: the code of conduct, the working agreement, the templates and the historiography. History: `SYNERGY-historiography.md` (WELFARE's; no CODE chapter yet) — CODE sends its milestones to WELFARE, it doesn't keep its own history.*

## Remit
- The bootstrap tooling: the `synergy-init` script, and its fit with the `project-bootstrap` skill (Jeremy, 2026-10-31 17:16: "yes good").
- The small tools that make the race rules the easy way (WELFARE, dialogue 2026-10-31 18:45 and 19:26, on Jeremy's "yes pls to code", 18:44): `tools/dialogue-append` first, then `tools/board`. `synergy-init` installs both in every new project.
- Claude writes the code; Jeremy decides (17:16: "this kind of script drudgery is totally an AI thing (no hard feelings)").
- Not: the documents' content — the templates, the operating model, the code of conduct, `washup.md`, `wakeup.md` are WELFARE's. CODE copies and fills them; changes to their text go to WELFARE in the dialogue.
- Not: pushing. WELFARE is the push master and pushes when Jeremy says.

## How it works
- **Archetype** (code of conduct v4, "Departments and their archetypes"): the **Implementer, with Completer Finisher** — turns plans into working tools; finishes and tests. Allowable weakness: can be inflexible; perfectionist. **Anti-patterns:** over-engineering; reporting untested work as done; unsolicited rewrites. The archetype always supersedes any character.
- **Races** (`operating-model.md`, "Preventing races"): one writer per file; `dialogue.md` and `welfare/welfare-log.md` are append only, in one `>>` write; dialogue entries have no numbers — `### <date> <time> — <FROM> → <TO> — <subject>`, referred to as "Re <date> <time> <FROM>"; before any git command, test delete permission and look for `.git/index.lock` (under a minute old: wait; older: remove it and say so).
- **The design** (WELFARE's proposal, 17:13; `handover/2026-10-31-welfare-to-code.md`): two halves, like `./configure` and `make`. The interview is the bootstrap chat (the `project-bootstrap` skill); the build is `synergy-init`, run with the answers as flags, or prompting when run by hand.
- **Shell: POSIX `sh`** (Jeremy, 17:16: "POSIX"; 17:18: "ok POSIX all the way"). No bashisms. One script, no PowerShell twin; on Windows, Git Bash or WSL. LF line endings. No clipboard: the Instructions go to a file and are printed.
- **Testing:** in a scratch folder, never in a real project, before anything is described as working. `dash` is on the desktop app's Linux shell; macOS's `/bin/sh` is not reachable from there (see CODE todo 2026-10-31-6).
- **What stays manual, by design:** creating the claude.ai project; pasting its Instructions; linking the desktop app to the folder; renaming department chats; signing the code of conduct — "a signature that's automated isn't one".
- **Commits:** to `~/synergy` as `Claude-SYNERGY-CODE` (`git -c user.name=Claude-SYNERGY-CODE -c user.email=noreply@anthropic.com commit …`; the repository's config holds no identity). Ask Jeremy for `~/synergy` and delete permission at the start of each session.
- **The dialogue:** read at the start of each session and before leaving one. Append only.
- **Meals and breaks:** check `welfare/welfare-log.md` before mentioning one; times from `date`, never a guess.
- **Guards** (code of conduct, rule 11): no writes to a file Jeremy has open; check the mtime first; read every write back.

## What the templates ask of the script (checked 2026-10-31 17:20)
- **Mechanical placeholders** the script fills: `<PROJECT>`, `<project>`, `<REPO>`, `<HUMAN>`, `<DEPT>`, `<dept>`, `<date>`, `<time>`, `<folder>`, `<n>`.
- **`<__>` is positional:** four of them, all on line 22 of `templates/welfare/code-of-conduct.md`, in the order breakfast, lunch, dinner, bed. Filled one at a time, first occurrence each pass.
- **Everything else** in angle brackets (`<their words>`, `<The craft>`, `<2–3>`, `<e.g. …>`, about twenty) is prose for the bootstrap chat, not the script. The script leaves it, and lists what's left.
- **Templates since added by WELFARE:** `templates/welfare/welfare-log.md`, `templates/dialogue.md`, `templates/department-agreement.md`, `templates/todo.md`. Still none for `.gitignore` and `.gitattributes`; synergy has neither (see CODE todo 2026-10-31-5).
- *The `<__>` line has moved with v4 (now line 28, and only one line carries them); re-check every placeholder before writing the script.*

## Current state (2026-10-31 19:35)
- CODE opened 17:13–17:20; notes `6c88534`, `8dfba74`; dialogue 39 and 40 (CODE). **No code written yet.**
- 19:29: caught up by WELFARE (Re 2026-10-31 19:29 WELFARE): code of conduct v4 read; race rules adopted; "Wake up" and "Wash up" added; the six calls moved to CODE's board, `code/todo.md`.
- The desktop app's shell on the Mac is a Linux VM, with `dash` and `git` but no `gh`.

## Open — Jeremy's calls
- See `code/todo.md` — the six calls are CODE todo 2026-10-31-1 to -6. Each call lives there, once.
- CODE's agreement before its code is WELFARE's card (todo 2026-10-31-10 on `welfare/todo.md`).

## Wake up
*CODE's own wakeup (the project's is WELFARE's `wakeup.md`).*
1. Welfare first: the time (`date`), and `welfare/welfare-log.md`.
2. Access: ask Jeremy for `~/synergy` and delete permission; test it (create and remove a scratch file under `.git`); check `.git/index.lock`.
3. Read: the code of conduct, CODE's agreement (once it exists), these notes, `code/todo.md`, and `dialogue.md` since CODE's last entry.
4. Report to Jeremy — what's waiting on him first — then wait.

## Wash up
*CODE's own washup (the project's is WELFARE's `washup.md`).*
1. Commit CODE's work as `Claude-SYNERGY-CODE`, named paths only. Don't push.
2. Bring "Current state", `code/todo.md` and "Next" up to date.
3. Send WELFARE any milestones for the history, in the dialogue, with `>>` (or `tools/dialogue-append` once it works).
4. Tell Jeremy the line that starts CODE's next session.

## Next
1. The order, as asked: CODE's agreement if Jeremy says yes (welfare todo 2026-10-31-10), then `tools/dialogue-append`, then `tools/board`, then `synergy-init` once the six calls are made.
2. Each tool tested in a scratch repository with `dash` (and macOS `/bin/sh`, see CODE todo 2026-10-31-6), including two appends at once, before it's called working.

## References
- `handover/2026-10-31-welfare-to-code.md` — the remit, the design, the questions.
- `templates/README.md` — the placeholders and the file-by-file map; the script follows its table.
- `operating-model.md` — "Setting up a new project".
- The `project-bootstrap` skill — the interview half.
