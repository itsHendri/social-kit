# Social kit

A starting point for planning and writing your social posts with Claude Code, in your own voice.

Nothing in here is filled in for you. The first time you open it, Claude reads your website, asks you questions in short rounds, and writes your own files: how you sound, how you look, which channels you use and what works on each, and the skills it uses to plan your posts. Every answer comes from you.

Nothing posts on its own. Claude writes drafts and you post them yourself.

## What you need

- Claude Code (the terminal, or the Code tab in the Claude desktop app).
- Your website's address.
- Your logo files. Drop them into `assets/logo/` before you start, or when Claude asks.
- If you make videos with Remotion: where that project is on your computer.
- If you've posted before: the Claude in Chrome extension, and Chrome signed in to YouTube Studio, Meta Business Suite (for Instagram) and any other channel's analytics. Claude reads your numbers there to learn what has already worked: nothing to export. It only reads, and you do any signing in yourself. What it reads stays in this folder and out of git.
- About an hour for setup. You can stop at any point and carry on later.

## Start

Open Claude Code in any folder and paste this:

```text
Set me up with the social kit at https://github.com/itsHendri/social-kit. Ask me where to put it, clone it there, then read its CLAUDE.md and follow .claude/skills/setup/SKILL.md from the start.
```

Claude asks where the folder should go, clones it, and starts setup. It explains what it's going to do, then works through it with you. Next time, open Claude Code in that folder and carry on.

Already have the folder? Open Claude Code in it and say "set me up".

## What you end up with

```
brand.md               the basics: name, what it is, goals, timezone
identity/
  voice.md             how you sound, with examples you picked
  visual.md            colours, type, logo use, image and thumbnail style
  tokens.json          your colours and fonts as design tokens
assets/                your logo and other final files
channels/<platform>.md one per channel: how often, when, what works there
content/
  incoming/            drop new media here (a subfolder is one carousel)
  YYYY-MM/YYYY-MM-DD-<slug>/post.md   a planned post, with its media
audits/                what your past posts say works, one write-up per audit
data/                  the numbers the audit read, and any exports (stays out of git)
learnings.md           what worked and what didn't, from audits and reviews
.claude/skills/        your skills, written during setup
```

## Day to day

- Put new photos or videos in `content/incoming/`. Add a line to `content/incoming/notes.md` about what each one is, if it isn't obvious.
- Say "plan posts" (or whatever you named that skill during setup).
- Each post folder has a `post.md` with the caption for every channel, ready to copy. Post it, then tell Claude it's posted and give it the link.
- When you rewrite a draft, tell Claude why. It offers to add that to `voice.md`, so the next drafts are closer.

## Changing things later

Edit any file yourself, or ask Claude: "add TikTok as a channel", "redo my voice file", "make me a skill for X". The setup skill can run again for just one part.

The `kit/` folder is what setup works from. Leave it in place so setup can run again.

When the kit gets better, ask Claude to "pull kit updates". It runs `git pull kit main`, which brings in the new `kit/` files and leaves your own files alone. If a file you both changed clashes, Claude shows you both versions and you pick.
