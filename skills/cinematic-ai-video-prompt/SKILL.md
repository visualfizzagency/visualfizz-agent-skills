---
name: cinematic-ai-video-prompt
description: Write generation prompts for story-built short AI videos (reels, Shorts, TikTok) — hook-first scenes, one message per scene, voiceover lines in English or Bangla inside the prompt, face-reference discipline, and a clean logo-only end card. Use when the user asks for a video prompt, a video concept, a storyboard, or a voiceover script for an AI-generated short video.
license: MIT
metadata:
  author: Md Ayub Mondol / VisualFizz
  language: English
---

# Cinematic AI Video Prompt

Every video is story-built: a small human story with a hook, not a mechanics lecture and not an ad description. One message per scene. The viewer should feel something in the first 2 seconds.

## When to use this skill

- Writing prompts for AI video generation (Veo, Flow, Gemini, or similar) for 9:16 reels, Shorts or TikTok.
- Planning a story video, a product promo, or a tool explainer video.
- Writing voiceover lines that go inside generation prompts.

## Structure of a video

1. **Hook (first 2 seconds).** The most surprising or emotional beat first. The viewer decides in 2 seconds whether to stay.
2. **Story beats, one message per scene.** Each scene carries exactly one idea. If a scene needs two ideas, split it.
3. **End card, 3-4 seconds only.** Logo reveal + services, nothing else. Never a long outro.

## Writing a generation prompt

Every clip prompt follows the same shape:

```
[Camera + framing, e.g. "Vertical 9:16, medium close-up, slow push-in"]
[Setting + light, e.g. "a Dhaka tea stall at night, warm tungsten light, light rain"]
[Character + action, e.g. "a man in his 30s in a light panjabi watches the small TV, then smiles"]
[The spoken line — see voiceover rules below]
[Language lock — see voiceover rules below]
```

- **Say the duration only if the tool respects it.** Many generators ignore durations — write the scene so it works at 5-10 seconds either way.
- **No subtitles, no on-screen text, no watermark** in the story scenes unless the concept explicitly needs a title card.
- **No dead or empty panel space.** Every frame should be full: subject, environment, light.
- **Never claim what the tool cannot do.** If the tool cannot hold a face, do not write the prompt as if it can.

## Voiceover rules

**Language is a choice, made once per video:**

- **English (default).** Write the spoken line in English and end the prompt with: `Spoken audio in English only.`
- **Bangla (option).** Write the line in Bangla script and end the prompt with: `Spoken audio in Bangla only — no English.`

Whichever language is chosen, these rules apply:

- **One line per clip.** If a line is long, split the clip — never cram two lines into one generation.
- **Voiceover first, animation second.** For coded/motion-graphics videos: make the voiceover first, then time the animation to the voice (word-level timing). Never animation-first.
- **Continuous narration** — no gaps between lines; visuals change UNDER the narration.
- **Bangla voiceover, when chosen, is formal Bangla, আপনি-form. Never তুমি-form.**

Example of a clip prompt (English voiceover):

```
Vertical 9:16, medium shot. A man in his 30s in a light panjabi sits at a
Dhaka tea stall at night, watching a small TV as the last over plays.
The lights go out. He looks up, then smiles at his neighbours.
He says: "You don't wait for the power to watch the match — the whole
neighbourhood is enough."
Spoken audio in English only.
```

Same beat, Bangla voiceover option:

```
He says in Bangla: "ম্যাচ দেখতে কারেন্টের অপেক্ষা করতে হয় না — পাড়াটাই যথেষ্ট।"
Spoken audio in Bangla only — no English.
```

## Face-reference discipline

- **When the user gives an identity photo, that face belongs on the main character.** Use the exact reference file the user provided (a suited portrait photo), never a different photo of the same person.
- **Verify the reference is attached and its preview is visible BEFORE the first Generate click.** If the upload fails or shows no preview, stop — never generate a faceless fallback and never substitute a text-description lookalike.
- **Two-man shots for dialogue.** When a second character speaks, write the clip as a two-man shot with the main character visible in frame. A pilot-only or single-character close-up can pull the reference face onto the wrong character.
- **Female slots stay generic models.** Only male-model slots use the user's face.
- **Likeness is ~50-60% at best** with current video tools. Say so honestly; never promise an exact match.
- **Never place the user in a female product's ad**, and never use the user's face for news-presenter videos — news videos use an AI character/presenter instead.

## End card

- Logo reveal + services only, 3-4 seconds maximum.
- No extra text, no new information, no second CTA.

## What NOT to do

- Mechanics lectures ("first click here, then click there") — tell the story, show the benefit.
- More than one message per scene.
- তুমি-form in any Bangla voiceover line.
- Mixed-language voiceover in one video — pick English or Bangla and commit.
- Generating without a verified face reference when the concept needs the user's face.
- Subtitles baked into story scenes.
- An end card longer than 4 seconds.
