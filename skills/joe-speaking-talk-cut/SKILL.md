---
name: joe-speaking-talk-cut
description: Use when cutting a recording of your own talk or demo at an event into a published video with a cover hook, captions, cards, feed covers and copy in your own voice.
---

# Talk recording to published cut

This is a portable teaching adaptation, not Joe's installed project. It was built from a real talk cut: Joe's live demo of his app at Shopify Builder Sundays (September 2026), filmed from the back of the room and reviewed over five rounds. Each rule came from one of his corrections.

## Read first
Read [workflow.md](references/workflow.md) and the [input brief](examples/input-brief.md). Ask only for decisions that change the edit.

## Inputs
stage recording / speaker photos / product screens / the speaker's post draft / destinations.

This folder is instructions, not a renderer: build or adapt a Remotion or FFmpeg project. Keep the original unchanged.

## Work in visible stages
1. Propose what to keep, with source timestamps, and the frame 0 cover. No render yet.
2. Build the draft, previewing only the changed part (the hook, the ending) until it is approved.
3. Before showing a draft, check loudness (about -14 LUFS, true peak at most -1 dBTP), music only under the opening and closing, every frame of the hook and transitions, and the first word and any restored line, transcribed from the final file.
4. After approval: the full render, any Chinese version (a Chinese line under each English caption), the covers, the copy.

## Rules, and why
- **Frame 0 is the cover,** because it becomes the thumbnail: the speaker's cut-out with eyes open, the product on a phone, the claim in the speaker's words.
- **The hook is one continuous camera move of about 3 s** into the product on the phone, which opens like a lens onto the talk. Joe rejected slammed type, jumpy whips, a bridging shot and a double exposure.
- **Never cut a spoken line.** Restore a truncated sentence from the audio. Words the speaker remembers but never said go in the copy only.
- **Keep the live demo whole,** pauses included. Drop the host set-up, Q&A, failed attempts and waits.
- **The closing music must carry energy.** A soft ending felt bleak.
- **Change the least.** Find the one thing a note means before redesigning.
- **Keep designed text honest:** the product tier, never the model behind it; no release date on screen; "uncut" only where literally true.
- **The copy is the speaker's own draft with the English fixed:** no softened claims, no added stats or selling lines.

## Example invocation
Read my talk recording and notes/brief.md. Propose what to keep, with source timestamps, and a frame 0 cover. Do not render yet.

## Done means
The speaker has watched and approved the export, each platform has a cover made for its crop, and only the latest HD render is kept. Publishing is a separate action.
