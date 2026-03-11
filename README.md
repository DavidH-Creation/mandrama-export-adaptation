# mandrama-export-adaptation

## 中文

把中国本土优先的网剧和漫剧，转成适合海外市场的国际化输出方案。

这是一个用于**改编策略**的 skill，不是逐字翻译工具。它帮助判断：
- 应该先打哪个市场
- 应该以哪种语言包为主
- 原作逻辑需要改写到什么程度
- 哪种形式最符合故事和制作现实

它目前优先适配**面向美国 / 英国 / 欧洲的出海工作**，但**并不锁死在英语或日语**。只要市场逻辑成立，西语、葡语、阿拉伯语、法语、德语、韩语等主语言方案也都可以成立。

### 为什么会有这个 skill

很多中国短剧和漫剧改编项目在海外表现不好，并不是因为情绪引擎不够强，而是因为出海包装方向错了：
- 社会逻辑太本地
- 对白听起来像翻译出来的
- 发布语言和变现计划不匹配
- 视觉形式和故事气质打架

这个 skill 提供了一套可以重复使用的修正方式。

### 它会做什么

- **为项目选路线**：英语主导、亚文化性能向、区域本地化优先、或多语言分层发布
- **改写文化摩擦点**：让情节逻辑脱离中文语境也能成立
- **本地化对白**：让台词更像目标市场母语创作
- **选择形式**：在 2D、anime-style、3D MetaHuman 或 hybrid 之间做判断
- **包装项目**：提供 logline、hook、标题、风险提示和下一步制作建议

### 快速示例

#### 输入

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

#### 输出形态

```text
Verdict: Anglophone premium export
Confidence: Medium-High
Best market: US / UK short-drama and YouTube audiences
Core reason: The premise travels well because betrayal, humiliation, and comeback are universal hooks. The sponsorable version works better in English-led packaging than subtitle-first release, but the social logic around inheritance and fake marriage needs rewriting for export clarity.

Recommended option: English-led launch with globally legible naming and prestige-melodrama positioning
Second-best option: Spanish-led LATAM test if distribution partner or dubbing advantage exists
Reject for now: Japanese-performance route because the material is luxury revenge, not fandom-native stylized romance
```

完整示例见 `examples/` 目录。

### 适合 / 不适合

**适合**
- 面向海外发行的中国网剧、短剧、漫剧改编项目
- 需要在语言策略、市场和形式之间做判断的制作方
- 希望把改编逻辑、包装建议和重写优先级一次理清的团队
- 需要兼顾可行性，而不是只要创意意见的 AI-native 流程

**不适合**
- 逐字翻译或只做字幕润色
- 更重视原语境保留、而不是出海可读性的历史题材或强文化作品
- 市场、语言和形式都已经锁定，只需要逐行修稿的团队
- 法务、版权或发行谈判建议

### 安装

把这个 skill 加入你的 Claude Code：

```bash
git clone https://github.com/DavidH-Creation/mandrama-export-adaptation.git ~/.claude/skills/mandrama-export-adaptation
```

也可以把它作为项目级 skill，克隆到项目的 `.claude/skills/` 目录中。

### 使用方式

你可以这样问 Claude Code：

- "Adapt this Chinese web drama for overseas YouTube."
- "Should this project be English-led, Spanish-led, or subtitle-first?"
- "Package this manhua drama for international release."
- "Is this script better as 2D anime or 3D photoreal?"
- "What should I preserve, replace, simplify, or remove for export?"

如果只是窄范围的路线选择问题，这个 skill 也可以输出简版决策，而不是强行给完整出海方案。

### 示例

- `examples/quick-route-decision.md`
- `examples/full-adaptation-package.md`

### 文件结构

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

### 许可证

MIT

---

## English

Turn China-first web dramas and manhua dramas into export-ready international packages.

This is a skill for **adaptation strategy**, not literal translation. It helps decide:
- which market to target first
- which language package to lead with
- how much of the source logic must be rewritten
- which format best fits the story and production reality

It is currently optimized for **US/UK/Europe-facing export work**, but it is **not locked to English or Japanese**. Spanish, Portuguese, Arabic, French, German, Korean, and other primary language packages are valid when the market logic supports them.

### Why this exists

Most Chinese short dramas and manhua adaptations do not fail overseas because the core emotional engine is weak. They fail because the export package is wrong:
- the social logic is too local
- the dialogue sounds translated
- the release language does not match the monetization plan
- the visual format fights the story tone

This skill gives you a repeatable way to fix that.

### What it does

- **Route the project** into Anglophone, performance-led subculture, region-first localized, or multilingual release strategies
- **Rewrite culture friction** so plot logic survives outside Chinese context
- **Localize dialogue** into native-sounding performance language
- **Choose format** across 2D, anime-style, 3D MetaHuman, or hybrid
- **Package the project** with loglines, hooks, titles, risk notes, and next-step production guidance

### Quick Example

#### Input

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

#### Output shape

```text
Verdict: Anglophone premium export
Confidence: Medium-High
Best market: US / UK short-drama and YouTube audiences
Core reason: The premise travels well because betrayal, humiliation, and comeback are universal hooks. The sponsorable version works better in English-led packaging than subtitle-first release, but the social logic around inheritance and fake marriage needs rewriting for export clarity.

Recommended option: English-led launch with globally legible naming and prestige-melodrama positioning
Second-best option: Spanish-led LATAM test if distribution partner or dubbing advantage exists
Reject for now: Japanese-performance route because the material is luxury revenge, not fandom-native stylized romance
```

See full sample outputs in `examples/`.

### Best For / Not For

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

### Installation

Add this skill to your Claude Code setup:

```bash
git clone https://github.com/DavidH-Creation/mandrama-export-adaptation.git ~/.claude/skills/mandrama-export-adaptation
```

Or add it as a project-level skill by cloning into your project's `.claude/skills/` directory.

### Usage

Ask Claude Code things like:

- "Adapt this Chinese web drama for overseas YouTube."
- "Should this project be English-led, Spanish-led, or subtitle-first?"
- "Package this manhua drama for international release."
- "Is this script better as 2D anime or 3D photoreal?"
- "What should I preserve, replace, simplify, or remove for export?"

For narrow route-selection questions, the skill can answer with a short decision brief instead of forcing a full export package.

### Examples

- `examples/quick-route-decision.md`
- `examples/full-adaptation-package.md`

### File Structure

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

### License

MIT
