# Agent-Skills

中文版 · [**English**](README.md)

AI agent 技能集。

## 安装

### skills.sh (Claude Code, Cursor, Codex 等)
```bash
# 互动安装技能
npx skills add kyan001/Agent-Skills  # 用 npx
bunx skills add kyan001/Agent-Skills  # 用 bunx


# 安装指定技能（用 npx）
npx skills add kyan001/Agent-Skills --skill japanese-lyrics-lint
npx skills add kyan001/Agent-Skills --skill english-lyrics-lint
npx skills add kyan001/Agent-Skills --skill officecli


# 安装指定技能（用 bunx）
bunx skills add kyan001/Agent-Skills --skill japanese-lyrics-lint
bunx skills add kyan001/Agent-Skills --skill english-lyrics-lint
bunx skills add kyan001/Agent-Skills --skill officecli
```

### Hermes Agent
```Shell
# 安装单个技能
hermes skills install kyan001/Agent-Skills/skills/japanese-lyrics-lint
hermes skills install kyan001/Agent-Skills/skills/english-lyrics-lint
hermes skills install kyan001/Agent-Skills/skills/officecli


# 添加 tap（一次添加，多次安装）
hermes skills tap add kyan001/Agent-Skills
hermes skills install japanese-lyrics-lint
hermes skills install english-lyrics-lint
hermes skills install officecli
```

## 技能列表
* [Japanese-Lyrics-Lint](skills/japanese-lyrics-lint/SKILL.md)：日文歌词格式化——汉字注音、平假名还原汉字、片假名标注原词、逐行直译。
* [English-Lyrics-Lint](skills/english-lyrics-lint/SKILL.md)：检查和修正英文歌词格式——歌曲标题大小写、歌词大小写规则。
* [OfficeCLI (第三方)](skills/officecli/SKILL.md)：通过命令行创建、分析、校对和修改 Office 文档（.docx、.xlsx、.pptx）。
