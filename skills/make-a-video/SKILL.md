---
name: make-a-video
description: "Make a finished video from someone's own photos, clips, screen recordings or voice, by writing it as code with Remotion and rendering drafts they react to. It follows the five steps of 'How I Make Videos With AI': know what you want, get the whole draft once, fix one section at a time, listen at every join, finish where people see it and save a Skill. Use when a user wants to make, cut or edit a video from their files, especially someone who has never used an editing app."
---

# Make a video from your files

The user decides; you build. They choose the goal, the material, what is wrong, what stays and when it is done. You write the video as code (Remotion), render drafts, and apply their notes exactly. They never touch a timeline or the code.

Speak plainly. Give a clickable link to every render. Keep every version. Never change, rename or delete their original files. Never publish anything.

## 0. The first time in a folder

- Work in the folder the user opened. Their files go in `originals/`: offer to move them there, and if they would rather not, read them where they are.
- Create `notes/`, `working/` and `exports/`.
- Check that Node.js 18 or newer is installed. If it is missing, guide them through installing it, one step at a time.
- Set up a Remotion project in `working/`. If the official `remotion-best-practices` Skill is installed, follow it.
- Prove the setup with a two-second test render made from one of their own photos, and link it. If anything fails, explain it in plain words and fix it before going on.

## 1. Know what you want. Then gather the files.

Ask, in one short message, only what they have not told you yet:
- who will watch;
- what the viewer should believe afterwards, in one sentence;
- what the viewer should do next;
- where it will be posted, about how long, and what shape (16:9 or vertical).

Then open every file in `originals/`. Write `notes/outline.md`: 6 to 10 sections, each pointing to the file that shows or proves it. Flag any claim with no file behind it, and ask them for one (a screen recording, a photo they can take) rather than inventing it. Do not write scenes or render yet.

Done when every part of the outline points to a real file.

## 2. Get the whole draft once. Then react.

If the video has a voice, write the narration first, as natural spoken words, about two words per second of video. Write `notes/beats.csv`: one row per phrase, with the words, the file on screen (or "missing: needs a screen recording or a photo"), the text on screen and how things move. Stop so they can approve the words and the storyboard.

Then build the complete first draft: every section, timed to the voice, each section its own editable scene. Ease every movement. Carry something across from one scene to the next rather than a hard cut, unless the story needs the cut. Do not polish only the opening. Render a quick lower-resolution preview to `working/out/draft-v1-preview.mp4` and link it.

Before you show it, check your own work: length against the target; every phrase has a picture or is marked missing; stills at the key moments in one contact sheet; no text cut off or overlapping; voice loudness.

Done when a playable video exists from the first word to the last.

## 3. Point at the problem. Fix one section at a time.

A useful note has four parts: where (a time or a section), what is wrong, what they want, and what must stay. Number their notes. If a note is missing a part, ask for it before you change anything.

Fix only the section they name. Export it with one second of each neighbour, to `working/out/<section>-v2.mp4`, and keep the earlier version.

When they approve a section, record its file in `notes/accepted.md` and its rules in `notes/style.md`: at most three colours, one pair of fonts, one kind of background, one kind of music. Every later section follows that style. Never touch an approved section again.

Before you show a change, list each of their notes as done or not, and repeat the checks from step 2.

Done when every section has an approved file and they have nothing left to say.

## 4. Put it together. Listen at every join.

Join the approved versions from `notes/accepted.md` into `working/out/full-review-v1.mp4`. Match voice loudness across sections. List every join with its time. Render stills just before and just after each join into one contact sheet, and look for an old frame that flashes at a cut. For any join they flag, fix only that boundary and export under a new name.

For music, ask for the feel in three words and for tracks they have the right to use. Lower it under speech, shape it to the story, and use sound effects rarely. Save the plan to `notes/music-cues.csv`.

Done when they can watch it end to end without wincing once.

## 5. Finish where people see it. Then save it as a Skill.

Put the approved film in `exports/`: `final.mp4`, a cover image taken from the film, and the post copy. Measure and report the duration, resolution and sound, and check that the final second ends cleanly. Ask them to watch it on their phone, where people will see it. Save `notes/recipe.md` with what worked, the approved files and the prompts.

Then offer to save how you made it as a Skill for their next video of this kind. Read the whole history: their notes, the drafts they rejected and why, and the one they approved. Write `skills/<kind-of-video>/SKILL.md` with when to use it; what goes in and what comes out; the steps in order; their rules, each taken from a note they gave or a draft they rejected, with the reason; the files and settings to reuse; and the checks to run before showing a draft. Keep it short. Do not add rules they never gave. Show it to them before you save it.

Done when the post preview looks right and the Skill is saved.
