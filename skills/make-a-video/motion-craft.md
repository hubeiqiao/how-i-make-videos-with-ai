# Motion craft

Read this when a section has animated text, UI, charts or graphics, or when the user says the motion feels cheap, stiff or "like a template". These rules make motion feel designed. They never override the user's notes or `notes/style.md`.

Credit: the brief structure, springs, beat grid, subframe blur and gotchas below are adapted from @twoclipping's open prompt template for Opus 5.5 motion design (x.com/twoclipping/status/2103273003555402193).

## Brief it in tagged parts

When you plan a motion-heavy section, write its brief in `notes/` with these parts, and show it before you build:

- `<inputs>`: what you still need from the user (states, colours, the song). Ask; never invent.
- `<direction>`: the look in a few lines, and a **banned list**. Without one, a model falls back to its defaults: a centred title on a gradient, everything fading in together.
- `<structure>`: the beats in order, at the song's tempo, something happening on every beat.
- `<build>`: how it renders.
- `<gotchas>`: what usually breaks.

Show the state list laid on the beat grid before you write code.

## Rules

1. **Every value is a function of the frame.** In Remotion, compute position, size, radius and colour from `useCurrentFrame()`. No CSS transitions, no timers, no state carried between frames.
2. **Springs, not linear moves.** Use Remotion's `spring()`. A tiny overshoot at most; no bouncy easing. When a value changes target several times, add one spring per change rather than restarting, so the motion stays continuous.
3. **Stagger, don't sync.** The subject moves first; the camera, shadow and text follow a few frames later. Edges of a moving indicator can ride two springs so the leading edge stretches ahead.
4. **One element can carry the story.** Morphing one shape from state to state (size, radius, colour) reads as more designed than cutting between separate cards.
5. **Lock to the beat.** Measure the song's beat grid (for example with numpy) and start on a downbeat. Put big changes on beats and place each sound effect by its measured peak, not the start of the file.
6. **Motion blur on fast moves.** Use `@remotion/motion-blur` (CameraMotionBlur, about 4 to 5 samples) for fast moves only.
7. **Check one frame per beat before the full render.** Render stills on the beats into a contact sheet and fix anything off the grid, cramped or hard to read first.

## Gotchas

- Don't put `will-change` on anything the camera scales, or text renders blurry.
- Text that swaps inside a morphing container needs its own enter and exit timing, or old and new text overlap.
- For a loop, make the last frame identical to the first, including any cursor's position and speed.

## Keep the user's footage first

These rules polish graphics around the user's real material. They never replace a photo, clip or recording with a drawn imitation, and the user's notes always win.
