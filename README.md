# Agent-Skills

[**中文版**](README-cn.md) · English

Skills for AI agents.

## Install

### skills.sh (Claude Code, Cursor, Codex, etc.)
```bash
# Install interactively
npx skills add kyan001/Agent-Skills  # using npx
bunx skills add kyan001/Agent-Skills  # using bunx

# Install a specific skill
npx skills add kyan001/Agent-Skills --skill japanese-lyrics-lint  # using npx
bunx skills add kyan001/Agent-Skills --skill japanese-lyrics-lint  # using bunx
```

### Hermes Agent
```bash
# Install a single skill
hermes skills install kyan001/Agent-Skills/skills/japanese-lyrics-lint


# Add as a tap (add once, install many)
hermes skills tap add kyan001/Agent-Skills
hermes skills install japanese-lyrics-lint
```

## Skills

| Name | Description |
|:-----|:------------|
| [Japanese-Lyrics-Lint](skills/japanese-lyrics-lint/SKILL.md) | Format Japanese lyrics: furigana for kanji, kanji for hiragana, original for katakana, line-by-line translation |
