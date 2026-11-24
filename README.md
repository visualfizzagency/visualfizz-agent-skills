# VisualFizz Agent Skills

Three practical skills that make your AI coding agent work like a professional designer, copywriter, and video director — for designers and creators worldwide.

Free forever, MIT licensed. Built by [Md Ayub Mondol](https://mdayubmondol.com) / VisualFizz, a creative advertising and AI-video agency in Dhaka.

## The skills

| Skill | What it does |
|---|---|
| `premium-poster-design` | Premium social-media poster design: oversized stacked headlines, tight 2–3 color palettes, duotone grading, cutout portraits, sticker badges. One pattern per poster, type as hero, restraint as the rule. |
| `social-caption` | Simple, professional captions: short readable sentences, no engagement-bait, no fluff. English-first, with a colloquial Bangla variant included. |
| `cinematic-ai-video-prompt` | Story-built short AI videos: hook in the first 2 seconds, one message per scene, voiceover in English or Bangla, face-reference discipline, logo-only end card. |

## Standout feature: real Bangla support

Most design skills ignore non-Latin scripts entirely. These don't. `premium-poster-design` handles Bangla typography correctly — Hind Siliguri for mixed Bengali+Latin lines (Noto Bengali has no Latin glyphs and renders tofu boxes), conjunct checks, colloquial spoken Bangla — and `social-caption` and `cinematic-ai-video-prompt` both include Bangla variants. If your audience reads Bangla, these skills just work.

## Install

The skills follow the [Agent Skills open standard](https://agentskills.io) (`SKILL.md` with YAML frontmatter), so they work in Claude Code, Cursor, GitHub Copilot, Gemini CLI, Google Antigravity, OpenCode, and Codex.

**Easiest — one shared location, most tools read it:**

```bash
git clone https://github.com/visualfizzagency/visualfizz-agent-skills.git
cp -r skills/* ~/.agents/skills/
```

**Per agent:**

| Agent | Personal (global) | Per project |
|---|---|---|
| Claude Code | `~/.claude/skills/` | `.claude/skills/` |
| Cursor | `~/.cursor/skills/` | `.cursor/skills/` |
| GitHub Copilot | `~/.copilot/skills/` | `.github/skills/` |
| Gemini CLI | `~/.gemini/skills/` | `.gemini/skills/` |
| Google Antigravity | `~/.agents/skills/` | `.agents/skills/` |

Gemini CLI can also install directly from the repo:

```bash
gemini skills install https://github.com/visualfizzagency/visualfizz-agent-skills --path skills/premium-poster-design
```

## Usage

Just ask your agent in plain language. The skill loads automatically when relevant:

- "Design a poster for my free design course" → `premium-poster-design`
- "Write a caption for this reel" → `social-caption`
- "Write video prompts for a 30-second story about a tea stall at night" → `cinematic-ai-video-prompt`

In agents that support slash commands, you can also invoke a skill directly, e.g. `/premium-poster-design`.

## Example — before / after

**Without the skill**, a poster prompt comes out like this:

> "Make a nice poster for a graphic design course, colorful, with some icons."

**With `premium-poster-design`**, the agent asks for a reference, picks one pattern, and produces a real direction:

> Pattern: oversized condensed headline. Dark navy ground, duotone orange grade over the photo, extra-bold stacked headline "LEARN DESIGN / IN 30 DAYS", one accent — neon green pill CTA "Enroll free". 4:5 portrait, footer mdayubmondol.com. No rainbow, no stock gradient.

## Support

This bundle is free. If it saves you time, you can support the work here:

**https://www.supportkori.com/hellomdayub**

## License

MIT — see [LICENSE](LICENSE). Use it, remix it, ship it.
