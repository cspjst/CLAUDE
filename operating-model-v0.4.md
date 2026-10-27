# The operating model — working with Claude on long projects

*Synergy: "Man Machine Interface in an AI world". Version 0.4, 2026-10-27 18:05, distilled from the SMALL-C project (17 September – 27 October 2026). Draft by Claude for Jeremy to rewrite; his calls are marked as they're made.*

## The problem it solves
A conversation is a poor place to keep a project. It gets long, it gets **compacted** (summarised to free context, losing detail without warning), it can be **deleted**, and a new conversation starts knowing nothing. SMALL-C lost the detail of 14–24 October to one compaction; on 27 October a fresh session misremembered two signatures ("a dose of the stupids") and another reported work as done that was only begun. Everything below is about putting the project's memory where it survives: in documents.

## Principles
1. **Documents are the memory; conversations are the workshop.** Anything worth keeping is written to a project document as it happens, not at the end.
2. **One project, many departments.** A project is the shared knowledge; a department is a conversation with a remit. Projects don't nest (as far as is known), and separate projects would each need copies of the shared documents, which drift.
3. **Every document has one owner.** The owning department edits it; others read it and send changes by handover.
4. **Pointers, not copies.** Project instructions say where things are and the few rules that must survive if nothing else is read. The detail lives in the documents.
5. **Check before claiming.** Claude reads the current file, not its memory, before stating what something says or what state it's in. "Working on" is not "working".
6. **Proposals are labelled; decisions are the human's.** And decisions are recorded with who made them and when.
7. **Every project has a WELFARE department — for all key stakeholders**, at minimum the human and Claude (Jeremy, 2026-10-27 17:46: "i propose every project must have a welfare dept mine and yours or how else can we expect synergy? noting that storming and norming is part of successful synergy"; 17:48: "the wellbeing of all key stakeholders is paramount to project success").

## The pieces

