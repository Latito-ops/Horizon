---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 37 items, 19 important content pieces were selected

---

1. [AI Unlocks First Reading of Herculaneum Scroll](#item-1) ⭐️ 9.0/10
2. [Superhuman Generals.io AI via Self-Play RL Open-Sourced](#item-2) ⭐️ 9.0/10
3. [Zig's endian-agnostic bitCast and LLVM backend boost](#item-3) ⭐️ 8.0/10
4. [Hacker News Trends: Google Trends for 18 years of comments](#item-4) ⭐️ 8.0/10
5. [Half-Life 2 Runs in a Web Browser via WebAssembly](#item-5) ⭐️ 8.0/10
6. [Anthropic Accuses Alibaba of Illicit Claude Model Extraction](#item-6) ⭐️ 8.0/10
7. [All routes lead to collapse: attention pathologies unified under norm-blind metric](#item-7) ⭐️ 8.0/10
8. [Fine-Tuning SLMs on Frontier Traces Cuts Costs, Maintains Quality](#item-8) ⭐️ 8.0/10
9. [DeepSWE: A New Benchmark for Evaluating Coding Agents](#item-9) ⭐️ 8.0/10
10. [LLM Inference Pricing Comparison Reveals Surprising Caching Costs](#item-10) ⭐️ 8.0/10
11. [Unit Tests Cannot Capture Code Taste](#item-11) ⭐️ 7.0/10
12. [Apple hikes MacBook and iPad prices amid rising memory costs](#item-12) ⭐️ 7.0/10
13. [SQLite database of MDN browser compatibility data](#item-13) ⭐️ 7.0/10
14. [LLM-Generated Job Applications Erode Authenticity](#item-14) ⭐️ 7.0/10
15. [Curated list of top open-source OCR models](#item-15) ⭐️ 7.0/10
16. [MuJoFil: GPU-native simulator for vision RL](#item-16) ⭐️ 7.0/10
17. [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](#item-17) ⭐️ 7.0/10
18. [Datasette 1.0a35 adds create/alter table interfaces](#item-18) ⭐️ 6.0/10
19. [OPFS + Pyodide Test Harness for Persistent Browser Storage](#item-19) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [AI Unlocks First Reading of Herculaneum Scroll](https://scrollprize.org/firstscroll) ⭐️ 9.0/10

For the first time, an AI-powered effort has successfully read text from a carbonized Herculaneum scroll that was buried by the eruption of Mount Vesuvius in 79 AD. The breakthrough was achieved through the Vesuvius Challenge, using machine learning to detect ink on 3D X-ray scans. This achievement opens a new frontier in archaeology and history, potentially recovering lost ancient texts that were thought to be permanently inaccessible. It also demonstrates the transformative power of AI for cultural heritage preservation. The scroll is part of the Herculaneum papyri collection, consisting of over 1,800 scrolls discovered in the Villa of the Papyri. The reading was accomplished by teams participating in the Vesuvius Challenge, which awarded over $1.8 million in prizes.

hackernews · verditelabs · Jun 25, 15:48 · [Discussion](https://news.ycombinator.com/item?id=48675179)

**Background**: The Herculaneum papyri were carbonized when Vesuvius erupted in 79 AD, making them extremely brittle and unreadable by conventional means. In 2019, a NEH grant funded development of machine-learning methods to detect ink on 3D X-ray scans, leading to the first successful reading of a scroll in 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vesuvius_Challenge">Vesuvius Challenge</a></li>
<li><a href="https://scrollprize.org/">Vesuvius Challenge — Reading the Herculaneum Scrolls with AI</a></li>
<li><a href="https://www.neh.gov/news/students-decipher-2000-year-old-herculaneum-scrolls">Students Decipher 2,000-Year-Old Herculaneum Scrolls</a></li>

</ul>
</details>

**Discussion**: Community comments show excitement and curiosity, with questions about translation tone and the technology's potential. A team member from the Vesuvius Challenge offered to answer questions, indicating active engagement. Some users expressed hope for reading entire ancient libraries.

**Tags**: `#AI`, `#archaeology`, `#Herculaneum`, `#Vesuvius Challenge`, `#ancient text`

---

<a id="item-2"></a>
## [Superhuman Generals.io AI via Self-Play RL Open-Sourced](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/) ⭐️ 9.0/10

A self-play reinforcement learning agent achieved #1 on the Generals.io 1v1 leaderboard, surpassing human performance. The entire pipeline, including a fast JAX-based simulator and a Vision Transformer-based agent, has been open-sourced. This demonstrates that scaling compute and model architecture (Vision Transformer, JAX) can achieve superhuman performance in imperfect-information real-time strategy games without complex hand-crafted features. The open-source release provides a valuable benchmark and toolkit for the RL community. The agent uses a Vision Transformer instead of a CNN, and the entire pipeline is implemented in JAX for faster training. The project started as a master's thesis and evolved through behavior cloning and RL fine-tuning before reaching superhuman level.

reddit · r/MachineLearning · /u/shrekofspeed · Jun 24, 16:18

**Background**: Generals.io is a fast-paced multiplayer strategy game where players command armies, protect their general, and capture enemies. Self-play reinforcement learning trains an agent by playing against itself, improving through iterative competition. Vision Transformers adapt the transformer architecture for image data by treating image patches as tokens.

<details><summary>References</summary>
<ul>
<li><a href="https://generals.io/">generals . io</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision_transformer">Vision transformer</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#self-play`, `#open-source`, `#game AI`, `#scaling`

---

<a id="item-3"></a>
## [Zig's endian-agnostic bitCast and LLVM backend boost](https://ziglang.org/devlog/2026/#2026-06-25) ⭐️ 8.0/10

Zig introduced endian-agnostic semantics for the @bitCast builtin, making bit-level operations behave identically across all targets. The LLVM backend also received optimizations for arbitrary-width integer lowering. This change significantly improves portability for bit-packed binary formats and reduces the need for manual endianness handling. The LLVM backend optimizations also enhance performance for systems using arbitrary-width integers. Under the new semantics, @bitCast operates on logical bit representation rather than memory layout, so bitcasting [2]u8 to u16 yields identical results on big- and little-endian targets. The LLVM backend now lowers arbitrary-width integers (e.g., u4, i13) to more efficient representations.

hackernews · kouosi · Jun 25, 14:19 · [Discussion](https://news.ycombinator.com/item?id=48673825)

**Background**: Zig is a systems programming language emphasizing safety and performance. The @bitCast builtin reinterprets the bits of a value as another type. Previously, its behavior depended on target endianness, causing portability issues. Arbitrary-width integers are integers with non-standard bit widths, often used in protocols and embedded systems.

<details><summary>References</summary>
<ul>
<li><a href="https://ziglang.org/devlog/2026/">Devlog ⚡ Zig Programming Language</a></li>
<li><a href="https://ziggit.dev/t/devlog-new-bitcast-semantics-and-llvm-backend-improvements/16336">Devlog ⚡ New @bitCast Semantics and LLVM Backend Improvements</a></li>
<li><a href="https://www.openmymind.net/Zigs-bitCast/">Zig's @bitCast - openmymind.net</a></li>

</ul>
</details>

**Discussion**: Commenters praised the devlog's technical depth and clarity, with one noting the new semantics will simplify working with bit-packed binary headers. However, some debated the value of arbitrary-width integers, suggesting manual packing might provide a clearer mental model of generated code.

**Tags**: `#zig`, `#programming-languages`, `#compiler`, `#llvm`, `#type-system`

---

<a id="item-4"></a>
## [Hacker News Trends: Google Trends for 18 years of comments](https://hackernewstrends.com/) ⭐️ 8.0/10

A user created Hacker News Trends, a web tool that visualizes how often keywords appear in Hacker News comments over the past 18 years, mirroring Google Trends functionality for HN content. This tool provides unique historical trend data for discussions on a major tech community platform, enabling researchers and enthusiasts to track technology discourse over time. The tool indexes 18 years of HN comments but may have data gaps, as noted in bug reports where results cut off at 2018-10 for certain keyword comparisons.

hackernews · ytkimirti · Jun 25, 14:08 · [Discussion](https://news.ycombinator.com/item?id=48673671)

**Discussion**: Comments highlighted alternative databases like ClickHouse for querying HN data, noted differences between search trends and text trends, reported bugs such as truncated results, and mentioned server rate-limiting issues.

**Tags**: `#Hacker News`, `#data visualization`, `#trends`, `#tool`, `#community`

---

<a id="item-5"></a>
## [Half-Life 2 Runs in a Web Browser via WebAssembly](https://hl2.slqnt.dev/) ⭐️ 8.0/10

A developer has successfully ported Half-Life 2 to run entirely within a web browser using WebAssembly, enabling playable gameplay without downloads or plugins. This demonstration showcases the advanced capabilities of WebAssembly for running complex, legacy games directly in the browser, potentially expanding accessibility and preservation of classic titles. The port is based on the source code of Half-Life 2 and compiled using Emscripten, but reportedly lacks some shaders such as character eyes, resulting in less accurate rendering compared to the original.

hackernews · panza · Jun 25, 06:00 · [Discussion](https://news.ycombinator.com/item?id=48669534)

**Background**: WebAssembly (Wasm) is a portable binary instruction format designed for high-performance execution in web browsers, often used as a compilation target for languages like C and C++. Emscripten is a compiler toolchain that converts C/C++ code into WebAssembly, enabling native applications to run on the web. This project demonstrates the feasibility of porting full-fledged games to the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="https://en.wikipedia.org/wiki/Emscripten">Emscripten</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted other similar projects like Quake 3 and Unreal Tournament in the browser, and noted that macOS users who cannot run the Steam version due to 32-bit deprecation can now play Half-Life 2 via this web port.

**Tags**: `#webassembly`, `#gaming`, `#browser`, `#emscripten`, `#porting`

---

<a id="item-6"></a>
## [Anthropic Accuses Alibaba of Illicit Claude Model Extraction](https://www.reuters.com/world/china/anthropic-says-alibaba-illicitly-extracted-claude-ai-model-capabilities-2026-06-24/) ⭐️ 8.0/10

Anthropic publicly accused Alibaba of using illicit methods to extract capabilities from its Claude AI models, potentially through systematic querying and distillation. This allegation highlights growing tensions over AI model theft and intellectual property in the industry, and could set legal precedents for protecting proprietary AI models. The accusation involves Chinese resellers offering Claude tokens at 70-90% below official prices, using payment fraud and pooling accounts, then selling output and reasoning traces as training data.

hackernews · htrp · Jun 24, 19:48 · [Discussion](https://news.ycombinator.com/item?id=48664814)

**Background**: Model extraction attacks allow adversaries to clone a proprietary LLM by querying its API and training a surrogate model. This is akin to 'knowledge distillation' but done without authorization, potentially violating terms of service. Such attacks can cost as little as $50 to approximate a model's behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2502.16065v1">A Survey of Model Extraction Attacks and Defenses in ...</a></li>
<li><a href="https://beyondscale.tech/blog/ai-model-extraction-attacks-defense-guide">AI Model Extraction Attacks: Stop LLM Theft | BeyondScale</a></li>
<li><a href="https://briandcolwell.com/an-introduction-to-ai-model-extraction/">An Introduction To AI Model Extraction - Brian D. Colwell</a></li>

</ul>
</details>

**Discussion**: Commenters debated the legality and ethics of model extraction: some argued that since Anthropic trained on unlicensed data, it cannot claim protection, while others noted that breaking terms of service is not necessarily illegal, but systematic distillation harms commercial interests.

**Tags**: `#AI`, `#model extraction`, `#security`, `#Anthropic`, `#Alibaba`

---

<a id="item-7"></a>
## [All routes lead to collapse: attention pathologies unified under norm-blind metric](https://www.reddit.com/r/MachineLearning/comments/1ufgwxl/r_all_routes_lead_to_collapse_attention_sinks/) ⭐️ 8.0/10

A new paper argues that attention sinks, representation collapse, and norm stratification in transformers are all manifestations of softmax attention using a norm-blind similarity metric, and demonstrates this across five different architectures including GPT-2, Pythia, GATs, Mamba, RWKV, and a Qwen3 variant. This insight could fundamentally change how researchers diagnose and fix attention-related issues in transformers, showing that many separate problems share a single root cause rather than requiring individual fixes. The key observation is that softmax attention can be rewritten as a Boltzmann distribution over Euclidean distances only if all keys have the same norm; standard attention throws away the key norm term, creating a norm-blind metric.

reddit · r/MachineLearning · /u/entropy_- · Jun 25, 17:38

**Background**: Transformers use softmax attention to compute weighted averages of values based on similarity between queries and keys. Over time, researchers observed several pathological behaviors: attention sinks (concentration on a few tokens), representation collapse (low-rank activations), and norm stratification (varying key norms). These were typically treated as separate issues requiring individual solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.11487">[2603.11487] Attention Sinks Are Provably Necessary in Softmax Transformers: Evidence from Trigger-Conditional Tasks</a></li>
<li><a href="https://www.emergentmind.com/topics/attention-sink-phenomenon">Attention Sink Phenomenon in Transformers</a></li>
<li><a href="https://proceedings.neurips.cc/paper_files/paper/2022/file/df4f371f1f89ec8ba5014b3310578048-Paper-Conference.pdf">On the Representation Collapse of</a></li>

</ul>
</details>

**Discussion**: The discussion is not provided in the input, but given the technical depth and the author's request for feedback, it is likely substantive. No specific comments are available to summarize.

**Tags**: `#transformer`, `#attention mechanisms`, `#representation collapse`, `#norm stratification`, `#machine learning theory`

---

<a id="item-8"></a>
## [Fine-Tuning SLMs on Frontier Traces Cuts Costs, Maintains Quality](https://www.reddit.com/r/MachineLearning/comments/1ufgpnh/r_compiling_agentic_workflows_into_llm_weights/) ⭐️ 8.0/10

Researchers propose compiling the orchestration logic of frontier LLMs into the weights of a small fine-tuned model, dubbed a 'subterranean agent', achieving near-frontier quality at roughly 1% of the cost. This method dramatically reduces inference costs and latency for deploying agentic workflows, making advanced AI capabilities accessible to more organizations without relying on expensive frontier models. The approach uses supervised fine-tuning on traces from frontier model orchestration (e.g., tool calls, planning steps) to embed the entire workflow into the weights of a small model, eliminating the need for external orchestration frameworks at runtime.

reddit · r/MachineLearning · /u/ThirdWaveCat · Jun 25, 17:31

**Background**: Agentic workflows involve multiple steps where a large language model calls tools, reasons, and performs actions, often orchestrated by frameworks like LangGraph or CrewAI. These external managers add cost and latency. The paper builds on prior work (e.g., FireAct, WorkflowLLM) that compiles agent capabilities into model weights, extending it to whole workflows orchestrated by frontier models.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.22502">[2605.22502] Compiling Agentic Workflows into LLM Weights: Near-Frontier Quality at Two Orders of Magnitude Less Cost</a></li>
<li><a href="https://arxiv.org/html/2605.22502v1">Compiling Agentic Workflows into LLM Weights: Near-Frontier Quality at Two Orders of Magnitude Less Cost</a></li>
<li><a href="https://franklineh.com/learn/research/TxUTZclHWIvPOf5W7cjm">Compiling Agentic Workflows into LLM Weights: Near-... | AI Research</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#agentic workflows`, `#fine-tuning`, `#cost efficiency`

---

<a id="item-9"></a>
## [DeepSWE: A New Benchmark for Evaluating Coding Agents](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE is a new open-source benchmark designed to evaluate frontier coding agents on real-world software engineering tasks, addressing contamination, diversity, complexity, and verification limitations of existing benchmarks. This benchmark provides a more realistic and reliable evaluation of coding agents, which is crucial for advancing AI-assisted software development and for comparing models like GPT-4 and Claude on practical coding challenges. DeepSWE tasks are written from scratch to avoid data contamination, span 91 repositories across 5 languages, and require 5.5 times more code than SWE-bench Pro, with hand-written verifiers testing software behavior.

reddit · r/MachineLearning · /u/we_are_mammals · Jun 24, 02:03

**Background**: Existing benchmarks like SWE-bench evaluate AI models on real-world GitHub issues by requiring them to generate patches. However, they suffer from data contamination (models may have seen solutions during training) and limited diversity. DeepSWE aims to overcome these issues by creating unique tasks and using diverse repositories.

<details><summary>References</summary>
<ul>
<li><a href="https://epoch.ai/benchmarks/swe-bench-verified">SWE-bench Verified | Epoch AI</a></li>
<li><a href="https://www.swebench.com/">SWE-bench Leaderboards</a></li>

</ul>
</details>

**Tags**: `#benchmark`, `#coding agents`, `#LLM evaluation`, `#software engineering`, `#AI`

---

<a id="item-10"></a>
## [LLM Inference Pricing Comparison Reveals Surprising Caching Costs](https://www.reddit.com/r/MachineLearning/comments/1ueavxn/i_compiled_llm_inference_pricing_across_7/) ⭐️ 8.0/10

A Reddit user compiled and shared a spreadsheet comparing LLM inference pricing across 7 providers, highlighting dramatic differences in cached versus uncached input token costs, especially for models like DeepSeek V4 Pro. This comparison is crucial for practitioners optimizing costs in applications with reusable context, such as agents, RAG pipelines, and multi-turn conversations, where caching policies can outweigh headline token prices. The spreadsheet tracks input/output token pricing, context windows, cached input pricing, and supported models from providers including OpenRouter, DeepSeek, Together AI, Fireworks, and Groq. The author notes that some providers document caching clearly while others barely mention it.

reddit · r/MachineLearning · /u/Technomadlyf · Jun 24, 11:28

**Background**: LLM inference caching stores previously computed results for repeated prompt prefixes, significantly reducing latency and cost. A cache hit can be tens of times cheaper than a cache miss, making caching strategy critical for cost-sensitive applications. Providers implement caching differently, with varying transparency and pricing models.

<details><summary>References</summary>
<ul>
<li><a href="https://machinelearningmastery.com/build-an-inference-cache-to-save-costs-in-high-traffic-llm-apps/">Build an Inference Cache to Save Costs in High-Traffic LLM ...</a></li>
<li><a href="https://towardsdatascience.com/why-care-about-promp-caching-in-llms/">Why Care About Prompt Caching in LLMs? | Towards Data Science</a></li>
<li><a href="https://aws.amazon.com/blogs/database/optimize-llm-response-costs-and-latency-with-effective-caching/">Optimize LLM response costs and latency with effective caching | Amazon Web Services</a></li>

</ul>
</details>

**Tags**: `#LLM pricing`, `#inference`, `#caching`, `#cost optimization`, `#model providers`

---

<a id="item-11"></a>
## [Unit Tests Cannot Capture Code Taste](https://dev.karltryggvason.com/you-cant-unit-test-for-taste/) ⭐️ 7.0/10

The article argues that qualitative aspects of code quality like 'taste' are beyond the reach of unit tests, challenging the notion that automated testing can fully ensure software excellence. This perspective highlights the limits of automation in software engineering, urging developers to rely on human judgment and experience for aspects that cannot be quantified. The article's score is 7.0/10, and it sparked a community discussion with 71 comments, reflecting its resonance with software engineers.

hackernews · kalli · Jun 24, 08:54 · [Discussion](https://news.ycombinator.com/item?id=48657049)

**Background**: In software engineering, 'taste' refers to the ability to make good design decisions that balance trade-offs, often developed through experience rather than formal rules. Unit tests verify specific behaviors but cannot assess higher-level qualities like elegance or maintainability. This distinction is central to discussions on the role of automation and AI in coding.

<details><summary>References</summary>
<ul>
<li><a href="https://www.seangoedecke.com/taste/">What is "good taste" in software engineering?</a></li>
<li><a href="https://thejackobrien.com/blog/taste-and-tradeoffs">Taste and Tradeoffs - Jack O'Brien</a></li>
<li><a href="https://davegriffith.substack.com/p/what-do-engineers-mean-when-we-say">What Do Engineers Mean When We Say "Taste"?</a></li>

</ul>
</details>

**Discussion**: Commenters express diverse views: some agree that taste is hard to externalize, while others argue it can be codified. One comment notes the challenge of evaluating messy real-world data compared to unit tests, and another contrasts human and AI legal arguments, illustrating the gap between cleverness and taste.

**Tags**: `#software-engineering`, `#testing`, `#code-quality`, `#ai-software-engineering`

---

<a id="item-12"></a>
## [Apple hikes MacBook and iPad prices amid rising memory costs](https://www.reuters.com/world/asia-pacific/apple-raises-prices-macbooks-ipads-memory-costs-skyrocket-2026-06-25/) ⭐️ 7.0/10

Apple has raised prices across its Mac and iPad lineup by $100 to $1,300 depending on the model, effective June 25, 2026, citing skyrocketing memory costs. This price hike affects consumers and businesses investing in Apple's ecosystem, potentially reducing demand and pressuring Apple's margins in a competitive market. Specific increases include the MacBook Neo from $599 to $699, and the M3 Ultra Mac Studio from $3,999 to $5,299; iPads also saw increases of $100 or more.

hackernews · virgildotcodes · Jun 25, 13:02 · [Discussion](https://news.ycombinator.com/item?id=48672732)

**Background**: Memory costs, particularly for DRAM and NAND flash, have risen due to increased demand from AI data centers and limited supply. Apple uses these components in its devices, and when costs increase, Apple often passes them to consumers.

**Discussion**: Comments on the news show a mix of shock and historical perspective. Some users compare the price hikes to the car market during COVID, noting that early buyers might profit from reselling. Others express frustration over AI companies' impact on memory prices, with one user sarcastically thanking OpenAI. A user also provides inflation-adjusted perspective, noting that computing is still cheaper than in the 1990s.

**Tags**: `#Apple`, `#pricing`, `#MacBook`, `#iPad`, `#memory costs`

---

<a id="item-13"></a>
## [SQLite database of MDN browser compatibility data](https://simonwillison.net/2026/Jun/24/browser-compat-db/#atom-everything) ⭐️ 7.0/10

Simon Willison created a SQLite database from the MDN browser-compat-data repository using sqlite-utils and AI-generated scripts, and made it available via GitHub CDN with open CORS headers. This tool gives developers fast, offline-accessible browser compatibility data without depending on MDN's API or MCP service, enabling efficient queries via SQL or tools like Datasette Lite. The ~66MB SQLite database is built by a GitHub Actions workflow and force-pushed to an orphan branch to leverage GitHub's CDN with open CORS headers, allowing direct browser access via Datasette Lite.

rss · Simon Willison · Jun 24, 23:59

**Background**: MDN's browser-compat-data is a large JSON repository containing browser support information for web features. sqlite-utils is a tool for creating and manipulating SQLite databases. GitHub CDN serves raw files from repositories, but releases lack CORS headers; storing files in a regular repo branch provides open CORS headers.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/mcp">MDN MCP server</a></li>
<li><a href="https://sqlite-utils.datasette.io/">sqlite - utils</a></li>
<li><a href="https://github.com/hola/cdn/blob/master/CORS.md">cdn/CORS.md at master · hola/cdn</a></li>

</ul>
</details>

**Tags**: `#browser-compat`, `#sqlite`, `#mdn`, `#tools`

---

<a id="item-14"></a>
## [LLM-Generated Job Applications Erode Authenticity](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 7.0/10

Tom MacWright observes that many job applications are now entirely LLM-generated, including portfolios and GitHub projects, making candidates indistinguishable and impersonal. This undermines authenticity in hiring, making it harder for employers to assess genuine skills and fit. It could lead to a homogenized workforce and devalue human creativity. MacWright describes a chain: application, portfolio site, GitHub projects, and commit messages all LLM-generated, resulting in candidates who have not 'put themselves out there.'

rss · Simon Willison · Jun 24, 18:13

**Background**: Large language models (LLMs) like GPT-4 can generate human-like text. In hiring, some applicants use LLMs to write resumes, cover letters, and even code projects. However, over-reliance on LLMs can produce generic outputs lacking personal voice and genuine experience.

**Tags**: `#ai`, `#careers`, `#llm`, `#hiring`, `#authenticity`

---

<a id="item-15"></a>
## [Curated list of top open-source OCR models](https://www.reddit.com/r/MachineLearning/comments/1ueiam6/find_the_best_opensource_ocr_models_in_one_place/) ⭐️ 7.0/10

The creator of Papers with Code has launched a dedicated page listing top open-source OCR models, including recent releases from Baidu (Unlimited OCR with 3B parameters and R-SWA) and Mistral (OCR v4 via API). This resource helps practitioners quickly identify state-of-the-art OCR models for document digitization and agentic RAG systems, which are critical for enabling chatbots and internal AI agents to process company data. Baidu's Unlimited OCR uses a novel Reference Sliding Window Attention (R-SWA) mechanism, achieving state-of-the-art results on OmniDocBench with only 500M activated parameters. Mistral OCR v4 is available via API but not open-source.

reddit · r/MachineLearning · /u/NielsRogge · Jun 24, 16:26

**Background**: OCR (Optical Character Recognition) converts scanned documents or PDFs into machine-readable text. Recent advances like R-SWA improve efficiency for long documents by focusing attention on relevant context. Agentic RAG combines retrieval-augmented generation with autonomous decision-making, allowing AI agents to use OCR output for smarter responses.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/BaiduAI_News/status/2069322806748410291">Baidu AI on X: "We’re open-sourcing Unlimited OCR — built to read long documents in one pass. With 3B total parameters and only 500M activated, Unlimited OCR sets new end-to-end SOTA results on OmniDocBench v1.5 and v1.6. The key innovation is Reference Sliding Window Attention (R-SWA), https://t.co/cBRqmyRUKN" / X</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/what-is-agentic-rag/">Agentic RAG - GeeksforGeeks</a></li>

</ul>
</details>

**Tags**: `#OCR`, `#open-source`, `#AI agents`, `#RAG`, `#models`

---

<a id="item-16"></a>
## [MuJoFil: GPU-native simulator for vision RL](https://www.reddit.com/r/MachineLearning/comments/1uemrch/mujoco_derived_simulator_for_high_fidelity_vision/) ⭐️ 7.0/10

A new open-source simulator called MuJoFil has been released, combining NVIDIA's Newton Physics Engine with Google's Filament render engine to enable high-fidelity vision-based reinforcement learning training entirely on GPU. MuJoFil addresses key limitations of existing simulators like MuJoCo's CPU dependency and NVIDIA Isaac's high hardware and licensing requirements, making high-fidelity vision RL more accessible to researchers and developers. The simulator supports PBR textures, parallel rendering of multiple simulations, and can import environments from GLB, OpenUSD, and other formats from online sources like Sketchfab and Poly Haven. It requires CUDA and is installable via pip install mujofil.

reddit · r/MachineLearning · /u/MT1699 · Jun 24, 19:07

**Background**: MuJoCo is a popular physics simulator for robotics but runs on CPU, limiting parallelization. MJX is a GPU-accelerated variant but not optimized for vision-based RL. NVIDIA Isaac offers high fidelity but requires powerful GPUs and a license. MuJoFil uses NVIDIA Newton (an open-source GPU-native physics engine based on MuJoCo's physics) and Google Filament (an open-source PBR render engine) to overcome these issues.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/newton-physics">Newton Physics Engine | NVIDIA Developer</a></li>
<li><a href="https://github.com/google/filament">GitHub - google/filament: Filament is a real-time physically based rendering engine for Android, iOS, Windows, Linux, macOS, and WebGL2 · GitHub</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#simulator`, `#GPU acceleration`, `#MuJoCo`, `#computer vision`

---

<a id="item-17"></a>
## [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](https://www.reddit.com/r/MachineLearning/comments/1uelcm9/high_dimensional_dynamic_rotary_positional/) ⭐️ 7.0/10

The author introduces HDD-RoPE, a high-dimensional dynamic rotary positional embedding that demonstrates faster convergence on the TinyStories dataset compared to the xPos baseline. This work challenges the assumption that positional encoding should be one-dimensional, potentially allowing transformer models to learn richer position representations across multiple levels of structure. HDD-RoPE uses chunks of size 4 (instead of 2 in standard RoPE), corresponding to a 6-dimensional position space, and makes the rotation data-dependent to adapt based on layer activations.

reddit · r/MachineLearning · /u/mikayahlevi · Jun 24, 18:16

**Background**: Rotary Position Embedding (RoPE) encodes position by rotating query and key pairs at predefined rates, allowing relative position learning. xPos is an enhancement that improves extrapolation and reduces oscillation of attention scores. HDD-RoPE extends these ideas by using higher-dimensional rotations and data-dependent dynamics.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.eleuther.ai/rotary-embeddings/">Rotary Embeddings: A Relative Revolution | EleutherAI Blog</a></li>
<li><a href="https://github.com/jploski/RotaryEmbedding">GitHub - jploski/RotaryEmbedding: Comparison of RoPE and xPos positional embeddings used in LLMs</a></li>
<li><a href="https://github.com/lucidrains/rotary-embedding-torch">GitHub - lucidrains/rotary-embedding-torch: Implementation of Rotary Embeddings, from the Roformer paper, in Pytorch · GitHub</a></li>

</ul>
</details>

**Tags**: `#positional embedding`, `#transformer`, `#rotary position encoding`, `#machine learning research`

---

<a id="item-18"></a>
## [Datasette 1.0a35 adds create/alter table interfaces](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 6.0/10

Datasette 1.0a35 introduces a new 'Create table' interface in the database actions menu and a new 'Alter table' table action, both backed by JSON APIs. This release significantly enhances Datasette's database management capabilities, moving from read-only exploration to enabling in-place schema changes through a user-friendly interface and API. The create table API supports defining columns, primary keys, custom types, NOT NULL constraints, literal and expression defaults, and single-column foreign keys. The alter table API allows adding, renaming, reordering, and dropping columns, as well as changing types, defaults, constraints, and table name.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing tabular data, providing a JSON API and a web interface for querying SQLite databases. Previously, creating or altering tables required manual SQL commands or external tools.

**Tags**: `#datasette`, `#release`, `#database`, `#JSON API`, `#open source`

---

<a id="item-19"></a>
## [OPFS + Pyodide Test Harness for Persistent Browser Storage](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison built a test harness to explore using the Origin Private File System (OPFS) for persistent SQLite database storage in browser-based Python applications via Pyodide. This exploration could enable Datasette Lite and similar web apps to persistently store and edit SQLite databases on the user's machine, bringing fuller offline capabilities to browser-based data analysis tools. The test harness is a playground UI built with Claude Code for web, allowing experimentation with OPFS across different browsers. It specifically targets the possibility of Datasette Lite editing persistent SQLite files.

rss · Simon Willison · Jun 23, 18:58

**Background**: The Origin Private File System (OPFS) is a browser storage API that provides a private, sandboxed virtual filesystem for files from the same origin. Pyodide compiles CPython to WebAssembly, enabling Python to run in the browser without a server. Datasette Lite is a WebAssembly-packaged version of the Datasette data exploration tool that runs entirely in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN</a></li>
<li><a href="https://web.dev/articles/origin-private-file-system">The origin private file system | Articles | web.dev</a></li>
<li><a href="https://pyodide.com/">Pyodide – Run Python in Browser with WebAssembly</a></li>

</ul>
</details>

**Tags**: `#opfs`, `#pyodide`, `#datasette-lite`, `#webassembly`, `#browsers`

---