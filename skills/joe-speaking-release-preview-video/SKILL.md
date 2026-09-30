---
name: joe-speaking-release-preview-video
description: Use when making the short preview video that goes with an app release post, showing each user-visible change in the real app inside a real phone frame.
---

# Release preview video

This is a portable teaching adaptation, not Joe's installed project. It was built from the release previews for his app, Joe Speaking: v0.9.3 and v0.9.4, each with a cut for X and a cut for RedNote. Each rule came from a draft Joe rejected.

## Read first
Read [workflow.md](references/workflow.md) and the [input brief](examples/input-brief.md). Ask only for decisions that change the video.

## Inputs
release notes / a test account with real data / [your phone frame image] / an instrumental track / [your ending card] / languages and sizes.

Output: a 20 to 30 s video with a short hook, at most three scenes (one change each, one first-person voice line each) and your standard ending. v0.9.3 had an English 16:9 cut for X and a Chinese 3:4 cut for RedNote; v0.9.4 used 3:4 for both. This folder is instructions, not a renderer: build or adapt a Remotion project.

## Work in visible stages
1. Pick the changes and write the lines. No recording yet.
2. Record the takes, then build the draft.
3. Before showing it, check: every voice line transcribed from the final mix and matched to the script; stills of frame 0, every ring, every zoom and the ending; -14 LUFS from one constant gain; no lurch or frozen run in a frame-difference scan.
4. Deliver both cuts with the copy. Leave tone and name pronunciation to a human ear.

## Rules, and why
- **Real content only:** screen recordings, not screenshots, of the release on a test account with real data. Never fabricate UI or numbers.
- **Record only the page, read-only.** An early capture caught private windows, so bracket each take with a full-screen marker colour and discard anything outside it. Never click destructive controls.
- **The hook is pure motion and does not explain the feature,** fully painted at frame 0, with no voice. A result hook and a question hook were both rejected.
- **Measure every highlight ring on the recording's pixels.** Positions logged during capture were 12 to 20 px off.
- **Hold, then glide.** In v0.9.4, eased-out moves lurched and froze, and a continuous drift felt slow. Joe wanted a hold, then one quick glide on the beat.
- **Duck the music a few dB and cut the voice's band from it, rather than dropping it away.** In v0.9.4, a 12 dB duck made it vanish and pump between lines.

The workflow holds the rest: no scrolling, a real phone frame, instrumental music, one voice.

## Example invocation
Read the release notes in notes/brief.md. Use this Skill to pick at most three user-visible changes, write one first-person line for each and plan the recordings. Do not record yet.

## Done means
Both cuts, the copy (each section naming its video file) and the production notes sit together, drafts are removed and sources are kept for a re-render. Publishing is a separate action.
