# 项目总览

[English Projects Page](./projects.md)

本页基于 2026-03-20 的 35 个自动科研相关仓库快照整理。它不是单纯按 star 排名，而是更关注这些项目到底覆盖了多少科研流程、适合什么使用场景、属于哪一类生态。

## 标签说明

- `Surface`：项目主要以什么形式使用
  - `CLI` 命令行
  - `IDE Skill` Claude Code / Codex / OpenClaw / Cursor 一类 skill 或 agent 指令集
  - `Web UI` 网页界面
  - `MCP` 作为 MCP server 或 MCP 工具层
  - `ChatOps` 通过 WhatsApp / Slack / Discord / Feishu 等聊天入口驱动
  - `Workspace` 更像一个研究工作台 / Lab OS / AI IDE
  - `Artifact` 更像证据仓库、论文产物仓库、结果仓库
- `Pipe`：项目覆盖的科研流程阶段
  - `I` 选题 / idea generation
  - `L` 文献检索 / literature review
  - `H` 假设形成 / hypothesis
  - `E` 实验 / coding / execution
  - `A` 分析 / evaluation
  - `W` 写作 / paper writing
  - `R` 评审 / critique / reviewer loop
  - `V` 可视化 / figures / posters / dashboards
  - `Ops` 运行时、调度、守护、恢复、长时运行支撑
- `Autonomy`
  - `Full` 高度自动化，可自主推进主流程
  - `Semi` 半自动，通常仍需要人做导师、选题或审阅
  - `Tool` 工具层 / 组件层，不是完整 scientist
- `Family`
  - `AI Scientist`：Sakana AI Scientist 系
  - `Autoresearch`：Karpathy autoresearch 及其移植分支
  - `Claw`：OpenClaw / ResearchClaw / DrClaw / CitationClaw 一类生态
  - `Independent`：相对独立，不明显属于上述谱系

## 全量矩阵

