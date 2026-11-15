# Blueprint: repurpose

For owners with long content: YouTube videos, talks, podcasts, blog posts. Finds the moments in one long piece that work on their own, and turns them into short posts for the owner's other channels. Setup writes it to `.claude/skills/<name>/SKILL.md`.

## What the skill must cover

1. Inputs: the long piece and its transcript, with timestamps for video or audio.
2. Read first: `brand.md`, `identity/voice.md`, the channel files, `learnings.md`.
3. Find five to ten moments that stand on their own. Kinds to look for:
   - a line worth quoting
   - a short story with a beginning and an end
   - one practical tip
   - an opinion people might argue with
   - a number or result
   - something behind the scenes
4. For each moment: the start and end time, the hook (a hook type from `voice.md`, filled with the moment's own detail), which channels it fits, and a caption per channel.
5. Show the list. The owner picks which to make.
6. For video clips:
   - Vertical (9:16) is the shape for Shorts, Reels and TikTok. A horizontal clip cropped to vertical usually does badly: reframe on the subject, or rebuild it as a vertical layout.
   - If the owner uses Remotion, make each clip a composition in their project, with captions and text kept inside each app's safe areas (the channel files say where). Check a few still frames before rendering the whole clip.
   - Copy finished renders into `content/incoming/`, so `plan-posts` puts them on the calendar.
7. For text posts and carousels, write them as drafts straight into `content/incoming/` with a line in `notes.md` saying where each came from.
8. Space clips from one piece over one or two weeks, not all on one day. `plan-posts` does the dates.

## Tailoring questions
- What long content do you have, and where is it?
- Which channels should short pieces go to?
- How do you cut clips today? (Remotion, an editing app, someone else.)
- Burned-in captions on every clip? In what style?
- How many short pieces from one long one, at most?