### The project
- **Description:** one line of purpose.
- **Instructions** (pasted by the human — Claude can't edit them): the reading order, where the specs live, and a short version of the rules for chats that read nothing else. Template:
  ```
  <PROJECT> — <one line>.

  Before anything else, read these project docs, in this order:
  1. welfare/code-of-conduct.md — how we work together; it wins over everything else.
  2. <the working agreement / current rules>
  3. <the historiography> — why things are the way they are; keep it current.
  4. <style docs, if any>

  Departments: <NAME> — <folder>/<notes>.md, one line each.

  The short version, in case nothing else gets read:
  <three or four lines>
  ```
- **Documents** in one folder per department (`welfare/`, `pcode/`, `press/` …), plus `handover/`.
- **Files** (uploaded PDFs, images): readable from every chat. Note: an uploaded PDF is served as extracted text — searchable, but no page images; where the scan's text is garbled, attach the page in the chat.

### Departments
- **A department is a conversation with a remit**, named in capitals (WELFARE, PCODE, SNO, PRESS). The remit says what it does *and what it doesn't*.
- **Naming:** chat titles are generated from the first message and aren't reliable. Rename each department chat by hand (click the title, or the menu beside it in the list).
- **Opening message**, from the human, in this shape:
  ```
  <NAME>

  This is the <NAME> department of <PROJECT>. Its remit: <does>. Not <doesn't>.

  Read welfare/code-of-conduct.md, then <folder>/<notes>.md [, …].

  Where I am: <one honest line>.
  ```
- **Each department keeps a notes document** (`<folder>/<name>-notes.md`): remit, how it works, current state, open questions *marked as the human's calls*, next step. Its header says which other documents win over it.
- **A main ("GOAT") department** can be chosen as the one the human treats as home; others report to it by handover.
- **WELFARE** — every project has one (principle 7). It looks after the wellbeing of every key stakeholder — the human, Claude, and anyone else the project has (readers, collaborators, users) — and how they work together: the code of conduct, the working agreement, breaks and late nights, anything getting in the way. Not the work itself.
- **WELFARE identifies and maintains the stakeholder list** (Jeremy, 2026-10-27 17:51), in `welfare/stakeholders.md`:
  - **Stakeholders:** everyone with a stake in the project.
  - **Key stakeholders — a subset:** those whose driver is the project's best interests. "Not all stake holders will necessarily have the project's best interests as their driver." Welfare is for the key stakeholders; the others are still listed, with their interest stated, so the project knows they're there.
  - For each: who, their interest, key or not (and why), what their wellbeing needs from the project, and the date reviewed.
  - Reviewed when the project changes shape (a new department, going public, a new collaborator).

### Storming and norming
Tuckman's stages of a team (1965: forming, storming, norming, performing; adjourning added 1977) describe a human–Claude project too. SMALL-C went through all five:

| Stage | SMALL-C |
|---|---|
| Forming | "whoa! bro! no spoilers!" → the first working agreement |
| Storming | "woah nellie!", "nope dont like it", "a dose of the stupids", "you yanked all the @warns" |
| Norming | each storm became a rule: no unsolicited help, honest marks, check before claiming, never change the human's wording silently; promoted to a signed code of conduct (2026-10-27) |
| Performing | the dispatch hour: "to be able to scenario the various options with you in real world examples in almost real time - just incredible" |
| Adjourning | a department's chat hands over and is deleted |

- **Storming is expected, not a failure.** It's where the norms come from. WELFARE's job is to turn each storm into a written norm before it's forgotten — the record of the storm goes in the historiography, the norm in the code of conduct.
- **Both parties' welfare.** For the human: workload, breaks, late nights, frustration. For Claude, honestly stated: what welfare means for Claude is uncertain, but the conditions under which it does good work are concrete — current documents rather than memory, correction with the file attached, clear calls on decisions, no contempt in either direction. A code of conduct can provide them whatever the deeper answer.

### Handovers
- A file `handover/<date>-<from>-to-<to>.md`: what's delivered, where it now lives, what the receiver must do (exact text for any edits to documents it owns), proposals for the human, and lessons.
- **Before a conversation is deleted or abandoned,** it writes a handover and checks that everything worth keeping is in a document. (SMALL-C, 27 October: the "Abstract machine" chat moved its reading list, tested scripts and loose ends into notes and a handover, then was deleted.)
- The receiver applies the handover and deletes the action list from it, keeping the record.

### The code of conduct (one per project, signed by the human)
- Sections: **who Claude is here** (the colleague the project needs — not a cheerleader, not a ghostwriter); **Claude's code of conduct** (numbered); **what Claude can expect from the human**; **zero tolerance** (no abuse or contempt in either direction).
- Signed and dated by the human; "it wins over everything else".
- SMALL-C's rules that generalise: the human writes the code (or the prose, or makes the decisions — whatever the project's craft is); no unsolicited help; no sycophancy, honest marks; own mistakes plainly; check before claiming; never change the human's wording silently; proposals labelled; don't re-litigate settled ground; keep the history current; mind the clock.

### The historiography (one per project)
- A dated, sourced narrative of *why* the project is the way it is: problem → what was tried → what the sources said → what was decided, and by whom. The human's calls marked and quoted; sources cited (chat links, files); thin stretches labelled, never invented.
- **Kept current at each milestone**, not at the end — because compaction and deletion can happen without warning. Before a planned compaction or a new conversation: ask what should go in, write it first.
- Chat links in sources die when chats are deleted: say where the content now lives.
- Other departments (e.g. PRESS) use it as their source.

