# Decisions: github-profile

Append-only. Newest last. Record corrections **as corrections**; never edit a wrong entry into a
right one, because how the error was made is the reusable part.

**🔴 This repo is PUBLIC and so is this file.** Studio-level reasoning goes in
`~/business/ops/docs/memory/decisions.md`, which is private. Entries here stay thin and point there.

## 2026-08-28 — joined the fleet, and the README became a pointer instead of a second CV

The profile README carried a full restatement of the CV: employment history, per-project write-ups,
a skills matrix, languages and personal details. That made it a fourth copy of the same facts, after
`portfolio/content/`, `cv.json` and the private corpus.

**It had already drifted, which is the whole argument.** Among other things it showed a former
employer as current, and described a client project at a different delivery stage than the CV did.
Nobody had edited either document wrongly; they were edited separately, which is enough.

**Replaced rather than corrected.** Correcting the copy leaves a copy, and it drifts again the next
time `cv.json` changes. The README now states who David is in two lines and links to davidjoni.dev
for the CV, the case studies and contact. The old version remains in git history.

**The repo also joined the fleet contract**: `AGENTS.md` real with `CLAUDE.md` symlinked,
`docs/memory/`, and registration with the brain gate so it is audited like the rest.

**One thing this repo has that the others do not: it is public.** The contract puts internal
instruction and memory files inside the repo, which is safe when the repo is private and is not here.
`AGENTS.md` carries the constraint in full. The short version: if a fact belongs in the private
corpus, it does not get explained here either.

Fleet-level reasoning for the write-it-once rule: `ops/docs/memory/decisions.md`.
