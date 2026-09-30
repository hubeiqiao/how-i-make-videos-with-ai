# Audio and efficient rendering

## Narration

Inventory takes by source, in/out, exact words, clarity, energy, and neighboring phrase. Select complete takes by listening when tools permit. Do not claim a take is best based only on transcript or loudness measurements.

Normalize perceived loudness and tonal consistency across sections, not just peaks. Adjust clip gain before light compression/EQ where needed. Preserve natural breath and consonants. Crossfades belong in compatible pauses or room tone, not over words. Listen to joins in context. Preserve isolated voice, music, and effects stems.

Do not prescribe universal loudness targets irrespective of destination. Measure integrated/short-term loudness and true peaks, choose delivery-appropriate targets, then listen on representative speakers/headphones. Lower the bed around speech as needed without obvious pumping.

## Music and effects

Choose music for the emotional arc, not merely a genre label. Audition against narration. For Joe's optimistic application-film tone: immediate invitation, forward pulse, growing possibility, and a bright release rather than tragic or military grandeur.

Create an audio cue sheet: opening gesture, chapter seam, result reveal, key word, final release. Align edits to musical phrases as well as visual beats. Avoid restarting the track at every chapter. A transition tail may bridge a cut; an abrupt change of energy may need a deliberate setup.

Use effects selectively: small contact, light sweep, spatial acceleration, brief celebration, or tonal resolution. Avoid whooshes on every movement and loud effects masking speech. Do not force synthesis or external music search if accepted audio already solves the task. Record source and usage terms for new third-party audio without turning this into an unrelated audit.

## Render dependency discipline

Record source project, composition, FPS, frame range convention, dependencies, and output profile before running commands. Derive bounds from actual timing and inspect whether the renderer uses inclusive or exclusive end frames.

For a local edit render its affected range with enough handles to hear/see entry and exit. For sound edits, audition an audio-only range first if that saves time. For an asset replacement update only used source ranges, then recomposite consumers.

Concat without re-encoding only when stream parameters and cut boundaries actually permit it. Otherwise encode affected boundaries or the delivery composition appropriately. Avoid repeated lossy generations. Preserve approved masters, original assets, and reproducible render commands.

## Diagnose apparent stutter

Separate source animation holds, duplicate/missing frames, FPS conversion cadence, render timing, decoding load, and browser playback. Inspect source and export metadata; examine motion intervals, not just the still opening frame. Compare local playback with the embedded player when possible. A nominal 60 FPS file alone does not prove smooth movement. Do not apply frame interpolation by default or change deliberate timing to hide a decoding problem.

## Final checks

- Full final phrase and natural audio tail, no word cut to meet composition duration.
- Similar perceived voice across chapter joins, music supporting rather than competing.
- No stale image/number at transitions, missing media, off-by-one flashes, logo doubles.
- Correct media dimensions, duration, frame cadence, audio streams and seek behavior.
- Normal-speed review plus targeted seam inspection; phone-size readability.

Document what was actually heard, watched, and measured. Never equate successful encoding with a creatively accepted film.
