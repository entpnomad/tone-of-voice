# tone-of-voice

A Claude Code skill that learns your voice — personal or brand, because sometimes the founder's voice *is* the brand — and enforces it across everything you write.

## Why

As a founder, I write most of the communication in my company — newsletters, landing pages, emails, social posts, READMEs. And yes, I unapologetically use AI. The ideas are mine. I dictate the core thinking using [Whispering](https://github.com/braden-w/whispering) on Mac, then have Claude write the draft. But AI without guardrails produces slop. Same structure, same phrasing, same lifeless corporate tone every time. This skill fixes that. It teaches Claude how I sound — my vocabulary, my opinions, my banned phrases — so the output reads like me, not a press release.

## How it works

First time you run `/tone-of-voice`, it asks 9 questions: who you are, your core belief, your audience, voice traits, vocabulary preferences, banned phrases, channels, and example writing. Answers are saved to Claude Code's memory system — persistent across sessions.

Every time after that, it applies your voice profile to whatever you're writing.

## Install

```bash
mkdir -p ~/.claude/skills/tone-of-voice
curl -sL https://raw.githubusercontent.com/entpnomad/tone-of-voice/main/SKILL.md \
  -o ~/.claude/skills/tone-of-voice/SKILL.md
```

## Use

```
/tone-of-voice
```

First run: interactive setup (~5 minutes). Subsequent runs: enforcement mode.

### Commands

| Command | What it does |
|---------|-------------|
| `/tone-of-voice` | Apply voice to current content or start setup |
| `update my tone-of-voice vocabulary` | Edit a specific section |
| `show my tone-of-voice` | Display your full voice profile |

## What it saves

Nine memory files covering your identity, beliefs, audience, traits, topics, vocabulary, banned phrases, channel rules, and reference examples. All stored in Claude Code's memory directory — you own the data.

## License

MIT