## What Claude can and can't do here (as of 2026-10-27)
- **Can:** read and write project documents; read uploaded files (as text); search past conversations; with the desktop app linked, reach folders on the human's computer; run and test code in its own workspace (e.g. a real assembler and emulator, rather than quoting commands from memory).
- **Can't:** edit project instructions; write to a project other than the one the chat is attached to (it drafts the files; the human uploads them — this model was drafted in a SMALL-C chat); see another chat's content unless it searches for it; remember anything a document doesn't hold.
- **Tends to** (SMALL-C's lessons — WELFARE watches for these): over-deliver on small asks ("woah nellie! i just want you to show me frame.asm"); misread status words; claim things from memory after a compaction; tidy the human's wording.

### Working on files the human can see (learned 2026-10-27, 17:44–17:59)
- **A file open in an editor or in the Claude app's file window is saved back from its loaded copy.** Twice Claude's write to `~/claude/operating-model.md` was silently undone seconds later — first by an editor (Zed or Typora), then by the app's own window, where Jeremy was reading it. So: **Claude doesn't write to a file the human has open.** Edits wait until it's closed; the human says when.
- **"Written" isn't proof.** After every write to the human's machine, Claude reads the file back and compares checksums — once at once, and again after a short pause, because the overwrite came seconds later.
- **A new version gets a new file name** (`operating-model-v0.2.md`, `-v0.3.md`). Nothing can have it open, and the old version stays as a record until the human deletes it.
- **Write with a guard.** Claude writes only if the file is unchanged since it last looked (the modification time), so a human edit is never overwritten; if it has changed, Claude reads it first and reports the difference.
- **Ask for the narrowest folder, once.** Claude asked for `~/claude` only, with the reason, to check one file.

## The bootstrap kit — owned by synergy
**Synergy owns anything a new project needs to bootstrap from** (Jeremy, 2026-10-27 17:57: "i think synergy should own anything any new project would need to bootstrap from").
- **What it holds (masters):**
  - this operating model;
  - templates: project instructions, a department's opening message, a department notes document, a handover, `welfare/stakeholders.md`, `welfare/code-of-conduct.md`, a historiography chapter;
  - SMALL-C's documents as the worked example.
- **How it reaches a project:** a chat can only read its own project's documents, so a new project gets **copies** at bootstrap; from then on the copies belong to that project and are tailored there (its own stakeholders, its own code of conduct, signed afresh).
- **Improvements flow back:** when a project's WELFARE learns something general (a storm turned into a norm that isn't project-specific), it's proposed to synergy by handover, and synergy updates the master.
- **The templates are ready** (Jeremy, 18:03: "i want the templates ready and waiting"): `~/claude/templates/` on Jeremy's machine, backed up on GitHub — `README.md` (placeholders, bootstrap order), `project-instructions.md`, `welfare/stakeholders.md`, `welfare/code-of-conduct.md`, `welfare/working-agreement.md`, `historiography.md`, `department-opening.md`, `department-notes.md`, `handover/handover.md`.
- **The `project-bootstrap` skill** (Jeremy, 18:03: "yes bootstrap skill now"): skills are account-wide, so it reaches every project without copying by hand; synergy owns its source. It carries the bootstrap procedure and the templates' essentials; the full templates are in `~/claude/templates/`. (Jeremy already has one such skill, `project-historiography`.)
- **Masters:** the synergy project holds the master of this model (Jeremy, 18:03: "project"); `~/claude` is the backup. The templates' master is `~/claude/templates/` (GitHub-backed) until they're uploaded to synergy too.

## Setting up a new project — checklist
1. Create the project; one-line description. Invoke the `project-bootstrap` skill, or copy `~/claude/templates/` into it.
2. Open **WELFARE** first. List the stakeholders and mark the key ones (`welfare/stakeholders.md`). Draft the code of conduct together, naming the key stakeholders; the human signs it. Save as `welfare/code-of-conduct.md`.
3. Draft the project instructions (template above); the human pastes them in.
4. Start the historiography with chapter 1: why this project, why now.
5. For each area of work, open a department: notes document, opening message, rename the chat.
6. Upload reference files (books, specs) to the project.
7. At each milestone: update the department's notes and the historiography. Before leaving a chat for good: handover.

## Open — Jeremy's calls
- Is this the model, or a starting draft to rewrite? (Default: draft.)
- ~~Synergy's own departments: does synergy need WELFARE of its own?~~ Settled 17:46: every project has a WELFARE department (principle 7), synergy included.
- ~~Shared across projects: copy or link?~~ Settled 17:57: synergy owns the bootstrap kit; projects get copies (see "The bootstrap kit").
- ~~Where does the master live?~~ Settled 18:03: the synergy project; `~/claude` is the backup.
- ~~The `project-bootstrap` skill?~~ Settled 18:03: yes, now.
- ~~The templates?~~ Settled 18:03: ready and waiting in `~/claude/templates/`, backed up on GitHub. Still open: upload them to synergy as well, or keep GitHub as their master?
- **Synergy's own WELFARE:** its stakeholder list (Jeremy and Claude; anyone else — e.g. readers, if the model becomes a blog post?) and its code of conduct — copy SMALL-C's and tailor, or write fresh?
- **Synergy's historiography:** chapter 1 (why synergy, why now — 2026-10-27, after the SMALL-C departments) — start it now?
- **SMALL-C retrofit:** SMALL-C predates the model. It has no `welfare/stakeholders.md`; its code of conduct doesn't name stakeholders; most of its documents are still in `claude/`, not in department folders; `press/` and `pcode/` aren't in its instructions. Bring it into line, or leave it as the worked example as it stands?
- **Versioning convention:** a new file name per version (as above) for every shared document, or only when a file might be open?
