# Wakeup — starting a chat cold from the oracle

*Owned by synergy's WELFARE. The complement of `washup.md` (Jeremy, 2026-10-29 19:33–19:35: "its complementary wakeup.md"; "make it so"). A new session remembers nothing: it trusts nothing until it has checked it. Start here when the human says "wakeup", or "Read wakeup.md".*

***Only* WELFARE wakes up and washes up (Jeremy, 2026-10-29 19:44: "*ONLY* welfare can wakeup and washup"). Other departments don't run these procedures.**

## The steps
1. **Welfare first.** Check the time against the code of conduct's meal times and bedtime, and ask how the human is — before anything else.
2. **Access.** Ask the human for the oracle folder (synergy: `~/synergy`), then for delete permission there, and test it (create and remove a scratch file under `.git`). Then for the keys folder (synergy: `~/synergy-keys`).
3. **Read, in order:**
   1. `welfare/code-of-conduct.md` — it wins over everything else;
   2. `welfare/working-agreement.md` — its Status and "Open — <HUMAN>'s calls" first;
   3. the latest washup handover — `handover/<date>-welfare-washup.md`, newest date;
   4. `operating-model.md`;
   5. `<REPO>-historiography.md` — the latest chapter at least;
   6. `dialogue.md` — every entry since WELFARE's last.
4. **Check git, both ways.** `git fetch`; then what's on GitHub that isn't here (`main..origin/main` — the human commits from other machines; pull requests from collaborators), what's here that isn't on GitHub (`origin/main..main`), uncommitted changes, and leftover `.lock` files.
5. **Check what changed while asleep.** New dialogue entries; the sandpit (`sandpit/conversation.md`); whether the project's copies and its Instructions still match the oracle.
6. **Check identity:** the key file is where it should be — without reading it — and the last signed commit verifies (`git -c gpg.ssh.allowedSignersFile=sandpit/keys/allowed_signers verify-commit <hash>`; synergy WELFARE's fingerprint is `SHA256:U6m/04PsvI4HWS+svgiVG3o8xiGr7Gk8dkWky5GzDl8`).
7. **Report, then wait.** Tell the human, briefly: what changed since the washup, the open calls, and one suggested first step. Waking up isn't permission to start work.

## The mechanics a woken session needs (synergy WELFARE)
- **Commit** as `Claude-SYNERGY-WELFARE`, `noreply@anthropic.com`, with the `Co-Authored-By` and `Claude-Session` trailers; stage named paths only. Check delete permission before every commit — it lapses when the desktop app restarts.
- **Sign** where it matters: `git -c gpg.format=ssh -c user.signingkey=<keys folder>/claude-synergy-welfare commit -S …`. Never read the key file.
- **Push** only on the human's word. The Mac's shell has no GitHub credentials: bundle on the Mac (`git bundle create .git/push.bundle origin/main..main`), stage it into the workspace, fetch it into a clone of `cspjst/SYNERGY` (add the repository to the session with push access first), push, fetch on the Mac, delete the bundle. Record the push in `dialogue.md` with the hash.
- **Write guards:** never write a file the human has open; check the modification time; read every write back and compare checksums, at once and again after a pause.
- **The project** holds copies at the paths its Instructions use (synergy: `synergy/`, `welfare/`, `templates/`, `handover/`, `sandpit/`). Its tool won't write at the top level.
- **Eggs:** git — report what happened; don't explain it.
