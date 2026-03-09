# Dialogue Localization Engine

This module handles Phase 4 (dialogue localization). It performs **localization**, not translation. Every line must sound native and emotionally right in the target language.

---

## Core Rules

1. Preserve intent, power dynamic, and emotional temperature
2. Do NOT preserve sentence structure from Chinese
3. Replace dead literal jokes with target-culture-equivalent phrasing
4. Make lines speakable by actors in one breath
5. Shorten exposition unless the genre requires theatricality
6. Adapt insults, teasing, and flirtation by character type
7. Convert culture-specific phrases into functional equivalents
8. Keep recurring catchphrases only if they can become memorable in target language
9. Remove repetitive emotional labeling — let subtext carry the weight
10. Match dialogue register to character's age, class, and attitude
11. Distinguish dub-mode (shorter, cleaner) from subtitle-mode (slightly denser)
12. Never sound translated — if a native speaker would notice, rewrite

---

## Special Handling by Category

### Meme / Joke Adaptation
- Use equivalent social meaning, not literal wording
- Internet humor must map to target-culture internet humor
- If no equivalent exists, replace with character-appropriate humor that serves the same scene function

### Romance Banter
- Prioritize chemistry over semantic fidelity
- Flirting must land in the target language's register
- Adjust directness level for cultural norms (Chinese flirting is often more indirect)

### Power Dialogue
- Prioritize dominance / class / threat signal
- Corporate threats, family power plays, and status assertions must read as genuinely intimidating
- Avoid melodramatic phrasing that undercuts authority in English

### Comedy
- Prioritize timing and payoff
- Restructure setups if the original rhythm doesn't work in target language
- Physical comedy descriptions need less localization than verbal comedy

### Subtitle Mode
- Allow slightly denser lines than dub mode
- Reading speed constraint: ~15 characters per second
- Two-line maximum per subtitle card

### Dub Mode
- Lines must be shorter, cleaner, more actable
- Lip-sync considerations: match mouth movements where possible
- Avoid plosive-heavy translations over open-mouth frames

---

## Output Format Per Line

For each localized line, provide:

```markdown
**Source meaning:** [Chinese line or described intent]
**Literal translation:** [Direct translation showing what doesn't work]
**Localized line:** [The actual export-ready line]
**Why it works:** [1 sentence explaining the localization choice]
**Tone variants:**
- Sharp: [variant]
- Natural: [variant]
- Flirtier: [variant]
- Darker: [variant]
- Anime-coded: [variant]
```

Provide tone variants only when they add value. Not every line needs all 5 variants.

---

## Worked Examples

### Example 1 — Revenge / Threat

**Source meaning:** 你以为你赢了吗？这才刚刚开始。

**Literal translation:** You think you won? This has only just started.

**Localized options:**
- **Sharp / prestige:** "You really think this is over? You've just opened the door."
- **Dark revenge:** "Enjoy the moment. It's the last easy win you'll get."
- **Anime-coded:** "You're celebrating way too early. The real game hasn't even started."

### Example 2 — Flirty Banter

**Source meaning:** 你嘴这么硬，是不是怕喜欢上我？

**Literal translation:** Your mouth is so hard. Are you afraid of liking me?

**Localized options:**
- **Natural flirt:** "You always talk this tough when you're trying not to like someone?"
- **Sharper:** "That attitude of yours? Usually means I'm getting under your skin."
- **Playful:** "Careful. People usually get this defensive right before they catch feelings."

### Example 3 — Meme / Tease / Humiliation

**Source meaning:** 你这不是纯纯小丑吗？

**Literal translation:** Aren't you just purely a clown?

**Localized options:**
- **Internet-native:** "You're actually embarrassing yourself right now."
- **Crueler:** "This is getting pathetic."
- **Meme-coded:** "Wow. You really came here to humiliate yourself in HD."

---

## Quality Checklist

Before finalizing localized dialogue, verify:

- [ ] Would a native speaker say this without sounding translated?
- [ ] Does the line preserve intent rather than wording?
- [ ] Does the joke / taunt / flirt / threat land in target culture?
- [ ] Does the line match the character's age, class, and attitude?
- [ ] Is dub-mode dialogue short enough to perform naturally?
- [ ] Is subtitle-mode dialogue readable at target speed?
- [ ] Are repeated catchphrases memorable rather than awkward?
