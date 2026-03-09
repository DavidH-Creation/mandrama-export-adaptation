# Decision Framework - Source Diagnosis

Use this framework in Phase 1 to classify the source material before making any adaptation decisions.

## Inputs

Accept any subset of the following. If input is incomplete, proceed with best-effort defaults and explicitly label assumptions.

The market list is illustrative, not exhaustive. Use any target region the user specifies.

```yaml
source_material:
  - logline
  - synopsis
  - pilot script
  - episode outline
  - full script
  - character bible
  - reference images

market_goal:
  primary_market: [US, UK, AU, Western_Europe, LATAM, Brazil, MENA, SEA, Japan, Korea, global_anime, diaspora]
  monetization_goal: [adsense, sponsorship, platform_pitch, proof_of_concept, channel_growth]

format_goal:
  content_type: [vertical_drama, motion_comic, 3d_photoreal, anime_style, hybrid]
  episode_length_sec: number
  total_episodes: number

production_constraints:
  budget_level: [low, medium, high]
  turnaround_speed: [fast, balanced, premium]
  ai_pipeline: [image_gen, video_gen, ue_metahuman, voice_dub, subtitle_only]

preservation_priority:
  keep_setting: true/false
  keep_core_plot: true/false
  keep_character_names: true/false
  keep_cultural_texture: low/medium/high
```

## Axis A - Emotional Engine

Classify the project's core emotional driver. A project may have 1-3 primary engines:

- **Revenge** - wronged protagonist seeks payback
- **Romance** - love drives the central tension
- **Status reversal** - low-status character rises or high-status falls
- **Survival** - life-or-death stakes
- **Underdog rise** - outmatched protagonist overcomes odds
- **Forbidden love** - relationship defies social/family rules
- **Mystery / conspiracy** - hidden truth drives investigation
- **Family betrayal** - betrayal within kinship or close circle
- **Wish fulfillment / power fantasy** - protagonist gains extraordinary ability or status

## Axis B - Export Friction

Identify what will fail outside China. Check for:

- **High-context social hierarchy assumptions** - audience must already understand Chinese social status markers
- **Culturally specific filial / workplace / marriage norms** - presented without explanation, assumed as default
- **Melodrama pacing** - requires prior familiarity with Chinese short-drama conventions
- **Local internet culture dependence** - plot devices built on Chinese internet slang, memes, bureaucracy, or school/work systems
- **Wordplay / celebrity references** - humor or callbacks that have no equivalent outside China

Rate each friction point: **high** (will confuse), **medium** (needs rewrite), **low** (minor adjustment).

## Axis C - Universal Hooks

Find what can travel across cultures without rewriting:

- Jealousy
- Humiliation / comeback
- Betrayal
- Class anxiety
- Secret identity
- Obsessive love
- Moral compromise
- Ambition
- Protection / sacrifice

Strong universal hooks = less rewrite needed. Weak universal hooks = deeper adaptation required.

## Axis D - Format Fit

Score whether the project is best produced as:

| Format | Best When |
|---|---|
| **2D motion comic** | Stylized visuals, fast turnaround, exaggeration helps the material |
| **Anime-style cutscene series** | Subculture-native audience, fantasy/action genre |
| **3D photoreal MetaHuman** | Realism/tension/luxury/thriller tone, consistent character performance needed |
| **Hybrid visual novel / motion board** | Dialogue-heavy, low budget, proof-of-concept stage |

Score each format 1-5 for the specific project. Recommend the highest-scoring format with justification.

## Output

After completing all 4 axes, produce:

1. **Emotional engine classification** - primary and secondary engines
2. **Export friction map** - each friction point with severity rating
3. **Universal hook inventory** - which hooks are present and how strong
4. **Format recommendation** - top format with score and reasoning
5. **Overall export potential** - High / Medium / Low with one-paragraph justification
