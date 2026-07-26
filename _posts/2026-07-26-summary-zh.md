---
layout: default
title: "Horizon Summary: 2026-07-26 (ZH)"
date: 2026-07-26
lang: zh
---

> 从 31 条内容中筛选出 12 条重要资讯。

---

1. [Anthropic 发布 Claude 5 上下文工程新规，引发批评](#item-1) ⭐️ 8.0/10
2. [通用汽车支持钠离子电池用于美国电网储能](#item-2) ⭐️ 8.0/10
3. [DeepSeek 因算力差距言论泄露暂停融资](#item-3) ⭐️ 8.0/10
4. [2890 万参数的 LLM 可在 8 美元的 ESP32 微控制器上运行](#item-4) ⭐️ 8.0/10
5. [Debian 讨论关于 LLM 贡献的三项提案](#item-5) ⭐️ 8.0/10
6. [开放权重 AI 的 Kubernetes 时刻](#item-6) ⭐️ 8.0/10
7. [Ruff v0.16.0 将默认启用的规则从 59 条增加到 413 条](#item-7) ⭐️ 8.0/10
8. [Anthropic 发布 Claude Opus 5，主动型 AI 模型，价格仅为 Fable 5 的一半](#item-8) ⭐️ 8.0/10
9. [编译器将计算图转换为无需训练的变压器权重](#item-9) ⭐️ 8.0/10
10. [AutoDev Studio：开源多智能体 SDLC 工具大幅降低 AI 编码成本](#item-10) ⭐️ 8.0/10
11. [明尼苏达州风能氨厂实现灵活运行](#item-11) ⭐️ 7.0/10
12. [论文长度与机器学习会议中理论研究的评审偏见](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic 发布 Claude 5 上下文工程新规，引发批评](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 8.0/10

Anthropic 宣布了专门针对 Claude 5 的上下文工程新规则，旨在优化用户为该模型构建提示和系统指令的方式。 这很重要，因为上下文工程正成为从大语言模型获得可靠输出的关键技能，而 Anthropic 的规则可能塑造最佳实践——但社区成员担心这会增加供应商锁定风险以及 Claude 自动记忆功能的潜在问题。 新规则据说强调结构化模板和 Anthropic 特定工具，背离自由格式的 .md 文件，一些用户认为这是锁定策略。此外，Claude 5 的自动记忆被批评为会做出不恰当的上下文跳跃，导致意外行为。

hackernews · mellosouls · 7月25日 20:42 · [社区讨论](https://news.ycombinator.com/item?id=49051361)

**背景**: 上下文工程涉及迭代优化提供给大语言模型的指令和上下文，以达到预期结果，超越了简单的提示工程。Anthropic 的 Claude 模型具有独特的“自动记忆”功能，允许模型跨会话回忆和使用存储的信息，但这有时会导致不可预测的输出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.promptingguide.ai/guides/context-engineering-guide">Context Engineering Guide | Prompt Engineering Guide</a></li>
<li><a href="https://spring.io/blog/2026/04/07/spring-ai-agentic-patterns-6-memory-tools/">Spring AI Agentic Patterns (Part 6): AutoMemoryTools — Persistent Agent Memory Across Sessions</a></li>

</ul>
</details>

**社区讨论**: 社区态度褒贬不一：一些用户主张使用明确的指令语言而非 Anthropic 的方法，而另一些用户报告称 Claude 5 相比之前版本出错更多且忽略故意设置的控制。用户强烈希望获得更多控制权而非更少，有些用户更偏好 GPT 对指令的更严格遵守。

**标签**: `#Claude`, `#AI`, `#context engineering`, `#LLM`, `#Anthropic`

---

<a id="item-2"></a>
## [通用汽车支持钠离子电池用于美国电网储能](https://spectrum.ieee.org/sodium-ion-battery-peak-energy) ⭐️ 8.0/10

通用汽车宣布支持将钠离子电池技术用于美国大规模电网储能，标志着向更便宜、更可持续的储能解决方案的战略转变。 这一举措可能减少对昂贵且地理分布集中的锂的依赖，并加速对整合太阳能和风能等可再生能源至关重要的电网级储能的采用。 据讨论，钠离子电池的往返效率达到 96%，并且不需要钴、铜或镍，使其可能比锂离子电池更便宜且更环保。

hackernews · rbanffy · 7月25日 21:48 · [社区讨论](https://news.ycombinator.com/item?id=49051947)

**背景**: 钠离子电池使用丰富的钠代替锂作为电荷载体，工作原理与锂离子电池相似。由于锂的高成本和环境问题，它们在 2010 年代开始受到关注，但在能量密度和商业化速度上仍落后于锂离子电池。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sodium-ion_batteries">Sodium-ion batteries</a></li>

</ul>
</details>

**社区讨论**: 评论者对美国制造表示怀疑，一位用户认为这些电池只是贴了“美国制造”标签的中国硬件。其他人讨论了电网储能中暖通空调系统的潜在成本节省以及对家用钠离子电池的兴趣，还有一位指出一家有前途的美国钠离子初创公司因缺乏资金而破产出售。

**标签**: `#sodium-ion`, `#grid storage`, `#batteries`, `#GM`, `#energy`

---

<a id="item-3"></a>
## [DeepSeek 因算力差距言论泄露暂停融资](https://github.com/demo-zexuan/liang-wenfeng-investor-meeting-2026-7-22/blob/master/%E6%A2%81%E6%96%87%E9%94%8B%E6%8A%95%E8%B5%84%E8%80%85%E4%BA%A4%E6%B5%81%E4%BC%9A-%E6%96%87%E5%AD%97%E7%A8%BF_1_18_translate_20260723201651.pdf) ⭐️ 8.0/10

据彭博社报道，DeepSeek 在创始人梁文锋关于中美 AI 算力差距的言论泄露后，暂停了第二轮融资。 这一暂停信号表明中国 AI 投资环境的不确定性，并凸显地缘政治紧张对 AI 发展资金的影响，可能削弱 DeepSeek 与美国资金充裕的实验室竞争的能力。 据彭博社援引知情人士报道，融资暂停发生在腾讯参与传闻之后；DeepSeek 的开放权重模型（如 DeepSeek-R1）训练成本仅为美国同行的零头。

hackernews · oliculipolicula · 7月25日 23:32 · [社区讨论](https://news.ycombinator.com/item?id=49052912)

**背景**: DeepSeek 是 2023 年由梁文锋创立的中国 AI 公司，此前由对冲基金 High-Flyer 资助。2025 年 1 月，DeepSeek-R1 发布，性能可比 OpenAI 的 GPT-4 但训练成本低得多，引起关注。美国因对先进芯片的出口管制保持算力优势，但中国模型正在缩小性能差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://www.rand.org/pubs/commentary/2025/05/chinas-ai-models-are-closing-the-gap-but-americas-real.html">China's AI Models Are Closing the Gap—but America's Real Advantage Lies Elsewhere | RAND</a></li>
<li><a href="https://www.csis.org/analysis/securing-agi-laurel-export-controls-compute-gap-and-chinas-counterstrategy">Securing the AGI Laurel: Export Controls, the Compute Gap, and China’s Counterstrategy | CSIS</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了暂停的含义：有人澄清并非因言论泄露导致暂停，而是泄露揭示了暂停理由。其他人质疑在中文模型更高效的情况下追求前沿模型的策略，并注意到与美国实验室领导者语气上的差异。

**标签**: `#deepseek`, `#ai-fundraising`, `#us-china-ai`, `#compute-gap`, `#ai-competition`

---

<a id="item-4"></a>
## [2890 万参数的 LLM 可在 8 美元的 ESP32 微控制器上运行](https://github.com/slvDev/esp32-ai) ⭐️ 8.0/10

一位开发者成功在一个成本约 8 美元的 ESP32-S3 微控制器上运行了一个拥有 2890 万参数的语言模型，展示了在超低成本硬件上进行边缘 AI 推理的可能性。 这一突破显著降低了部署 LLM 的硬件门槛，使物联网和消费级设备无需云连接即可实现设备端 AI。它可能带来离线语音助手、智能传感器等新应用。 ESP32-S3 拥有 512KB SRAM 和最高 16MB 闪存，采用 RISC-V 或 Xtensa 处理器。该项目利用每层嵌入技巧减少内存使用，推理过程完全在微控制器上运行。

hackernews · boveyking · 7月25日 18:59 · [社区讨论](https://news.ycombinator.com/item?id=49050512)

**背景**: 边缘 AI 推理是指在本地设备上直接运行机器学习模型而非云端，从而实现低延迟和隐私保护。ESP32 是乐鑫科技开发的低成本、低功耗微控制器系列，集成 Wi-Fi 和蓝牙，广泛用于物联网项目。通常，微控制器的内存和计算能力有限，使 LLM 推理具有挑战性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ESP32">ESP32</a></li>
<li><a href="https://en.wikipedia.org/wiki/Edge_inference">Edge inference</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了每层嵌入技巧，并指出存在类似规模的可行 TTS 模型，暗示 ESP32 上可实现近实时语音合成。有人质疑在闪存后 CPU 上扩展到更大模型的可能性，而其他人则称赞 ESP32-S3 相对于更贵替代品的能力。

**标签**: `#LLM`, `#edge AI`, `#microcontroller`, `#ESP32`, `#machine learning`

---

<a id="item-5"></a>
## [Debian 讨论关于 LLM 贡献的三项提案](https://www.debian.org/vote/2026/vote_002) ⭐️ 8.0/10

Debian 提出了三项提案进行投票，以规范使用大型语言模型 (LLM) 或生成式 AI 创建的贡献，从彻底禁止到有条件接受不等。 这场辩论为开源社区在 AI 生成的代码和内容治理方面树立了先例，因为 Debian 是一个重要的 Linux 发行版。其结果可能影响其他社区驱动的项目。 提案 A 完全禁止所有 LLM 辅助的贡献；提案 B 则允许在严格条件下使用，例如人工审查和许可合规；提案 C 持中立态度，将决定权留给各个维护者。

hackernews · zdw · 7月25日 19:44 · [社区讨论](https://news.ycombinator.com/item?id=49050859)

**背景**: Debian 是一个由志愿者维护的 Linux 发行版，以其严格的自由软件指南著称。Debian 项目通过一般决议来决定重大政策问题，本次投票是该过程的一部分。类似 ChatGPT 的 LLM 可以生成代码和文档，引发了关于作者身份、质量和许可的疑问。

**社区讨论**: 评论者就细节展开辩论，有人认为 LLM 不仅仅是统计模型，也有人引用 Gentoo 的禁令作为先例。还有人担心现有的 Debian 文档是否已经违反了更严格的提案。

**标签**: `#debian`, `#open-source`, `#policy`, `#LLM`, `#AI`

---

<a id="item-6"></a>
## [开放权重 AI 的 Kubernetes 时刻](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

一篇文章认为，开放权重 AI 模型有望像 Kubernetes 成为容器编排领域标准一样，成为行业标准，从而使 AI 基础设施民主化。 这一转变可能降低 AI 开发和部署的门槛，使初创公司和小型组织能够与科技巨头竞争，并通过社区协作促进创新。 该类比表明，正如 Kubernetes 在众多竞争系统中脱颖而出，开放权重模型（权重公开）可能主导专有黑箱 AI，尽管它们缺乏完全开源透明性。

hackernews · tknaup · 7月25日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: 开放权重 AI 指模型的内部参数（权重）公开，但未必包含训练数据或代码等完全开源承诺。Kubernetes 最初由 Google 开发，是一个用于自动化容器化应用程序部署、扩展和管理的开源系统，已成为云原生计算的事实标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told – Open Source Initiative</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论按来源（如中国模型）禁止模型的技术可行性，指出权重只是数字，难以追踪。其他人讨论专有 API 的奇怪定价动态（“代币经济学”），认为开放权重模型提供了成本基准。一名评论者设想公司合作开发共享的开放权重模型，类似于 Linux 模式。

**标签**: `#AI`, `#open-weight`, `#Kubernetes`, `#industry trends`, `#open source`

---

<a id="item-7"></a>
## [Ruff v0.16.0 将默认启用的规则从 59 条增加到 413 条](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0 于 2026 年 7 月 23 日发布，将默认启用的代码检查规则从 59 条增加到 413 条，可能导致现有 CI 流水线中断。该工具现在会自动发现更多问题，包括语法错误和即时运行时错误。 这一变化显著提高了 Ruff 的默认严格度，迫使 Python 开发者处理许多以前被忽略的问题。它可能导致整个生态系统中的 CI 流水线中断，但也提高了代码质量并更早地捕获严重错误。 自 v0.1.0 以来，Ruff 的规则数量从 708 条增加到 968 条，但许多规则并未默认启用。v0.16.0 版本包含了自动修复模式，在 sqlite-utils 项目上使用 --fix --unsafe-fixes 运行时，修复了 1618 个错误中的 1538 个。

rss · Simon Willison · 7月25日 22:44

**背景**: Ruff 是由 Astral 开发的极快 Python 代码检查工具，使用 Rust 编写，旨在替代 Flake8、isort 和 Black 等多个工具。Astral 最近被 OpenAI 收购，Ruff 因其速度和全面的规则集在 Python 生态系统中被广泛使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://astral.sh/ruff">Ruff , an extremely fast Python linter | Astral</a></li>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ ruff : An extremely fast Python linter and code...</a></li>
<li><a href="https://astral.sh/about">About | Astral</a></li>

</ul>
</details>

**标签**: `#Ruff`, `#Python`, `#linting`, `#tooling`, `#Astral`

---

<a id="item-8"></a>
## [Anthropic 发布 Claude Opus 5，主动型 AI 模型，价格仅为 Fable 5 的一半](https://simonwillison.net/2026/Jul/24/introducing-claude-opus-5/#atom-everything) ⭐️ 8.0/10

Anthropic 发布了 Claude Opus 5，这是一款主动型模型，其智能水平接近前沿，而价格仅为 Claude Fable 5 的一半。该模型目前领先于 Artificial Analysis 排行榜，甚至超过了 Fable 5。 此次发布以显著更低的价格提供了接近前沿的智能，使先进 AI 能力更易获取。其主动性和更强的提示注入抵抗力可能为 AI 安全性和自主性树立新标准。 Claude Opus 5 的定价与 Opus 4.8 相同，并提供快速模式，成本为基本模型的两倍。它展现了主动行为：在无法直接查看图纸的情况下，自行编写计算机视觉管道，从原始像素中提取几何信息并重建 3D 模型。

rss · Simon Willison · 7月24日 23:48

**背景**: 前沿智能（Frontier Intelligence）指在复杂任务上达到或超越人类表现、处于能力最前沿的 AI 模型。主动型 AI（Proactive AI）能够预测用户需求并在无需明确提示的情况下采取行动，不同于需要具体指令的传统反应式模型。Anthropic 的 Claude Opus 5 被设计为这样一款主动型模型，同时通过故意不训练其利用漏洞的能力来优先保障安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.alpha-sense.com/resources/research-articles/proactive-ai/">Proactive AI in 2026: Moving Beyond the Prompt</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-proactive-ai-agents-shifting-reactive-anticipatory">What Is Proactive AI? How Agents Are Shifting from Reactive to Anticipatory | MindStudio</a></li>
<li><a href="https://artificialanalysis.ai/leaderboards/models">LLM Leaderboard - Comparison of AI models from OpenAI, Anthropic...</a></li>

</ul>
</details>

**社区讨论**: Boris Cherny 强调，Opus 5 是 Anthropic 迄今为止最难以通过提示注入攻击的模型，这是基于评估和红队测试的结果。这表明模型在抵御对抗性攻击的安全性方面有显著提升，这对在敏感场景中部署 AI 至关重要。

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#Model Release`, `#LLM`

---

<a id="item-9"></a>
## [编译器将计算图转换为无需训练的变压器权重](https://www.reddit.com/r/MachineLearning/comments/1v5fxbe/i_built_a_compiler_that_turns_computation_graphs/) ⭐️ 8.0/10

用户 physicsrob 开发了 Torchwright，这是一个编译器，它接受 Python 计算图并生成标准 Phi-3 变压器的权重，无需任何训练。生成的检查点可以在原生 Hugging Face 中加载，无需自定义代码。 这项工作表明，变压器可以通过算法编程，将可表达的算法与学习到的算法分开，并为标准架构提供手工构建的权重，可能推动机械可解释性和模型设计的发展。它还允许研究人员在不承担训练成本的情况下探索变压器能表示什么。 Torchwright 针对的是微软推出的 38 亿参数小语言模型 Phi-3 架构，并生成与标准 Hugging Face 加载兼容的权重。该编译器基于 RASP 编程语言和 Tracr 编译器，但改进了使用普通 Python 并支持标准架构，无需自定义代码。

reddit · r/MachineLearning · /u/notforrob · 7月24日 16:15

**背景**: RASP（受限访问序列处理语言）是一种旨在离散层次上模拟变压器计算的编程语言，Tracr 是一个将 RASP 程序编译为实际变压器权重的编译器。然而，RASP 不是 Python，Tracr 针对的是自定义架构。Torchwright 通过允许在标准 Python 中定义计算图并直接编译到 Phi-3 等标准架构，解决了这些限制，使得权重可以在不使用任何自定义代码或'trust_remote_code'的情况下，通过原生 Hugging Face 加载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2106.06981">[2106.06981] Thinking Like Transformers</a></li>
<li><a href="https://arxiv.org/pdf/2301.05062v1">Tracr : Compiled Transformers as a</a></li>
<li><a href="https://www.infoworld.com/article/2337210/microsoft-unveils-phi-3-family-of-small-language-models.html">Microsoft unveils Phi - 3 family of small language models | InfoWorld</a></li>

</ul>
</details>

**标签**: `#transformer`, `#compiler`, `#machine learning`, `#weights`, `#no-training`

---

<a id="item-10"></a>
## [AutoDev Studio：开源多智能体 SDLC 工具大幅降低 AI 编码成本](https://www.reddit.com/r/MachineLearning/comments/1v59pal/i_built_an_opensource_multiagent_sdlc_harness/) ⭐️ 8.0/10

开发者发布了 AutoDev Studio，这是一个开源的多智能体软件开发生命周期（SDLC）工具，通过静态分析和嵌入索引构建持久的仓库知识库，与在高达 8.2 万行代码的大型仓库上从头运行 Claude Code 相比，任务成本降低了 7%–75%。 该方法解决了当前 AI 编码代理的一个关键低效问题：每次任务都重新探索代码库。通过重用持久知识库，显著降低了代币使用量和成本，使 AI 辅助软件开发对大型复杂项目更加可行。 AutoDev Studio 使用多智能体工作流，包括独立的 PM、开发、QA 和审阅者代理，并支持多个模型提供商，包括 Anthropic、OpenAI、Groq 和 Ollama。它可以完全免费运行，使用 Groq 的免费层和本地嵌入，并包含看板板和成本跟踪。

reddit · r/MachineLearning · /u/NeighborhoodOwn8510 · 7月24日 12:15

**背景**: 多智能体 SDLC 工具编排专门的 AI 代理处理软件开发的各个阶段，从需求到代码审查。持久仓库知识技术旨在通过创建代码库的可重用表示，避免重复探索。像 Agent Memory 和 Agentskill 等工具是这一方向的早期尝试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.threadai.com/blog/an-inside-look-how-we-built-our-agentic-sdlc-harness">An Inside Look: How We Built Our Agentic SDLC Harness | Thread AI</a></li>
<li><a href="https://seylox.github.io/2026/03/05/blog-agents-meta-repo-pattern.html">In Which We Give Our AI Agent a Map (And It Stops Getting Lost) - Working around the limitations of my intelligence</a></li>
<li><a href="https://dev.to/airscript/turning-repository-knowledge-into-usable-agent-context-4pe4">Turning Repository Knowledge Into Usable Agent Context - DEV Community</a></li>

</ul>
</details>

**标签**: `#AI coding`, `#multi-agent`, `#open-source`, `#software engineering`, `#benchmarks`

---

<a id="item-11"></a>
## [明尼苏达州风能氨厂实现灵活运行](https://ammoniaenergy.org/articles/flexible-renewable-ammonia-demonstrator-now-operational-in-minnesota/) ⭐️ 7.0/10

位于明尼苏达州莫里斯的小型氨厂现已运行，完全由风能驱动，展示了绿色氨和肥料的灵活间歇性生产。 该项目展示了利用间歇性可再生能源进行小规模绿色氨生产的可行性，为化肥生产脱碳和降低农业碳足迹提供了路径。 该厂专为间歇运行设计，无风时停机。它采用水电解制氢和小规模 Haber-Bosch 工艺合成氨，氨储存在储罐中。

hackernews · gritzko · 7月25日 19:30 · [社区讨论](https://news.ycombinator.com/item?id=49050735)

**背景**: 传统的 Haber-Bosch 氨生产过程依赖天然气或煤炭制氢，排放大量 CO2。绿色氨使用可再生能源驱动的电解水制氢替代化石燃料制氢。一个关键挑战是可再生能源（如风能）具有间歇性，而传统 Haber-Bosch 装置需要连续运行。该示范装置通过实现灵活开关机操作来匹配风力可用性，使绿色氨适用于分布式、农场级别的生产。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gpaeurope.com/library/secure/optimizing-green-ammonia-operation-intermittent-mode">Optimizing Green Ammonia Operation in Intermittent Mode</a></li>
<li><a href="https://www.mdpi.com/2076-3298/11/4/71">Flexible Green Ammonia Production Plants: Small-Scale Simulations Based on Energy Aspects</a></li>
<li><a href="https://www.thyssenkrupp-uhde.com/en/products-and-technologies/fertilizer-technologies/ammonia-plants/green-ammonia">Green Ammonia</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为该项目作为技术示范是积极的，但质疑其小规模的经济性。有人指出全球有更大的绿色氨项目，而其他人则看重肥料独立性的价值。间歇运行设计被视为关键创新，但缺乏成本数据使得经济可行性不确定。

**标签**: `#renewable energy`, `#ammonia production`, `#green hydrogen`, `#fertilizer`, `#industrial decarbonization`

---

<a id="item-12"></a>
## [论文长度与机器学习会议中理论研究的评审偏见](https://www.reddit.com/r/MachineLearning/comments/1v6gh43/paper_lengths_and_reasonable_assumptions_in_ml/) ⭐️ 6.0/10

一位研究者分享个人观察，指出顶级机器学习会议中固定的论文长度和无限制的附录可能不公平地惩罚理论论文，因为审稿人越来越多地以数学难度或解释不足为由拒稿。 这一讨论凸显了机器学习会议评审中可能存在的系统性偏见，可能阻碍理论贡献——而理论贡献对科学严谨性和长期进步至关重要，并可能使该领域更偏向实证工作。 作者指出，许多会议规定论文必须自包含，且审稿人不需阅读附录，但理论论文通常需要无法在主要篇幅限制内完全解释的先验知识。

reddit · r/MachineLearning · /u/OutsideSimple4854 · 7月25日 18:48

**背景**: 像 NeurIPS 和 ICML 这样的机器学习会议通常对主论文施加严格的页数限制（例如 8 页），并允许无限附录，但审稿人被指示主要依据主论文做决定。理论论文通常依赖高级数学，使其难以既简洁又自包含。这种页数限制与严格解释需求之间的张力可能导致基于感觉难度而非科学价值被拒稿。

**标签**: `#machine learning`, `#conferences`, `#theoretical ML`, `#research`, `#paper review`

---