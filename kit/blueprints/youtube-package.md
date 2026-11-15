# Blueprint: YouTube package

For owners who make long YouTube videos. For each video, writes the title, description, chapters and pinned comment, and makes the thumbnail. Setup writes it to `.claude/skills/<name>/SKILL.md`.

## What the skill must cover

1. Inputs: the video (or a link to it), a transcript or captions file if there is one, and the owner's notes on what it's about. If there is no transcript, ask for the main points and rough timestamps, or suggest exporting captions from YouTube Studio or the editing app.
2. Read first: `brand.md`, `identity/voice.md`, `identity/visual.md`, `channels/youtube.md`, `learnings.md`.
3. Title: write four to six options in different shapes (a plain description, a question, a result, a choice). Put the point in the first words, since long titles get cut off. Stay under the limit in `channels/youtube.md`. The owner picks one or edits.
4. Description:
   - The first two lines say what the video is and who it's for, because that's all that shows before "more".
   - Then the links the owner always includes, in their usual order.
   - Then the chapters.
5. Chapters, from the transcript or the owner's timestamps. The first one starts at 0:00. YouTube needs at least three, each at least 10 seconds long. Name each one for what happens in it, not "Part 2".
6. Pinned comment: a question or a next step, in the owner's voice, that isn't engagement bait.
7. Thumbnail:
   - Read the thumbnail section of `visual.md`. Sketch three or four clearly different ideas first, as quick drafts the owner can compare (different ideas, not the same layout in new colours). The owner picks.
   - Make the pick at 1280×720 (16:9) with the brand's tokens, fonts and logo from `assets/`.
   - If the owner uses Remotion, make it a still composition in their project, so it can be changed and remade. Render with `npx remotion still <composition-id> <out.png>`.
   - Check it at the size people see it: shrink it to about 320 pixels wide. If the words can't be read, cut words or make them bigger.
   - Check YouTube's current file size and format limits before exporting.
8. Write it all into the post folder: `post.md` for the text, the thumbnail in `media/`.

## Tailoring questions
- What do your titles usually look like? Show two or three you liked.
- What goes in every description (links, socials, gear, a newsletter)?
- Thumbnails: face or no face? How many words at most? Two or three you like, yours or anyone's.
- Do you have transcripts or captions files, and where do they live?
- Do you want a pinned comment on every video?
- Do you make the thumbnails in Remotion, or elsewhere?
