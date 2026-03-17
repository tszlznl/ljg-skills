# ljg-skills

My custom skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code).

## Skills

| Skill | Description |
|-------|-------------|
| **ljg-card** | Content caster — transforms content into PNG visuals (long card, infograph, poster). Infograph mode uses a content-adaptive design system: the AI analyzes content density, structure, and emotion to generate unique visual compositions from scratch — no fixed template, style serves thought. |
| **ljg-paper** | Paper reader — academic paper analysis pipeline |
| **ljg-paper-flow** | Paper workflow — reads papers + casts cards in one go (combines ljg-paper and ljg-card) |
| **ljg-plain** | Plain language rewriter — makes complex content accessible |
| **ljg-skill-map** | Skill map viewer — visual overview of all installed skills |
| **ljg-word** | English word mastery — deep-dive word deconstruction |
| **ljg-writes** | Writing engine — think through an idea by writing it out |

## Install

### Via Marketplace (Recommended)

```
/plugin marketplace add lijigang/ljg-skills
```

### Manual Install

```bash
git clone https://github.com/lijigang/ljg-skills.git ~/.claude/plugins/ljg-skills
```

Then restart Claude Code.

### ljg-card Dependencies

`ljg-card` requires Playwright for screenshot capture:

```bash
cd ~/.claude/plugins/ljg-skills && bash scripts/install.sh
```

Or manually:

```bash
cd ~/.claude/plugins/ljg-skills/skills/ljg-card && npm install && npx playwright install chromium
```
