# 外部候选 Skills / 工具清单

> 调研时间：2026-11-24 · Stars 为当日查询值 · License 已通过 GitHub API 核验。
> 本清单只记录候选，**未安装、未迁入**。任何候选安装前仍须按安全规则全文审计。

## 网文写作（优先关注）

| 项目 | Stars | License | 亮点 | 结论 |
| :--- | ---: | :--- | :--- | :--- |
| [zenstory-ai/oh-story-claudecode](https://github.com/zenstory-ai/oh-story-claudecode) | 8.8k | MIT | 扫榜、拆文、大纲细纲、长短篇连载、伏笔追踪、去 AI 味、封面；覆盖起点/番茄/晋江 | 强烈候选：可补现有流水线的「扫榜拆文」环节 |
| [PenglongHuang/chinese-novelist-skill](https://github.com/PenglongHuang/chinese-novelist-skill) | 5.5k | MIT | 从零生成 10–50 章中文小说，三层问答、创作记忆、悬念钩子、自动校验 | 候选：适合快速起稿；与现有全流程引擎重叠，需比对 |
| [xiaofeng-928/chinese-longnovel-skill](https://github.com/xiaofeng-928/chinese-longnovel-skill) | 75 | MIT | 分层上下文、50 章分阶段细纲、事实锁、伏笔追踪、双审查自动修复 | 备选：长篇一致性机制值得借鉴 |
| [WindXRan/fanqie-radar](https://github.com/WindXRan/fanqie-radar) | 28 | MIT | 番茄榜单数据、扫榜选书、题材热度/趋势差分、仿写六维评分、MCP Server | 数据向补充：可补选题判断，需验证数据时效性 |

## 去 AI 味 / 文字质感

| 项目 | Stars | License | 亮点 | 结论 |
| :--- | ---: | :--- | :--- | :--- |
| [conorbronsdon/avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) | 6.1k | MIT | 审查并改写 AI 写作痕迹，兼容多 agent | 候选：与 `meiguofeilu` 去 AI 腔模块对照 |
| [KKKKhazix/human-writing](https://github.com/KKKKhazix/human-writing) | 4.6k | MIT | 让中文 AI 文本像具体的人在说话，通用创作与改稿 | 候选：中文语感更强，值得试 |

## 索引与资料

| 项目 | Stars | License | 说明 |
| :--- | ---: | :--- | :--- |
| [UnderleveledBuilder/awesome-novel-skills](https://github.com/UnderleveledBuilder/awesome-novel-skills) | 2.8k | CC0-1.0 | 网文 skill 精选索引，作为持续发现来源 |
| [AlephAITech/WorkBuddyGuide](https://github.com/AlephAITech/WorkBuddyGuide) | 3.9k | MIT | WorkBuddy 实战指南：工作流、Skills、MCP、自动化 |
| [adsorgcn/WorkBuddy](https://github.com/adsorgcn/WorkBuddy) | 134 | MIT | 公众号爆文结构专家 skill（素材→成稿，12 项自查，去 AI 味） |

## 安装审计规则

1. 任何候选**安装前**必须全文审计 `SKILL.md` 与 `scripts/` 下全部脚本。
2. 红线：可疑网络请求（外传数据 / 静默上报 / 远程拉取执行代码）、文件删除覆盖、凭据读取（token / 私钥 / cookie / `~/.workbuddy` 凭证）、prompt injection。命中任一即拒绝安装。
3. 流程：审计通过 → 本机试跑 → 确认与现有 skill 不冲突 → 再迁入或安装。
