# Design and motion decisions

## Meaning and composition

Give each shot one primary reading and secondary evidence. Dense environments can express scope, but foreground content must remain distinguishable. Select assets for what they communicate, not to fill a count. Avoid repeated photos assigned to unrelated labels.

A semantic emphasis changes the scene: “unlock” can reveal the receipt and result; “ambitious” can expand perceived space; a role introduction can clear the previous scene and establish a new focus. A larger word alone may not supply meaning. Keep emphasis readable long enough to register.

For original-layout reuse, preserve typography, copy, proportions, and identity. Animate focus within it through staged reveals, underlines, grouping, or a controlled camera move. Do not leave the text inert while only its avatar moves.

## Physical continuity

Use deterministic frame-based motion in video renders. Avoid wall-clock randomness or unstable per-frame spring initialization. Mass and damping are decisions about the element's role; not everything needs overshoot.

During holds, use a small coordinated response, slow environmental movement, or gentle breathing where useful. Do not combine several oscillations on the same subject: this produces jitter. Reading areas can remain still while the surrounding scene stays alive.

For a transition, specify outgoing and incoming velocity, direction, scale, and focus. When productivity becomes ambition, choose a dominant transformation rather than simultaneously crossfading words, expanding the camera, spinning frames, and revealing a new background.

Parent labels and connecting lines to the same transform or compute endpoints from the same animated coordinates. Anchors must align on their first visible frame, not only after settling.

## Magic Move contract

Track the moving element's identity, start/end rectangles, crop, background, opacity, stacking order, and timing. Prefer one continuously rendered element. When a source/destination swap is required, align their geometry before swapping and avoid a frame with both or neither visible.

Example: avatar flying into a QR badge. Its circular background can disappear during the flight; the endpoint must match the badge's transparent avatar, size, aspect, and location. The destination must not appear underneath early and create a flash. Keep the QR scan area stable after settling.

Audit start, midpoint, arrival, and several frames around the handoff. Confirm at normal speed. Abrupt camera changes can still feel wrong even if endpoints match.

## Hook and ending

The opening quickly establishes identity and purpose with a legible composition and an intentional sound gesture. Do not rely on a tiny logo or long atmospheric lead-in.

The ending has anticipation, release, and readable rest. Synchronize the emotional change to the actual recorded phrase; never truncate the recording to fit animation. Hold contact/QR information for a useful duration, chosen for the delivery format, with restrained life. Do not invent an unrelated walk-away shot, duplicate logos, or new slogans.

## Lessons grounded in the Stripe revisions

- Carleton: institution → outreach → email/result → coursework, not a static proof collage.
- Ambitious: preserve the accepted spatial entrance and framing when changing its background.
- FDA: role, supporting labels, and lines form one connected system.
- Ending: matching pixels and backgrounds matters as much as trajectory.
- Original founder layout: animate the existing right-hand content as well as the avatar.

These examples explain decisions; their names, figures, and branding are not defaults for new films.
