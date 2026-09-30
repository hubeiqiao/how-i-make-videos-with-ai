# Release preview video
Portable teaching adaptation of Joe's joe-speaking-release-preview-video workflow. Not the original project, its scripts or its brand assets.

Inputs: release notes, a test account with real data, your phone frame image, an instrumental track, your ending card.
1. Story first. Pick at most three user-visible changes from the release notes, one per scene. Write one short first-person line for each from a real user's point of view (about 4.5 s at most), then a closing call to action. Keep the plan in a production notes file.
2. Record. Script each take: clicks, waits for loads, no scrolling (recorded smooth scrolling juddered). Hide development banners and assistant overlays first; a stray cursor and glow once reached a take. Start and end each take on a full-screen marker colour, keep only what lies between, and delete the raw capture. v0.9.4 recorded the page alone in a headless browser.
3. Frame. Put each take in the real phone frame image, cast its shadow from the image's own alpha, and render video at its final size (scaled-up elements came out blurry).
4. Hook. About 2.5 s of motion built from real frames of the takes and the version number. Keep any beat pulse subtle; a stronger one read as shaky. Joe's is a tunnel of real app frames around the version number, which shatters on the second kick.
5. Camera. Hold, glide for about 15 frames on the beat, settle. One phone stays on screen and its screen swaps mid-glide, so there are no hard cuts. Keep each screen short: v0.9.4 cut its longest from 8 s to 5.5 s. On a phone, show a touch, not a mouse arrow.
6. Rings. Measure each target on the recording at several times; identical boxes prove it did not move.
7. Music. Transcribe every new track first: lyrics come out as sentences, an instrumental as nothing or a stock phrase. Start the track at its drop.
8. Voice. One TTS model and one voice for the whole track, because two models differ audibly in timbre and pacing. Place each line from its measured length and refuse any line that overruns its scene. v0.9.4 ducked the music about 5 dB under speech, not 12, and cut the voice's frequency band from the track. If the music masks a word, move the line off the kick; 0.25 s fixed one.
9. Balance to -14 LUFS with one constant gain, not a dynamic normalizer.
10. Copy: one file per release, an X section and a RedNote section, each naming its video file. On RedNote: the core keyword in the title and in the body's first 50 characters, the changes numbered, 5 to 10 tags with your own first, and no links; its cut ends without a URL.
11. Hand over finished, verified videos, not commands or unchecked drafts. The release folder keeps only the finals, the copy, the voice lines and the notes. Keep videos out of your app's code repository.
