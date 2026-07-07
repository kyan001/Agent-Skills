# Agent-Skills

中文版 · [**English**](README.md)

AI agent 技能集。

## 安装

### skills.sh (Claude Code, Cursor, Codex 等)
```bash
# 互动安装技能
npx skills add kyan001/Agent-Skills  # 用 npx
bunx skills add kyan001/Agent-Skills  # 用 bunx

# 安装指定技能
npx skills add kyan001/Agent-Skills --skill japanese-lyrics-lint  # npx
bunx skills add kyan001/Agent-Skills --skill japanese-lyrics-lint  # bunx
```

### Hermes Agent
```Shell
# 安装单个技能
hermes skills install kyan001/Agent-Skills/skills/japanese-lyrics-lint


# 添加 tap（一次添加，多次安装）
hermes skills tap add kyan001/Agent-Skills
hermes skills install japanese-lyrics-lint
```

## 技能列表

| 名称 | 说明 |
|:-----|:------|
| [Japanese-Lyrics-Lint](skills/japanese-lyrics-lint/SKILL.md) | 日文歌词格式化：汉字注音、平假名还原汉字、片假名标注原词、逐行直译 |
