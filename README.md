# tone-of-voice

A Claude Code skill for defining and enforcing a consistent brand voice across all content channels.

## What it does

Gives Claude a structured reference for your voice when writing blog posts, social media, emails, READMEs, and any other public-facing copy. Covers non-negotiables, writing rules, channel-specific guidelines, vocabulary tables, and examples — all in one file you own and control.

## Install

```bash
mkdir -p ~/.claude/skills/tone-of-voice
cp SKILL.md ~/.claude/skills/tone-of-voice/SKILL.md
```

## Customize

Edit `SKILL.md` and replace every `[PLACEHOLDER]` with your own details:

| Placeholder | What to fill in |
|-------------|-----------------|
| `[YOUR_NAME]` | Your name or brand name |
| `[YOUR_ROLE]` | What you do |
| `[YOUR_CORE_TOPICS]` | What you write about |
| `[YOUR_CENTRAL_THESIS_IN_ONE_SENTENCE]` | The belief that unifies your content |
| `[YOUR_AUDIENCE]` | Who you're writing for |
| Vocabulary table | Terms specific to your niche |
| Channel guidelines | Your actual platforms and CTAs |
| Examples | Real opening lines from your best content |

The structure is intentionally opinionated — contrarian, direct, anti-fluff. Keep it if it fits. Strip what doesn't.

## Use

Invoke the skill in any Claude Code session when writing content:

```
/tone-of-voice
```

Or reference it inline:

```
Write a Twitter thread about [topic] using my tone-of-voice skill.
```

Claude will apply your voice guidelines to the output.

## What's in the skill

- **Voice non-negotiables** — the 5-6 traits that define how you write
- **Writing rules** — openings, sentence structure, bolding, opinions
- **Banned phrases** — instant-delete list across all channels
- **Vocabulary tables** — preferred terms vs. rejected ones
- **Channel guidelines** — blog, social, email, README, community
- **Examples** — annotated templates for each content type

## License

MIT
