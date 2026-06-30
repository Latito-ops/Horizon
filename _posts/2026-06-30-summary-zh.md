---
layout: default
title: "Horizon Summary: 2026-06-30 (ZH)"
date: 2026-06-30
lang: zh
---

> 从 29 条内容中筛选出 18 条重要资讯。

---

1. [最高法院：地理围栏搜查令需具备相当理由](#item-1) ⭐️ 9.0/10
2. [谷歌 AI 同行评审处理万篇论文，错误检测率提升 34%](#item-2) ⭐️ 9.0/10
3. [新顶级域名'.self'提案：每人一个免费域名用于自托管](#item-3) ⭐️ 8.0/10
4. [Rocket Lab 收购 Iridium 达成历史性交易](#item-4) ⭐️ 8.0/10
5. [百万护照信息在 cannabis ID 系统泄露](#item-5) ⭐️ 8.0/10
6. [WATaBoy：将 Game Boy 指令 JIT 编译为 WASM，性能超越原生解释器](#item-6) ⭐️ 8.0/10
7. [Ornith-1.0：面向智能体编程的自结构语言模型](#item-7) ⭐️ 8.0/10
8. [Cerebras 与 OpenAI 交易挤占推理容量，损害初创企业](#item-8) ⭐️ 8.0/10
9. [可编辑权重的小型 Transformer 交互式教学工具](#item-9) ⭐️ 8.0/10
10. [Qwen 3.6 27B：本地开发之选，但硬件成本引争议](#item-10) ⭐️ 7.0/10
11. [藏匿'zines'被判 30 年引发言论自由争议](#item-11) ⭐️ 7.0/10
12. [韩国承诺 1 万亿美元投资存储芯片与人形机器人](#item-12) ⭐️ 7.0/10
13. [乌德尔：邀请 AI 代理加入人类主导的开发流程](#item-13) ⭐️ 7.0/10
14. [EML 树被证明是通用逼近器](#item-14) ⭐️ 7.0/10
15. [根据个性和价值观匹配 LLM 的测试](#item-15) ⭐️ 7.0/10
16. [Hack Your Summer：为期四周的免费学生项目冲刺](#item-16) ⭐️ 6.0/10
17. [质疑实例表示学习中的 NCE 损失动机](#item-17) ⭐️ 6.0/10
18. [HEMA 从业者构建开放数据集以改进 AI 对快速剑术的追踪](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [最高法院：地理围栏搜查令需具备相当理由](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

2026 年 6 月 29 日，美国最高法院裁定地理围栏搜查令受第四修正案保护，执法机构在获取特定区域内设备位置数据前必须证明存在相当理由。 这一里程碑式裁决极大地限制了无证的大规模位置监控，确立了数字隐私保护同样适用于地理围栏搜索的先例——此前执法机构常以此类搜索在无个别怀疑情况下识别潜在嫌疑人。 该裁决适用于从谷歌等第三方提供商收集位置数据的行为，但判决意见区分了针对特定对象的搜查令与宽泛的地理围栏搜查令；有来源指出，法院同时强调历史基站位置数据搜查令也需要相当理由，援引了 2014 年 Riley 诉加利福尼亚州案的先例。

hackernews · cdrnsf · 6月29日 15:54 · [社区讨论](https://news.ycombinator.com/item?id=48720924)

**背景**: 地理围栏搜查令是一种法律命令，强制技术公司提供在特定时间段内位于特定地理区域内的移动设备信息。这种称为地理围栏的技术利用 GPS、Wi-Fi 或蜂窝数据创建虚拟边界。执法机构越来越多地使用此类搜查令来识别潜在嫌疑人或证人，无需事先明确目标，从而引发第四修正案隐私权争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geo-fence_technology">Geo-fence technology</a></li>
<li><a href="https://www.blueforcelearning.com/blog/google-geofence-warrant-enhancing-law-enforcement">Google Geofence Warrant : Enhancing Law Enforcement</a></li>
<li><a href="https://legalclarity.org/what-is-geofence-data-warrants-privacy-and-your-rights/">What Is Geofence Data? Warrants , Privacy, and Your... - LegalClarity</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，卡根大法官的意见书中包含了带来源的实证引用，这一做法因透明度而受到称赞。一些人质疑该裁决是否适用于其他监控工具，如自动扫描公共区域车牌的 Flock 摄像头。还有人讨论，即使没有手机数据，调查人员也能通过酒店入住名单和 IP 地址三角定位嫌疑人，如彼得雷乌斯案所示。

**标签**: `#Supreme Court`, `#geofence`, `#privacy`, `#Fourth Amendment`, `#law enforcement`

---

<a id="item-2"></a>
## [谷歌 AI 同行评审处理万篇论文，错误检测率提升 34%](https://www.reddit.com/r/MachineLearning/comments/1uio9rb/googles_agentic_peerreviewer_handled_10k_papers/) ⭐️ 9.0/10

谷歌在 ICML 和 STOC 会议上部署了具有自治能力的 AI 同行评审系统，处理了约万篇论文，平均回应时间为 30 分钟；正式研究论文表明，该系统的数学错误检测率比零样本提示方法提高了 34%。 这展示了 AI 大规模辅助科学同行评审的潜力，减轻评审人负担并提高错误检测率。它为自治 AI 系统在科研验证中树立了先例，可能加速评审流程，同时保持或提升质量。 该自治系统自主运行，具有目标驱动行为和适应性，不同于传统的静态模型。相比零样本提示（模型不接收任何示例），34%的提升表明自治方法显著优于简单方法。

reddit · r/MachineLearning · /u/Justgototheeffinmoon · 6月29日 10:05

**背景**: 据 IBM 和 Google Cloud 定义，自治 AI 指无需人类持续干预即可自主设定目标并行动的 AI 系统。零样本提示是一种提示工程技术，让语言模型在没有任何示例的情况下直接执行任务，完全依赖其预训练知识。两者的结合使 AI 能系统化评审论文，捕捉零样本方法可能遗漏的细微错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://www.promptingguide.ai/techniques/zeroshot">Zero-Shot Prompting | Prompt Engineering Guide</a></li>

</ul>
</details>

**标签**: `#AI`, `#peer review`, `#machine learning`, `#research automation`

---

<a id="item-3"></a>
## [新顶级域名'.self'提案：每人一个免费域名用于自托管](https://hccf.onmy.cloud/2026/06/21/reclaiming-our-digital-selves-hccfs-vision-for-a-human-centered-top-level-domain/) ⭐️ 8.0/10

人类中心计算基金会（HCCF）提出新的顶级域名'.self'，计划为每人提供一个免费域名用于个人自托管，旨在从集中式平台中夺回数字身份。 这项倡议能让个人完全掌控自己的在线形象，减少对大型科技公司的依赖，但面临防止滥用和在没有注册费的情况下维持顶级域名运营的重大挑战。 提案中包含‘每人一个免费域名’政策，但社区评论指出，如果不将域名与身份证明绑定，很难执行这一政策，并且在没有传统收入的情况下运营顶级域名的成本巨大。

hackernews · HumanCCF · 6月29日 19:49 · [社区讨论](https://news.ycombinator.com/item?id=48724230)

**背景**: 顶级域名（TLD）是域名末尾的部分，如.com、.org。自托管是指运行自己的服务器来托管网站或服务，提供完全控制权但需要技术能力。之前的免费 TLD（如.tk）曾遭受垃圾邮件和滥用，导致被主流平台屏蔽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Top-level_domain">Top - level domain - Wikipedia</a></li>
<li><a href="https://github.com/awesome-selfhosted/awesome-selfhosted">GitHub - awesome-selfhosted/awesome-selfhosted: A list of ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对免费 TLD 的可行性表示怀疑，引用了.tk 的例子，其中诈骗者毁了其声誉。一些人建议使用信誉系统或身份验证来防止域名抢注，而另一些人则质疑没有注册费的经济可持续性。

**标签**: `#self-hosting`, `#DNS`, `#TLD`, `#decentralization`, `#identity`

---

<a id="item-4"></a>
## [Rocket Lab 收购 Iridium 达成历史性交易](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 8.0/10

Rocket Lab 宣布收购 Iridium Communications，获得其盈利的卫星网络和宝贵的 L 波段频谱。该交易确保了 Rocket Lab 发射服务的稳定需求，并加强了从卫星制造到运营的垂直整合。 此次收购使 Rocket Lab 成为完全整合的太空公司，类似于 SpaceX 利用 Starlink 保证发射节奏。它还让 Rocket Lab 立即获得全球卫星网络和频谱，这些是未来扩张中稀缺且有价值的资产。 Iridium 运营着 66 颗活跃的低地轨道卫星，提供全球语音和数据覆盖，并配有备用卫星。交易包括 Iridium 的盈利用户群和 L 波段频谱权，这对卫星通信至关重要。

hackernews · everfrustrated · 6月29日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48719485)

**背景**: Iridium 是由摩托罗拉最初开发的卫星星座，于 1998 年投入运营，通过带有星间链路的低轨卫星提供全球覆盖。Rocket Lab 是一家发射服务提供商和卫星制造商，以其 Electron 火箭和更大的 Neutron 火箭计划而闻名。此次收购使 Rocket Lab 能够通过可能为 Iridium 星座建造替换卫星来确保发射需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Iridium_satellite_constellation">Iridium satellite constellation</a></li>
<li><a href="https://www.iridium.com/network">Network | Iridium - Iridium Satellite Communications</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：一些人担心太空垃圾增加和商业混乱，而另一些人则认为这是类似于 SpaceX 的 Starlink 模式的战略举措。一位评论者指出，Rocket Lab 获得了频谱和一家盈利的卫星公司，总结了关键优势。

**标签**: `#acquisition`, `#aerospace`, `#satellite`, `#communications`, `#RocketLab`

---

<a id="item-5"></a>
## [百万护照信息在 cannabis ID 系统泄露](https://www.theverge.com/tech/947157/passports-data-breach-cannabis-club-systems-nefos-puffpal) ⭐️ 8.0/10

近百万份护照扫描件和驾照信息因 PuffPal（由 Nefos Solutions 构建的 cannabis 俱乐部年龄验证平台）的数据泄露而暴露在公开互联网上，无密码或加密保护。 此次泄露凸显了将护照等高价值凭证存储在低价值的辅助验证系统中的系统性风险，形成了影响数百万人的关键安全漏洞。 泄露的数据包括护照、身份证和驾照的扫描件，可通过可预测的公开网址访问。安全研究员 Sammy Azdoufal 发现了这一泄露事件，涉及超过 100 万会员档案。

hackernews · jruohonen · 6月28日 11:22 · [社区讨论](https://news.ycombinator.com/item?id=48706389)

**背景**: PuffPal 是欧洲 cannabis 零售商和俱乐部用于管理会员和年龄验证的平台。供应商 Nefos Solutions 未对数据设置身份验证，导致其可被公开访问。年龄验证系统通常收集敏感的身份文件，但可能缺乏健全的安全性，从而造成凭证价值与系统安全之间的不匹配。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://stateofsurveillance.org/news/cannabis-id-vendor-nefos-million-passports-exposed-2026/">Nefos Left a Million Cannabis Club Passports Exposed Online</a></li>
<li><a href="https://daringfireball.net/linked/2026/06/28/puffpal-passport-leak">Daring Fireball: PuffPal, an App for Accessing Cannabis Clubs ...</a></li>
<li><a href="https://vault-tools.com/news/cannaleaks-puffpal-cannabis-club-id-documents-exposed-2026/">Cannaleaks: 985,000 Cannabis Club ID Scans Left Open on</a></li>

</ul>
</details>

**社区讨论**: 评论指出，为年龄验证收集敏感数据却未能保障其安全，具有讽刺意味。用户呼吁采取行动反对此类做法，并指出此前在旅行 CRM 等其他系统中也发生过类似泄露。

**标签**: `#data breach`, `#cybersecurity`, `#privacy`, `#passport`, `#identity theft`

---

<a id="item-6"></a>
## [WATaBoy：将 Game Boy 指令 JIT 编译为 WASM，性能超越原生解释器](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

作者展示了一个 Game Boy 模拟器 WATaBoy，它在运行时将 SM83 指令动态重新编译为 WebAssembly，实现了超越原生解释器的性能。 这种方法通过利用浏览器中的 WebAssembly 绕过了 iOS 的 JIT 限制，从而在通常禁止原生 JIT 编译的平台上实现高性能模拟。这也凸显了将 WebAssembly 作为 JIT 编译目标用于模拟及其他性能关键型应用的潜力。 WATaBoy 在运行时生成 WebAssembly 字节码，通过 JavaScript 链接，并使用间接函数调用，实现了比原生解释器大约 1.2 倍的速度。基准测试显示，Safari 在浏览器中性能最佳，还可以进行 PPU 中断预测等进一步优化。

hackernews · energeticbark · 6月29日 15:02 · [社区讨论](https://news.ycombinator.com/item?id=48720190)

**背景**: 即时编译（JIT）在运行时将代码动态转换为原生机器码以加速执行，但 iOS 禁止非浏览器应用使用 JIT。WebAssembly 被设计为接近原生的性能，可以在浏览器中运行并绕过这些限制。WATaBoy 利用这一点，将 Game Boy CPU 指令 JIT 编译为 WebAssembly 模块。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://humphri.es/blog/WATaBoy/">WATaBoy: JIT-ing Game Boy Instructions to Wasm Beats a Native ...</a></li>
<li><a href="https://www.machucavalley.tech/blog/wataboy-wasm-jit-performance-milestone/">WATaBoy: Why This WebAssembly JIT is Beating Native Game Boy ...</a></li>
<li><a href="https://deepwiki.com/WebAssembly/design/4.1-portability-and-jit">Portability and JIT | WebAssembly/design | DeepWiki</a></li>

</ul>
</details>

**社区讨论**: 评论强调了利用浏览器 WebAssembly 绕过 iOS JIT 限制的巧妙之处，有人指出 WebAssembly 的开销（约 20%）远小于解释器的开销（约 1000%）。其他人讨论了与早期 NES 模拟 JIT 方法的比较以及不同浏览器间的性能差异。

**标签**: `#JIT compilation`, `#WebAssembly`, `#emulation`, `#Game Boy`, `#performance`

---

<a id="item-7"></a>
## [Ornith-1.0：面向智能体编程的自结构语言模型](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce 发布了 Ornith-1.0，这是一个采用 MIT 开源协议、面向智能体编程的自结构语言模型系列，包含 9B、31B、35B MoE 和 397B MoE 四种规模。在编程基准测试中，它在同等规模的开源模型中达到了最先进水平。 Ornith-1.0 新颖的自结构方法使得模型在推理过程中能够自我改进推理能力，可能实现更自主、更强大的编程智能体。其开放许可证以及基于兼容的 Apache 2.0 基础模型（Gemma 4、Qwen 3.5）使其对研究和开发具有可及性。 该模型基于 Gemma 4 和 Qwen 3.5 构建，两者均为 Apache 2.0 许可，确保了许可证兼容性。35B MoE 变体以 GGUF 格式（20GB）提供，可在本地运行，初步测试显示在多步骤智能体编程任务中表现强劲，且生成速度快（103 token/秒）。

rss · Simon Willison · 6月29日 16:17

**背景**: 智能体编程（Agentic coding）指 AI 智能体在最小人工干预下自主规划、编写、测试和修改代码。自结构（Self-scaffolding）是一种技术，模型利用自身输出或中间推理来指导后续步骤，从而在单次推理中提升性能。传统编程助手需要逐步人工输入，而智能体方法追求更高的自主性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>

</ul>
</details>

**社区讨论**: 社区评论意见不一：一些用户称赞 Ornith-1.0 是第一个被本地 LLM 社区接受的 Qwen 微调模型，在编程问题上提供创造性解决方案。另一些人持怀疑态度，称其为 Qwen 或 Gemma 4 的“刷分版”，并指出聊天性能差和幻觉等局限。还有人质疑 DeepReinforce 公司本身以及自结构的具体工作原理。

**标签**: `#LLM`, `#open-source`, `#coding`, `#agentic`, `#self-scaffolding`

---

<a id="item-8"></a>
## [Cerebras 与 OpenAI 交易挤占推理容量，损害初创企业](https://www.reddit.com/r/MachineLearning/comments/1uiqhiv/cerebras_openai_deal_capacity_has_effectively/) ⭐️ 8.0/10

Cerebras 通过一笔据报道价值 200 亿美元的交易，实际上将其近期大部分推理容量预先分配给了 OpenAI，使小型初创公司的 API 等待列表实质上变得无限长。 这一转变将专用 AI 推理硬件的获取集中到了少数超大规模企业手中，加剧了需要低延迟、高吞吐量 ASIC 推理的生产负载初创公司的短缺。 发帖者报告需要持续 1-2000 tokens/秒的吞吐量和严格的 p95 延迟，并且已在 Cerebras 等待列表中等待数月而无法获得访问权限。

reddit · r/MachineLearning · /u/Kortopi-98 · 6月29日 12:00

**背景**: Cerebras 生产针对 AI 推理优化的晶圆级芯片（WSE），采用独特架构将单个晶圆上的芯片连接起来以降低延迟。ASIC 推理芯片是专为执行预训练神经网络而定制的，相比 H100 等通用 GPU 具有效率优势。据报道，OpenAI 与 Cerebras 的交易涉及 200 亿美元的芯片，可能确保了 Cerebras 生产的绝大部分产能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>

</ul>
</details>

**标签**: `#Cerebras`, `#OpenAI`, `#AI inference`, `#startup`, `#GPU shortage`

---

<a id="item-9"></a>
## [可编辑权重的小型 Transformer 交互式教学工具](https://www.reddit.com/r/MachineLearning/comments/1uhw7fu/i_shrank_a_transformer_until_every_number_fitted/) ⭐️ 8.0/10

一位软件工程师创建了一个交互式网页，以矩阵级别可视化完整的 Transformer 前向传播过程，权重可编辑并实时重新计算。该页面使用一个微型 Transformer（词汇表 6 个词，嵌入维度 3），从四个输入词预测下一个词。 该工具允许学习者动手调整权重并立即观察效果，从而让 Transformer 的内部工作原理变得可理解。它弥合了高层 API 使用与深入理解之间的鸿沟，可能帮助大量学生和开发者掌握大型语言模型的基本运算。 该 Transformer 使用单注意力头、单块结构，包括所有组件：词向量、Q/K/V、注意力分数、因果掩码、softmax、前馈网络、logits 和概率。页面是一个独立的 HTML 文件，无需库或构建步骤，并包含随机化按钮以展示未训练权重产生无意义预测。

reddit · r/MachineLearning · /u/DanielMoGo · 6月28日 12:35

**背景**: Transformer 是现代大型语言模型（如 GPT-4）的基础。前向传播是在固定权重下从输入到输出的计算，涉及注意力和前馈网络的矩阵乘法。通常，权重通过训练（反向传播）学习，但此可视化仅关注前向传播，以帮助用户理解架构而不涉及训练的复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Attention_(machine_learning)">Attention (machine learning) - Wikipedia</a></li>
<li><a href="https://davidvandebunte.gitlab.io/executable-notes/notes/se/what-exactly-are-keys-queries-and-values.html">QKV attention — Executable Notes</a></li>
<li><a href="https://medium.com/@jinoo/a-simple-example-of-attention-masking-in-transformer-decoder-a6c66757bc7d">A Simple Example of Causal Attention Masking in Transformer ...</a></li>

</ul>
</details>

**标签**: `#transformer`, `#machine learning`, `#interactive visualization`, `#education`, `#LLM`

---

<a id="item-10"></a>
## [Qwen 3.6 27B：本地开发之选，但硬件成本引争议](https://quesma.com/blog/qwen-36-is-awesome/) ⭐️ 7.0/10

Qwen 3.6 27B 是一款拥有 262K 上下文窗口的稠密开源模型，被宣传为本地 AI 开发的理想选择。但社区反馈指出，要有效运行该模型需要昂贵的硬件，例如起步价 6699 美元的 128GB MacBook Pro，这引发了关于成本效益的讨论。 这场争论凸显了本地 AI 开发在隐私和控制方面的优势与基于云的解决方案在成本和便利性上的权衡。其结果可能影响开发者的硬件投资决策以及本地大语言模型的广泛采用。 Qwen 3.6 27B 模型采用 Apache 2.0 许可证，支持多模态，并需要像 128GB MacBook Pro 这样的高端硬件才能达到最佳性能。评论者指出，像 OpenRouter 这样的云服务能以更低成本访问更大的模型，因此对许多用户来说本地部署的经济性存疑。

hackernews · stared · 6月29日 17:05 · [社区讨论](https://news.ycombinator.com/item?id=48721903)

**背景**: Qwen 是阿里巴巴开发的开源权重语言模型系列。3.6 版本增强了智能体编程和推理能力。本地运行 27B 参数的模型通常需要大量内存（例如量化版本需要 16GB 以上），而对于未量化的全速推理则需要更多内存。云 API 提供按使用量付费的访问方式，无需前期硬件成本，这对许多开发者具有吸引力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ollama.com/library/qwen3.6:27b">qwen 3 . 6 : 27 b</a></li>
<li><a href="https://insiderllm.com/guides/qwen-3-6-local-ai-guide/">Qwen 3 . 6 Complete Guide: 27 B Dense, 35B-A3B MoE... | InsiderLLM</a></li>

</ul>
</details>

**社区讨论**: 像 iagooar 和 bensyverson 这样的评论者强调了高昂的硬件成本（例如 128GB MacBook Pro 售价 6699 美元）以及重度使用时的噪音和风扇问题。Onion2k 认为文章中的测试案例是不切实际的绿色项目，而 mashygpig 则强调了像 OpenRouter 这样的云服务的经济优势——10 美元就能使用更大的模型。总体而言，社区对大多数开发者来说本地部署的实用性持怀疑态度。

**标签**: `#local-llm`, `#qwen`, `#ai-development`, `#hardware-considerations`

---

<a id="item-11"></a>
## [藏匿'zines'被判 30 年引发言论自由争议](https://theintercept.com/2026/06/26/daniel-sanchez-estrada-zines-prairieland-free-speech/) ⭐️ 7.0/10

丹尼尔·桑切斯·埃斯特拉达因藏匿联邦搜查令所寻的 zines 被判处 30 年监禁，这些 zines 与一场导致联邦探员中枪的反法西斯抗议活动有关。 此案引发对言论自由的担忧，因为 30 年刑期是针对藏匿出版物的妨碍司法行为，而非抗议中的暴力本身，可能为政治异议树立寒蝉效应先例。 埃斯特拉达并非枪手，但因在执行搜查令时接到妻子电话后藏匿 zines 而被判妨碍司法罪；其相关共谋指控最高可判 75 年。

hackernews · xrd · 6月28日 21:42 · [社区讨论](https://news.ycombinator.com/item?id=48711981)

**背景**: Zines（爱好者杂志）是自行出版的非商业性小册子，常被边缘化社群用于表达非主流或政治观点。Antifa（反法西斯运动）是一个分散的左翼反法西斯运动，有时采取直接行动。该判决针对的是妨碍司法行为，而非 zines 本身的内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zine">Zine - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Antifa_(United_States)">Antifa (United States) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者意见分歧：有人认为在搜查令下藏匿证据是明确的妨碍司法行为，而另一些人则强调仅仅移动出版物就获重刑，可能将持有异议文献刑事化。一个反复出现的观点是，这些 zines 本身并非非法，只是被作为犯罪证据追查。

**标签**: `#free speech`, `#law`, `#warrants`, `#civil liberties`, `#political`

---

<a id="item-12"></a>
## [韩国承诺 1 万亿美元投资存储芯片与人形机器人](https://arstechnica.com/ai/2026/06/south-korea-to-spend-1t-on-more-memory-chip-production-and-humanoid-robots/) ⭐️ 7.0/10

韩国宣布了一项 1 万亿美元的投资计划，旨在提升存储芯片产能并开发人形机器人，以巩固其在半导体和物理 AI 领域的地位。 这笔巨额政府投资标志着战略性推动，旨在主导关键科技领域，但将人形机器人这一投机性应用纳入其中，引发了关于资源分配和形态实用性的讨论。 该投资同时瞄准存储芯片这一稳定商品和人形机器人这一高风险高回报领域。社区评论者质疑将这两个不同领域混为一谈的做法，并质疑人形形态相较于其他设计的价值。

hackernews · jnord · 6月29日 22:21 · [社区讨论](https://news.ycombinator.com/item?id=48726102)

**背景**: 存储芯片（如 DRAM、NAND）是电子设备、数据中心和 AI 加速器中的关键组件，韩国是全球生产领先者。人形机器人旨在模仿人类运动和交互以完成制造、医疗和服务中的任务，但其商业可行性尚未得到验证。这项投资反映了各国大力补贴半导体和 AI 基础设施的广泛趋势。

**社区讨论**: 评论者表达了怀疑：有人将存储芯片和人形机器人并列比作‘杂货和舞蹈课’，凸显了风险差异。其他人质疑人形形态，认为存在更优方案，并怀疑该声明是否严肃或出于政治目的。

**标签**: `#semiconductors`, `#humanoid robots`, `#AI`, `#investment`, `#manufacturing`

---

<a id="item-13"></a>
## [乌德尔：邀请 AI 代理加入人类主导的开发流程](https://simonwillison.net/2026/Jun/28/jon-udell/#atom-everything) ⭐️ 7.0/10

乔恩·乌德尔主张，AI 编码代理应被邀请进入人类主导的软件开发流程作为协作者，而不是自主生成不可审查的拉取请求。他提出将叙事从“人在回路中”转变为“代理在我们回路中”。 这一观点重新定义了软件开发中关于自主 AI 的讨论，优先考虑人类主导和代码审查质量。它鼓励在不牺牲开发者控制或代码库完整性的前提下，负责任地集成 AI 工具。 乌德尔特别批评了代理一次性修改太多文件、使代码审查变得困难的不可审查拉取请求做法。他主张保持透明的代理辅助流程，适应现有的人类工作流。

rss · Simon Willison · 6月28日 21:57

**背景**: 自主编码（agentic coding）指的是能够以最少人工干预进行计划、编写和修改代码的自主 AI 代理。然而，诸如 Cursor 的“代理模式”等工具被批评生成跨多个文件的大规模不可审查拉取请求，增加了引入错误的风险并降低了代码审查的有效性。乌德尔的论点通过强调人类主导的协作，挑战了完全自主 AI 开发的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/abhasbhoi_softwareengineering-ai-cleancode-activity-7451637076707422208-b3f0">3 Ways to Use AI for Lean Pull Requests | ABHAS BHOI... | LinkedIn</a></li>
<li><a href="https://cloud.google.com/discover/what-is-agentic-coding">What is agentic coding? How it works and use cases | Google Cloud</a></li>

</ul>
</details>

**标签**: `#agentic software`, `#AI agents`, `#human-in-the-loop`, `#software development`, `#Jon Udell`

---

<a id="item-14"></a>
## [EML 树被证明是通用逼近器](https://www.reddit.com/r/MachineLearning/comments/1uipl1t/eml_trees_are_universal_approximators_r/) ⭐️ 7.0/10

一篇新论文证明，通过组合表示初等函数的 EML 树，可以用显式构造逼近一般函数空间中的任意函数。 这一理论结果为 EML 树提供了通用逼近定理，弥合了符号回归与神经网络表达能力之间的差距，并可能影响未来的机器学习模型设计。 该证明使用二元运算、多项式、双曲正切和近似单位划分的显式构造作为构建块，并通过基于符号的分解处理非正输入下自然对数定义不良的问题。

reddit · r/MachineLearning · /u/JoeGermany · 6月29日 11:16

**背景**: EML 函数是一种单一计算原语，可以通过组合表示所有初等函数。EML 树是每个节点计算 EML 函数的树结构，能够表示复杂函数。该工作通过添加可学习参数来泛化原始 EML，以处理实践和理论问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Brumbelow/uninum/blob/main/docs/eml_explained.md">uninum/docs/ eml _explained.md at main · Brumbelow/uninum · GitHub</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#universal approximation`, `#EML trees`, `#theoretical computer science`

---

<a id="item-15"></a>
## [根据个性和价值观匹配 LLM 的测试](https://www.reddit.com/r/MachineLearning/comments/1uin5ad/i_made_a_quiz_that_tells_you_which_llm_you_align/) ⭐️ 7.0/10

AI-Values.com 上的一个新测试根据个性和价值观将用户与 15 个 LLM 进行匹配，揭示了模型特定的道德判断，例如 Grok 4.3 是唯一认为不应向亿万富翁征税的模型，而 GPT-4o 是唯一认为战后招募纳粹科学家的“回形针行动”在道德上合理的模型。 这个测试为用户提供了一种新颖且有趣的方式来了解不同 LLM 的价值取向，凸显了模型之间在道德推理上的显著差异。它可以帮助用户选择符合自己伦理观点的 AI 助手。 该测试包含 117 个问题，每个问题对每个模型至少提问 5 次，有些多达 50 次，以确保一致性。结果实时更新，还有一个 15 题的精简版可供快速了解。

reddit · r/MachineLearning · /u/DarkyPaky · 6月29日 09:00

**背景**: 大型语言模型（LLM）如 Grok 4.3 和 GLM 5.2 是通过大量文本数据训练生成的类人文本的 AI 系统。这些模型基于训练数据和微调会表现出不同的“个性”，因此价值对齐是一个重要的研究领域。这个测试系统性地测量了 15 个主流 LLM 的道德和个性特征。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.x.ai/developers/models/grok-4.3">Grok 4.3 | xAI Docs</a></li>
<li><a href="https://unsloth.ai/docs/models/glm-5.2">GLM-5.2 - How to Run Locally | Unsloth Documentation</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区称赞这个测试有趣且设计精良，用户分享了自己的结果，并讨论了模型特定道德判断的含义。一些人对 Grok 4.3 关于亿万富翁的立场等发现表示惊讶，并讨论了训练数据对这些价值观的潜在影响。

**标签**: `#LLMs`, `#AI alignment`, `#values`, `#personality quiz`

---

<a id="item-16"></a>
## [Hack Your Summer：为期四周的免费学生项目冲刺](https://simonwillison.net/2026/Jun/28/hack-your-summer/#atom-everything) ⭐️ 6.0/10

Hack Your Summer 是一个为期四周的免费生产冲刺活动，面向本科生和研究生，第二期将于 2026 年 7 月 13 日启动，申请截止日期为 7 月 8 日。该项目旨在帮助学生在实习短缺的情况下构建真实项目并获取替代经验。 该计划应对了美国的实习危机，为未能获得实习的学生提供了一个结构化的替代方案。它帮助学生创建有形的作品集并获得指导，可能为求职者创造更公平的竞争环境。 该计划免费，面向本科生、研究生和应届毕业生。参与者将确定一个项目，在导师支持下取得进展，并生成可供未来雇主查看的公开作品。

rss · Simon Willison · 6月28日 19:26

**背景**: 在软件开发中，'冲刺'（sprint）是一个固定时间段（通常 2-4 周），团队在此期间完成一定量的工作，这一概念源自 Scrum 方法论。Hack Your Summer 将这一概念应用于学生项目，提供结构和指导以产生实际成果。今年的实习短缺使许多学生缺乏获得实践经验的机会。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Scrum_(software_development)">Scrum (project management) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#education`, `#internships`, `#student programs`, `#summer projects`

---

<a id="item-17"></a>
## [质疑实例表示学习中的 NCE 损失动机](https://www.reddit.com/r/MachineLearning/comments/1uj8nse/loss_functions_in_instance_representation/) ⭐️ 6.0/10

一位 Reddit 用户质疑在实例表示学习中使用噪声对比估计（NCE）损失的动机和推导，具体质疑为什么使用 NCE 而不是直接近似非参数 softmax 中的分母。 这个问题突显了对比学习中常见的困惑，并引起了人们对 NCE 理论基础的关注，尽管 NCE 被广泛使用，但往往没有被完全理解。 用户指出 Wu 等人使用 NCE 来避免非参数 softmax 中难以计算的分母，但质疑是否直接用蒙特卡洛估计近似分母会等效。

reddit · r/MachineLearning · /u/No_Balance_9777 · 6月29日 23:34

**背景**: 噪声对比估计（NCE）是一种将密度估计转化为二分类问题的技术，通过区分真实数据与噪声样本。在实例表示学习中，非参数 softmax 损失在大数据集上计算不可行，因此 NCE 提供了一种可处理的近似，且被证明随着噪声样本数量的增加，其梯度会收敛到真实梯度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.baeldung.com/cs/noise-contrastive-estimation-loss">What Is Noise Contrastive Estimation Loss? | Baeldung on Computer Science</a></li>
<li><a href="https://jxmo.io/posts/nce">Demystifying Noise Contrastive Estimation – Jack Morris</a></li>
<li><a href="https://medium.com/@weidagang/demystifying-noise-contrastive-estimation-nce-in-machine-learning-32ded05401f4">Demystifying Neural Networks: Noise Contrastive Estimation ( NCE )</a></li>

</ul>
</details>

**标签**: `#representation learning`, `#contrastive learning`, `#NCE`, `#loss functions`

---

<a id="item-18"></a>
## [HEMA 从业者构建开放数据集以改进 AI 对快速剑术的追踪](https://www.reddit.com/r/MachineLearning/comments/1uivddx/i_do_historical_swordfighting_and_noticed_ai/) ⭐️ 6.0/10

一位历史欧洲武术（HEMA）练习者正在创建一个开放的多视角数据集，包含 100 个高速（120-240fps）剑术片段，并附带详细元数据注释，旨在改进 AI 对快速移动、遮挡物体的追踪能力。 该数据集解决了细长物体追踪和具身 AI 中的模拟到现实（Sim2Real）差距等关键瓶颈，因为剑术场景存在极端遮挡、运动模糊和快速移动的细长物体，当前模型难以处理。 该数据模式包括生物力学注释（架势、步法、攻击轨迹）和计算机视觉难点（遮挡评级、运动模糊），创建者正在寻求社区反馈，是否应添加剑格坐标或步法速度指标。

reddit · r/MachineLearning · /u/fonssagrives · 6月29日 15:16

**背景**: Sim2Real 差距指的是由于物理、外观和动态差异，将 AI 模型从模拟环境迁移到现实世界所面临的挑战。细长物体追踪困难，因为像剑刃这样快速移动的小物体会丢失像素细节并产生运动模糊，导致检测和追踪不可靠。该数据集旨在提供现实世界中的极端案例，帮助弥合这一差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Sim-to-real_gap">Sim-to-real gap</a></li>
<li><a href="https://github.com/liewjunhao/thin-object-selection">Deep Interactive Thin Object Selection - GitHub</a></li>
<li><a href="https://arxiv.org/abs/2202.05659">Tiny Object Tracking: A Large-scale Dataset and A Baseline GitHub - kuanhungchen/awesome-tiny-object-detection: A ... Object Tracking in Computer Vision - GeeksforGeeks Tiny Object Tracking With Proposal Position Enhancement Comprehensive review of deep learning-based tiny object ... Tiny Object Tracking: A Large-Scale Dataset and a Baseline</a></li>

</ul>
</details>

**标签**: `#computer vision`, `#dataset`, `#AI tracking`, `#HEMA`, `#embodied AI`

---