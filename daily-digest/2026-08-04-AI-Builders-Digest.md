---
date: 2026-08-04
type: auto-digest
source: follow-builders
domains: [AI, 资讯]
builders: 12
tweets: 26
podcasts: 1
blogs: 0
---


# AI Builders Digest — 2026-08-04 (周二)

> 来源：[follow-builders](https://github.com/zarazhangrui/follow-builders) | 自动生成时间：08:01

# 🤖 AI Builder 日报

### 🎙️ 播客精选

**Training Data | Building the Automated AGI Lab: Core Automation's Jerry Tworek and Rohan Anil**
本期播客深度对话了 **Core Automation** 联合创始人 Jerry Tworek（前 OpenAI 副总裁，主导 Strawberry 推理团队）与 Rohan Anil（前 Gemini 预训练负责人，曾主导 Google Brain 与 Anthropic 核心研究）。核心论点直指当前大模型发展的架构瓶颈：团队认为，过去六年 AI 领域已彻底攻克大规模预训练与大规模强化学习（RLHF）两大范式，Transformer 架构的潜力已被充分榨取。下一步突破的关键不在于单纯堆叠参数量或做推理效率优化（如 MoE 路由），而在于**重新审视并设计下一代基础架构**。Jerry 强调，必须深刻理解 Transformer 的“强项与弱项”，才能避开重复造轮子，真正瞄准其长程依赖与逻辑表达能力的短板。值得深挖的论断是：尽管 Codex 等编码 Agent 已展现出强大的工作流自动化能力，但“为什么仍有大量日常任务无法被完全自动化？”这一追问才是 AGI 实验室的核心课题。团队主张将研究重心从 Scaling Law 转向 Agentic 系统的自主任务拆解与持续环境交互，预示着 AI 研发范式正从“模型规模竞赛”转向“自动化架构探索”。[原文](https://www.youtube.com/watch?v=2RJiaf0SY8s)

---

### 💬 X/Twitter 核心动态

**Guillermo Rauch (@rauchg)**
Vercel CEO 详细披露了公司内部 AI Agent 架构的演进路径。面对早期各团队独立部署 Agent 导致的“碎片化”体验与资源浪费，Vercel 推出了统一调度平台 `@v`，将其定位为兼具路由（Router）与单体（Monolith）特性的超级中枢。该 Agent 不仅内置金融、工程、营销等垂直技能，还能通过子 Agent（Sub-agents）进行动态任务委派，并具备长期记忆与个性化工作流学习能力。目前该中枢已深度嵌入日常运营，Token 消耗量与交互频次呈指数级增长，印证了企业级 AI 正从“单点工具试用”迈向“多智能体协同编排”阶段。[原文](https://x.com/rauchg/status/2084042561690456157)

**Peter Yang (@petergyang)**
针对开源大模型普遍存在的“幻觉与低质输出（Slop）”问题，Peter 披露了 NousResearch 联合创始人 Karan 对 **Hermes 模型** 的自优化机制。Hermes 内置了一个名为 `Hermes Curator` 的后台守护进程，能够定期自动审查并清理 Agent 的技能库与记忆池，主动识别低效或冗余内容。更重要的是，该机制完全开源且支持用户自定义“低质标准”，使模型能够根据具体业务场景动态重写自身知识权重。这一设计为开源 Agent 的自我进化与上下文治理提供了新思路，有效缓解了长期运行中的记忆污染与性能衰减问题。[原文](https://x.com/petergyang/status/2083968605432267139)

**Aaron Levie (@levie)**
Box CEO 提出了一个反直觉的行业观察：数学、网络安全与代码编写等“高难度”领域，反而因其**可验证性（Verifiability）**成为最先被 AI 自动化的方向。这些领域具备客观的正确性判定标准，为模型训练提供了清晰的 Reward Signal（奖励信号），同时在推理阶段也能通过自动化测试快速验证输出结果。这一逻辑解释了为何 Coding Agent 与 Math Solver 能率先突破，也预示着未来 AI 在具备明确评估体系的垂直领域将呈现降维打击态势，传统“难度越高越难自动化”的假设已被彻底打破。[原文](https://x.com/levie/status/2083965372747882741)

**Dan Shipper (@danshipper)**
Dan 提出了“Agency Rupture（能动性断裂）”概念，深入剖析了 AI 接管人类任务时的心理与社会学影响。当大模型能够无缝完成过去依赖人工逐步推进的工作时，用户会经历强烈的身份认同危机，因为“任务输出”传统上被视为个人职业价值的核心锚点。但他指出，这种断裂遵循可预测的演进模式：从初期的抗拒与自我怀疑，逐渐过渡到重新定义人类在“监督-决策”链条中的新角色。同时，他援引“ought implies can”的哲学命题，强调技术边界的扩张将直接重塑人类的道德直觉与社会规范。[原文](https://x.com/danshipper/status/2084038453831020916)

**Thariq (@trq212) & Amjad Masad (@amasad)**
两位 Builder 分别从经济学与工程实践角度验证了 AI 对复杂系统的重构效应。Thariq 指出，AI 在数学领域的应用正显现**杰文斯悖论（Jevons Paradox）**：随着计算与抽象门槛的降低，研究者得以在更高维度进行协作与讨论，反而推高了市场对“高阶数学思维”的需求。Amjad 则同步部署了自主运行的 LLM 国际象棋引擎，该 Agent 已在 Lichess 平台以 1253 Elo 的评分独立参与人机对弈，并能同时处理 3 局并发游戏。两者共同表明，AI 并未消灭复杂智力活动，而是将其推向了更高阶的抽象层与自动化博弈场景。[原文](https://x.com/trq212/status/2083977795290734975) | [原文](https://x.com/amasad/status/2083926395403821427)

**Swyx (@swyx)**
在筹备 Computer Use 播客期间，Swyx 记录了 Codex CUA（Computer Use Agent）在真实客服场景中的实战表现。该 Agent 被用于接管技术支持聊天窗口，不仅成功应对了人类客服的常规追问，甚至在面对“归责推诿”时能精准调取完整操作日志（Receipts）进行逻辑反驳，且全程未被人类客服察觉为机器人。这一案例直观展示了具备视觉与操作闭环的 Desktop Agent 已具备处理非结构化、高对抗性业务流程的能力，为 B 端自动化客服与 IT 运维提供了极具说服力的 PoC。[原文](https://x.com/swyx/status/2084156733027701164)

**Nikunj Kothari (@nikunj)**
从一级市场投资视角，Nikunj 揭示了当前 AI 融资市场的结构性错配。他指出，早期至中期 VC 市场已演变为“Vibes Capital（情绪资本）”，估值逻辑与基本面完全脱钩：部分缺乏实质进展的项目能拿到天价融资，而具备扎实技术壁垒的团队却面临 Series A 紧缩。这种市场情绪与底层技术成熟度的背离，预示着未来 12-18 个月内将经历一轮残酷的估值出清，具备清晰 Unit Economics 与真实 Agentic 落地场景的项目将重新掌握定价权。[原文](https://x.com/nikunj/status/2083873335998333227)

---

### 🔍 今日洞察

1. **企业 Agent 架构正从“去中心化试错”转向“中枢路由化”**：Vercel 的内部实践表明，早期各自为战的独立 Agent 已遭遇严重的 UX 割裂与上下文孤岛。通过构建具备路由分发、记忆共享与子任务委派能力的“超级 Agent 单体”，企业级 AI 正解决多智能体协同的规模化瓶颈。这不仅是工程架构的升级，更是 AI 基础设施从“单模型调用”向“自主决策网络”演进的关键分水岭。
2. **“可验证性”成为 AI 自动化落地的第一性原理**：Aaron Levie 的观察与开源社区的实践共同印证，高价值但难以量化的创意工作并非 AI 的首选目标。相反，代码、数学、安全等具备明确反馈回路与客观验证标准的领域将率先被重构。这要求开发者在构建 Agentic 应用时，优先设计可测试、可审计的 Reward 机制与沙盒环境，而非盲目追求通用泛化能力。
3. **技术平权正在重塑人类认知与道德的“基线”**：杰文斯悖论在数学领域的显现与“能动性断裂”理论形成强烈呼应。当 AI 将底层计算与执行成本压至趋近于零时，人类的核心价值将不可逆地向“定义问题、抽象建模与价值判断”迁移。这不仅会彻底改写劳动力市场的技能溢价曲线，更将迫使社会重新校准“能力边界”与“责任归属”的伦理框架，为下一代人机协作立法提供理论依据。

---


## 原文链接汇总


### 播客

- [Building the Automated AGI Lab: Core Automation's Jerry Tworek and Rohan Anil](https://www.youtube.com/watch?v=2RJiaf0SY8s) — Training Data

### X/Twitter


**Andrej Karpathy** (@karpathy)
- [More on the pelican on the bicycle test from @simonw: https://t.co/OXm...](https://x.com/karpathy/status/2083948654377996480)

**Swyx** (@swyx)
- [haven't seen a full cycle of this guy but this place absolutely can ch...](https://x.com/swyx/status/2084171901451268599)
- [in prep for our computer use pod, gonna store a running list of codex ...](https://x.com/swyx/status/2084156733027701164)
- [@akshaynathan_ @AriX live now! https://t.co/I7vcXbQEqf...](https://x.com/swyx/status/2084155512573288478)

**Peter Yang** (@petergyang)
- [Went to a community center in Canada and it has a full swimming pool, ...](https://x.com/petergyang/status/2084065527081980285)
- [One of the biggest benefits of Hermes is that it builds its own skills...](https://x.com/petergyang/status/2083968605432267139)
- [Personality matters! A smart friend that's annoying to talk to is no g...](https://x.com/petergyang/status/2083947480136421384)

**Thariq** (@trq212)
- [i think there are lots of parallels to what happened with chess...](https://x.com/trq212/status/2083978109376987365)
- [you can already see Jevons paradox at work in mathematics  there is mo...](https://x.com/trq212/status/2083977795290734975)

**Amjad Masad** (@amasad)
- [Woah https://t.co/d20LLYD88E...](https://x.com/amasad/status/2084017252152856716)
- [You can watch the games live on the website. Mf is playing 3 concurren...](https://x.com/amasad/status/2083936067355635948)
- [My LLM chess engine is now on LiChess autonomously playing real games ...](https://x.com/amasad/status/2083926395403821427)

**Guillermo Rauch** (@rauchg)
- [PS: we've obviously had agents for a while. In fact, we had too many. ...](https://x.com/rauchg/status/2084060157085143512)
- [We built an agent that powers our company's internal operations called...](https://x.com/rauchg/status/2084042561690456157)
- [AI alone is cool. But mastery + creativity + AI hits on a whole differ...](https://x.com/rauchg/status/2083969120270450911)

**Aaron Levie** (@levie)
- [We’re going to be in for a strange dynamic which is that some of the “...](https://x.com/levie/status/2083965372747882741)

**Ryo Lu** (@ryolu_)
- [my early mentors were these apps, especially Rdio, Mailbox, and Apple ...](https://x.com/ryolu_/status/2083939454017053179)

**Garry Tan** (@garrytan)
- [Growth is good  AI will create unimaginable economic growth and that i...](https://x.com/garrytan/status/2083957110711386439)
- [The sense of wonder disappeared right at the moment the amount of wond...](https://x.com/garrytan/status/2083923385193828612)
- [Everyone mistakes the map for the territory  Meritocracy is that the t...](https://x.com/garrytan/status/2083920039208693996)

**Nikunj Kothari** (@nikunj)
- [Warm NYC nights are magic 🪄 https://t.co/KGpckLDaAo...](https://x.com/nikunj/status/2083925904598733088)
- [What a wild world we’re living through. I wrote about the Series A squ...](https://x.com/nikunj/status/2083873335998333227)

**Peter Steinberger** (@steipete)
- [That's a fairly new kind of spam. https://t.co/nwdRM5e7Hv https://t.co...](https://x.com/steipete/status/2083976289485230449)

**Dan Shipper** (@danshipper)
- [if you haven’t read War and Peace or some of the historical accounts o...](https://x.com/danshipper/status/2084144207254663417)
- [when you experience a language model doing a task that used to require...](https://x.com/danshipper/status/2084038453831020916)
- [if ought implies can, and technology reshapes the field of human abili...](https://x.com/danshipper/status/2084024211539116466)
