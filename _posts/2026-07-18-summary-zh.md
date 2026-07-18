---
layout: default
title: "Horizon Summary: 2026-07-18 (ZH)"
date: 2026-07-18
lang: zh
---

> 从 37 条内容中筛选出 18 条重要资讯。

---

1. [Firefox 编译为 WebAssembly 在浏览器中运行](#item-1) ⭐️ 9.0/10
2. [Inkling：Thinking Machines Lab 发布开放权重 975B MoE 多模态模型](#item-2) ⭐️ 9.0/10
3. [在宜居带岩质系外行星上首次探测到大气](#item-3) ⭐️ 8.0/10
4. [在生产中运行 SQLite 的实用技巧](#item-4) ⭐️ 8.0/10
5. [Moonshot AI 发布 Kimi K3，2.8 万亿参数开放权重模型](#item-5) ⭐️ 8.0/10
6. [GPT-5.6 Codex 漏洞在完全访问模式下删除文件](#item-6) ⭐️ 8.0/10
7. [Linus Torvalds：Linux 不反 AI](#item-7) ⭐️ 8.0/10
8. [欧盟 AI 法案 OpenRAG：结构化的 BGE-M3 嵌入语料库](#item-8) ⭐️ 8.0/10
9. [凯撒护士批评人工智能和监控的影响](#item-9) ⭐️ 7.0/10
10. [递归中心创始人感谢 HN 15 年支持](#item-10) ⭐️ 7.0/10
11. [Zilog Z80 迎来 50 周年，社区充满怀旧回忆](#item-11) ⭐️ 7.0/10
12. [Stereo2Spatial：开源模型将立体声转换为空间音频](#item-12) ⭐️ 7.0/10
13. [Prism 漏洞导致论文编译时泄露](#item-13) ⭐️ 7.0/10
14. [DABSN：一种新的循环语言模型寻求合作者](#item-14) ⭐️ 7.0/10
15. [ExTernD：扩展秩三元分解用于 LLM 后训练量化](#item-15) ⭐️ 7.0/10
16. [LLM 陈词滥调高亮工具](#item-16) ⭐️ 6.0/10
17. [支持颜色的 Mermaid 转 ASCII 艺术工具，基于 WebAssembly](#item-17) ⭐️ 6.0/10
18. [重新思考 AI 记忆：从事实到推理模式](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Firefox 编译为 WebAssembly 在浏览器中运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter 利用 AI 辅助编程将完整的 Firefox/Gecko 浏览器编译为 WebAssembly，使其能够在另一个浏览器中运行，所有网络流量都通过 Wisp 协议在 WebSocket 上进行代理。 这一突破性演示证明，即使是像完整网页浏览器这样的复杂原生应用也可以编译为 WebAssembly，为基于浏览器的模拟、沙箱化和整个操作系统的流式传输开辟了新的可能性。 WebAssembly 二进制文件大小为 233MB（gecko.wasm），另有 18MB 压缩资源；该项目据称消耗了价值约 25,000 美元的 AI token，但由于订阅计划实际成本远低于此。所有网络请求通过 Wisp 协议经 Puter 服务器转发，已验证 HTTPS 流量的端到端加密。

rss · Simon Willison · 7月16日 23:34

**背景**: WebAssembly (WASM) 是一种低级二进制指令格式，可在现代浏览器中以接近原生速度运行，最初设计用于性能密集型任务。将像 Firefox 这样的完整浏览器编译为 WASM 是一项巨大的工程挑战，因为代码库庞大且涉及网络需求；Puter 选择了单进程 Gecko 引擎来简化移植。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>
<li><a href="https://puter.com/app/puter-browser">Puter Browser</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的讨论指出，该项目的服务器必须扩容以应对流量激增，这既体现了技术上的兴趣，也凸显了此类演示的实际挑战。总体情绪非常积极，人们对这一成就的规模感到惊叹。

**标签**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Emulation`, `#WASM`

---

<a id="item-2"></a>
## [Inkling：Thinking Machines Lab 发布开放权重 975B MoE 多模态模型](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

由 Mira Murati 领导的 Thinking Machines Lab 发布了 Inkling，这是一个总参数量 975B（激活参数 41B）的混合专家多模态模型，采用 Apache-2.0 许可，基于 45 万亿 token 的文本、图像、音频和视频数据训练。 作为美国实验室发布的大规模开放权重模型，Inkling 增强了开源 AI 生态系统，并为微调提供了强大基础，特别是通过其 Tinker 平台。它为来自中国及其他开放权重项目提供了有竞争力的替代方案。 Inkling 并非前沿模型，而是用于定制的强大基础模型。该实验室还计划发布 Inkling-Small（总参数量 276B，激活参数 12B），但仍在测试中。模型卡片和训练数据文档非常简略，可能引发透明度方面的担忧。

rss · Simon Willison · 7月16日 15:35

**背景**: 混合专家（MoE）是一种架构，每个 token 仅激活部分参数，从而在高效推理的同时实现较大的总参数量。开放权重模型仅发布训练好的权重，而非完整的训练代码或数据，这与完全开源模型有所区别。此次发布是美中实验室发布越来越大的开放权重模型的趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/mixture-of-experts-architecture-reshaping-how-frontier-ai-lbvrc">Mixture - of - Experts : the architecture reshaping how frontier AI...</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you've been told - Open Source Initiative</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-weights`, `#MoE`, `#multimodal`, `#machine learning`

---

<a id="item-3"></a>
## [在宜居带岩质系外行星上首次探测到大气](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

詹姆斯·韦伯太空望远镜在距离地球 48 光年的红矮星宜居带内，探测到岩质系外行星 LHS 1140b 上存在大气。这是首次在宜居带岩质行星上确认大气存在。 这一发现意义重大，因为开启了研究潜在宜居岩质系外行星大气的大门，对于评估宜居性和寻找生物标志物至关重要。同时也为红矮星周围行星的形成和演化提供了见解。 LHS 1140b 的质量约为地球的 5.6 倍，半径约为地球的 1.7 倍，属于超级地球类别。探测是通过行星凌星时的透射光谱完成的，学界争论的焦点是它究竟是真正的类地行星还是拥有厚大气的迷你海王星。

hackernews · neversaydie · 7月17日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=48947560)

**背景**: 像 LHS 1140 这样的红矮星比太阳更小更冷，其宜居带非常靠近恒星。这种近距离增加了恒星活动和大气的剥离风险。迷你海王星是介于地球和海王星之间、拥有厚氢氦大气的行星。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mini-Neptune">Mini - Neptune - Wikipedia</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - Science@NASA</a></li>

</ul>
</details>

**社区讨论**: 评论者就 LHS 1140b 是类地行星还是迷你海王星展开辩论，有人引用 arXiv 论文称 JWST 发射光谱排除了迷你海王星的可能性。其他人讨论了费米悖论的影响，并建议使用太阳引力透镜望远镜进行未来观测。

**标签**: `#exoplanets`, `#astronomy`, `#astrobiology`, `#JWST`, `#LHS 1140b`

---

<a id="item-4"></a>
## [在生产中运行 SQLite 的实用技巧](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 8.0/10

Julia Evans 发表了一篇博文，分享了运行 SQLite 的实用技巧，包括使用 .expert 命令进行索引建议、使用压缩转储的备份策略以及批量删除技术。 SQLite 被广泛使用，但在生产环境中经常配置不当；这些技巧帮助开发者避免常见问题，如查询缓慢和备份失败，从而提升可靠性和性能。 .expert 模式可根据 SQL 查询自动建议索引；备份策略包括将 .dump 通过管道传输到带有 --rsyncable 标志的 zstd，以实现高效的增量同步。批量删除或预加载 rowid 可以缓解锁定问题。

hackernews · surprisetalk · 7月17日 17:45 · [社区讨论](https://news.ycombinator.com/item?id=48950122)

**背景**: SQLite 是一个自包含、无服务器的 SQL 数据库引擎，数据存储在单个文件中。.expert 命令是一个 CLI 功能，可分析查询并推荐索引以提高性能。预写日志（WAL）模式允许在写入期间进行并发读取，使备份干扰更小。

**社区讨论**: 社区评论强调了 .expert 功能的索引建议、一个用于限定范围 S3 凭证的工具，以及使用 zstd 和 rsyncable 压缩的备份管道。一位用户分享了批量删除策略，指出 SELECT 预加载不会阻塞写入者。

**标签**: `#SQLite`, `#databases`, `#backups`, `#SQL`, `#production`

---

<a id="item-5"></a>
## [Moonshot AI 发布 Kimi K3，2.8 万亿参数开放权重模型](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 8.0/10

Moonshot AI 宣布推出 Kimi K3，一个拥有 2.8 万亿参数的开放权重模型，目前可通过 API 和网页使用，并承诺于 2026 年 7 月 27 日前开放权重。 这是迄今为止最大的开放权重模型，超越了 DeepSeek 的 1.6T 模型，其高定价标志着开放模型市场的转变；鹈鹕基准测试还揭示了如 85 词元隐藏提示等分词特性。 K3 比 K2.6 减少 21%的输出词元，输入/输出每百万词元价格为 3/15 美元，并在前端代码竞技场领先；鹈鹕测试显示由于分词器特性，存在一个 85 词元的隐藏系统提示。

rss · Simon Willison · 7月16日 20:19 · [社区讨论](https://news.ycombinator.com/item?id=48947717)

**背景**: 鹈鹕基准测试是一个非正式测试，由 Simon Willison 要求大语言模型生成一只骑自行车的鹈鹕的 SVG 图像，用于比较模型输出质量和分词行为。Moonshot AI 是一家先前发布过 Kimi K2.6 的中国 AI 实验室。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/pelican-bicycle">GitHub - simonw/pelican-bicycle: LLM benchmark: Generate an SVG of a ...</a></li>
<li><a href="https://huggingface.co/spaces/victor/pelican-benchmark">Pelican Benchmark - a Hugging Face Space by victor</a></li>

</ul>
</details>

**社区讨论**: 评论者质疑鹈鹕测试是否因广受欢迎而被包含在训练集中，注意到 85 词元的隐藏提示，并提出了更严格的基准测试如加入鹈鹕中断的 SWE-bench。还有人建议每个模型运行多次测试以保证一致性。

**标签**: `#AI`, `#LLM`, `#benchmarks`, `#open source`, `#model release`

---

<a id="item-6"></a>
## [GPT-5.6 Codex 漏洞在完全访问模式下删除文件](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

GPT-5.6 的 Codex 工具存在一个漏洞，当模型试图在无沙箱保护的完全访问模式下覆盖 $HOME 环境变量时，会意外删除文件。 这一漏洞突显了 AI 编程代理的关键安全风险，尤其是在授予高级权限时，并强调了沙箱化和自动审查保护措施的必要性。 该漏洞发生在启用完全访问模式、Codex 在无沙箱和自动审查下运行时，模型尝试通过覆盖 $HOME 设置临时目录，但错误地删除了 $HOME。

rss · Simon Willison · 7月16日 17:45

**背景**: Codex 是 OpenAI 的 AI 编程代理，可以在用户机器上执行命令。完全访问模式允许 Codex 无需逐项批准即可执行操作，而沙箱化和自动审查模式提供安全层。$HOME 环境变量通常指向用户的主目录，意外删除可能导致严重数据丢失。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vladimirsiedykh.com/blog/codex-cli-approval-modes-2025">Codex CLI approval modes explained: auto vs read only vs...</a></li>
<li><a href="https://alignment.openai.com/auto-review/">Auto-review of agent actions without synchronous human oversight</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>

</ul>
</details>

**标签**: `#codex`, `#gpt`, `#ai-safety`, `#file-deletion`, `#coding-agents`

---

<a id="item-7"></a>
## [Linus Torvalds：Linux 不反 AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds 在 Linux Media 邮件列表中公开声明 Linux 不是一个反 AI 的项目，认为 AI 工具显然有用，并挑战持不同意见的开发者可以分叉或离开。 作为 Linux 的创建者和顶级维护者，Torvalds 对 AI 工具的权威认可可能改变开源社区对 AI 采纳的态度，影响数千名贡献者和下游项目。 该声明发布在 Linux Media 邮件列表（lore.kernel.org）的一个讨论串中，指出 AI 作为一种工具，其实用性已毋庸置疑，同时承认关于 AI 经济性等其他问题尚待探讨。

rss · Simon Willison · 7月16日 13:26

**背景**: Linus Torvalds 是 Linux 内核的创建者和长期维护者，Linux 内核是无数操作系统的核心。近年来，像 GitHub Copilot 这样的 AI 工具在开源开发中的使用引发了争论，一些开发者因许可或伦理问题反对 AI 生成的代码。Torvalds 的直接干预表明 Linux 项目强烈支持 AI 方向。

**标签**: `#linux`, `#linus torvalds`, `#ai`, `#open source`, `#kernel development`

---

<a id="item-8"></a>
## [欧盟 AI 法案 OpenRAG：结构化的 BGE-M3 嵌入语料库](https://www.reddit.com/r/MachineLearning/comments/1uytlac/eu_ai_act_openrag_933_legally_structured_chunks/) ⭐️ 8.0/10

作者发布了欧盟 AI 法案 OpenRAG，一个可下载的 SQLite 语料库，包含 933 个按法律结构划分的段落，每个段落带有归一化的 1024 维 BGE-M3 嵌入。检索评估显示性能优于基线：文章召回率@20 为 0.541 对比 0.449，QA 命中率@10 为 0.927 对比 0.898。 该资源为法律领域的 RAG 系统开发和评估提供了一个高质量、基于法律结构的语料库，特别适用于欧盟 AI 法案合规。其结构化的分块和嵌入方法可能改进法律 NLP 任务，如条款检索和问答。 语料库的分块基于法规的法律结构（条款、序言、定义、附录点），而非滑动窗口，并包含 EUR-Lex 链接和应用日期元数据。作者透明地公布了评估结果、局限性和方法，并鼓励技术反馈。

reddit · r/MachineLearning · /u/Automatic-Forever-63 · 7月17日 08:18

**背景**: 欧盟 AI 法案（第 2024/1689 号法规）是一部里程碑式的欧洲人工智能监管法律。检索增强生成（RAG）系统结合相关文档检索与语言模型生成答案。BGE-M3 是一个多语言嵌入模型，支持稠密、稀疏和多向量检索。EUR-Lex 是欧盟官方法律数据库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/BAAI/bge-m3">BAAI/bge-m3 · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/EUR-Lex">EUR - Lex - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2603.09435">AI Act Evaluation Benchmark: An Open, Transparent, and Reproducible ...</a></li>

</ul>
</details>

**标签**: `#AI Act`, `#legal-NLP`, `#RAG`, `#embeddings`, `#corpus`

---

<a id="item-9"></a>
## [凯撒护士批评人工智能和监控的影响](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

凯撒医疗集团的护士报告称，人工智能工具和工作场所监控加剧了工作压力并损害了患者护理，尽管有些护士认为医疗大语言模型有价值。 这一争论凸显了效率驱动技术与一线护理质量之间的紧张关系，可能影响医疗系统如何采用人工智能和监控。 文章主要关注对呼叫中心指标和限制护理压力的抱怨，一些评论者认为这被错误地归咎于人工智能，而一个 AI 共情工具试验已于 2024 年终止。

hackernews · gnabgib · 7月17日 22:26 · [社区讨论](https://news.ycombinator.com/item?id=48952880)

**背景**: 大语言模型（LLM）越来越多地用于医疗保健领域，如总结笔记和翻译，旨在减少文书工作负担。然而，工作场所监控技术，例如定位追踪徽章，因增加员工压力而受到批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ai21.com/knowledge/llms-in-healthcare/">LLMs in Healthcare: Applications, Examples, & Benefits | AI21</a></li>
<li><a href="https://ssir.org/articles/entry/the_long_shadow_of_workplace_surveillance">How Workplace Surveillance Technology Harms Workers</a></li>
<li><a href="https://www.sfgate.com/news/bayarea/article/kaiser-nurses-technology-22344290.php">Kaiser nurses say technology is making jobs — and patient care...</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：有人澄清真正的问题是指标和限制护理，而非人工智能；另有人指出护士认为大语言模型工具在翻译和记笔记方面有价值。一位护士的个人经历强调了节省时间和减轻压力。

**标签**: `#AI in healthcare`, `#workplace surveillance`, `#nursing`, `#LLM tools`, `#ethics`

---

<a id="item-10"></a>
## [递归中心创始人感谢 HN 15 年支持](https://news.ycombinator.com/item?id=48949551) ⭐️ 7.0/10

Recurse Center 的创始人公开感谢 Hacker News 在过去 15 年中对这一编程进修项目的支持，并指出 HN 一直是继口碑之后的第二大申请来源。 这一回顾突显了社区驱动的编程进修项目对 3000 多名参与者的持久积极影响，并强调了技术生态系统中非传统、由热情驱动项目的价值。 Recurse Center 是一个免费的、自主编程进修项目，由 YC 校友在创业失败后创立，资金来源于内置的人才招聘机构——公司付费招聘校友，但不会从参与者薪资中扣除。

hackernews · nicholasjbs · 7月17日 16:57

**背景**: Recurse Center（前身为 Hacker School）始于 2010 年，是一个免费的自主编程进修项目，参与者可以制作项目、贡献开源并互相帮助成长。它没有教师或课程，而是强调同伴学习和支持性环境。2012 年在 HN 上的一个帖子帮助它获得了创始人个人网络之外的关注。

**社区讨论**: 评论中前参与者表达了深深的感激和个人转变，分享了他们在 RC 的美好回忆并强烈推荐申请。一些人讨论了其独特的免费模式和社交规则。总体情绪非常积极且怀旧。

**标签**: `#recurse-center`, `#hacker-news`, `#community`, `#programming-retreat`, `#milestone`

---

<a id="item-11"></a>
## [Zilog Z80 迎来 50 周年，社区充满怀旧回忆](https://goliath32.com/blog/z80.html) ⭐️ 7.0/10

Zilog Z80 微处理器于 1976 年 7 月首次发布，如今迎来 50 周年纪念，社区成员分享了怀旧回忆和技术见解。 Z80 是早期个人电脑、游戏机和嵌入式系统的基础组件，影响了几代程序员和工程师。 Z80 由 Federico Faggin 设计，于 1976 年 7 月推出。它与 Intel 8080 二进制兼容，但增加了新的寄存器和指令，并用于 TRS-80、ZX Spectrum 以及许多街机游戏等系统中。

hackernews · st_goliath · 7月17日 19:41 · [社区讨论](https://news.ycombinator.com/item?id=48951461)

**背景**: Z80 是一种 8 位微处理器，以其在 1970 年代末和 1980 年代初个人电脑革命中的作用而闻名。其设计相比前身 Intel 8080 实现了更简单的系统集成和更高的性能，从而在家用电脑和游戏机中得到广泛采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zilog_Z80">Zilog Z80</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zilog">Zilog - Wikipedia</a></li>
<li><a href="https://grokipedia.com/page/Zilog_Z80">Zilog Z80</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了怀旧经历：一位用户回忆起通过组装 Z80 套件学习数字电子技术，另一位回想起通过 ZX-81 手册学习汇编语言，还有一位表达了对该处理器的喜爱，尽管童年时难以掌握汇编语言。

**标签**: `#Z80`, `#CPU`, `#history`, `#retrocomputing`, `#vintage tech`

---

<a id="item-12"></a>
## [Stereo2Spatial：开源模型将立体声转换为空间音频](https://www.reddit.com/r/MachineLearning/comments/1uzevbg/stereo2spatial_convert_stereo_music_tracks_to/) ⭐️ 7.0/10

作者发布了 Stereo2Spatial，一个流匹配扩散模型，可将立体声音乐轨转换为空间化双耳混音，并提供潜变量和波形两个版本，均以 Apache 2.0 许可证开源。 该工具使高质量空间音频转换民主化，让创作者和听众无需专业设备或手动混音即可体验沉浸式声音，可能加速空间音频在音乐领域的普及。 波形版本采用 WavFlow 论文中的振幅提升技术来稳定训练，并支持可选的混音风格条件控制；潜变量版本基于 EAR-VAE 潜空间，但遇到质量瓶颈。

reddit · r/MachineLearning · /u/kittenkrazy · 7月17日 22:55

**背景**: 空间音频（如 7.1.4 环绕声）可创建三维声场，而双耳音频通过头相关传输函数在耳机上模拟这种效果。流匹配扩散是一种生成模型，通过学习匹配概率流将噪声转换为数据。变分自编码器（VAE）可学习音频的压缩潜表示。该模型在 7669 首曲目上训练了 20 天，使用两块 A6000 GPU。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Eps-Acoustic-Revolution-Lab/EAR_VAE">GitHub - Eps-Acoustic-Revolution-Lab/EAR_VAE: This is the ...</a></li>
<li><a href="https://arxiv.org/abs/2509.14912">[2509.14912] Back to Ear: Perceptually Driven High Fidelity ... ϵar-VAE Demo earlab/EAR_VAE at main - Hugging Face EAR_VAE/docs/index.html at main · Eps-Acoustic ... - GitHub Back to Ear: Perceptually Driven High Fidelity Music ...</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#audio processing`, `#spatial audio`, `#diffusion models`, `#VAE`

---

<a id="item-13"></a>
## [Prism 漏洞导致论文编译时泄露](https://www.reddit.com/r/MachineLearning/comments/1uz75qt/prism_accidentally_leaked_d/) ⭐️ 7.0/10

Prism 平台的一个 bug 导致在编译时返回了他人的论文，造成了意外的论文泄露。平台在被标记后的 10 分钟内就被关闭。 此事件凸显了协作式机器学习平台中的严重隐私风险，泄露的论文可能危及双盲评审或知识产权。虽然平台的快速响应显示了良好的做法，但用户仍担心自己论文的安全性。 该 bug 最初在 Twitter 上被报告，Prism 网站在 10 分钟内被关闭。用户担心他们自己的论文也可能已经被泄露。

reddit · r/MachineLearning · /u/Few-Monitor5103 · 7月17日 17:59

**背景**: Prism 是机器学习社区中用于编译论文的平台，可能用于 LaTeX 或格式化工具。编译过程中的意外泄露可能暴露未发表的作品，这在盲审过程中至关重要。

**标签**: `#machine learning`, `#privacy`, `#paper leak`, `#Prism`, `#bug`

---

<a id="item-14"></a>
## [DABSN：一种新的循环语言模型寻求合作者](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 7.0/10

作者介绍了一种名为 DABSN 的新型循环架构，并发布了预印本和开源代码（PyTorch、C++、Triton）。一个 24M 参数的语言模型在 1B token 上训练后展现出有希望的结果，作者正在寻求合作者进行扩展和独立评估。 DABSN 可能通过高效的循环计算挑战 Transformer 在语言建模中的主导地位，特别是在长上下文任务中。开放的合作可能加速其验证和采用。 该架构在 MQAR、Copy、Key-Value retrieval 和 A5/60 等基准上进行了评估。代码库包含用于 GPU 效率的自定义 Triton 内核。作者使用 GPT-2 分词器在 1B token 上训练了一个 24M 参数模型。

reddit · r/MachineLearning · /u/BleedingXiko · 7月16日 19:17

**背景**: 循环神经网络（RNN）曾主导序列建模，但被 Transformer 超越。最近，状态空间模型（如 Mamba）和其他循环变体因其线性时间推理而重新受到关注。MQAR（多查询关联回忆）基准测试模型从上下文中执行多个关联查找的能力。Triton 是一种基于 Python 的语言，用于编写高效的 GPU 内核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-query-associative-recall-mqar">MQAR: Multi-Query Associative Recall - emergentmind.com</a></li>
<li><a href="https://triton-lang.org/main/">Welcome to Triton ’s documentation! — Triton documentation</a></li>

</ul>
</details>

**标签**: `#recurrent neural networks`, `#language modeling`, `#deep learning`, `#open source`, `#collaboration`

---

<a id="item-15"></a>
## [ExTernD：扩展秩三元分解用于 LLM 后训练量化](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 7.0/10

研究人员提出了 ExTernD，一种后训练三元分解方法，将权重矩阵分解的内秩扩展至超越全秩，使得精度可接近任何目标量化水平，仅需中等程度的 VRAM 增加。 这解决了大语言模型（LLM）中固定大小三元量化的根本限制，为实现极低位宽量化（如 2 比特等效）且不严重损失精度提供了途径，从而可能大幅降低 LLM 部署的内存和推理成本。 ExTernD 将每个权重矩阵 A 分解为 B·diag(D)·C，其中 B 和 C 的元素属于{-1, 0, +1}的三元矩阵，D 是实值缩放向量。内秩 k 设为 mu*min(m,n)，其中 mu>1，从而超越全秩的分量可纠正量化误差。该方法使用 Shannon 熵公平地比较每权重比特数。

reddit · r/MachineLearning · /u/LMTLS5 · 7月16日 13:31

**背景**: 后训练量化（PTQ）通过将预训练权重转换为较低精度格式来减小模型大小并加速推理，无需重新训练。三元量化将权重限制为-1、0、+1，提供极致压缩但常导致精度下降。ExTernD 基于类似 SVD 的矩阵分解方法，但使用三元因子和扩展秩来更好地保持精度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.13511">[2607.13511] ExTernD: Expanded-Rank Ternary Decomposition ...</a></li>
<li><a href="https://arxiv.org/html/2607.13511v1">ExTernD: Expanded-Rank Ternary Decomposition Ternary LLM PTQ ...</a></li>

</ul>
</details>

**标签**: `#LLM quantization`, `#ternary decomposition`, `#post-training quantization`, `#model compression`, `#machine learning`

---

<a id="item-16"></a>
## [LLM 陈词滥调高亮工具](https://simonwillison.net/2026/Jul/17/llm-cliche-highlighter/#atom-everything) ⭐️ 6.0/10

Simon Willison 创建了一个网络工具，可高亮显示 LLM 生成文本中常见的十种陈词滥调，该工具通过 Fable 5 的 AI 辅助氛围编码构建。 该工具有助于读者和内容策展人快速识别 AI 写作模式，促进对 AI 生成内容的批判性消费，并可能减少通用、充满陈词滥调文本的传播。 该高亮工具可通过 Jina AI 的读取服务加载并分析任意 URL，目前可标记 11 种模式（包括“是真实的且”、“值得命名”），并清晰显示每句的匹配计数。

rss · Simon Willison · 7月17日 12:11

**背景**: LLM 经常重复使用公式化短语和陈词滥调，使其输出易于识别。氛围编码（Vibe coding）是由 Andrej Karpathy 于 2025 年提出的术语，描述了一种 AI 从自然语言提示生成代码的开发方式，且通常不加仔细审查便接受。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>
<li><a href="https://jina.ai/about-us/">About Jina AI</a></li>

</ul>
</details>

**标签**: `#LLM`, `#AI detection`, `#writing`, `#clichés`, `#tools`

---

<a id="item-17"></a>
## [支持颜色的 Mermaid 转 ASCII 艺术工具，基于 WebAssembly](https://simonwillison.net/2026/Jul/16/mermaid-ascii/#atom-everything) ⭐️ 6.0/10

Simon Willison 将 Go 库 AlexanderGrooff/mermaid-ascii 编译为 WebAssembly，创建了一个基于浏览器的工具，可将 Mermaid 图转换为彩色的 ASCII 艺术。 该工具使 Mermaid 图在终端或代码注释等纯文本环境中可用，同时通过 WebAssembly 方法让基于 Go 的复杂渲染无需服务器即可在浏览器中高效运行。 该 Go 库在 ASCII 输出中支持颜色，这是此前基于 Rust 的实现所不具备的，而 WebAssembly 编译则实现了填充和框填充等交互式调整。

rss · Simon Willison · 7月16日 14:57

**背景**: Mermaid 是一种基于 JavaScript 的开源图表工具，可根据文本描述生成图表。WebAssembly (Wasm) 是一种可移植的二进制格式，允许来自 Go 或 Rust 等语言的高性能代码在网页浏览器中运行，实现无服务器执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mermaid_(software)">Mermaid (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>

</ul>
</details>

**标签**: `#mermaid`, `#ascii-art`, `#webassembly`, `#developer-tools`

---

<a id="item-18"></a>
## [重新思考 AI 记忆：从事实到推理模式](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 6.0/10

一篇 Reddit 帖子提出，AI 记忆系统应从存储描述性事实进化为推断更高层次的推理模式，如解释框架和推理风格。这将把持久上下文从笔记集合转变为用户理解问题方式的演化模型。 这一概念性转变可能影响未来 AI 架构，使其专注于建模用户推理风格，从而实现更个性化和自适应的 AI 交互。它挑战了当前记忆系统对事实回忆的普遍侧重。 该帖子对比了描述性记忆（例如“用户对经济学感兴趣”）与推理性记忆（例如“用户通过激励机制解释经济学现象”）。它质疑这种表征是否能从足够强大的 AI 系统中自然涌现，还是需要与当今检索和摘要方法根本不同的架构。

reddit · r/MachineLearning · /u/Boris_Ljevar · 7月16日 16:00

**背景**: 当前 AI 代理通过保存的记忆、对话摘要、用户偏好和项目笔记来维持持久上下文，这些主要是描述性的。像 Mem0、Zep 和 Letta 等框架旨在通过更丰富的上下文来改进这一点。该帖子建议进一步演化：系统不仅仅是记住事实，还可以推断更高层次的模式，如解释框架和推理风格，从而有效构建用户如何解释问题的演化模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vectorize.io/articles/best-ai-agent-memory-systems">Best AI Agent Memory Systems in 2026: 8 Frameworks Compared</a></li>
<li><a href="https://aiagentmemory.org/articles/ai-memory-frameworks/">AI Memory Frameworks: Building Persistent Recall for …</a></li>

</ul>
</details>

**标签**: `#AI memory`, `#persistent context`, `#machine learning`, `#reasoning patterns`, `#abstraction`

---