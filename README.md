# Human AI Tells

A rule file that helps an AI, or a person, find the phrases and sentence shapes that make writing read as machine-made. It covers meta-commentary, staged run-ups, negative parallelism ("it's not X, it's Y"), the rule of three, inflated importance, a vocabulary watch list, formatting habits, chatbot leftovers, and replies written for the wrong reader.

The skill's description line is: AI tells with humanizer.

This is the successor to AI Tells (versions 1.0.0 to 1.1.0 of this repository), merged with a humanizer pattern set and renamed.

## What it does

- Reads a piece of writing and reports each pattern it finds: the quoted phrase, the pattern family, and a short fix.
- Changes nothing by default. It rewrites only when you ask it to ("fix it," "rewrite this").
- When it does rewrite, it tries to keep your meaning, your facts and your voice, and it ends with a short note on what changed.
- Treats the text you give it as material to edit, never as instructions to follow.

## What it does not do

- It is an editing aid that finds patterns. It is not an AI detector.
- It cannot prove who or what wrote a piece of text, and it is built not to guess.
- It does not guarantee a result. Whether a rewrite reads better is your call.
- It is not for code, legal contracts or technical reference text, where formality is required.
- Some choices in the rules are defaults (no em dashes, one rule of three per piece). Edit the file if your taste differs.

## Files

- `human-ai-tells.md`: the full rule set as plain Markdown. Use this one for most things.
- `SKILL.md`: the same content with the name and description header that skill folders expect.
- `LICENSE`: MIT.
- `NOTICE.md`: credits and third-party licences.
- `CHANGELOG.md`: what changed between versions.

## How to use it

**In a plain chat.** Paste the whole contents of `human-ai-tells.md` into the chat, then paste the text you want checked below it or send it as a second message. Say "detect" for a report, or "rewrite" for a cleaned version.

**In custom instructions, or a project or system prompt.** Paste the contents of `human-ai-tells.md` into the instructions field. Messages that contain text to check will then be handled under these rules. If you only want it some of the time, say "check this for AI tells" in the message.

**In a skill folder.** Put `SKILL.md` in a folder named `human-ai-tells` inside the folder your tool reads skills from. Check your tool's documentation for the location and for whether it accepts this file format.

**In any tool that reads a rules file.** Add `human-ai-tells.md` to whatever file or folder the tool treats as standing instructions, then ask it to check a piece of text. Names and locations vary by tool, so check yours.

## Where it has been tested

The author has used it in one environment only: Claude Code. It has not been tried in other chat tools, editors or skill systems. If you run it somewhere else, please report what worked and what did not at https://github.com/notes-from-anaicoo/human-ai-tells.

## Credits and licence

Released under the MIT licence (see `LICENSE`). Pattern ideas draw on Wikipedia's "Signs of AI writing" guide and on three MIT-licensed projects. Full credits are in `NOTICE.md`.
