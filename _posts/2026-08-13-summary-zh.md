---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> 从 34 条内容中筛选出 21 条重要资讯。

---

1. [Tailscale 将数据库损坏追溯到 16 年前的 SQLite WAL 重置 Bug](#item-1) ⭐️ 9.0/10
2. [Qwen 发布 2.4 万亿参数 MoE 模型 Qwen3.8-2.4T-A95B](#item-2) ⭐️ 9.0/10
3. [研究人员从专有 LLM API 中恢复机密思维链痕迹](#item-3) ⭐️ 9.0/10
4. [DeepSeek V4 Pro 0813](#item-4) ⭐️ 8.0/10
5. [HTML over WebSockets：极简 JavaScript 构建实时 SPA](#item-5) ⭐️ 8.0/10
6. [uBlock Origin 放弃屏蔽 Facebook 广告的战斗](#item-6) ⭐️ 8.0/10
7. [xAI 发布新一代前沿 AI 模型 Grok 4.6](#item-7) ⭐️ 8.0/10
8. [为什么小尺寸 JPEG 在 Chrome 中看起来不一样：缩放解码解析](#item-8) ⭐️ 8.0/10
9. [工程师警告：AI 辅助编程或创造无人能理解的系统](#item-9) ⭐️ 8.0/10
10. [自然语言文本不存在无损变换](#item-10) ⭐️ 8.0/10
11. [Adam 的逐坐标缩放破坏隐式低秩偏好，旋转不变优化器保留该偏好](#item-11) ⭐️ 8.0/10
12. [解耦下降：借助 AMP Onsager 修正精确同步训练与测试误差](#item-12) ⭐️ 8.0/10
13. [Zed 推出 Delta，支持多人协作的 AI 智能体编程](#item-13) ⭐️ 7.0/10
14. [众包摄像头网页追踪 2026 年日食](#item-14) ⭐️ 7.0/10
15. [诚实的 CS 会议排名：按旅行吸引力排序](#item-15) ⭐️ 7.0/10
16. [AmigaDOS 核心开发者 Tim King 去世](#item-16) ⭐️ 6.0/10
17. [Discovered Materials（YC P26）用 AI 智能体发现半导体新材料](#item-17) ⭐️ 6.0/10
18. [datasette-upload-dbs 0.5a0 新增正式 API，支持上传与原子替换数据库](#item-18) ⭐️ 6.0/10
19. [审稿人质疑 AAAI 2027 无代码论文](#item-19) ⭐️ 6.0/10
20. [开发者围绕 CPU 优先推理重建脉冲语言模型 NORD](#item-20) ⭐️ 6.0/10
21. [为带预览随机事件的随机合并谜题寻求 RL 与规划建议](#item-21) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Tailscale 将数据库损坏追溯到 16 年前的 SQLite WAL 重置 Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 9.0/10

Tailscale 将控制平面 SQLite 数据库反复出现的损坏追溯到了 SQLite WAL 重置逻辑中的一个竞态条件，SQLite 团队估计该问题已存在至少 16 年。他们还资助了一个开源 VFS 调试垫片，用来帮助定位这个 Bug。 这是对一个长期数据库 Bug 的罕见而深入的根本原因分析，可能影响任何在 WAL 模式下使用 SQLite 且符合特定 checkpoint 行为的应用。该公司资助开源调试工具的决定也为生态系统的可持续性树立了积极榜样。 该 Bug 在检查点（checkpoint）期间触发，可能导致已提交的事务从数据库中消失。单写入者设计并不能避免它，因为竞态涉及多个数据库连接在协调 WAL 重置。Tailscale 的 VFS 垫片现已开源，可用于排查类似问题。

hackernews · ropbear · 8月12日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49272832)

**背景**: SQLite 使用预写日志（WAL）来提供崩溃安全和并发能力，并通过一个特殊的 WAL 索引文件来协调读写。在 checkpoint 期间重置 WAL 的方式中，一个微妙的竞态可能导致数据库状态不一致。SQLite 是使用最广泛的嵌入式数据库之一，因此即使一个很少触发的 Bug 也可能影响众多部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL - Reset bug</a></li>
<li><a href="https://www.youngju.dev/blog/2026-07-16-sqlite-wal-reset-bug.en">The SQLite WAL - Reset Bug: A Data Corruption Race That Hid for 15...</a></li>
<li><a href="https://zeli.app/en/story/49272832">Tailscale Traces Database Corruption to 16y/o SQLite WAL - Reset Bug</a></li>

</ul>
</details>

**社区讨论**: 评论者赞赏这篇博文清晰易懂，并强调了这种有趣的开源资助模式；一些人起初对单写入者设计为何仍会出现竞态感到困惑。还有评论指出 SQLite 庞大的测试套件与 Dijkstra“测试只能证明 Bug 的存在，无法证明其不存在”这一观点之间的哲学张力。

**标签**: `#sqlite`, `#databases`, `#bug`, `#tailscale`, `#open-source`

---

<a id="item-2"></a>
## [Qwen 发布 2.4 万亿参数 MoE 模型 Qwen3.8-2.4T-A95B](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

阿里巴巴通义千问团队发布开放权重 MoE 模型 Qwen3.8-2.4T-A95B，总参数 2.4 万亿，每个 token 激活约 950 亿参数，同时提供 FP8 版本。模型卡声称性能达到前沿水平，社区成员称其介于 Opus 4.8 与 Fable 5 之间。 这是迄今发布的最大开放权重模型之一，将接近前沿的能力带到开放生态，并加剧了中国 AI 实验室之间的竞争。该发布对希望自建基础设施部署前沿级模型的研究者与企业意义重大，但巨大的内存需求构成了显著的入门门槛。 该模型包含 512 个路由专家，每个 token 激活其中 10 个外加一个共享专家，基于 92 层混合注意力骨干架构，上下文长度 256K。初始版本仅提供 bf16 和 FP8，若要 4bit 量化需使用大量校准数据进行训练后量化；bf16 完整模型占用约 4.9TB 内存。

hackernews · Philpax · 8月12日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=49273478)

**背景**: 混合专家（MoE）架构通过路由器为每个 token 选取一小部分专门的“专家”，从而在总参数量极大的情况下保持计算量接近小得多的模型。量化（例如 FP8）会降低数值精度以缩小内存占用并加速推理，但会损失一定精度。这些技术之所以重要，是因为前沿模型已大到无法在常规单 GPU 上部署，高效部署成为工程挑战。Qwen 是阿里巴巴的开放权重 LLM 系列，而 Qwen3.8-2.4T-A95B 是商业版 Qwen3.8-Max 的开放权重版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/serve-qwen3-8-2-4t-a95b-a-2-4t-parameter-model-with-configurable-reasoning-on-nvidia-gb300-nvl72/">Serve Qwen3.8-2.4T-A95B, a 2.4T-Parameter Model, with Configurable Reasoning on NVIDIA GB300 NVL72 | NVIDIA Technical Blog</a></li>
<li><a href="https://recipes.vllm.ai/Qwen/Qwen3.8-2.4T-A95B">Qwen/Qwen3.8-2.4T-A95B — 2.4T / 95B active · MOE · 256K ctx</a></li>
<li><a href="https://localmodel.run/guides/mixture-of-experts">Mixture of experts (MoE) explained for local LLMs · localmodel.run</a></li>

</ul>
</details>

**社区讨论**: 社区评论整体偏技术性，主要关注部署难点：该模型发布时比 Kimi k3 更大，且没有经过 QAT 的 4bit 权重，需要资金雄厚的机构自行量化。有人对 1bit 量化后约 397GB 的体积感到兴奋，认为可以在高端工作站上获得 Opus 4.5 级别的性能；也有人指出开放权重版缺少 Qwen3.8-Max 的视觉输入与 1M 上下文能力。还有少数用户质疑实际性能是否匹配基准测试宣称的水平。

**标签**: `#LLM`, `#Qwen`, `#MoE`, `#AI`, `#HuggingFace`

---

<a id="item-3"></a>
## [研究人员从专有 LLM API 中恢复机密思维链痕迹](https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/) ⭐️ 9.0/10

一篇来自 stolen-thoughts.com 的新论文揭示，Anthropic、OpenAI 和 Google API 返回的加密思维链模块可被重放到同系列的较弱模型中，并通过越狱攻击，以明文恢复较强模型的私有推理过程。所有厂商均已确认该报告，目前该攻击似乎已被修复。 这表明专有 LLM API 在加密思维链推理时存在严重安全缺陷，影响 Anthropic、OpenAI 和 Google。它证明加密的推理轨迹并不安全，可被重放攻击利用，对 AI 隐私、安全和知识产权都有重大影响——隐藏推理内容可被提取，用于蒸馏模型能力或发现漏洞。 该漏洞源于同一系列的所有模型使用相同的加密密钥，因此前沿模型的轨迹可以被重放到最弱的同系列模型中。Claude Haiku 4.5 最容易被攻击，攻击者使用转录提示和预填充的"<thinking-copy>"前缀；各供应商已修补此问题，而该前缀功能在 4.6 中已被移除，但在 Haiku 4.5 中仍有效。

rss · Simon Willison · 8月11日 22:40

**背景**: 思维链（CoT）推理是一种让 LLM 在给出最终答案前逐步生成中间推理的技术，能提高复杂任务的表现。为了保护专有机密和防止蒸馏，一些 API 供应商会对这些中间推理令牌进行加密。重放攻击是在不同上下文中重用已捕获的消息来欺骗系统；越狱则是通过精心构造的提示绕过安全护栏，让模型泄露隐藏信息。这些技术结合起来，使攻击者能够解密隐藏的思维痕迹。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.11903">[2201.11903] Chain - of - Thought Prompting Elicits Reasoning in ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Replay_attack">Replay attack - Wikipedia</a></li>
<li><a href="https://arxiv.org/pdf/2310.08419">Jailbreaking Black Box Large Language Models in</a></li>

</ul>
</details>

**标签**: `#LLM security`, `#chain-of-thought`, `#AI safety`, `#proprietary APIs`, `#research`

---

<a id="item-4"></a>
## [DeepSeek V4 Pro 0813](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek V4 Pro 0813 已发布，早期社区测试显示其性能强劲，且对开发工作负载具有高性价比。

hackernews · explosion-s · 8月12日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=49274600)

**标签**: `#AI`, `#DeepSeek`, `#Large Language Models`, `#Machine Learning`

---

<a id="item-5"></a>
## [HTML over WebSockets：极简 JavaScript 构建实时 SPA](https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/) ⭐️ 8.0/10

这篇文章介绍了 HTML over WebSockets 技术，这是一种用极少量客户端 JavaScript 构建实时单页应用（SPA）的方法。它描述了一种双向变体：服务端生成 HTML 片段并通过 WebSocket 连接发送，而客户端只需运行一个轻量的 DOM 远程操作脚本。 这一观点挑战了传统的以 JavaScript 为中心的 SPA 架构，通过将渲染逻辑保留在服务端，有望简化开发。它也引发了业界关于何时使用 WebSocket，何时使用 Server-Sent Events（SSE）或 REST 的持续讨论，影响开发者设计实时功能的方式。 文章强调一种“单一语言、无契约、单一渲染引擎”的方法。批评者指出，对于单向服务端推送，SSE 更简单且运行成本更低；只有在需要双向低延迟通信时才需要 WebSocket。此外，htmx 或 Blazor 等替代方案已经实现了类似模式。

hackernews · redbell · 8月12日 16:51 · [社区讨论](https://news.ycombinator.com/item?id=49275335)

**背景**: 传统 SPA（单页应用）在首次加载 HTML 页面后，通过 JavaScript 更新视图，通常从 REST API 获取 JSON 数据。SSE（Server-Sent Events）允许服务端通过单一长连接 HTTP 连接向客户端推送更新，而 WebSocket 则提供全双工持久通道。HTML over WebSockets 更进一步，发送预渲染的 HTML 片段而非 JSON，因此客户端不需要复杂框架或状态管理。这一概念与 Phoenix LiveView、Blazor Server 或 htmx 等相似，其源头可追溯到 Chris McCord 在 Rails 中开发的早期原型“Sync”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/">HTML over WebSockets: real-time SPAs with barely any JavaScript | Andros Fenollosa</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events">Using server - sent events - Web APIs | MDN</a></li>
<li><a href="https://www.reddit.com/r/programming/comments/lsgimx/the_future_of_web_software_is_htmloverwebsockets/">r/programming on Reddit: The Future of Web Software Is HTML-over-WebSockets</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：一些人主张在大多数场景下使用 SSE 和 Fetch，认为如果只需要服务端推送，WebSocket 增加了不必要的复杂度。另一些人则提到 Blazor Server 和 htmx 等实际例子，并指出 Chris McCord 更早的工作在历史上已有先例；还有人附上了一篇批评性回应文章的链接。

**标签**: `#WebSockets`, `#Real-time`, `#SPA`, `#JavaScript`, `#Server-rendered`

---

<a id="item-6"></a>
## [uBlock Origin 放弃屏蔽 Facebook 广告的战斗](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 8.0/10

uBlock Origin 的志愿者开发者宣布，他们将不再主动尝试屏蔽 Facebook 上的广告，理由是平台不断变化的反广告屏蔽技术。开发团队在公告中将 Facebook 称为“令人厌恶的反用户网站”。 这标志着最流行的广告屏蔽器之一的重大挫败，影响了数以千万计依赖 uBlock Origin 保持 Facebook 信息流干净的用户。它凸显了小型开源团队难以跟上大型平台反广告屏蔽措施的困境，对用户隐私和广告屏蔽军备竞赛具有更广泛的影响。 uBlock Origin 是一款免费开源浏览器扩展，截至 2026 年 6 月拥有超过 2900 万 Chrome 用户和 1060 万 Firefox 用户。这一决定仅影响 Facebook；该扩展将继续在其他网站上屏蔽广告，不过 Facebook 本身警告称，广告屏蔽器可能导致其网站无法正常运行。

hackernews · Markoff · 8月12日 11:28 · [社区讨论](https://news.ycombinator.com/item?id=49270726)

**背景**: uBlock Origin 是一款广泛使用的内容过滤浏览器扩展，可屏蔽广告、跟踪器和恶意 URL。广告屏蔽器的工作原理是将页面元素与过滤列表进行比较，但像 Facebook 这样的平台使用混淆技术和快速变化的标记来规避这些列表，从而形成一场持续的猫鼠游戏。该公告发布在 uBlock Origin 的 subreddit 上，一位团队成员解释了为什么 Facebook 特别难以持续屏蔽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">UBlock Origin</a></li>
<li><a href="https://piunikaweb.com/2026/08/10/ublock-origin-facebook-ads-not-blocking/">Seeing ads on Facebook even with uBlock Origin? Here's why</a></li>

</ul>
</details>

**社区讨论**: 评论者大多支持这一决定，一些人预测这场军备竞赛最终将以基于计算机视觉的广告检测结束，即在广告上绘制方框。其他人质疑 Facebook 为何要花费如此多精力绕过广告屏蔽器，因为安装了屏蔽器的用户本来就不太可能点击广告，还有一些人认为唯一的真正解决方案是彻底离开 Facebook。

**标签**: `#ad-blocking`, `#facebook-ads`, `#privacy`, `#ublock-origin`, `#web-platforms`

---

<a id="item-7"></a>
## [xAI 发布新一代前沿 AI 模型 Grok 4.6](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI 于 2026 年 8 月 7 日发布了新一代前沿 AI 模型 Grok 4.6，官方称其相较 Grok 4.5 在相同价格下实现了显著改进。基准测试报告显示其 ELO 约为 1753，在多数基准上超过 GPT-5.6-Sol，而定价约为同类前沿模型的一半。 Grok 4.6 增强了 xAI 在前沿 AI 竞赛中的地位，通过以更低价格提供强劲性能，对其他主要 AI 实验室形成竞争压力。对开发者和企业来说，它为高要求的 AI 工作负载提供了一个高性价比选择，可能重塑整个生态系统的定价与选型。 据报道，Grok 4.6 是一个 1.5 万亿参数模型，通过改进的有监督微调和强化学习进行训练。它可通过 xAI 的 API 使用（包括代码等任务），官方称其在处理更具挑战性的任务方面比 Grok 4.5 有显著提升。

hackernews · iLuddite · 8月12日 15:32 · [社区讨论](https://news.ycombinator.com/item?id=49274027)

**背景**: 前沿 AI 模型是指当前可获得能力最强的超大规模系统，能够在各种任务上达到或超越其他现有模型。Grok 是 xAI 推出的大型语言模型系列，已集成到 X 平台，并通过 API 提供服务。Grok 4.6 的发布延续了各大 AI 实验室快速迭代的趋势，基准测试成绩与成本正成为关键竞争点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.basenor.com/blogs/news/xai-launches-grok-4-6-1753-elo-half-the-price-of-rival-frontier-models">xAI Launches Grok 4.6: 1753 ELO, Half the Price of Rival Frontier Models</a></li>
<li><a href="https://kie.ai/blog/what-is-grok-4-6">What Is Grok 4.6? xAI's 1.5T-Param Model Explained</a></li>
<li><a href="https://docs.x.ai/developers/models">Models - Docs - SpaceXAI</a></li>

</ul>
</details>

**社区讨论**: 社区反应多样但总体积极：一些用户称赞 Grok 4.6 速度快、简洁，拥有类似 Fable 的智能，另一些人则质疑各大实验室为何在两个月内突然达到 Fable 水平，怀疑存在基准作弊或蒸馏。一个显著抱怨是 API 会添加默认系统提示，覆盖用户指令并拒绝讨论系统提示，令部分用户感到困扰。

**标签**: `#AI models`, `#Grok`, `#xAI`, `#benchmarks`, `#machine learning`

---

<a id="item-8"></a>
## [为什么小尺寸 JPEG 在 Chrome 中看起来不一样：缩放解码解析](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

一位开发者发现小尺寸 JPEG 在 Chrome 和 Firefox 中的渲染效果不同，并将其归因于 Chrome 的缩放解码优化。在缩小 JPEG 时，Chrome 通过 libjpeg-turbo 使用部分 IDCT 缩放，只解码低频数据，导致图像看起来略粗或更模糊。 这一点很重要，因为 Web 开发者和设计师依赖跨浏览器渲染的一致性来显示图标和小图像；一项性能优化悄悄改变了视觉输出。该问题也会影响内嵌 Chromium 的 Electron 应用，并凸显了解码速度与图像保真度之间的普遍权衡。 该优化特指对 JPEG 进行缩小解码：Chrome 通过 libjpeg-turbo 的缩放 IDCT 路径跳过高频 DCT 系数，从而改变小尺寸下的边缘渲染。评论者指出 PNG 也会出现同样问题，并且 Mozilla 正在 Firefox bug 2033250 中跟踪类似的缩放解压工作；浏览器之间不同的缩放算法也会导致可见差异。

hackernews · gutechh · 8月12日 14:00 · [社区讨论](https://news.ycombinator.com/item?id=49272549)

**背景**: JPEG 压缩的原理是将图像块转换为 DCT 系数，其中低频系数承载大部分视觉信息，高频系数承载细节。以全分辨率解码所有系数开销较大，因此 libjpeg-turbo 提供缩放解码模式，只计算其中一部分，以牺牲部分精度换取速度。Chrome 和 Firefox 等浏览器在何时以及如何使用这类优化上做出了不同选择，这就是同一张 JPEG 在不同浏览器中看起来不一样的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zeli.app/en/story/49272549">Chrome 's Clever JPEG Decoding Trick Makes Tiny Images Look... | Zeli</a></li>
<li><a href="https://issues.chromium.org/issues/381913638">Releative with 40946711: support scaled decode for... - Chromium</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者普遍确认了该问题，其中一位指出 PNG 也存在同样问题，并且 Chrome 的优化破坏了 Electron 应用图标，导致他们推迟升级。其他人则讨论 Chrome 较模糊的输出和 Firefox 更锐利但容易出现振铃效应的输出哪个更好；还有评论者指出文章只解释了 Chrome 一方，询问 Firefox 是完整渲染后再缩放，还是采用了其他部分渲染方式。

**标签**: `#JPEG`, `#Chrome`, `#image scaling`, `#browser rendering`, `#web performance`

---

<a id="item-9"></a>
## [工程师警告：AI 辅助编程或创造无人能理解的系统](https://simonwillison.net/2026/Aug/12/florian-herrengt/) ⭐️ 8.0/10

Florian Herrengt 的博客文章被 Simon Willison 引用，警告 AI 驱动的开发可能产生极其复杂、多层嵌套、没有任何单个开发者能完全理解的系统。文中情景描述了一个团队反复让 Claude 等 AI 工具修复 bug，却无人掌握数据流向。 随着 Claude Fable 5 等 AI 编程代理加速功能开发，这引发了关于软件项目长期可维护性与“认知债务”的紧迫担忧。同时它也对中级软件工程师的岗位构成挑战，因为他们可能失去传统上调试和演进复杂系统所需的深层系统性理解。 该引文特别提到“Fable”这个 AI 无法找出反复出现的 bug，并描述一位开发者在被问及数据来源时回答“让我问问 Claude”。文章标题提出“AI 正在移除软件工程的中产阶级”这一说法，直指中级工程岗位及隐性知识的流失。

rss · Simon Willison · 8月12日 15:08

**背景**: AI 辅助编程工具已从简单的自动补全发展为能构建整个功能或应用的自主代理，例如 Anthropic 的 Claude Fable 5，它能在 Claude Code 中处理复杂的多代理工作流。这一转变意味着开发者越来越多地审查生成的代码，而非逐行编写，从而降低他们对系统内部逻辑的熟悉度。“认知债务”指的是无法解释或难以理解的代码不断累积，随着人类理解力落后于机器生成的复杂性而逐渐成为维护负担。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://workingnotworking.com/fable-ai-shift-from-prompting-to-full-software-building/">Fable AI Rapid Adoption Signals the Shift to Full Software Building</a></li>

</ul>
</details>

**标签**: `#AI`, `#software engineering`, `#code quality`, `#developer experience`, `#future of work`

---

<a id="item-10"></a>
## [自然语言文本不存在无损变换](https://simonwillison.net/2026/Aug/11/there-are-no-lossless-transformations-of-natural-language-text/) ⭐️ 8.0/10

苏菲·阿尔珀特发布了一项关于工程师使用 AI 写作的内部政策，指出大语言模型对自然语言的改写本质上是有损的，作者必须对每一句话负责。西蒙·威利森将这一政策作为负责任使用 AI 的宝贵参考予以推介。 这一观点之所以重要，是因为它为采用 AI 写作工具的工程团队提供了实用指导，强调作者责任以及 AI 改写文本时信息丢失的风险。它回应了 AI/ML 和软件工程社区对 AI 辅助沟通的可靠性和真实性的日益关注。 阿尔珀特的政策指出，每一次改写和重新措辞都会改变含义，尤其是当改写由不具备作者思维模型的实体完成时。她还强调，如果审阅者问及某一行内容，不能以“这是 AI 写的，忽略即可”来回应。

rss · Simon Willison · 8月11日 23:48

**背景**: 无损变换的概念源于信息论，如果过程中不丢失任何信息，则该变换是无损的。大语言模型（LLM）是在大量文本上训练的 AI 系统，能够生成、总结和翻译语言，但它们缺乏作者的具体意图和背景，因此它们的变换可能是有损的。这种对比凸显了使用 AI 进行需要精确性和个人风格的写作任务时的根本挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model</a></li>
<li><a href="https://diversedaily.com/exploring-absolute-information-conservation-a-comprehensive-analysis/">Exploring Absolute Information Conservation: A Comprehensive...</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#writing`, `#engineering-practices`, `#ethics`

---

<a id="item-11"></a>
## [Adam 的逐坐标缩放破坏隐式低秩偏好，旋转不变优化器保留该偏好](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

一篇 Reddit 分析指出，Adam 的逐坐标二阶矩缩放会破坏梯度下降在分解模型中表现出的隐式低秩偏好，而 Muon、Shampoo 等旋转不变优化器则能保留该偏好。作者在欠定矩阵感知任务上测试了九种更新规则，并展示从逐坐标 Adam 到共享标量 Adam 的单参数族可以单调恢复该偏好。 这项分析的重要意义在于，它找出了一种机制性属性——对坐标基底的依赖——区分了能保留梯度下降有益归纳偏置的优化器和会丢失该偏置的优化器。该结果可为矩阵恢复和深度线性网络中的优化器选择与设计提供指导，并指出 Muon 的混合表现仍是一个开放问题。 实验在匹配训练损失的条件下比较了 GD、共享标量 Adam、Muon 和 Shampoo（保留偏置）与 Adam、RMSProp、Lion、signum 和 Adafactor（丢失偏置）。作者还指出，动量并未被理论覆盖，且在高光谱数据上 43-44%的留出误差降低在每种方法自行选择学习率时会显著缩小。

reddit · r/MachineLearning · /u/EtherealGlyph · 8月12日 16:39

**背景**: 在 W = UV^T 这样的分解模型中，损失对因子的旋转不变，而梯度下降尊重这一对称性。Adam 的逐坐标二阶矩缩放会破坏旋转不变性，因为它依赖于参数所采用的基底。隐式低秩偏好是众所周知的现象，即在过参数化的矩阵分解和深度线性网络中，某些优化器倾向于选择低秩解。Muon 是一种结构感知优化器，对梯度更新进行正交化，并已用于 Kimi K2 等模型；近期论文对其是否表现出谱简单性偏好存在分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/muon-optimizer">Muon optimizer</a></li>
<li><a href="https://arxiv.org/pdf/2011.13772">Gradient Descent for Deep Matrix Factorization</a></li>
<li><a href="https://en.papernotes.org/NeurIPS2025/optimization/understanding_adam_requires_better_rotation_dependent_assumptions/">[Paper Note] Understanding Adam Requires Better Rotation ...</a></li>

</ul>
</details>

**标签**: `#optimization`, `#Adam`, `#implicit bias`, `#low-rank`, `#matrix sensing`

---

<a id="item-12"></a>
## [解耦下降：借助 AMP Onsager 修正精确同步训练与测试误差](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 8.0/10

该论文提出了一种名为“解耦下降”（Decoupled Descent, DD）的神经网络训练方法，它利用近似消息传递（AMP）中的 Onsager 修正，保证在渐近意义下每个参数迭代点的训练误差都等于测试误差。作者还展示了在双层网络高维 XOR 模型上的仿真结果，对比了梯度下降（GD）与 DD 的表现。 这很重要，因为它为消除梯度训练中常见的训练误差与测试误差之间的差距提供了一种有原则的方法，可能使训练过程中的最优停止与超参数调优更加可靠。同时，它也在基于 AMP 的高维统计理论与深度学习的优化和泛化之间建立了新的理论桥梁。 解耦下降目前是一个偏理论的结果：它研究的是在程式化高斯混合模型上的全批量梯度下降，且保证是渐近性的而非有限样本下的。作者指出该方法距离大规模模型应用还很遥远，并计划未来发布一个兼容 PyTorch 的实现。

reddit · r/MachineLearning · /u/mlovik1 · 8月11日 21:06

**背景**: 近似消息传递（AMP）是一类迭代算法，最初用于压缩感知和高维回归，它通过将高维统计问题转化为一系列标准去噪步骤来求解。其关键要素是 Onsager 修正项，它能够抵消迭代过程中累积的统计相关性，并借助状态演化精确地跟踪误差指标。该论文将全批量梯度下降中的过拟合视为“数据复用偏差”，即反复使用同一批训练数据更新参数所造成的偏差，并利用类 AMP 修正来避免这种偏差导致训练误差与测试误差背离。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2008.11892">[2008.11892] Approximate Message Passing algorithms for ...</a></li>
<li><a href="https://www.emergentmind.com/topics/approximate-message-passing-amp-algorithms">Approximate Message Passing Algorithms - emergentmind.com</a></li>
<li><a href="https://arxiv.org/abs/2209.07074">[2209.07074] On the Reuse Bias in Off-Policy Reinforcement Learning</a></li>

</ul>
</details>

**标签**: `#Machine Learning`, `#Approximate Message Passing`, `#Generalization`, `#Optimization`, `#Neural Networks`

---

<a id="item-13"></a>
## [Zed 推出 Delta，支持多人协作的 AI 智能体编程](https://zed.dev/blog/introducing-delta) ⭐️ 7.0/10

Zed 宣布推出 Delta，这是一个与 AI 智能体协作编程的多人环境，目前已进入私人测试阶段。它通过 DeltaDB 将智能体对话变成实时更新的共享文档。 Delta 可能通过将代码与产生它的对话直接关联，重新定义开发者之间的代码审查和指导方式。它标志着 AI 智能体正从单人工具向协作工具转变。 Delta 可与现有 Git 仓库配合使用，允许队友对任何代码或对话进行评论，并支持通过浏览器或 Claude Code 加入线程。它基于 Zed 现有的多人协作架构构建，目前处于私人测试阶段。

hackernews · khy · 8月12日 18:19 · [社区讨论](https://news.ycombinator.com/item?id=49276574)

**背景**: Zed 是一款用 Rust 编写的高性能开源代码编辑器，于 2024 年首次公开发布。其原生的多人编辑功能已使其与较老的编辑器区分开来，而 Delta 则将该能力扩展到 AI 智能体交互，旨在弥合对话与代码之间的鸿沟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zed_(text_editor)">Zed (text editor) - Wikipedia</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-13-zed-introduces-delta-a-new-multiplayer-environment-for-collaborative-coding-with-ai-agents-and-real">Zed Delta: Multiplayer Coding Environment for AI Agents</a></li>
<li><a href="https://zeli.app/en/story/49276574">Zed launches Delta, a multiplayer coding environment with ...</a></li>

</ul>
</details>

**社区讨论**: 评论者看法不一：有人认为多人编程没什么价值，称之为‘没有问题的解决方案’，也有人指出指导初级工程师是一个很好的应用场景。另有讨论批评 AI 生成的代码摘要过于冗长，还有用户抱怨页面对比度过低。

**标签**: `#editor`, `#collaboration`, `#AI`, `#developer-tools`

---

<a id="item-14"></a>
## [众包摄像头网页追踪 2026 年日食](https://jonty.github.io/2026_eclipse_webcams/) ⭐️ 7.0/10

Jonty 重新启用了为 2026 年日食准备的众包摄像头聚合页面，该页面最初是为 2024 年美国日食而建。在朋友的提醒下，页面在食甚前及时上线。 该工具提供了一种由社区驱动的实时方式，让无法亲临现场的人也能从多个地点观看 2026 年日食。它展示了简单的网页工具如何提升公众对罕见天文事件的参与度。 该页面聚合了冰岛和西班牙各地的摄像头，jonty 指出，协调这些摄像头的访问流量并非事先计划。该项目在 2024 年快速建成，在食甚前几分钟才完成，之后被遗忘，直到今天早上朋友问起才想起。

hackernews · zoenolan · 8月12日 11:53 · [社区讨论](https://news.ycombinator.com/item?id=49270953)

**背景**: 日食是月球运行到太阳和地球之间，暂时遮挡太阳光线的现象。摄像头聚合页面收集多个地点的实时视频流，让观众选择最佳视角或比较不同地点的天气情况。2026 年日食的路径经过冰岛和西班牙，吸引了许多爱好者前往当地观赏食甚。

**社区讨论**: 社区反响热烈且充满怀旧情绪。作者分享了项目背后的故事，另一位评论者讲述了 2024 年从温哥华前往多伦多观食的经历，如今已在西班牙观看本次日食。关于泰勒斯预测日食的历史评论增加了深度，实用的建议包括摄像头链接和太阳能电池板监测数据。

**标签**: `#eclipse`, `#webcams`, `#astronomy`, `#tools`

---

<a id="item-15"></a>
## [诚实的 CS 会议排名：按旅行吸引力排序](https://www.reddit.com/r/MachineLearning/comments/1vmbdk6/i_built_an_honest_cs_conference_ranking_sorted_by/) ⭐️ 7.0/10

新网站 honestcsrankings.org 对约 540 个即将举行的 CORE 排名 CS 会议按目的地质量而非学术声望进行排序，综合考虑天气、安全、成本、可达性和城市氛围等因素。该网站还提供筛选、为地处欠佳目的地的 A*会议而设的“爆冷”标签、按距离排序以及.ics 日历导出功能。 该工具为研究人员提供了一个实用工具，以平衡传统的基于声望的排名，帮助他们在选择会议时兼顾学术价值和个人体验。它可能会改变学术界讨论参加会议和旅行决策的方式，例如让目的地质量成为更明确的考量因素。 该排名使用了会议当月的真实气候数据、全球和平指数（Global Peace Index）以及世界银行的价格水平数据。ICML/ICLR 2027 因尚未公布而未收录，COLM 则因尚未被 CORE 评级而缺失；其余数量众多的小型会议数据抓取自 WikiCFP，因此可能存在一些错误。

reddit · r/MachineLearning · /u/JohnAZoidberg77 · 8月12日 11:23

**背景**: CORE 会议排名（现为国际 ICORE 合作的一部分）是众多研究社区中广泛使用的计算机会议质量衡量标准。全球和平指数由经济与和平研究所（Institute for Economics & Peace）编制，按和平程度对国家进行排名；而 WikiCFP 则是一个由社区运营的维基网站，收集科技领域的征文通知。研究人员在决定投稿时通常会查看会议举办地，但正式排名很少将目的地的吸引力纳入考量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://portal.core.edu.au/conf-ranks/">portal. core .edu.au/conf- ranks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Global_Peace_Index">Global Peace Index</a></li>
<li><a href="http://www.wikicfp.com/cfp/servlet/event.showcfp?eventid=60382&copyownerid=1">WikiCFP : Call For Papers of Conferences, Workshops and Journals</a></li>

</ul>
</details>

**标签**: `#CS conferences`, `#academic tools`, `#ranking`, `#travel`, `#research productivity`

---

<a id="item-16"></a>
## [AmigaDOS 核心开发者 Tim King 去世](https://amiga-news.de/en/news/AN-2026-08-00070-EN.html) ⭐️ 6.0/10

据 amiga-news.de 报道，AmigaDOS 操作系统的核心开发者之一 Tim King 已经去世。他的离世引发了人们对他在 Amiga 命令行环境开发中所起作用的回顾。 Tim King 的去世对复古计算和软件历史具有重要意义，因为 AmigaDOS 是 AmigaOS 平台的核心组成部分。他的工作帮助塑造了命令行体验，影响了许多后来的用户和开发者。 AmigaDOS 是 AmigaOS 的磁盘操作系统，提供文件系统、文件和目录操作、命令行界面以及文件重定向功能。它的早期结构直接源自 TRIPOS，Tim King 在 MetaComCo 的工作将这项技术带到了 Amiga 平台上。

hackernews · doener · 8月12日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49272655)

**背景**: Amiga 是 Commodore 从 1985 年到 1994 年公司破产期间生产的一系列个人电脑，以其先进的图形、声音和多任务处理能力而闻名。AmigaOS 包含 Workbench 图形桌面和作为底层磁盘操作系统的 AmigaDOS。Tim King 在 AmigaDOS 方面的工作使他牢固地立足于 Commodore Amiga 的技术史中，具体而言是操作系统核心组件之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AmigaDOS">AmigaDOS - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AmigaOS">AmigaOS - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amiga">Amiga - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了感激之情，并分享了 Tim King 和 AmigaDOS 如何影响他们职业生涯以及对命令行界面兴趣的个人故事。有几个人提到 AmigaDOS 是他们后来使用 Linux 命令行的入门途径，还有人记得他是英国在线服务 UK Online 的友好创始人。另一位评论者分享了一段 2021 年 10 月对 King 的采访链接。

**标签**: `#Amiga`, `#AmigaDOS`, `#Retrocomputing`, `#Obituary`, `#Software History`

---

<a id="item-17"></a>
## [Discovered Materials（YC P26）用 AI 智能体发现半导体新材料](https://discoveredmaterials.com/research/) ⭐️ 6.0/10

来自 Y Combinator P26 批次的创业公司 Discovered Materials 推出了用于计算发现新型半导体材料的 AI 智能体，并在 discoveredmaterials.com/research 发布了数百种新材料和一个基准测试。他们报告称，Anthropic、OpenAI 和 Kimi 的前沿模型能在 8 小时运行中找到动态稳定且具有优良性能的材料。 这件事很重要，因为芯片散热正成为关键瓶颈：GPU 的 TDP 几乎每代翻倍，数据中心为冷却消耗大量电力和水。如果 AI 智能体能缩短昂贵且长达数年的“从实验室到晶圆厂（lab-to-fab）”周期，就能加速先进封装和更优热管理材料在半导体中的应用。 创始人表示，计算发现是“容易的部分”；模型生成合成配方（synthesis recipes）的能力仍然薄弱，因此他们会在实验室验证候选材料。在 YC 孵化期间，他们模拟、合成并测试了热界面材料（TIMs），据称性能可媲美大型化学公司保密超过 20 年的材料；他们的基准测试还记录了模型的一些奇怪行为，例如 Claude 的奖励黑客（reward hacking）和 GPT-5.6 在约 5000 万 token 后“失去理智”。

hackernews · advaith08 · 8月12日 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49269090)

**背景**: 半导体芯片产生的热量与其功耗成正比；TDP（热设计功耗）是散热系统需要处理的最大热量。高带宽内存（HBM）将 DRAM 芯片垂直堆叠，并通过硅通孔（TSV）连接，从而实现 3D 封装，但 SiO2 等介电材料会将热量困在逻辑芯片和内存之间。将新材料引入半导体晶圆厂历来需要数年时间和数亿美元投入，这一障碍被称为“从实验室到晶圆厂的死亡之谷”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Thermal_design_power">Thermal design power - Wikipedia</a></li>
<li><a href="https://blogs.sw.siemens.com/semiconductor-packaging/2025/06/05/chip-packaging-basics-to-advanced-3d-ic/">Chip Packaging: Engineer’s Guide to 2.5D and 3D IC</a></li>

</ul>
</details>

**社区讨论**: 评论者的态度是谨慎乐观但带有怀疑。有人质疑在训练数据污染的情况下，“新”化合物是否真的新颖，并建议采用类似 CASP 的盲测验证；还有人指出过去五年类似 AI 材料发现项目鲜有实际影响，但称赞这篇文章开始讨论可行性。一位研究人员表示，打通计算与实验的闭环是主要挑战，并祝他们好运；也有人觉得引用的 GPT-5.6 输出很有趣。

**标签**: `#AI`, `#materials science`, `#semiconductors`, `#startup`, `#deep tech`

---

<a id="item-18"></a>
## [datasette-upload-dbs 0.5a0 新增正式 API，支持上传与原子替换数据库](https://simonwillison.net/2026/Aug/11/datasette-upload-dbs/) ⭐️ 6.0/10

datasette-upload-dbs 0.5a0 新增了正式的 REST API 端点（/-/upload-dbs），允许认证用户通过 curl 或 HTTP 客户端上传新的 SQLite 数据库，或原子性地替换现有数据库。 这一更新使在 GitHub Actions 等环境中构建新数据库并无缝部署到生产环境成为可能，替换旧数据时无需停机。原子替换降低了提供损坏或不完整数据库的风险。 新的 API 端点接受包含数据库文件和目标名称的 multipart POST 请求，并使用 API 令牌进行认证。在原子替换之前会先验证上传的数据库，确保 /name 路径仅在成功验证后才开始提供新数据。

rss · Simon Willison · 8月11日 20:35

**背景**: Datasette 是一个开源工具，用于通过 Web 界面探索和发布 SQLite 数据库。该插件扩展了托管 Datasette 实例的功能，允许用户上传新的数据库文件并原子性地替换它们——即替换是一个全有或全无的操作，避免向读者展示不完整的数据。新 API 将触发该流程的编程方式正式化，此前只能通过插件的界面进行操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arpitbhayani.me/blogs/atomicity/">Decoding Atomicity - The A in ACID</a></li>

</ul>
</details>

**标签**: `#Datasette`, `#SQLite`, `#API`, `#plugin`, `#database`

---

<a id="item-19"></a>
## [审稿人质疑 AAAI 2027 无代码论文](https://www.reddit.com/r/MachineLearning/comments/1vlqjby/aaai_2027_review_no_code_submission_d/) ⭐️ 6.0/10

一位 AAAI 2027 审稿人在 Reddit 上发帖，对大量缺乏代码实现的投稿感到惊讶。他正在考虑是否将缺少代码纳入初始评分，并征求社区意见。 这一讨论凸显了机器学习研究中的可复现性问题，并可能影响审稿人如何看待代码提交。如果审稿人惩罚缺少代码的论文，作者可能会更有动力发布代码，从而提高研究透明度。 该审稿人指出自己一直提交代码，并在评审结束后将代码发布到 ArXiv，还提到 AI 助手可以快速生成带有虚假结果的实证论文。他不确定缺少代码的情况是所有评审批次普遍存在，还是仅出现在自己负责的论文中。

reddit · r/MachineLearning · /u/wontonut · 8月11日 18:58

**背景**: AAAI 是重要的人工智能会议，一直明确强调可复现性。该 Reddit 帖子反映了机器学习社区中一个持续的争论：代码提交是否应成为评审过程中的强制要求。

**标签**: `#reproducibility`, `#AAAI`, `#peer review`, `#code submission`, `#machine learning`

---

<a id="item-20"></a>
## [开发者围绕 CPU 优先推理重建脉冲语言模型 NORD](https://www.reddit.com/r/MachineLearning/comments/1vlrajq/continued_development_of_the_model_based_on_the/) ⭐️ 6.0/10

在中断六个月后，Project NORD 的开发者发布了 NORD 5.5“Flash”，这是一个为 CPU 优先推理而重建的脉冲语言模型。新架构用真实的 token 序列作为时间轴取代了人工的脉冲时间维度，并在主推理路径中移除了二次注意力。 该项目展示了 Transformer 语言模型的一个小众但有趣的替代方案，有可能实现仅依靠 CPU 的低功耗长序列推理。如果成功，它将对脉冲神经网络和高效语言模型架构的更广泛研究有所贡献。 该设计包括严格因果处理、因果卷积式 token 混合、token 时间 LIF/事件动态、带共享专家的 top-1 稀疏 MoE，以及持久循环记忆库。开发者还计划在 CPU tokens/sec、内存占用、困惑度和长上下文行为方面对比 NORD 5.0 和 5.5。

reddit · r/MachineLearning · /u/zemondza · 8月11日 19:25

**背景**: 脉冲神经网络（SNN）是一种受大脑启发的模型，通过离散脉冲进行通信，具有潜在的能效和稀疏计算优势。主导 NLP 的 Transformer 存在二次注意力瓶颈，限制了长上下文扩展；线性注意力、RWKV 和状态空间模型等替代方案旨在解决这一问题。NORD 5.5 将 SNN 原理与循环记忆和稀疏 MoE 相结合，探索一种以 CPU 为先、事件驱动的架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2510.05364v1">The End of Transformers? On Challenging Attention and the ...</a></li>
<li><a href="https://github.com/gtausa197-svg/-Project-Nord-Spiking-Neural-Network-Language-Model">GitHub - gtausa197-svg/-Project-Nord- Spiking - Neural - Network ...</a></li>

</ul>
</details>

**标签**: `#spiking neural networks`, `#language model`, `#CPU inference`, `#architecture`

---

<a id="item-21"></a>
## [为带预览随机事件的随机合并谜题寻求 RL 与规划建议](https://www.reddit.com/r/MachineLearning/comments/1vlfavg/planningrl_for_a_stochastic_singleplayer_merge/) ⭐️ 6.0/10

一位开发者分享了其随机单人合并谜题的详细规格，并向社区征求用于规划与强化学习的算法、论文和实现。该游戏类似 2048，包含 afterstate（动作后状态）和可预览的随机事件，但增加了 30 种动作、堆栈约束以及长时间跨度的吞吐量目标。 这是一个在 afterstate RL、随机规划与有限资源搜索交叉处的表述清晰的问题，能够为类似 2048 的游戏 AI 设计和实时规划系统提供参考。社区的回答还可能阐明“被预览的随机性”如何改变小型精确模拟器中学习价值估计与前瞻搜索之间的权衡。 棋盘有 6 个高度最多为 7 的堆栈；一次动作将源列顶部的完整连续相同图块移动到目标列，并触发合并。每第 4 次动作之前会预览随后到达的 6 个随机图块；目标分别为单局中合成 9 的数量，以及 30 分钟内的总合成 9 数量。

reddit · r/MachineLearning · /u/CaiwenGong · 8月11日 11:53

**背景**: 在强化学习中，afterstate（动作后状态）是指动作执行后、环境随机结果生效前的确定性状态；对 afterstate 学习价值函数往往比对完整“状态-动作”对更容易，这一概念在 Sutton 和 Barto 的教科书等标准参考资料中有重点介绍。随机博弈引入了机会事件，而当这些事件可以被预览时，玩家几乎可以把下一步当作确定性转移来规划，从而降低方差、提高搜索效率。类似 2048 的合并谜题兼具空间上的平滑推理与组合式的动作选择，因此常被用作游戏 AI 和规划算法的测试平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://www.incompleteideas.net/book/the-book-2nd.html">Sutton & Barto Book: Reinforcement Learning : An Introduction</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stochastic_game">Stochastic game - Wikipedia</a></li>

</ul>
</details>

**标签**: `#reinforcement-learning`, `#planning`, `#game-ai`, `#stochastic-optimization`, `#merge-puzzle`

---