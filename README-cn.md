# Agent-Skills

中文版 · [**English**](README.md)

AI agent 技能集。

## 安装

### skills.sh (Claude Code, Cursor, Codex 等)
* 可将 `npx` 替换为 `bunx`。

```bash
# 互动安装技能
npx skills add kyan001/Agent-Skills


# 安装指定技能
npx skills add kyan001/Agent-Skills --skill japanese-lyrics-lint
npx skills add kyan001/Agent-Skills --skill english-lyrics-lint
npx skills add kyan001/Agent-Skills --skill dict
npx skills add kyan001/Agent-Skills --skill officecli
```

### Hermes Agent

```shell
# 安装单个技能
hermes skills install kyan001/Agent-Skills/my-skills/japanese-lyrics-lint
hermes skills install kyan001/Agent-Skills/my-skills/english-lyrics-lint
hermes skills install kyan001/Agent-Skills/my-skills/dict
hermes skills install kyan001/Agent-Skills/optimized-skills/officecli


# 添加 tap（一次添加，多次安装）
hermes skills tap add kyan001/Agent-Skills
hermes skills install kyan001/Agent-Skills/japanese-lyrics-lint
hermes skills install kyan001/Agent-Skills/english-lyrics-lint
hermes skills install kyan001/Agent-Skills/dict
hermes skills install kyan001/Agent-Skills/officecli
```

## 技能列表
* [Japanese-Lyrics-Lint](my-skills/japanese-lyrics-lint/SKILL.md)：日文歌词格式化——汉字注音、平假名还原汉字、片假名标注原词、逐行直译。
* [English-Lyrics-Lint](my-skills/english-lyrics-lint/SKILL.md)：检查和修正英文歌词格式——歌曲标题大小写、歌词大小写规则。
* [Dict](my-skills/dict/SKILL.md)：解析英文/日文单词、短语、句子——释义、词根词缀、结构与语用。
* [OfficeCLI (第三方)](optimized-skills/officecli/SKILL.md)：通过命令行创建、分析、校对和修改 Office 文档（.docx、.xlsx、.pptx）。
