---
project: davidjonidev/davidjonidev
stack: none
role: site
framework_pin: "none. A single README.md rendered by GitHub, with no build step and no dependency on wp-base or anything else, so there is nothing to pin. The key is present because the contract requires it for role: site."
status: "The GitHub profile README for `davidjonidev`, rendered at github.com/davidjonidev. Joined the fleet 2026-08-28. **It is PUBLIC**, unlike every other repo here, which constrains what may be written in this file and in decisions.md. It is DOWNSTREAM of `portfolio`: it holds no facts about David and exists to point at davidjoni.dev. It previously carried a full CV restatement and had drifted from the corpus in several places; that content was replaced rather than corrected."
next: "Nothing outstanding. If it grows past a screen, that is the signal it has started restating the corpus again."
blocked_on: "Nothing."
---

# Current state

## What is here

`README.md`, and nothing else. GitHub renders it on the profile page straight off `main`. No build,
no CI, no deploy step.

## Why it is short

It used to be long: employment history, per-project write-ups, a skills matrix, languages, personal
details. That made it a fourth copy of "who David is", after `portfolio/content/`, `cv.json` and the
private corpus in `applicator`. Copies drift, and this one had: it showed a former employer as
current, and put a client project at a different delivery stage than the CV did.

The fix was deletion rather than correction. Correcting it would have left a copy to drift again on
the next change to `cv.json`.

## The two rules that matter

- **PUBLIC.** No rates, no availability strategy, no non-public client names, nothing about work
  being sought, nothing from `applicator/profile.md`. This applies to `docs/memory/` too, which is
  why entries here are thin and point at `ops` instead.
- **Downstream of `portfolio`.** A fact about David goes in `portfolio/content/` and this file links
  to where it renders. Adding one here recreates the problem.

## Do NOT

- Do NOT restate the CV, the employment history or the case studies. Link to them.
- Do NOT use em dashes or en dashes. House style, and the loudest AI tell.
