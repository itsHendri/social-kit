# Blueprint: your own skill

For anything the owner does by hand, again and again, that Claude could do or prepare. For example: a newsletter from the month's posts, captions for a photo dump, replies to common questions, a monthly content idea list, a podcast show-notes page.

## Questions to ask
- What's the task, in one sentence?
- When do you do it, and what do you say when you want it done? (These words become the skill's description.)
- What goes in: files, links, notes, a video?
- What comes out, and where should it be saved?
- What makes it good? Show one you were happy with, if there is one.
- What must it never do?

## What to write
`.claude/skills/<kebab-name>/SKILL.md` with:
- Frontmatter: `name`, and a `description` saying what it does and when to use it, in the owner's words.
- What to read first: always `brand.md` and `identity/voice.md`, plus what this task needs.
- The steps, numbered, each one something Claude can do or check.
- Where the result goes, and what to show the owner at the end.
- What it must never do (the owner's answer, plus: never post, send or publish anything).

Then run it once with the owner on a real example, and fix the skill from what they say.
