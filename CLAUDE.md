# study-math

This repository is for math notes. The deliverable is prose and notation, not
code — do not scaffold projects, add build tooling, or set up tests here unless
asked. A short script to check a computation is fine, but it does not get
committed unless it is the thing being learned.

## Where notes come from

Anything I learn about mathematics, in any session, in any project — a
definition that finally clicked, a theorem I had to look up twice, a technique
that turned out to generalize. Recording it is a standing instruction everywhere;
this repository is the one place the results accumulate.

Notes are written in the same reply as the learning, not at session end. A
session can be interrupted, and an unwritten note is a lost one.

## Structure

- `INDEX.md` — one line per note, grouped by area. This is what gets read first,
  so the hook has to say what the note is actually good for.
- `notes/<area>/<topic>.md` — one idea per file. Create the area directory when
  the first note needs it.
- `_config.yml`, `_layouts/default.html`, `home.md` — the GitHub Pages site at
  <https://ctbot000.github.io/study-math/>. Asked for, so it is the one
  exception to "no build tooling" above; leave it in place. Adding a note
  needs no change here — it is published on the next push to `main`.

Areas: `algebra`, `analysis`, `calculus`, `discrete`, `geometry`,
`linear-algebra`, `number-theory`, `probability`, `statistics`. Add a new one
only when nothing existing fits — and add its section to `INDEX.md` too.

Filenames are kebab-case and name the idea, not the occasion:
`eigenvalue-geometric-meaning.md`, not `today-linear-algebra.md`.

## Note format

```markdown
---
title: <the claim or the concept, as a phrase>
area: <one of the areas above>
tags: [<3 or fewer>]
added: <YYYY-MM-DD, Korean calendar day>
---

## Idea

One or two sentences. What this is, in plain language, before any notation.

## Definition

The formal statement. Notation as `$…$` inline or `$$…$$` display — GitHub
renders both.

## Why it holds

The argument in outline, or the one step that makes it work. Not a full proof
unless the proof is the point.

## Example

The smallest concrete case that shows the idea working.

## Pitfalls

What I got wrong, or what the definition quietly rules out.

## See also

Links to related notes: `[title](../area/file.md)`.
```

**Every section is optional except `Idea`.** A note that is three lines and a
formula is a good note. Sections exist to keep the shape predictable, not to be
filled in.

## Writing rules

**Brief beats complete.** If a note cannot be reread in under a minute, it is
two notes, or it is a textbook chapter that does not belong here.

**Write the idea, not the session.** "The determinant is the signed volume
scale factor" is a note. "Worked through determinant problems today" is not. No
dates in the body, no "I was trying to…".

**One idea per file.** When a note starts covering two things, split it.

**Add a note only when it is new.** Read `INDEX.md` first. If the idea is
already recorded, sharpen that note rather than adding a second one, and say so
in the reply.

**Update the index in the same commit.** A note missing from `INDEX.md` is a
note that will never be found.

## What does not go here

- Full solutions to exercises, or copied textbook material. Record what the
  exercise taught, not the exercise.
- Per-session or per-date files. No study logs.
- General engineering knowledge — that belongs in the knowledge base at
  `../knowledge-base`.
- Notes about my English — those go to `../study-english`.
