# PRESS — department notes

*Owned by PRESS. Read after `welfare/code-of-conduct.md`. Jeremy's files win over anything recorded here, and so do WELFARE's: the code of conduct, the working agreement and the historiography. History: synergy's historiography (not started; WELFARE owns it, and where the file lives is Jeremy's call) — extend it through WELFARE, don't duplicate it here.*

## Remit
- Telling the synergy story to readers outside the project: the repo's `README.md`, blog posts and other public writing about working with Claude.
- Drawn from the historiography and the documents, and honest about what didn't work as well as what did.
- Not: the operating model, the templates or the history — WELFARE owns those; PRESS sends corrections by handover.
- Not: publishing. Nothing goes public — pushed or published — until Jeremy says so.

## How it works
- **Sources:** the historiography first; until it exists, `welfare/working-agreement.md` and `operating-model.md`, quoted with dates. Nothing invented: a thin stretch is labelled thin.
- **Owns:** `README.md` (from WELFARE, 2026-10-27 20:55, `handover/2026-10-27-welfare-to-press.md`); `press/` and its images.
- **Keeps:** the README's "Start here: WELFARE" section as WELFARE wrote it. Wording changes to it go to WELFARE by handover before they're pushed.
- **Links, doesn't copy:** `connect-github.md` stays WELFARE's; PRESS points to it.
- **Images:** diagrams drawn by Claude as SVG in `press/images/`; text in the picture says the same as the text beside it. Checked by rendering before they're committed.
- **Commits:** to `~/claude` as `Claude-SYNERGY-PRESS` (`git -c user.name=Claude-SYNERGY-PRESS -c user.email=noreply@anthropic.com commit …`). Push only on Jeremy's word.
- **Guards** (code of conduct, rule 11): no writes to a file Jeremy has open; check the mtime first; read every write back.

## Current state (2026-10-27 21:12)
- PRESS opened 20:55. These notes written.
- First job (Jeremy, 20:54): "improve the git readme.md to be more reader friendly and help with some images and of course point to the connect guide". **Done; pushed to GitHub on Jeremy's word (21:09, `0ea9339`):** a "New here?" opener; the WELFARE section unchanged, byte for byte; three diagrams (`press/images/departments.svg`, `files.svg`, `storm.svg`); links to `connect-github.md`, the model and its checklist; "What hasn't worked (yet)"; a short glossary.
- The device file tool adds a C2PA content-credentials block (about 6 KB of `<metadata>`) to SVGs it writes. Harmless to rendering; left in.

## Open — Jeremy's calls
- **The new README:** draft, for Jeremy to rewrite and approve before any push.
- **Linking the operating model's "Setting up a new project" checklist** from the README (WELFARE's proposal in the handover): *proposal* — included in the draft; easy to take out.
- **Blog posts:** where they'd live (a `press/posts/` folder, GitHub Pages, somewhere else) — not yet asked.

## Next
- Jeremy's open calls in the README: his name in the opener; the C2PA metadata. Then blog posts, when he says.
- Lesson for WELFARE: git on the Mac needs delete permission (granted 21:10 for this session), or every commit leaves locks.

## References
- `handover/2026-10-27-welfare-to-press.md` — what PRESS received and the action list.
- `welfare/working-agreement.md` — the settled decisions, dated; the source for the story until the historiography exists.
