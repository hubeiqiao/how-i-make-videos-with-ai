# The Skills

A Skill is a folder of instructions your assistant reads before it works. It is not an app and it does not render by itself; it tells Claude Code or Codex how to make the video with you.

## Start here: make-a-video

`make-a-video` is the method from How I Make Videos With AI, written for your assistant. Open a folder with your own photos, clips or recordings and say what you want, for example:

> Use the make-a-video Skill. Make a 30-second video from the files in this folder. It is for [who will watch].

It sets up everything it needs the first time (the folders and a small Remotion project), asks you a few questions, and renders a complete first draft. Then you give numbered notes, it fixes one section at a time, and at the end it offers to save how you made it as your own Skill.

## Examples: Skills I saved from my own videos

Each of these was written the way step 5 describes: after a video was approved, the assistant turned my notes and the drafts I rejected into rules. Read one to see what a saved Skill looks like, or use it if your job is the same.

| Job | Skill | Built from |
| --- | --- | --- |
| A film using real work | evidence-led-film | My Stripe film (September 2026) |
| A recording into a finished episode | joe-speaking-video | The interview episodes for my app, Joe Speaking |
| A finished episode into a short | ai-candidate-growth-short | My AI Candidate series: EP04 to EP11 were each accepted on the first render |
| A talk at an event into a published cut | joe-speaking-talk-cut | My live demo at Shopify Builder Sundays (September 2026) |
| An app release into a short preview | joe-speaking-release-preview-video | The Joe Speaking v0.9.3 and v0.9.4 release previews |
| A screen recording into an in-app feature video | joe-speaking-feature-in-app-video | 17 Joe Speaking feature demos, then the Advanced examiner film |

They do not include my private projects, recordings or branding. Where a Skill names my app or videos, it shows where a rule came from; use your own.

## Install

In Claude Code or any assistant that supports Skills:

    npx skills add hubeiqiao/how-i-make-videos-with-ai

Or copy the `skills` folder into your project and say: "Read skills/make-a-video/SKILL.md and use it."

For better Remotion code, also add the official Remotion Skill (https://www.remotion.dev/docs/ai/skills):

    npx skills add remotion-dev/skills
