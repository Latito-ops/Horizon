---
layout: default
title: "Horizon Summary: 2026-06-24 (ZH)"
date: 2026-06-24
lang: zh
---

> 从 35 条内容中筛选出 22 条重要资讯。

---

1. [Rhombus 1.0 发布：基于 Racket 的宏可扩展语言](#item-1) ⭐️ 8.0/10
2. [Swift Package Index 加入苹果](#item-2) ⭐️ 8.0/10
3. [Meta 因数据泄露暂停员工追踪计划](#item-3) ⭐️ 8.0/10
4. [Datasette 1.0a35 新增带 JSON API 的表创建与修改功能](#item-4) ⭐️ 8.0/10
5. [提示注入即角色混淆](#item-5) ⭐️ 8.0/10
6. [使用 Claude Code 将 Moebius 0.2B 图像修复模型移植到浏览器中](#item-6) ⭐️ 8.0/10
7. [DeepSWE：面向前沿编程模型的无污染基准测试](#item-7) ⭐️ 8.0/10
8. [漏洞报告因 LLM 生成的垃圾信息而失去价值](#item-8) ⭐️ 7.0/10
9. [FUTO Swipe 开源滑行输入模型](#item-9) ⭐️ 7.0/10
10. [AI 构建的开源所见即所得 TikZ 编辑器](#item-10) ⭐️ 7.0/10
11. [维生素 D 补充剂：对大多数人夸大其词，但对严重缺乏者有效](#item-11) ⭐️ 7.0/10
12. [机器学习安全测试落后于软件标准](#item-12) ⭐️ 7.0/10
13. [非确定性漏洞检测基准系统](#item-13) ⭐️ 7.0/10
14. [uv 0.11.24 新增 CPython 3.15b3 支持及可重定位环境](#item-14) ⭐️ 6.0/10
15. [杰里的地图：六十年虚构地图绘制](#item-15) ⭐️ 6.0/10
16. [纪念红绿波浪线拼写检查发明者托尼·克鲁格](#item-16) ⭐️ 6.0/10
17. [凯文·米特尼克向帮助将他送进监狱的人赠送梦想汽车](#item-17) ⭐️ 6.0/10
18. [OPFS + Pyodide 测试工具实现浏览器中持久化 SQLite](#item-18) ⭐️ 6.0/10
19. [云 GPU 提供商选择痛点讨论](#item-19) ⭐️ 6.0/10
20. [Hugging Face 用新功能复活 Papers with Code](#item-20) ⭐️ 6.0/10
21. [寻求面向扩散 LLM 句法的鲁棒 NLI](#item-21) ⭐️ 6.0/10
22. [发现 ICLR 2026 博客文章中潜在错误](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Rhombus 1.0 发布：基于 Racket 的宏可扩展语言](https://blog.racket-lang.org/2026/06/rhombus-v1.0.html) ⭐️ 8.0/10

基于 Racket 的 Rhombus 语言发布了 1.0 版本，引入了一个强大的 `...` 宏运算符，支持对嵌套数据结构进行模式匹配和类似 map 的操作。 Rhombus 1.0 是 Racket 生态系统的一个重要里程碑，它提供了传统语法和 Racket 宏系统的全部能力，可能降低新用户的门槛并扩大语言的影响力。 `...` 运算符并非内置功能，而是一个宏，展示了 Rhombus 的宏可扩展性；它能够区分绑定上下文和表达式上下文，从而实现上下文特定的行为。

hackernews · Decabytes · 6月22日 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48633473)

**背景**: Racket 是一种 Lisp 家族语言，以其强大的卫生宏系统而闻名，但使用 S-表达式（括号）可能会构成障碍。Rhombus 最初被称为 'Racket2'，旨在提供更传统的语法，同时保留宏能力。`...` 宏运算符是 Rhombus 允许自定义语法扩展的关键示例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://beautifulracket.com/appendix/thoughts-on-rhombus.html">Beautiful Racket: Thoughts on Rhombus (formerly known as Racket2)</a></li>
<li><a href="https://github.com/racket/rhombus">GitHub - racket/rhombus: Rhombus programming language · GitHub</a></li>
<li><a href="https://news.ycombinator.com/item?id=48633473">Rhombus Language 1.0 - Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞 `...` 运算符的通用性和强大功能，有人指出它感觉像一个 splat 运算符但更灵活。其他人则表示更喜欢 S-表达式，并且有兴趣在会议上听到关于 Rhombus 的演讲。

**标签**: `#Rhombus`, `#Racket`, `#Programming Languages`, `#Macros`, `#Language Design`

---

<a id="item-2"></a>
## [Swift Package Index 加入苹果](https://swiftpackageindex.com/blog/swift-package-index-joins-apple) ⭐️ 8.0/10

苹果收购了社区维护的 Swift 包注册表 Swift Package Index (SPI)，SPI 团队加入苹果，并承诺保持项目开源。 此次收购将重要的社区资源置于苹果控制之下，既带来了对 Swift Package Manager 集成改进的希望，也引发了对苹果开源记录及可能对包索引施加新限制的担忧。 SPI 目前索引超过 11,000 个 Swift 包的元数据，是 Swift.org 的默认包搜索工具。苹果明确提到开发者身份作为未来方向，引起部分社区成员的怀疑。

hackernews · JDevlieghere · 6月23日 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48648779)

**背景**: Swift Package Manager (SPM) 是苹果用于管理 Swift 代码分发和依赖的工具。Swift Package Index (SPI) 由社区创建，提供可搜索的 Swift 包索引，填补了缺乏官方包注册表的空白。SPI 被 Swift 开发者广泛用于发现和评估包。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5mac.com/2026/06/23/swift-package-index-joins-apple-pledges-to-remain-open-source/">Swift Package Index joins Apple, pledges to remain open source</a></li>
<li><a href="https://swiftpackageindex.com/">Swift Package Index</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂：有人祝贺 SPI 团队（如 dragon-hn），也有人对苹果的掌控表示怀疑（如 jshier）。少数人提到与类似网站的混淆，一位评论者因 SPI 仅支持 GitHub 而计划构建竞争对手。

**标签**: `#swift`, `#apple`, `#package-manager`, `#open-source`, `#acquisition`

---

<a id="item-3"></a>
## [Meta 因数据泄露暂停员工追踪计划](https://www.wired.com/story/meta-pauses-employee-tracking-program-following-internal-security-breach/) ⭐️ 8.0/10

Meta 已暂停其备受争议的员工追踪计划，该计划监控键盘输入等活动以用于 AI 训练，此前一次内部数据泄露将敏感员工信息暴露给了全公司。 这一事件凸显了工作场所监控的隐私风险，并引发了对 Meta 处理敏感数据方式的质疑，尤其是在其利用员工行为训练 AI 的背景下。它还加剧了对 Meta 文化及其对信任更广泛影响的批评。 泄露的数据包括来自追踪程序的明文私人对话和绩效信息，该程序涉及全屏录制。Meta 原本打算对数据进行匿名化处理，但未能做到，导致了泄露。

hackernews · 1vuio0pswjnm7 · 6月24日 00:28 · [社区讨论](https://news.ycombinator.com/item?id=48653575)

**背景**: Meta 的员工追踪计划是一项通过记录员工与笔记本电脑的交互来训练 AI 代理的举措的一部分。此类计划因隐私问题而备受争议，而这次泄露表明在缺乏适当保护措施的情况下收集敏感数据的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wired.com/story/meta-accidentally-let-employees-access-each-others-keystroke-data/">Meta Exposed Data Internally From Its Controversial Employee-Tracking Program | WIRED</a></li>
<li><a href="https://www.businessinsider.com/meta-ai-training-data-leak-exposed-employee-activity-across-company-2026-6">Meta pauses an AI training program that tracks employees' keystrokes after an internal leak</a></li>
<li><a href="https://www.reddit.com/r/technology/comments/1uczyyq/meta_pauses_employeetracking_program_following/">Meta Pauses Employee-Tracking Program Following Internal Data Leak | The move comes after the company left potentially sensitive data from the initiative exposed internally - Reddit</a></li>

</ul>
</details>

**社区讨论**: 评论者绝大多数持批评态度，许多人表达了对 Meta 的不信任，并引用此事件作为该公司无视隐私和道德的证据。一些人指出，即使遵守规则的员工也可能因被解读为‘按章工作’的行为而受到处罚。其他人则指出 Meta 使用泄露数据的监控具有讽刺意味，削弱了其自身的安全立场。

**标签**: `#Meta`, `#surveillance`, `#privacy`, `#data leak`, `#employee tracking`

---

<a id="item-4"></a>
## [Datasette 1.0a35 新增带 JSON API 的表创建与修改功能](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a35 引入了“创建表”和“修改表”界面，每个界面都有专用的 JSON API 端点支持编程式表操作。该版本还包含了全面的模板上下文文档，该文档被视为自定义模板的稳定 API。 这些新功能显著增强了 Datasette 作为数据库管理工具的实用性，允许用户通过 UI 和 JSON API 创建和修改 SQLite 表。这为稳定的 1.0 版本铺平了道路，使 Datasette 对开发者和数据发布者更加强大。 “创建表” JSON API 支持定义列、主键、自定义类型、NOT NULL 约束、文字和表达式默认值以及单列外键。“修改表” API 可以添加、重命名、重新排序和删除列，更改列类型、默认值、约束、主键、外键，重命名表，并且还包含一个删除表按钮。

rss · Simon Willison · 6月23日 21:34

**背景**: Datasette 是一个用于探索和发布 SQLite 数据库的开源工具，提供 Web 界面和 JSON API 进行数据交互。SQLite 是一个广泛使用的嵌入式数据库引擎。JSON API 允许程序化访问数据库，此版本增加了用于模式修改的端点，此前这些操作仅限于手动 SQL 或外部工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.datasette.io/en/stable/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="http://datasette.io/blog/2026/api-extras">Datasette 1.0a33 with JSON extras in the API - Datasette Blog</a></li>

</ul>
</details>

**标签**: `#datasette`, `#release`, `#database`, `#JSON API`, `#open source`

---

<a id="item-5"></a>
## [提示注入即角色混淆](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

Charles Ye、Jasmine Cui 和 Dylan Hadfield-Menell 的研究表明，LLM 优先考虑角色标签的风格而非实际内容，从而引发了新的提示注入攻击。他们发现，对输入文本进行“去风格化”处理可将攻击成功率从 61% 降至 10%。 这揭示了 LLM 安全中的一个根本漏洞，即模型无法仅凭角色标签可靠区分可信指令与不可信用户输入。它强调，没有真正的角色感知能力，提示注入防御将始终是一场困难的猫鼠游戏。 论文引入了“角色混淆”概念，模型根据文本与内部思考块（如 <think>、<assistant>）在风格上的相似性进行解读，而非显式标签。当改变风格同时保留语义时，攻击成功率从 61% 急剧下降至 10%。

rss · Simon Willison · 6月22日 23:59

**背景**: 提示注入攻击利用了 LLM 处理指令的方式，恶意输入可能覆盖系统提示。角色标签如 <system> 和 <user> 旨在区分上下文，但这项研究表明，模型更依赖文本的“风格”而非标签本身。这一洞察解释了为何简单的格式更改就能绕过安全措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.12277">[2603.12277] Prompt Injection as Role Confusion</a></li>

</ul>
</details>

**标签**: `#prompt injection`, `#AI safety`, `#LLM security`, `#jailbreaks`

---

<a id="item-6"></a>
## [使用 Claude Code 将 Moebius 0.2B 图像修复模型移植到浏览器中](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison 借助 AI 编程助手 Claude Code，将轻量级图像修复模型 Moebius 0.2B 移植到浏览器中，通过 WebGPU 运行。目前可访问 simonw.github.io/moebius-web/ 体验在线演示。 这表明小型 AI 模型可以通过 WebGPU 在浏览器中实现实用的性能，从而在不依赖云端的情况下进行图像编辑。同时，它也展示了 Claude Code 等 AI 编程代理能够加速复杂的模型移植工作。 原版 Moebius 模型依赖 PyTorch 和 NVIDIA CUDA，但 Simon 采用了 ONNX Runtime Web 的 WebGPU 后端实现浏览器端推理。演示工具支持用户上传图片、涂抹要移除的区域，并在本地完成修复。

rss · Simon Willison · 6月22日 23:43

**背景**: 图像修复是指用合理的内容填充图像中缺失或被移除的区域。Moebius 是一个 0.2B 参数的模型，声称具有与 FLUX.1-Fill-Dev 等 10B+ 模型相当的性能，同时推理速度提升超过 15 倍。WebGPU 是一种用于底层 GPU 访问的网页标准，能够在浏览器中运行计算密集型的 AI 推理任务。Claude Code 是 Anthropic 开发的 AI 软件开发助手。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hustvl.github.io/Moebius/">Moebius Project Page</a></li>
<li><a href="https://simonwillison.net/2026/Jun/22/porting-moebius/">Porting the Moebius 0.2B image inpainting model to run in the browser with Claude Code</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebGPU">WebGPU</a></li>

</ul>
</details>

**标签**: `#image inpainting`, `#WebGPU`, `#browser AI`, `#model porting`, `#machine learning`

---

<a id="item-7"></a>
## [DeepSWE：面向前沿编程模型的无污染基准测试](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE 是一个新的开源基准测试，用于评估前沿编程模型，其特点包括：任务从头编写确保无污染、覆盖 91 个代码库和 5 种语言的高多样性、真实世界复杂度以及手写验证器。 该基准测试解决了现有代码生成评估中的关键弱点，尤其是数据污染问题，通过确保任何模型在预训练期间都未见过解决方案，从而可以更可靠地评估 AI 编程能力。 DeepSWE 提示的长度约为 SWE-bench Pro 的一半，但解决方案需要多 5.5 倍的代码和约 2 倍的输出 token，其手写验证器测试的是软件行为而非实现细节。

reddit · r/MachineLearning · /u/we_are_mammals · 6月24日 02:03

**背景**: 现有的基准测试如 SWE-bench 使用真实世界的 GitHub 问题评估 AI 模型，但可能存在数据污染问题，即模型在训练过程中可能见过类似任务。无污染基准测试如 LiveCodeBench 通过随时间收集新问题来避免这一问题。DeepSWE 在此基础上更进一步，从头创建全新任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://epoch.ai/benchmarks/swe-bench-verified">SWE-bench Verified | Epoch AI</a></li>
<li><a href="https://www.swebench.com/">SWE-bench Leaderboards</a></li>
<li><a href="https://livecodebench.github.io/">LiveCodeBench: Holistic and Contamination Free Evaluation of Large Language Models for Code</a></li>

</ul>
</details>

**标签**: `#benchmark`, `#code generation`, `#AI`, `#software engineering`, `#evaluation`

---

<a id="item-8"></a>
## [漏洞报告因 LLM 生成的垃圾信息而失去价值](https://words.filippo.io/vuln-reports/) ⭐️ 7.0/10

根据 Filippo Valsorda 最近的一篇文章，大量低质量、由 LLM 生成的漏洞报告和垃圾信息使得真实的安全披露更难被区分。 这一趋势威胁到漏洞报告的可信度，可能导致真正的问题被忽略，并增加了维护者的负担，同时也凸显了对更好自动化检测工具的需求。 Valsorda 指出，一半的主动报告是 LLM 生成的或勒索企图，甚至真实研究人员也面临怀疑；这一情况是由 LLM 使用成本低于人力成本驱动的。

hackernews · goranmoomin · 6月23日 23:42 · [社区讨论](https://news.ycombinator.com/item?id=48653216)

**背景**: 漏洞报告是安全研究人员或自动化工具发现并向软件维护者披露安全漏洞的过程。传统上，这些报告很少且很有价值。然而，随着 LLM 的兴起，自动化工具现在可以生成更多的报告，包括误报和垃圾信息，使维护者不堪重负，降低了信噪比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/huhusmang/Awesome-LLMs-for-Vulnerability-Detection">GitHub - huhusmang/Awesome-LLMs-for-Vulnerability-Detection: The community's most comprehensive, continuously-updated index of research on Large Language Models for software vulnerability detection — papers across function-level, repository-level, agentic, and smart-contract detection, plus datasets, benchmarks, and surveys.</a></li>
<li><a href="https://claroty.com/team82/research/hands-free-what-llm-driven-vulnerability-research-looks-like">Hands Free: What LLM Driven Vulnerability Research Looks Like | Claroty</a></li>
<li><a href="https://vulnrepo.com/">VULNRΞPO - Vulnerability Report Generator & Repository</a></li>

</ul>
</details>

**社区讨论**: 评论反映了挫折与谨慎乐观的混合情绪。一些用户报告频繁收到垃圾报告，而另一些用户则认为 LLM 最终将有助于修复漏洞并减少误报，从而带来更安全的生态系统。

**标签**: `#security`, `#vulnerability reporting`, `#LLM`, `#spam`, `#software engineering`

---

<a id="item-9"></a>
## [FUTO Swipe 开源滑行输入模型](https://swipe.futo.tech/) ⭐️ 7.0/10

FUTO Swipe 是由 FUTO 发布的全新开源滑行输入模型及算法套件，旨在提高移动键盘的准确性并减少词语重叠。目前该模型已集成至 FUTO 键盘，并欢迎社区广泛采用。 这很重要，因为长期以来高质量的滑行输入功能被专有且侵犯隐私的键盘应用所垄断。FUTO Swipe 提供了一种免费、开源的选择，有可能让更多平台获得滑行输入能力，并让用户对自己的输入数据拥有更大控制权。 该模型使用社区贡献的滑行数据进行训练，支持多种语言和键盘布局。它专门针对“词语重叠”问题——即相似的滑行路径产生歧义结果——这是滑行输入中常见的痛点。

hackernews · futohq · 6月23日 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48648619)

**背景**: 滑行输入（也称为手势输入）允许用户通过在键盘上滑动手指而不抬起来输入单词。传统的高质量滑行模型（如 Gboard 中的模型）是专有的，通常需要联网或收集用户数据。FUTO Swipe 是开源的，允许开发者将其集成到任何键盘应用中，同时保护用户隐私。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://swipe.futo.tech/">FUTO Swipe</a></li>
<li><a href="https://news.ycombinator.com/item?id=48648619">FUTO Swipe – A new swipe typing model | Hacker News</a></li>
<li><a href="https://swipe.futo.org/">FUTO Keyboard Swipe Training</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，用户反映新滑行模型已可与 Gboard 媲美。部分用户提到了一些小问题，如随机大写和缺乏上下文感知建议，但总体认为这是对以往开源键盘的重大改进。

**标签**: `#mobile keyboard`, `#swipe typing`, `#HCI`, `#user experience`, `#input method`

---

<a id="item-10"></a>
## [AI 构建的开源所见即所得 TikZ 编辑器](https://tikz.dev/editor/) ⭐️ 7.0/10

一款开源所见即所得 TikZ 编辑器发布，可同时显示 TikZ 源代码和渲染图形，允许通过拖拽和调整大小进行可视化编辑，并保持两个视图同步。该编辑器几乎完全由 AI 编码代理 Codex 构建。 这解决了 LaTeX 用户手动编写 TikZ 图形的长期痛点，可能节省大量时间并降低学习曲线。同时，它展示了 AI 编码代理构建复杂、小众软件的能力，这类软件对人类来说过于繁琐。 该编辑器解析 TikZ 代码并跟踪每个对象的源代码位置，从而在不改变格式的情况下覆盖坐标。一个明显限制是生成的代码使用绝对坐标，而 TikZ 通常受益于相对定位。

hackernews · DominikPeters · 6月23日 14:24 · [社区讨论](https://news.ycombinator.com/item?id=48645437)

**背景**: TikZ 是一个强大的 LaTeX 包，用于在文档中创建矢量图形，但需要手动编写坐标并重新编译才能看到结果。由于解析 TikZ 的复杂性，LaTeX 图形的所见即所得编辑器一直很少见。该项目主要由 AI Codex 构建，使用了约 7 亿个 token，ChatGPT 订阅费用约 500 美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.overleaf.com/learn/latex/TikZ_package">TikZ package - Overleaf, Online LaTeX Editor</a></li>
<li><a href="https://www.overleaf.com/learn/latex/LaTeX_Graphics_using_TikZ:_A_Tutorial_for_Beginners_(Part_1)—Basic_Drawing">LaTeX Graphics using TikZ: A Tutorial for Beginners (Part 1)—Basic Drawing - Overleaf, Online LaTeX Editor</a></li>

</ul>
</details>

**社区讨论**: 社区反馈赞扬了 UI 和概念，但批评生成的代码大量使用绝对坐标。创建者分享了使用 Codex 的成本细节，用户提到了类似的工具如 quiver.app 和 CircuitTikZ 集成。

**标签**: `#LaTeX`, `#TikZ`, `#WYSIWYG`, `#open-source`, `#editor`

---

<a id="item-11"></a>
## [维生素 D 补充剂：对大多数人夸大其词，但对严重缺乏者有效](https://dynomight.net/vitamin-d/) ⭐️ 7.0/10

这挑战了建议全民补充维生素 D 的主流健康建议，可能促使公共卫生指南转向针对确诊缺乏者的定向使用。 分析指出，许多研究未能考虑参与者的基线维生素 D 水平，且阳光的益处远不止于产生维生素 D，因此口服补充剂并非良好的替代品。

hackernews · surprisetalk · 6月23日 16:30 · [社区讨论](https://news.ycombinator.com/item?id=48647486)

**背景**: 维生素 D 是一种对钙吸收和骨骼健康至关重要的脂溶性维生素，通常通过皮肤暴露在阳光下合成。北方纬度地区缺乏现象普遍，导致广泛推荐补充。然而，针对非骨骼健康益处的随机对照试验结果不一，引发了持续的科学争论。

**社区讨论**: 评论者普遍称赞文章的中立态度，有人分享了服用维生素 D 后情绪和免疫力改善的个人经历。其他人强调阳光对健康的多种益处远超维生素 D。一位评论者指出 NHANES 缺乏调查因季节和纬度数据收集限制而存在方法论问题。

**标签**: `#health`, `#vitamin D`, `#science`, `#nutrition`, `#analysis`

---

<a id="item-12"></a>
## [机器学习安全测试落后于软件标准](https://www.reddit.com/r/MachineLearning/comments/1uddtws/are_model_security_risks_extraction_poisoning/) ⭐️ 7.0/10

Reddit 用户 Xorphian 发文指出，许多机器学习团队在部署模型时跳过了对抗性安全测试，这与经过严格安全审查的常规软件形成对比。 这一疏忽使组织面临模型窃取和投毒攻击的风险，可能导致知识产权被盗和模型完整性受损，凸显了在机器学习生产中采用与传统软件相当的安全实践的紧迫性。 模型窃取攻击是指对手通过系统查询 API 来窃取模型行为，而模型投毒攻击则是操纵训练数据或参数以改变模型行为。该帖邀请行业从业者分享他们所在公司是否实际进行了此类测试。

reddit · r/MachineLearning · /u/Xorphian · 6月23日 10:52

**背景**: 对抗性机器学习是研究机器学习模型攻击与防御的学科。模型窃取攻击使拥有查询权限的攻击者通过构建副本窃取模型功能。模型投毒攻击在训练过程中注入恶意数据以改变模型输出。尽管存在这些风险，部署前的对抗性测试在许多机器学习团队中尚未成为标准做法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.praetorian.com/blog/stealing-ai-models-through-the-api-a-practical-model-extraction-attack/">Stealing AI Models Through the API: A Practical Model Extraction Attack | Praetorian</a></li>
<li><a href="https://owasp.org/www-project-machine-learning-security-top-10/docs/ML10_2023-Model_Poisoning">OWASP Machine Learning Security Top Ten 2023 | ML10:2023 Model Poisoning | OWASP Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adversarial_machine_learning">Adversarial machine learning - Wikipedia</a></li>

</ul>
</details>

**标签**: `#model security`, `#adversarial testing`, `#ML production`, `#AI safety`, `#software security`

---

<a id="item-13"></a>
## [非确定性漏洞检测基准系统](https://www.reddit.com/r/MachineLearning/comments/1ud0rft/nondeterministic_vulnerability_detection/) ⭐️ 7.0/10

这是一个正在进行的基准测试，它修改 Juliet 测试用例使其看起来像真实代码，并注入各种评论情感，以评估 LLM 漏洞检测的鲁棒性。 该基准测试通过隐藏已知模式并测试对评论情感的敏感性，解决了基于 LLM 的漏洞检测的一个已知局限性，这对于实际部署至关重要。 该基准测试使用覆盖数百个 CWE 的 Juliet 测试用例，将其修改为类似真实代码库，并注入 LLM 生成的准确、误导或中性情感的评论。

reddit · r/MachineLearning · /u/Psychological_Meat_6 · 6月22日 23:34

**背景**: Juliet 测试用例是漏洞检测的标准基准，包含常见弱点枚举（CWE）的例子。LLM 在检测漏洞方面表现出色，但可能被简单的修改或误导性评论欺骗。该基准旨在通过模糊测试用例来源并引入情感偏见来提供更真实的评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/find-sec-bugs/juliet-test-suite">GitHub - find-sec-bugs/juliet-test-suite: :microscope: A collection of test cases in the Java language. It contains examples for 112 different CWEs. · GitHub</a></li>
<li><a href="https://www.castsoftware.com/pulse/juliet-and-owasp-benchmark-results-how-cast-tests">Juliet and OWASP Benchmark Results: How CAST Tests Against 2 Most Important Application Security Standards in 2019</a></li>

</ul>
</details>

**标签**: `#vulnerability detection`, `#benchmark`, `#LLM`, `#security`, `#machine learning`

---

<a id="item-14"></a>
## [uv 0.11.24 新增 CPython 3.15b3 支持及可重定位环境](https://github.com/astral-sh/uv/releases/tag/0.11.24) ⭐️ 6.0/10

uv 0.11.24 增加了对 CPython 3.15.0b3 的支持，并引入了可重定位项目环境的预览功能，同时包含性能改进和错误修复。 该版本使 uv 保持与最新 Python 测试版同步，便于早期测试；可重定位环境预览功能解决了长期存在的 Python 环境可移植需求。紧凑索引等性能优化进一步巩固了 uv 作为快速包管理器的声誉。 可重定位环境功能需在预览标志下启用，且仅影响项目环境。此版本还修复了存档 ID 冲突以及项目环境中透明 Python 升级等错误。

github · github-actions[bot] · 6月23日 21:16

**背景**: uv 是一个用 Rust 编写的快速现代 Python 包管理器，旨在作为 pip 和 pip-tools 的直接替代品。可重定位环境允许将 Python 虚拟环境移动或复制到不同路径而不会损坏，这对部署和 CI 场景很有用。用于惰性版本映射的紧凑索引减少了依赖解析时的内存使用量。本次发布中可使能禁用的 'exclude-newer' 选项有助于通过忽略指定日期后发布的包来创建可重现的环境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://relenv.readthedocs.io/en/v0.4.1/">Relenv - Build and use relocatable Python environments</a></li>
<li><a href="https://pydevtools.com/handbook/how-to/how-to-use-exclude-newer-for-reproducible-python-environments/">Use uv --exclude-newer for Reproducible Installs | pydevtools</a></li>

</ul>
</details>

**标签**: `#Python`, `#package management`, `#uv`, `#release`

---

<a id="item-15"></a>
## [杰里的地图：六十年虚构地图绘制](http://www.jerrysmap.com/the-map) ⭐️ 6.0/10

自 1963 年以来，艺术家杰里一直持续绘制和扩展一张虚构大陆的地图，并使用一副特制卡牌来决定每块新地图图块的特征。 这个项目体现了局外人艺术和生成性创作约束的力量，激发了关于创造力、系统以及长期艺术投入的讨论。 该过程涉及抽取一张卡牌，决定下一块图块是否包含河流、山脉、城市或其他特征；地图已扩展到多张图纸，并可在线上查看。

hackernews · turtleyacht · 6月23日 18:40 · [社区讨论](https://news.ycombinator.com/item?id=48649435)

**背景**: 杰里的地图是一个长期运行的局外人艺术项目。局外人艺术指的是在官方文化边界之外创作的艺术，通常由自学成才的个人完成。杰里使用一套卡牌系统来指导他的创作决策，确保结构性与自发性的结合。该项目因其沉思和不断演变的特性而获得了一批追随者。

**社区讨论**: 评论者们分享了自己童年类似绘制地图的经历，赞赏卡牌驱动的创作过程，并提供了相关视频和互动版本的链接。一些人指出其与局外人艺术以及《矮人要塞》等游戏的关联。

**标签**: `#art`, `#map`, `#creative process`, `#outsider art`, `#Hacker News`

---

<a id="item-16"></a>
## [纪念红绿波浪线拼写检查发明者托尼·克鲁格](https://devblogs.microsoft.com/oldnewthing/20260622-00/?p=112451) ⭐️ 6.0/10

雷蒙德·陈的文章向托尼·克鲁格致敬，他引入了如今无处不在的红色和绿色波浪下划线，用于文字处理器的实时拼写检查。 这个看似微小的用户体验创新从根本上改变了人们与文本交互的方式，使错误检测变得即时且不突兀。它已成为几乎所有现代文字处理器的标准功能，影响了几十年的软件设计。 文章指出，托尼·克鲁格将拼写检查功能移植到了 Microsoft Word，而波浪下划线的概念可能源于更早的程序，如 Amiga 上的 ProWrite，它使用红色波浪线标记拼写错误的单词。

hackernews · saikatsg · 6月23日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=48648959)

**背景**: 在实时拼写检查出现之前，用户必须在写作后手动运行单独的拼写检查程序。波浪下划线在不中断打字流程的情况下提供即时视觉反馈。红色下划线通常表示拼写错误，绿色则表示语法问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Spell_checker">Spell checker - Wikipedia</a></li>
<li><a href="https://support.microsoft.com/en-us/office/check-spelling-and-grammar-in-office-5cdeced7-d81d-47de-9096-efd0ee909227">Check spelling and grammar in Office | Microsoft Support</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了不同的看法：一些人称赞这一创新的影响，而另一些人指出在多语言环境中，由于语言检测不正确，波浪线用处不大。一位评论者指出了陈的文章与维基百科之间存在循环引用问题。

**标签**: `#computing history`, `#spell check`, `#Raymond Chen`, `#ux`

---

<a id="item-17"></a>
## [凯文·米特尼克向帮助将他送进监狱的人赠送梦想汽车](https://www.thedrive.com/news/this-man-was-gifted-his-dream-car-by-the-notorious-hacker-he-put-in-prison) ⭐️ 6.0/10

曾经臭名昭著的黑客凯文·米特尼克将他梦想中的汽车赠送给了帮助抓捕并监禁他的肖恩·纳利，作为多年后建立的友谊的表示。 这个故事说明了高调案件中可能出现的意想不到的个人联系，使传奇黑客和帮助抓捕他的人都更加人性化，并凸显了米特尼克出狱后转型为安全顾问的过程。 肖恩·纳利曾在一家电信公司工作，在追踪米特尼克的电话活动并导致其 1995 年被捕中发挥了关键作用。米特尼克后来成为安全顾问和作家，于 2023 年 7 月去世。

hackernews · mauvehaus · 6月22日 18:03 · [社区讨论](https://news.ycombinator.com/item?id=48633643)

**背景**: 凯文·米特尼克是 1990 年代最受通缉的计算机黑客之一，以侵入大型公司系统而闻名。他在肖恩·纳利的帮助下被抓获，因此被判五年监禁。获释后，米特尼克重新塑造自己为安全顾问、作家和主题演讲者，并最终与纳利成为了朋友。

**社区讨论**: 社区评论指出，米特尼克的咨询工作有时缺乏技术深度，侧重于物理安全而非常见的 SQL 注入等漏洞。然而，许多人对他影响了一代黑客如乔治·霍兹表示钦佩，并赞赏他与纳利后期友谊中展现的人性。也有人遗憾米特尼克和 Shimomura 从未和解。

**标签**: `#Kevin Mitnick`, `#hacker culture`, `#cybersecurity history`, `#human interest`

---

<a id="item-18"></a>
## [OPFS + Pyodide 测试工具实现浏览器中持久化 SQLite](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison 创建了一个测试工具，将源私有文件系统 (OPFS) 与 Pyodide 结合，探索 Datasette Lite 是否可以在浏览器中完全编辑存储在用户计算机上的持久化 SQLite 文件。 这一实验可以使通过 WebAssembly 运行的 Python Web 应用程序实现完全客户端、持久化的数据编辑，减少对服务器后端的依赖，并提升像 Datasette Lite 这样的工具的离线能力。 该测试工具使用了 OPFS API（一种高性能、源私有、用户不可见的虚拟文件系统）和 Pyodide（一种基于 WebAssembly 的浏览器端 Python 发行版）。

rss · Simon Willison · 6月23日 18:58

**背景**: Pyodide 是一个基于 WebAssembly 的 Python 发行版，可在浏览器和 Node.js 中运行，使 Python 代码能在浏览器中执行。源私有文件系统 (OPFS) 是文件系统 API 的一部分，提供了一个沙盒化、源特定的高性能存储区域。Datasette Lite 是通过 Pyodide 完全在浏览器中运行的 Datasette 数据探索工具版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN</a></li>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.0</a></li>

</ul>
</details>

**标签**: `#browsers`, `#pyodide`, `#webassembly`, `#datasette-lite`, `#opfs`

---

<a id="item-19"></a>
## [云 GPU 提供商选择痛点讨论](https://www.reddit.com/r/MachineLearning/comments/1udfovh/whats_your_biggest_pain_point_when_choosing/) ⭐️ 6.0/10

一位机器学习工程师在 Reddit 上发帖，询问社区在比较用于 LLM 推理的云 GPU 提供商时，通常采用的方法和遇到的痛点。 该讨论反映了众多机器学习从业者在选择高性价比和可靠的 GPU 资源时面临的实际挑战，这直接影响 LLM 应用的开发和部署成本。 该工程师提到目前使用电子表格手动比较$/小时、$/token、吞吐量和可靠性等指标，并询问是否有工具或资源能简化这一过程。

reddit · r/MachineLearning · /u/Technomadlyf · 6月23日 12:24

**标签**: `#cloud GPU`, `#LLM inference`, `#cost comparison`, `#ML engineering`, `#discussion`

---

<a id="item-20"></a>
## [Hugging Face 用新功能复活 Papers with Code](https://www.reddit.com/r/MachineLearning/comments/1ucm508/some_new_updates_to_papers_with_code_p/) ⭐️ 6.0/10

Hugging Face 的 Niels 宣布了 Papers with Code 的新功能，包括用于前三名基准分数的 SOTA 徽章、结合 GitHub 星标和 Hugging Face 活动的趋势分数、支持外部评估以及更多基准和任务。 这些改进提升了 SOTA 模型和热门研究的可发现性，帮助社区在彼此工作的基础上继续发展。这标志着在 Meta 于 2025 年 7 月关闭后，Papers with Code 的重要复兴，现在与 Hugging Face 生态系统整合。 趋势分数现在同时考虑 GitHub 星标速度和 Hugging Face 工件（模型、数据集、Spaces）。如果某篇论文在基准测试中排名前三，则会显示 SOTA 徽章；外部评估功能允许在论文自身结果旁显示第三方基准结果。

reddit · r/MachineLearning · /u/NielsRogge · 6月22日 14:29

**背景**: Papers with Code 曾是一个广泛使用的平台，用于索引机器学习论文、链接代码并跟踪基准上的 SOTA 结果。Meta 在 2025 年 7 月关闭了该平台，将域名重定向到 Hugging Face Trending Papers。Hugging Face 现在正以 paperswithcode.co 的形式复活它，并利用 Hugging Face Hub（如模型和数据集）增加新功能。这些新功能旨在使研究发现更具可重复性和社区驱动性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.codesota.com/papers-with-code">Papers With Code Alternative: SOTA Leaderboards and Archived Data | CodeSOTA | CodeSOTA</a></li>
<li><a href="https://posttrainbench.com/">PostTrainBench</a></li>
<li><a href="https://arxiv.org/abs/2603.08640">[2603.08640] PostTrainBench: Can LLM Agents Automate LLM Post-Training?</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#papers with code`, `#open source`, `#SOTA`, `#huggingface`

---

<a id="item-21"></a>
## [寻求面向扩散 LLM 句法的鲁棒 NLI](https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/) ⭐️ 6.0/10

一位 Reddit 用户询问关于句法鲁棒的自然语言推理（NLI）的文献，以评估扩散大语言模型（LLM）生成的不完美文本的语义正确性。 这突显了评估扩散 LLM 时的一个空白，这些模型经常生成句法有噪声的文本，使得标准 NLI 的使用复杂化。解决这个问题可以提高 LLM 评估框架的可靠性。 用户特别提到像 LLaDA 这样的扩散 LLM，以及在应用 NLI 评估正确性时句法噪声的挑战。他们寻求句法鲁棒 NLI 的最新技术水平。

reddit · r/MachineLearning · /u/RepresentativeBee600 · 6月22日 21:51

**背景**: 自回归 LLM 逐个 token 生成文本，而扩散 LLM（如 LLaDA）通过逐渐去噪随机序列生成文本，可能导致句法错误。NLI 是一项任务，用来判断给定前提时假设是蕴含、矛盾还是中立，常用于评估 LLM 输出。标准 NLI 模型对句法变化敏感，因此对扩散 LLM 输出的鲁棒性较差。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/">Syntactically robust NLI for semantics of imperfectly generated text? [R] - Reddit</a></li>
<li><a href="https://github.com/ML-GSAI/LLaDA">GitHub - ML-GSAI/LLaDA: Official PyTorch implementation for "Large Language Diffusion Models" · GitHub</a></li>
<li><a href="https://aclanthology.org/2023.iwcs-1.29.pdf">[PDF] AMR4NLI: Interpretable and robust NLI measures from semantic graph - ACL Anthology</a></li>

</ul>
</details>

**标签**: `#NLI`, `#LLM evaluation`, `#diffusion LLMs`, `#syntax robustness`, `#semantics`

---

<a id="item-22"></a>
## [发现 ICLR 2026 博客文章中潜在错误](https://www.reddit.com/r/MachineLearning/comments/1ud9i2g/found_a_potential_mistake_in_an_iclr_2026/) ⭐️ 6.0/10

一位 Reddit 用户报告了 ICLR 2026 博客文章中的一个潜在错误，已创建 GitHub issue 并联系作者，但数周未获回复。 这凸显了社区同行评审在预印本和博客文章平台中的重要性，尤其是对于 ICLR 这样的顶级会议。 具体错误在 iclr-blogposts/2026 仓库的 GitHub issue #218 中有详细说明，但用户寻求验证后再升级问题。

reddit · r/MachineLearning · /u/metalwhaledev · 6月23日 06:39

**背景**: ICLR（国际学习表征会议）是顶级机器学习会议，除传统论文外还发布博客文章投稿。ICLR 博客论文轨让研究人员以更易读的形式呈现新想法或批评。社区驱动的错误检测是开放科学中的常见做法。

**标签**: `#ICLR`, `#machine learning`, `#blog post review`, `#community inquiry`

---