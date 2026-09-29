# Agent-Skills

[**中文版**](README-cn.md) · English

Skills for AI agents.

## Install

### skills.sh (Claude Code, Cursor, Codex, etc.)
* You can replace `npx` with `bunx` if you use bunx.

```bash
# Install interactively
npx skills add kyan001/Agent-Skills


# Install a specific skill
npx skills add kyan001/Agent-Skills --skill japanese-lyrics-lint
npx skills add kyan001/Agent-Skills --skill english-lyrics-lint
npx skills add kyan001/Agent-Skills --skill dict
npx skills add kyan001/Agent-Skills --skill officecli
```

### Hermes Agent

```bash
# Install a single skill
hermes skills install kyan001/Agent-Skills/my-skills/japanese-lyrics-lint
hermes skills install kyan001/Agent-Skills/my-skills/english-lyrics-lint
hermes skills install kyan001/Agent-Skills/my-skills/dict
hermes skills install kyan001/Agent-Skills/optimized-skills/officecli


# Add as a tap (add once, install many)
hermes skills tap add kyan001/Agent-Skills
hermes skills install kyan001/Agent-Skills/japanese-lyrics-lint
hermes skills install kyan001/Agent-Skills/english-lyrics-lint
hermes skills install kyan001/Agent-Skills/dict
hermes skills install kyan001/Agent-Skills/officecli
```

## Skills
* [Japanese-Lyrics-Lint](my-skills/japanese-lyrics-lint/SKILL.md): Format Japanese lyrics: furigana for kanji, kanji for hiragana, original for katakana, line-by-line translation.
* [English-Lyrics-Lint](my-skills/english-lyrics-lint/SKILL.md): Check & fix English song title and lyrics capitalization (title case rules).
* [Dict](my-skills/dict/SKILL.md): Explain English/Japanese words, phrases and sentences: meaning, roots & affixes, structure, usage, register.
* [OfficeCLI (3rd Party)](optimized-skills/officecli/SKILL.md): Create, analyze, proofread, and modify Office documents (.docx, .xlsx, .pptx) via CLI.
