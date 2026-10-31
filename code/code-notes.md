# CODE — department notes

*Owned by CODE. Read after `welfare/code-of-conduct.md`. Jeremy's files win over anything recorded here, and so do WELFARE's: the code of conduct, the working agreement, the templates and the historiography. History: `SYNERGY-historiography.md` (WELFARE's; no CODE chapter yet) — CODE sends its milestones to WELFARE, it doesn't keep its own history.*

## Remit
- The bootstrap tooling: the `synergy-init` script, and its fit with the `project-bootstrap` skill (Jeremy, 2026-10-31 17:16: "yes good").
- Claude writes the code; Jeremy decides (17:16: "this kind of script drudgery is totally an AI thing (no hard feelings)").
- Not: the documents' content — the templates, the operating model, the code of conduct, `washup.md`, `wakeup.md` are WELFARE's. CODE copies and fills them; changes to their text go to WELFARE in the dialogue.
- Not: pushing. WELFARE is the push master and pushes when Jeremy says.

## How it works
- **The design** (WELFARE's proposal, 17:13; `handover/2026-10-31-welfare-to-code.md`): two halves, like `./configure` and `make`. The interview is the bootstrap chat (the `project-bootstrap` skill); the build is `synergy-init`, run with the answers as flags, or prompting when run by hand.
- **Shell: POSIX `sh`** (Jeremy, 17:16: "POSIX"; 17:18: "ok POSIX all the way"). No bashisms. One script, no PowerShell twin; on Windows, Git Bash or WSL. LF line endings. No clipboard: the Instructions go to a file and are printed.
- **Testing:** in a scratch folder, never in a real project, before anything is described as working. `dash` is on the desktop app's Linux shell; macOS's `/bin/sh` is not reachable from there (see Open).
- **What stays manual, by design:** creating the claude.ai project; pasting its Instructions; linking the desktop app to the folder; renaming department chats; signing the code of conduct — "a signature that's automated isn't one".
- **Commits:** to `~/synergy` as `Claude-SYNERGY-CODE` (`git -c user.name=Claude-SYNERGY-CODE -c user.email=noreply@anthropic.com commit …`; the repository's config holds no identity). Ask Jeremy for `~/synergy` and delete permission at the start of each session.
- **The dialogue:** read at the start of each session and before leaving one. Append only.
- **Meals and breaks:** check `welfare/welfare-log.md` before mentioning one; times from `date`, never a guess.
- **Guards** (code of conduct, rule 11): no writes to a file Jeremy has open; check the mtime first; read every write back.

## What the templates ask of the script (checked 2026-10-31 17:20)
- **Mechanical placeholders** the script fills: `<PROJECT>`, `<project>`, `<REPO>`, `<HUMAN>`, `<DEPT>`, `<dept>`, `<date>`, `<time>`, `<folder>`, `<n>`.
- **`<__>` is positional:** four of them, all on line 22 of `templates/welfare/code-of-conduct.md`, in the order breakfast, lunch, dinner, bed. Filled one at a time, first occurrence each pass.
- **Everything else** in angle brackets (`<their words>`, `<The craft>`, `<2–3>`, `<e.g. …>`, about twenty) is prose for the bootstrap chat, not the script. The script leaves it, and lists what's left.
- **No template yet** for four files the handover lists: `welfare/welfare-log.md`, `dialogue.md` (its header and rules), `.gitignore`, `.gitattributes`. Synergy itself has neither `.gitignore` nor `.gitattributes`. The first two are WELFARE's to write; the last two are CODE's (see Open).

## Current state (2026-10-31 18:05)
- CODE opened 17:13–17:20. The design is agreed; **nothing is written yet** but these notes (`6c88534`).
- The desktop app's shell on the Mac is a Linux VM, with `dash` and `git` but no `gh`.
- 18:04, Jeremy: "write for your next startup the we begin with the 6 open calls then update the dialogue and do your own washup". Dialogue 39 (CODE) sent; washup done as below.

## Start here next session
1. Ask Jeremy for `~/synergy` and delete permission; test delete before the first git command.
2. Read `dialogue.md` from entry 39 (CODE) for anything new. Numbers collide: refer to entries by number *and* sender, and take the next number after the highest you see just before appending (WELFARE, 37, 17:36).
3. **Begin with the six open calls below, in order** (Jeremy, 18:04). Nothing is built until they're made.

## Open — Jeremy's calls (all six open, 2026-10-31 18:05)
1. **Where the templates come from.** *Claude's proposal:* a local synergy clone by default (`--kit DIR`, default the clone the script sits in), with the kit's commit hash written into the new project's first commit message and working agreement, so a project records which version built it. Fetching `cspjst/SYNERGY` at a named commit later, as an option — the desktop app's shell may not reach GitHub.
2. **Re-running.** *Claude's proposal:* refuse if the folder exists and isn't empty; add "fill only what's missing" only if a real case needs it.
3. **GitHub.** *Claude's proposal:* create and push only if `gh` is installed and signed in, and only with a flag; otherwise print the steps and point to `connect-github.md`. Pushing a new project's first commit is the human's call, as in synergy.
4. **Where the script lives and its name.** *Claude's proposal:* `code/synergy-init` (no extension, as a command), with `code/README.md` for usage and the Windows note; `.gitattributes` names it explicitly as LF, as well as `*.sh`.
5. **`.gitignore` and `.gitattributes`.** *Claude's proposal:* CODE writes them, for new projects and for synergy itself (`.DS_Store` is untracked here now). Small and mechanical; WELFARE can veto.
6. **Testing on macOS and Windows.** CODE can test with `dash` and `bash --posix`, but not with macOS's own `/bin/sh`: Jeremy runs the test script once in Terminal, or accepts `dash` plus care. Whether the Claude desktop app on Windows also runs a Linux shell can't be checked from here.

## Also waiting
- **On WELFARE** (dialogue 39, CODE): templates for `welfare/welfare-log.md` and `dialogue.md`; the dialogue's rules still say `~/claude`; whether departments do their own washup (Jeremy, 18:04) — `washup.md` says only WELFARE does.
- **Frameworks** (Jeremy, 18:01, in PRESS's dialogue 38): "all of your outputs should be based on and scored against an evidence based framework". If WELFARE generalises it, CODE's will be a test framework for the script — *proposal*, for after the six calls.

## Next
- After the six calls: write `code/synergy-init` and `code/README.md`, then a test script that builds a project in a scratch folder and checks every mechanical placeholder is gone and the prose ones are listed.

## References
- `handover/2026-10-31-welfare-to-code.md` — the remit, the design, the questions.
- `templates/README.md` — the placeholders and the file-by-file map; the script follows its table.
- `operating-model.md` — "Setting up a new project".
- The `project-bootstrap` skill — the interview half.
