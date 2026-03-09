# mandrama-export-adaptation

Turn China-first web dramas and manhua dramas into export-ready international packages.

This is a skill for **adaptation strategy**, not literal translation. It helps decide:
- which market to target first
- which language package to lead with
- how much of the source logic must be rewritten
- which format best fits the story and production reality

It is currently optimized for **US/UK/Europe-facing export work**, but it is **not locked to English or Japanese**. Spanish, Portuguese, Arabic, French, German, Korean, and other primary language packages are valid when the market logic supports them.

## Why this exists

Most Chinese short dramas and manhua adaptations do not fail overseas because the core emotional engine is weak. They fail because the export package is wrong:
- the social logic is too local
- the dialogue sounds translated
- the release language does not match the monetization plan
- the visual format fights the story tone

This skill gives you a repeatable way to fix that.

## What it does

- **Route the project** into Anglophone, performance-led subculture, region-first localized, or multilingual release strategies
- **Rewrite culture friction** so plot logic survives outside Chinese context
- **Localize dialogue** into native-sounding performance language
- **Choose format** across 2D, anime-style, 3D MetaHuman, or hybrid
- **Package the project** with loglines, hooks, titles, risk notes, and next-step production guidance

## Quick Example

### Input

```text
Adapt this revenge romance short drama for overseas YouTube.

Source:
- A wealthy heiress is framed by her fiance and cousin
- She enters a fake marriage with a cold CEO to take back her company
- Tone: high melodrama, humiliation/comeback, luxury revenge

Goal:
- Find the best first export market
- Recommend language strategy
- Recommend whether this should be 2D, anime-style, or 3D
```

### Output shape

```text
Verdict: Anglophone premium export
Confidence: Medium-High
Best market: US / UK short-drama and YouTube audiences
Core reason: The premise travels well because betrayal, humiliation, and comeback are universal hooks. The sponsorable version works better in English-led packaging than subtitle-first release, but the social logic around inheritance and fake marriage needs rewriting for export clarity.

Recommended option: English-led launch with globally legible naming and prestige-melodrama positioning
Second-best option: Spanish-led LATAM test if distribution partner or dubbing advantage exists
Reject for now: Japanese-performance route because the material is luxury revenge, not fandom-native stylized romance
```

See full sample outputs in [examples/](C:/Users/david/Desktop/mandrama-export-adaptation/examples).

## Best For / Not For

**Best for**
- Chinese web dramas, short dramas, and manhua-derived stories intended for overseas release
- Producers deciding between language strategies, markets, and formats
- Teams that need adaptation logic, packaging guidance, and rewrite priorities in one pass
- AI-native pipelines that need feasibility-aware recommendations, not just creative notes

**Not for**
- Literal translation or subtitle-only cleanup
- Historical or culturally specific works where preserving original context matters more than export legibility
- Teams that already have a locked market, locked language, locked format, and only need line-by-line script polishing
- Legal, licensing, or distributor-negotiation advice

## Installation

Add this skill to your Claude Code setup:

```bash
git clone https://github.com/DavidH-Creation/mandrama-export-adaptation.git ~/.claude/skills/mandrama-export-adaptation
```

Or add it as a project-level skill by cloning into your project's `.claude/skills/` directory.

## Usage

Ask Claude Code things like:

- "Adapt this Chinese web drama for overseas YouTube."
- "Should this project be English-led, Spanish-led, or subtitle-first?"
- "Package this manhua drama for international release."
- "Is this script better as 2D anime or 3D photoreal?"
- "What should I preserve, replace, simplify, or remove for export?"

For narrow route-selection questions, the skill can answer with a short decision brief instead of forcing a full export package.

## Examples

- [Quick route decision](C:/Users/david/Desktop/mandrama-export-adaptation/examples/quick-route-decision.md)
- [Full adaptation package](C:/Users/david/Desktop/mandrama-export-adaptation/examples/full-adaptation-package.md)

## File Structure

```text
SKILL.md                          # Entry point - workflow and resource routing
references/
  decision-framework.md           # Source diagnosis (emotional engine, friction, hooks, format)
  market-strategy-rules.md        # Route logic + production format rules
  adaptation-layers.md            # 6 rewrite layers (logline to packaging)
  dialogue-localization-engine.md # Full dialogue module with worked examples
  red-lines.md                    # Hard constraints / red flags
  rubrics.md                      # Scoring rubric
  archetype-glossary.md           # Chinese archetype to global role mappings
templates/
  quick-decision.md               # Short-form verdict template for route/format questions
  output-package.md               # Full-package output template
  adaptation-memo.md              # Preserve/replace/simplify/intensify/remove
  risk-register.md                # Risk assessment
  packaging-sheet.md              # Titles, thumbnails, metadata, hooks
  assumption-table.md             # Fact / inference / assumption tracking
examples/
  quick-route-decision.md         # Lightweight route-selection sample
  full-adaptation-package.md      # Full export-package sample
```

## License

MIT
