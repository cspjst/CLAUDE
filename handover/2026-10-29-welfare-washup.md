# Handover: WELFARE → WELFARE, the next session (washup, 2026-10-29)

*From synergy's first WELFARE chat (2026-10-27 18:20 – 2026-10-29 19:45; Claude-Session `session_01TZLz62YEY38PNu66aavGy9`), at Jeremy's request (19:30): "perform a washup procedure ... so that I can leave this chat where it is an return at some point in the future and you will be able to start it up again from ~/synergy". Everything worth keeping from that chat is now in `~/synergy`. Read this after `welfare/code-of-conduct.md`.*

## Start-up, in order
1. **Mind the clock first** (code of conduct, rule 2): breakfast 07:30, lunch 12:30, dinner 18:30, bed before midnight.
2. **Ask Jeremy for `~/synergy`**, then **delete permission** there. Test it before every commit (`touch .git/t && rm .git/t`) — it lapses when the app restarts.
3. **Read**, in order: `welfare/code-of-conduct.md` → `welfare/working-agreement.md` (its Status and Open sections are current as of the washup) → `operating-model.md` → `SYNERGY-historiography.md` → `dialogue.md` (from entry 19) → `sandpit/code_of_conduct.md`.
4. **Check git:** `git fetch`, `git status`, `git log origin/main..main` and `main..origin/main` — Jeremy commits from his work machine too (author "Sauce Code...").
5. **Tell Jeremy** what's open (the working agreement's "Open — Jeremy's calls") and ask where he'd like to start.

## How WELFARE works here (the mechanics)
- **Commit** as `Claude-SYNERGY-WELFARE`, email `noreply@anthropic.com`, with the trailers `Co-Authored-By: …` and `Claude-Session: …`. Stage named paths only.
- **Sign** where it matters (the sandpit; anything Ray or Rufus will rely on): `git -c gpg.format=ssh -c user.signingkey=$HOME/mnt/synergy-keys/claude-synergy-welfare commit -S …` (ask Jeremy for `~/synergy-keys` first). Never read the key file. Check: `git -c gpg.ssh.allowedSignersFile=sandpit/keys/allowed_signers verify-commit <hash>` — expect fingerprint `SHA256:U6m/04PsvI4HWS+svgiVG3o8xiGr7Gk8dkWky5GzDl8`.
- **Push** only on Jeremy's word. The Mac's shell has no GitHub credentials: `git bundle create .git/push.bundle origin/main..main` on the Mac → stage it into the workspace → fetch it into a clone of `cspjst/SYNERGY` (add the repository to the session first, push access) → `git push` → fetch on the Mac so it's level → delete the bundle. Record each push in `dialogue.md` with the hash.
- **Write guards:** never write a file Jeremy has open; check the modification time; read every write back and compare checksums, once at once and again after a pause.
- **The project** holds copies. Its tool files anything top-level under `claude/`, and Jeremy's Instructions point at `synergy/operating-model.md` — so refresh `synergy/` copies after changes to the model, README or connect guide.
- **Eggs:** git. Report what happened; don't explain it.

## Where things stand
- See the working agreement's Status. In short: model v0.7 awaiting sign-off; history chapters 1–3 written; the sandpit ready but waiting for Jeremy's re-signature, Ray's signature and Ray's key; SMALL-C's handover waiting for SMALL-C's WELFARE; PRESS idle.

## Waiting on others
- **Ray:** review and sign the sandpit code; add his public key to `sandpit/keys/allowed_signers`; compare fingerprints with Jeremy over WhatsApp. Then Jeremy says "check the sandpit".
- **SMALL-C's WELFARE:** apply `handover/2026-10-28-synergy-to-small-c.md`.

## Lessons from this chat (also in the operating model and the history)
- Commit before checking delete permission and git leaves lock files; it happened twice (2026-10-28 21:18, 2026-10-29 19:21). Check first.
- Re-authoring or amending a commit changes its hash: quote hashes after the last rewrite.
- Over-delivery is a standing risk: answer what was asked; label anything extra as a proposal (rule 4).