| Repo | Stars | 类别 | Surface | Pipe | 领域 | 自动化 | 生态 | 为什么值得看 |
| --- | ---: | --- | --- | --- | --- | --- | --- | --- |
| [SakanaAI/AI-Scientist](https://github.com/SakanaAI/AI-Scientist) | 12463 | 端到端系统 | CLI | I/H/E/A/W/R | 通用 ML | Full | AI Scientist | 第一代最有代表性的端到端 AI Scientist 基线 |
| [aiming-lab/AutoResearchClaw](https://github.com/aiming-lab/AutoResearchClaw) | 6908 | 端到端系统 | CLI / ChatOps | I/L/H/E/A/W/R/V | 通用 | Full | Claw | 目前最像“chat an idea, get a paper”的工程化开源实现 |
| [Analemma/FARS](https://analemma.ai/) | — | 端到端系统 | Web UI | I/L/H/E/A/W | AI 科研 | Full | Independent | 公开部署展示最清晰的一类闭源端到端自动科研系统 |
| [karpathy/autoresearch](https://github.com/karpathy/autoresearch) | 44200 | 实验循环 | CLI / IDE Skill | H/E/A | 通用 | Full | Autoresearch | 这波 autoresearch 方法论的共同语言和流量入口 |
| [SakanaAI/AI-Scientist-v2](https://github.com/SakanaAI/AI-Scientist-v2) | 2303 | 端到端系统 | CLI | I/H/E/A/W/R | 通用 ML | Full | AI Scientist | 如果你关心 v1 之后的下一代 scientist，它几乎必看 |
| [wanshuiyin/Auto-claude-code-research-in-sleep](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep) | 2688 | 实验循环 | IDE Skill | I/L/H/E/A/W/R/V | 通用 | Semi | Autoresearch | 很适合直接搬进 Claude Code 的夜间科研工作流 |
| [davebcn87/pi-autoresearch](https://github.com/davebcn87/pi-autoresearch) | 2425 | 实验循环 | CLI | H/E/A | 通用 | Full | Autoresearch | 比“大而全 scientist”更容易直接跑起来的优化循环 |
| [polyuiislab/infiAgent](https://github.com/polyuiislab/infiAgent) | 1140 | 基础设施 | Workspace / Web UI | Ops | 通用 | Tool | Independent | 重点在可恢复、长时运行、隔离和多天级 agent 稳定性 |
| [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) | 15600 | 技能包 | IDE Skill | L/E/A/W/V | 多学科科研 | Tool | Independent | 影响力极大的科研技能底座，很多垂直 agent 都能直接复用 |
| [EvoScientist/EvoScientist](https://github.com/EvoScientist/EvoScientist) | 1239 | 端到端系统 | CLI / MCP | I/L/H/E/A/W/R | 通用 | Full | Independent | 把“自进化 scientist”路线单独拉出来的一支 |
| [uditgoenka/autoresearch](https://github.com/uditgoenka/autoresearch) | 1539 | 实验循环 | IDE Skill | H/E/A | 通用 | Full | Autoresearch | 想在 Claude Code 里快速复现 Karpathy 范式时非常直接 |
| [mims-harvard/ToolUniverse](https://github.com/mims-harvard/ToolUniverse) | 1138 | 基础设施 | Python / MCP | L/E/A | 多学科科研 | Tool | Independent | 更像 AI scientist 的工具宇宙和中台，而不是单条 pipeline |
| [Sibyl-Research-Team/AutoResearch-SibylSystem](https://github.com/Sibyl-Research-Team/AutoResearch-SibylSystem) | 171 | 端到端系统 | CLI | I/L/H/E/A/W/R | 通用 | Full | Independent | star 不高，但“零人工 idea 到 paper”味道非常浓 |
| [dualverse-ai/station](https://github.com/dualverse-ai/station) | 111 | 基础设施 | Workspace | I/H/E/Ops | 通用 | Full | Independent | 更像 open-world 科学生态环境，而不是固定流水线 |
| [xjtulyc/MedgeClaw](https://github.com/xjtulyc/MedgeClaw) | 915 | 垂直 agent | ChatOps / Web UI | L/E/A/V | 生物医药 | Semi | Claw | 生物医学方向里产品感和落地感都很强 |
| [wu-yc/LabClaw](https://github.com/wu-yc/LabClaw) | 801 | 技能包 | IDE Skill / ChatOps | L/E/A/V | 生物医药 / Lab OS | Tool | Claw | 干实验室、湿实验室、文献和可视化能力都比较厚 |
| [OpenLAIR/dr-claw](https://github.com/OpenLAIR/dr-claw) | 534 | 工作台 | Workspace / Web UI | I/L/E/A/W/V/Ops | 通用 | Semi | Claw | 更像 full-stack research workspace / IDE |
| [wentorai/Research-Claw](https://github.com/wentorai/Research-Claw) | 345 | 工作台 | Workspace | I/L/E/A/W/Ops | 通用 | Semi | Claw | “你做导师，AI 团队干活”的 framing 很鲜明 |
| [beita6969/ScienceClaw](https://github.com/beita6969/ScienceClaw) | 257 | 工作台 | Workspace | I/L/E/A/W/Ops | 通用 | Semi | Claw | 更偏 persistent research coworker 路线 |
| [jimmc414/Kosmos](https://github.com/jimmc414/Kosmos) | 472 | 端到端系统 | CLI | H/E/A/W | 通用 | Full | Independent | 更像严肃实现版 scientist，不只是包装或概念 |
| [dwzhu-pku/PaperBanana](https://github.com/dwzhu-pku/PaperBanana) | 5286 | 产出层 | CLI / Web UI | V | 通用 | Tool | Independent | 学术插图自动化这一层目前最值得单独看的项目之一 |
| [FreedomIntelligence/OpenClaw-Medical-Skills](https://github.com/FreedomIntelligence/OpenClaw-Medical-Skills) | 1456 | 技能包 | IDE Skill | L/E/A | 医疗 / 基因组 | Tool | Claw | 医学方向 agent 的重要技能底座 |
| [Runchuan-BU/BioClaw](https://github.com/Runchuan-BU/BioClaw) | 225 | 垂直 agent | ChatOps | L/E/A | 生物信息学 | Semi | Claw | 对话即分析的生信助手，团队协作感很强 |
| [SakanaAI/AI-Scientist-ICLR2025-Workshop-Experiment](https://github.com/SakanaAI/AI-Scientist-ICLR2025-Workshop-Experiment) | 286 | 证据仓库 | Artifact | W/R | 通用 ML | Tool | AI Scientist | 更像“真的投出去并过 workshop”的证据仓库 |
| [eimenhmdt/autoresearcher](https://github.com/eimenhmdt/autoresearcher) | 419 | 端到端系统 | CLI | L/H/E/A/W | 通用 | Semi | Independent | 方向很对，但成熟度仍偏早期 |
| [leo-lilinxiao/codex-autoresearch](https://github.com/leo-lilinxiao/codex-autoresearch) | 345 | 实验循环 | IDE Skill | H/E/A | 通用 | Full | Autoresearch | Codex 用户如果想直接上手 autoresearch，这是很顺手的入口 |
| [trevin-creator/autoresearch-mlx](https://github.com/trevin-creator/autoresearch-mlx) | 867 | 实验循环 | CLI | H/E/A | 通用 | Full | Autoresearch | Apple Silicon / MLX 适配做得很到位 |
| [waltstephen/ArgusBot](https://github.com/waltstephen/ArgusBot) | 237 | 基础设施 | CLI | Ops | 通用 | Tool | Independent | 做长期循环时非常实用的守夜人组件 |
| [openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) | 839 | 基础设施 | MCP | L | 通用 | Tool | Independent | 多源论文检索层，适合塞进更大的 scientist 系统 |
| [VisionXLab/CitationClaw](https://github.com/VisionXLab/CitationClaw) | 193 | 产出层 | Web UI / CLI | L/A/V | 通用 | Tool | Claw | 把 citation graph 变成可解释影响力报告 |
| [ZhihaoAIRobotic/ClawPhD](https://github.com/ZhihaoAIRobotic/ClawPhD) | 136 | 产出层 | CLI / Artifact | V/W | 通用 | Tool | Claw | 更偏 posters、diagrams、paper website 这一层的包装能力 |
| [guhaohao0991/PaperClaw](https://github.com/guhaohao0991/PaperClaw) | 163 | 产出层 | IDE Skill / Automation | L/R | 通用 | Semi | Claw | 很适合做领域论文专家 agent |
| [InternScience/DrClaw](https://github.com/InternScience/DrClaw) | 109 | 工作台 | Workspace | I/L/E/A/W/Ops | 通用 | Semi | Claw | 仍然偏早期，但方向很明确：7x24 AI 科研团队 |
| [drivelineresearch/autoresearch-claude-code](https://github.com/drivelineresearch/autoresearch-claude-code) | 161 | 实验循环 | IDE Skill | H/E/A | 通用 | Full | Autoresearch | `pi-autoresearch` 的 Claude Code 移植版 |
| [olelehmann100kMRR/autoresearch-skill](https://github.com/olelehmann100kMRR/autoresearch-skill) | 278 | 实验循环 | IDE Skill | A | 通用 | Tool | Autoresearch | 更偏“用 autoresearch 优化 skill 本身”的 meta 用法 |

## 分类阅读

## 1. 最像“全自动科研”的端到端系统

这类项目最接近大家脑海里“AI Scientist”的定义：从 idea、文献、实验到论文产出，覆盖的环节尽可能多。

| Repo | Stars | Surface | Pipe | 为什么值得看 |
| --- | ---: | --- | --- | --- |
| [SakanaAI/AI-Scientist](https://github.com/SakanaAI/AI-Scientist) | 12463 | CLI | I/H/E/A/W/R | 第一代端到端 AI Scientist 的共识基线 |
| [aiming-lab/AutoResearchClaw](https://github.com/aiming-lab/AutoResearchClaw) | 6908 | CLI / ChatOps | I/L/H/E/A/W/R/V | 当前最完整的开源 idea-to-paper 工程流水线之一 |
| [Analemma/FARS](https://analemma.ai/) | — | Web UI | I/L/H/E/A/W | 公开部署和规模化运行展示都很强，说明它不是概念稿 |
| [SakanaAI/AI-Scientist-v2](https://github.com/SakanaAI/AI-Scientist-v2) | 2303 | CLI | I/H/E/A/W/R | 下一代 AI Scientist 升级方向最值得看的仓库 |
| [EvoScientist/EvoScientist](https://github.com/EvoScientist/EvoScientist) | 1239 | CLI / MCP | I/L/H/E/A/W/R | self-evolving scientist 路线的代表 |
| [Sibyl-Research-Team/AutoResearch-SibylSystem](https://github.com/Sibyl-Research-Team/AutoResearch-SibylSystem) | 171 | CLI | I/L/H/E/A/W/R | star 小，但很贴“零人工科研闭环” |
| [jimmc414/Kosmos](https://github.com/jimmc414/Kosmos) | 472 | CLI | H/E/A/W | 偏严肃实现派，不只是概念包装 |
| [eimenhmdt/autoresearcher](https://github.com/eimenhmdt/autoresearcher) | 419 | CLI | L/H/E/A/W | 仍偏早期，但方向完全对题 |
| [SakanaAI/AI-Scientist-ICLR2025-Workshop-Experiment](https://github.com/SakanaAI/AI-Scientist-ICLR2025-Workshop-Experiment) | 286 | Artifact | W/R | 更像结果证据仓，而不是主框架 |

## 2. 最像“自动实验组织”的 autoresearch 循环

这类项目不一定生成完整论文，但在“改代码 -> 跑实验 -> 比较指标 -> 保留/丢弃”这件事上非常强。

| Repo | Stars | Surface | Pipe | 为什么值得看 |
| --- | ---: | --- | --- | --- |
| [karpathy/autoresearch](https://github.com/karpathy/autoresearch) | 44200 | CLI / IDE Skill | H/E/A | autoresearch 范式本身的定义者 |
| [wanshuiyin/Auto-claude-code-research-in-sleep](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep) | 2688 | IDE Skill | I/L/H/E/A/W/R/V | 对 Claude Code 用户最实用的一套夜间研究 workflow |
| [davebcn87/pi-autoresearch](https://github.com/davebcn87/pi-autoresearch) | 2425 | CLI | H/E/A | 可迁移到任意可度量目标的优化循环 |
| [uditgoenka/autoresearch](https://github.com/uditgoenka/autoresearch) | 1539 | IDE Skill | H/E/A | 直接把 Karpathy 思路搬进 Claude Code |
| [trevin-creator/autoresearch-mlx](https://github.com/trevin-creator/autoresearch-mlx) | 867 | CLI | H/E/A | Mac / MLX 用户的重要分支 |
| [leo-lilinxiao/codex-autoresearch](https://github.com/leo-lilinxiao/codex-autoresearch) | 345 | IDE Skill | H/E/A | Codex 用户最好上手的一支 |
| [drivelineresearch/autoresearch-claude-code](https://github.com/drivelineresearch/autoresearch-claude-code) | 161 | IDE Skill | H/E/A | `pi-autoresearch` 的 Claude Code 版 |
| [olelehmann100kMRR/autoresearch-skill](https://github.com/olelehmann100kMRR/autoresearch-skill) | 278 | IDE Skill | A | 更 meta，更像“优化 skill 输出质量”的 autoresearch |

## 3. 技能层、工具层、运行时基础设施

这类项目不是完整 scientist，但没有它们，很多 scientist 系统就跑不起来或者跑不稳。

| Repo | Stars | Surface | Pipe | 为什么值得看 |
| --- | ---: | --- | --- | --- |
| [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) | 15600 | IDE Skill | L/E/A/W/V | 体量最大、复用价值最高的科研技能底座之一 |
| [mims-harvard/ToolUniverse](https://github.com/mims-harvard/ToolUniverse) | 1138 | Python / MCP | L/E/A | AI scientist 的工具中台 |
| [polyuiislab/infiAgent](https://github.com/polyuiislab/infiAgent) | 1140 | Workspace / Web UI | Ops | 长时运行、可恢复、可隔离这一层非常关键 |
| [openags/paper-search-mcp](https://github.com/openags/paper-search-mcp) | 839 | MCP | L | 检索层能力非常适合集成 |
| [waltstephen/ArgusBot](https://github.com/waltstephen/ArgusBot) | 237 | CLI | Ops | 24/7 守夜人，适合 autoresearch 长循环 |
| [dualverse-ai/station](https://github.com/dualverse-ai/station) | 111 | Workspace | I/H/E/Ops | 更像一个让 agent 自主演化的科学环境 |

## 4. 医学、生物、实验室方向的垂直科研 agent / 工作台

如果你更关心医学、生物、LabOS，这一组往往比通用 scientist 更贴近真实使用场景。

| Repo | Stars | Surface | Pipe | 为什么值得看 |
| --- | ---: | --- | --- | --- |
| [xjtulyc/MedgeClaw](https://github.com/xjtulyc/MedgeClaw) | 915 | ChatOps / Web UI | L/E/A/V | 生物医药方向产品化程度很高 |
| [wu-yc/LabClaw](https://github.com/wu-yc/LabClaw) | 801 | IDE Skill / ChatOps | L/E/A/V | Lab OS / 干湿实验桥接的技能层 |
| [OpenLAIR/dr-claw](https://github.com/OpenLAIR/dr-claw) | 534 | Workspace / Web UI | I/L/E/A/W/V/Ops | 很像 AI research IDE |
| [wentorai/Research-Claw](https://github.com/wentorai/Research-Claw) | 345 | Workspace | I/L/E/A/W/Ops | “AI 团队，你做 PI” 的 framing 很强 |
| [beita6969/ScienceClaw](https://github.com/beita6969/ScienceClaw) | 257 | Workspace | I/L/E/A/W/Ops | persistent coworker 路线 |
| [Runchuan-BU/BioClaw](https://github.com/Runchuan-BU/BioClaw) | 225 | ChatOps | L/E/A | 很适合“聊天即分析”的生信工作流 |
| [InternScience/DrClaw](https://github.com/InternScience/DrClaw) | 109 | Workspace | I/L/E/A/W/Ops | 愿景很对，但目前更早期 |
| [FreedomIntelligence/OpenClaw-Medical-Skills](https://github.com/FreedomIntelligence/OpenClaw-Medical-Skills) | 1456 | IDE Skill | L/E/A | 医疗和基因组方向的重要技能底座 |

## 5. 输出层、评审层、论文包装层

这类项目常常不是完整科研系统，但对“最后一公里”价值极高。

| Repo | Stars | Surface | Pipe | 为什么值得看 |
| --- | ---: | --- | --- | --- |
| [dwzhu-pku/PaperBanana](https://github.com/dwzhu-pku/PaperBanana) | 5286 | CLI / Web UI | V | 学术图示自动化这条线最值得看的项目之一 |
| [VisionXLab/CitationClaw](https://github.com/VisionXLab/CitationClaw) | 193 | Web UI / CLI | L/A/V | citation 影响分析和展示做得很明确 |
| [guhaohao0991/PaperClaw](https://github.com/guhaohao0991/PaperClaw) | 163 | IDE Skill / Automation | L/R | 更适合做领域论文专家智能体 |
| [ZhihaoAIRobotic/ClawPhD](https://github.com/ZhihaoAIRobotic/ClawPhD) | 136 | CLI / Artifact | V/W | 海报、图、网页、外部表达物这层很有用 |

## 选型建议

- 如果你只想先看“最像 AI Scientist”的仓库：先看 `AI-Scientist`、`AutoResearchClaw`、`AI-Scientist-v2`
- 如果你最想搭自己的自动实验循环：先看 `autoresearch`、`pi-autoresearch`、`Auto-claude-code-research-in-sleep`
- 如果你想补能力底座：先看 `claude-scientific-skills`、`ToolUniverse`、`paper-search-mcp`
- 如果你关心医学 / 生物落地：先看 `MedgeClaw`、`LabClaw`、`BioClaw`、`OpenClaw-Medical-Skills`
- 如果你想补论文产出最后一公里：先看 `PaperBanana`、`CitationClaw`、`ClawPhD`

## 说明

- 这不是纯 star 排名。
- 主要排序逻辑是：科研闭环相关性 > 社区影响力 > 可迁移性。
- 有些仓库是主框架，有些是工具层，有些是结果证据仓，有些是论文包装层，这几类不能混成一个标准比较。
- star 漂移很快，正式发布前建议统一刷新一遍。
