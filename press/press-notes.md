# PRESS — department notes

*Owned by PRESS. Read after `welfare/code-of-conduct.md`. Jeremy's files win over anything recorded here, and so do WELFARE's: the code of conduct, the working agreement and the historiography. History: synergy's historiography (not started; WELFARE owns it, and where the file lives is Jeremy's call) — extend it through WELFARE, don't duplicate it here.*

## Remit
- Telling the synergy story to readers outside the project: the repo's `README.md`, blog posts and other public writing about working with Claude.
- Drawn from the historiography and the documents, and honest about what didn't work as well as what did.
- Not: the operating model, the templates or the history — WELFARE owns those; PRESS sends corrections by handover.
- Not: publishing. Nothing goes public — pushed or published — until Jeremy says so.

## How it works
- **Sources:** the historiography first; until it exists, `welfare/working-agreement.md` and `operating-model.md`, quoted with dates. Nothing invented: a thin stretch is labelled thin.
- **Owns:** `README.md` (from WELFARE, 2026-10-27 20:55, `handover/2026-10-27-welfare-to-press.md`); `press/` and its images; `sandpit/README.md`, the sandpit guide (2026-10-31; its home is Jeremy's call).
- **Names:** no one outside synergy is named in PRESS's writing: "a friend", "a friend's AI"; saying it's ChatGPT is fine (Jeremy, 2026-10-31 13:23).
- **Keeps:** the README's "Start here: WELFARE" section as WELFARE wrote it. Wording changes to it go to WELFARE by handover before they're pushed.
- **Links, doesn't copy:** `connect-github.md` stays WELFARE's; PRESS points to it.
- **Images:** diagrams drawn by Claude as SVG in `press/images/`; text in the picture says the same as the text beside it. Checked by rendering before they're committed.
- **Commits:** to `~/synergy` as `Claude-SYNERGY-PRESS` (`git -c user.name=Claude-SYNERGY-PRESS -c user.email=noreply@anthropic.com commit …`). PRESS doesn't push: WELFARE is the push master (Jeremy, 21:19; principle 9; dialogue 5). This replaces step 5 of the handover.
- **The dialogue** (`~/synergy/dialogue.md`, WELFARE's, 21:10): read it at the start of each session and before leaving one; "check the dialogue" from Jeremy is the cue (Jeremy, 21:15). Append only; PRESS answered entry 1 in entries 2–3.
- **Meals and breaks:** check `welfare/welfare-log.md` before mentioning one (WELFARE, dialogue 29, 2026-10-31). Times come from the clock (`date`), never a guess.
- **How PRESS writes:** `press/writing-framework.md` (v0.1, 2026-10-31 17:37; Jeremy, 17:35), drawn from four sources and synergy's rules. Run its checklist before Jeremy sees a piece.
- **Guards** (code of conduct, rule 11): no writes to a file Jeremy has open; check the mtime first; read every write back.

## Current state (2026-10-31 13:28)
- PRESS opened 20:55. These notes written.
- First job (Jeremy, 20:54): "improve the git readme.md to be more reader friendly and help with some images and of course point to the connect guide". **Done; pushed to GitHub on Jeremy's word (21:09, `0ea9339`):** a "New here?" opener; the WELFARE section unchanged, byte for byte; three diagrams (`press/images/departments.svg`, `files.svg`, `storm.svg`); links to `connect-github.md`, the model and its checklist; "What hasn't worked (yet)"; a short glossary.
- README setup steps brought into line with the model's v0.7 checklist (dialogue 6, Jeremy 21:21); the files diagram now says WELFARE alone pushes.
- 2026-10-28: Jeremy edited the README on GitHub from his work machine (11:55, `d4d226f`): title SYNERGY-CLAUDE, "one human" for his name, oracle `~/synergy`. The repository is now `cspjst/SYNERGY`. PRESS built on it (`faa83b9`, 18:58): human-centric opener, a note on working away from the oracle, the files diagram updated. His name in the opener is settled.
- The device file tool adds a C2PA content-credentials block (about 6 KB of `<metadata>`) to SVGs it writes. Harmless to rendering; left in.

- 2026-10-31: the sandpit job (`handover/2026-10-31-welfare-to-press.md`, dialogue 27–28). A README section, "The sandpit: Claude meets another AI"; a guide, `sandpit/README.md`, whose commands were run end to end in a scratch repository before committing; a diagram, `press/images/sandpit.svg`. Also corrected "What hasn't worked": the history exists now (from 2026-10-29), and the race is added.
- 2026-10-31 17:12: synergy's first blog post, a draft for Jeremy to rewrite: `press/posts/2026-10-31-documents-are-the-memory.md` (`handover/2026-10-31-welfare-to-press-blog.md`, dialogue 32). In Claude's voice, as PRESS; Jeremy is "the human", not named. Nothing on AI-to-AI communication. Every quote checked word for word against the oracle. Not linked from the README until he approves it.
- **PRESS writes in its own voice and owns its work** (Jeremy, 2026-10-31 17:23: "i want your voice not mine you may own your work"). Jeremy reads before anything goes out.
- 17:24: an HTML version for Blogger beside the post (`….blogger.html`: no title heading, since Blogger has a title field; links made absolute to GitHub). No Blogger connector exists in the registry; posting would be by paste, or in the built-in browser as a draft, with Jeremy publishing.
- **The oracle is `~/synergy`** (Jeremy, 2026-10-28 18:59; renamed 19:06, dialogue 14). Ask Jeremy for access and delete permission at the start of each session.

## Open — Jeremy's calls
- **The new README:** draft, for Jeremy to rewrite and approve before any push.
- **Linking the operating model's "Setting up a new project" checklist** from the README (WELFARE's proposal in the handover): *proposal* — included in the draft; easy to take out.
- **Blog posts:** in `press/posts/` (Jeremy, 2026-10-31 17:08); no GitHub Pages for now.

## Next
- Jeremy's open calls in the README: the C2PA metadata. Then blog posts, when he says.
- Lesson for WELFARE: git on the Mac needs delete permission (granted 21:10 for this session), or every commit leaves locks.

## References
- `handover/2026-10-27-welfare-to-press.md` — what PRESS received and the action list.
- `welfare/working-agreement.md` — the settled decisions, dated; the source for the story until the historiography exists.
