# mandrama-export-adaptation

A Claude Code skill for adapting Chinese web dramas and manhua-drama scripts into export-ready international packages.

## What it does

- **Market routing** — chooses between English-led, Japanese-performance, or multilingual release strategies based on audience economics
- **Culture-friction rewriting** — identifies and replaces culture-locked plot devices, social logic, and character archetypes with globally legible equivalents
- **Dialogue localization** — localizes (not translates) dialogue into native-sounding target-language performance with tone variants
- **Format selection** — recommends 2D, anime, 3D MetaHuman, or hybrid based on story tone and production capability
- **Full output package** — generates loglines, character bios, episode hooks, packaging assets, risk registers, and production plans

This is a **market-aware adaptation system**, not a translation tool.

## Installation

Add this skill to your Claude Code setup:

```bash
# Clone into your Claude Code skills directory
git clone https://github.com/hongsmail77667-create/mandrama-export-adaptation.git ~/.claude/skills/mandrama-export-adaptation
```

Or add it as a project-level skill by cloning into your project's `.claude/skills/` directory.

## Usage

The skill triggers when you ask Claude Code to:

- "Adapt this Chinese web drama for overseas YouTube"
- "Rewrite this domestic plot for English-speaking audiences"
- "Should this project be English-led or Japanese-led?"
- "Package this manhua drama for international release"
- "Is this script better as 2D anime or 3D photoreal?"

## File Structure

```
SKILL.md                          # Entry point — workflow and resource routing
references/
  decision-framework.md           # Source diagnosis (emotional engine, friction, hooks, format)
  market-strategy-rules.md        # Route A/B/C + production format rules
  adaptation-layers.md            # 6 rewrite layers (logline → packaging)
  dialogue-localization-engine.md # Full dialogue module with worked examples
  red-lines.md                    # 6 hard constraints / red flags
  rubrics.md                      # 9-dimension scoring rubric
  archetype-glossary.md           # Chinese archetype → global role mappings
templates/
  output-package.md               # Master 9-section output template
  adaptation-memo.md              # Preserve/replace/simplify/intensify/remove
  risk-register.md                # 5-category risk assessment
  packaging-sheet.md              # Thumbnails, titles, metadata, hooks
  assumption-table.md             # Assumption tracking with confidence levels
```

## License

MIT
