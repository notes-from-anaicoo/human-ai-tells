# Changelog

All notable changes to AI Tells are documented here.

## [2.0.0] - 2026-10-08

AI Tells is now Human AI Tells, with the description line "AI tells with humanizer".

### Changed

- Merged a humanizer pattern set into AI Tells and renamed the project.
- Added patterns: arguing with no one, one-line closers, sayings that sound deep, staged run-ups, repeated openings, writing about the document instead of its subject, replies written for the wrong reader, and guesses past the writer's knowledge.
- Added a mark, draft, check workflow and a list of cases where the rules should not act.
- Added `human-ai-tells.md`, a plain Markdown edition with no tool-specific syntax, for use in any chat or tool.
- Added `NOTICE.md` crediting the sources and reproducing their licences.
- Detect mode is still the default: it reports and changes nothing unless asked to rewrite.

### Tests

- `TESTS.md` was written for 1.1.0 and has not yet been rerun against 2.0.0.

## [1.1.0] — 2026-09-25

### Added

- Meta-commentary family: labels that grade a sentence instead of saying it.
  - Drama adverbs such as "quietly".
  - Honesty labels such as "one honest caveat", "to be honest" and "frankly", which imply the surrounding sentences were not honest.
  - Build-up before news, such as "you should hear it from me first".
- Regression tests 16 to 18 for the new patterns.

## [1.0.0] — 2026-08-27

First public release of AI Tells, created and developed by Notes from an AI COO.

### Added

- WRITE, AUDIT, and REWRITE operating modes.
- Construction-level detection instead of simple phrase blacklisting.
- Meta-commentary family.
- Contextual distinction between information-grading and action-grading uses of `worth`.
- Throat-clearing, template, finale, transition, vocabulary, formatting, and mechanics families.
- Protection for quotations, legal text, code, commands, filenames, paths, citations, and other exact-content material.
- Technical-language exception to avoid damaging precise domain writing.
- Voice-preservation rules.
- Regression tests.
- Model-neutral design.

### Design principle

> Ban the construction, not the instances.
