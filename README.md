# SkillNav Skill for Claude Code

在 Claude Code 中搜索 3,900+ MCP Server、获取每日 AI 日报、发现热门工具。

数据来自 [skillnav.dev](https://skillnav.dev) 编辑团队人工筛选。

## 安装

```bash
mkdir -p ~/.claude/skills/skillnav && curl -sL https://raw.githubusercontent.com/skillnav-dev/skillnav-skill/main/SKILL.md -o ~/.claude/skills/skillnav/SKILL.md
```

## 使用

### 今日 AI 日报

```
/skillnav brief
```

返回今日精选 AI 动态：头条 + 亮点速览 + 编辑点评。

### 搜索 MCP Server

```
/skillnav mcp database
/skillnav mcp github
/skillnav mcp slack
```

返回匹配的 MCP Server，包含：
- 中文描述 + 编辑点评
- Star 数量
- **一键安装命令**（可直接复制粘贴）

### 本周热门工具

```
/skillnav trending
```

返回本周 Star 增长最快的 MCP Server 和 Skills。

## 与 WebSearch 的区别

| | SkillNav Skill | WebSearch |
|---|---|---|
| MCP 数据 | 3,900+ 经编辑筛选 | 搜索引擎随机结果 |
| 安装命令 | 直接提供，可复制 | 需要自己找 |
| 编辑点评 | 人工编写的中文点评 | 无 |
| 每日日报 | 结构化 AI 资讯 | 无 |
| 延迟 | < 500ms API | 数秒级网页搜索 |

## 数据来源

- [skillnav.dev](https://skillnav.dev) — 中文开发者的 AI 智能体工具站
- 每日更新：15+ RSS 源 + 5 份 Newsletter 自动采集，编辑团队审核
- MCP 数据：3,900+ Server，持续更新 Star、安全评分、编辑点评

## License

MIT
