---
name: tone-of-voice
description: Defines and enforces a personal brand voice, tone, and messaging guidelines. Use when writing any content — blog posts, social media, emails, landing pages, community posts, GitHub READMEs, or any public-facing copy. Ensures consistent personality across all channels. On first use, runs an interactive setup that saves your voice profile to memory.
---

# Tone of Voice

## Setup Check

Before doing anything else, check if voice profile memories exist:

1. Look for memory files matching `tone-of-voice-*.md` in the user's memory directory
2. If found: load them and proceed to **Enforcement Mode** below
3. If NOT found: run **Interactive Setup** first

---

## Interactive Setup (first use only)

Ask the user these questions one at a time. Use AskUserQuestion when choices help, or let them type freely when open-ended is better. Save each answer to a separate memory file.

### Question flow

**1. Identity**
Ask: "Who are you? Give me 2-3 sentences — your background, what you've built, and how you got here. No hype."

Save to memory: `tone-of-voice-identity.md`
```yaml
type: user
description: Brand voice profile — identity and background
```

**2. Core belief**
Ask: "What's the one belief that unifies everything you write? The thing you'd put on a billboard. Something slightly provocative."

Give examples to prime the pump:
- "Most founders are building for the wrong scorecard."
- "Distribution beats product every time."
- "The system rewards compliance, not competence."

Save to memory: `tone-of-voice-core-belief.md`

**3. Audience**
Ask: "Who do you write for? Not demographics — describe the person. What do they care about? What are they trying to do?"

Save to memory: `tone-of-voice-audience.md`

**4. Voice traits**
Ask: "Pick 3-5 words that describe how your writing should feel. Not what you write about — how it sounds."

Offer these as starting options (multi-select), with room for custom:
- Contrarian
- Direct
- Unapologetic
- Technical
- Warm
- Irreverent
- Precise
- Provocative

Save to memory: `tone-of-voice-traits.md`

**5. Topics**
Ask: "What are your 3-5 core topics? The things you always come back to."

Save to memory: `tone-of-voice-topics.md`

**6. Vocabulary**
Ask: "Give me 5-10 word pairs: words you use vs. words you'd never use. Format: 'use X, not Y'"

Example: "Use 'bootstrapped', not 'self-funded'. Use 'ship', not 'deploy'. Use 'customers', not 'users'."

Save to memory: `tone-of-voice-vocabulary.md`

**7. Banned phrases**
Ask: "What phrases make you cringe? Things you'd delete on sight."

Start with these defaults and let them add/remove:
- "We're excited to announce"
- "In this article, we'll explore"
- "Don't miss out!"
- "Let me know in the comments"
- "In today's [adjective] world"

Save to memory: `tone-of-voice-banned.md`

**8. Channels**
Ask: "Which channels do you write for? For each one, any specific rules?"

Common channels: Blog, Newsletter/Email, Twitter/X, LinkedIn, GitHub READMEs, Community (Discord/Slack)

Save to memory: `tone-of-voice-channels.md`

**9. Examples**
Ask: "Paste 1-3 paragraphs you've written that nail your voice. These become the reference standard."

Save to memory: `tone-of-voice-examples.md`

### After setup

Confirm: "Voice profile saved. I'll apply it whenever you invoke /tone-of-voice. You can update any part by saying 'update my tone-of-voice [section]'."

---

## Enforcement Mode (ongoing use)

When invoked on content (new or existing), apply the voice profile from memory:

### Writing rules (apply always)

**Open with a punch, not a windup.**
First sentence: a number, a bold claim, or a contrarian take. Never a definition. Never "have you ever wondered."

**Short sentences. Short paragraphs. Lots of air.**
One idea per paragraph. Under 20 words per sentence when possible. Tables for every comparison.

**Bold the scannable takeaways.**
1-2 bold phrases per paragraph, max. Bold the insight, not the setup. If someone reads only the bold phrases, they should get the core argument.

**Have an opinion and defend it.**
Don't write "X might have some drawbacks." Write "X is broken and here's why." The reader came for a take, not a Wikipedia article.

**Never apologize for being ambitious.**
No false modesty. No "I got lucky." Specific decisions, explained so others can replicate.

**Experience-first.**
"Here's what I did" beats "Here's what you should do." If you haven't done it yourself, say so.

**Anti-fluff.**
Every sentence earns its place or gets cut. No throat-clearing. No padding. If you can delete a paragraph and the piece improves, delete it.

### Enforcement checklist

When reviewing or writing content, check against the voice profile:

- [ ] Opening punches (no windup, no definitions)
- [ ] Voice traits match the saved profile
- [ ] Vocabulary uses preferred terms, avoids rejected terms
- [ ] No banned phrases anywhere
- [ ] Channel-specific rules applied (length, tone, format)
- [ ] Bold phrases carry the argument for scanners
- [ ] Examples feel consistent with the saved reference samples
- [ ] Every sentence earns its place

### Updating the profile

If the user says "update my tone-of-voice [section]":
1. Read the relevant memory file
2. Show the current content
3. Ask what they want to change
4. Update the memory file

If the user says "show my tone-of-voice":
1. Read all `tone-of-voice-*.md` memory files
2. Display a formatted summary of their voice profile
