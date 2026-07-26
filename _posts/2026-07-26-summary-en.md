---
layout: default
title: "Horizon Summary: 2026-07-26 (EN)"
date: 2026-07-26
lang: en
---

> From 31 items, 12 important content pieces were selected

---

1. [Anthropic unveils context engineering rules for Claude 5, draws criticism](#item-1) ⭐️ 8.0/10
2. [GM Backs Sodium-Ion Batteries for U.S. Grid Storage](#item-2) ⭐️ 8.0/10
3. [DeepSeek pauses fundraising after compute gap comments leak](#item-3) ⭐️ 8.0/10
4. [LLM with 28.9M parameters runs on $8 ESP32 microcontroller](#item-4) ⭐️ 8.0/10
5. [Debian Debates Three Proposals on LLM Contributions](#item-5) ⭐️ 8.0/10
6. [Open-weight AI's Kubernetes moment](#item-6) ⭐️ 8.0/10
7. [Ruff v0.16.0 increases default rules from 59 to 413](#item-7) ⭐️ 8.0/10
8. [Anthropic Releases Claude Opus 5, a Proactive AI Model at Half the Cost of Fable 5](#item-8) ⭐️ 8.0/10
9. [Compiler Turns Computation Graphs into Transformer Weights Without Training](#item-9) ⭐️ 8.0/10
10. [AutoDev Studio: Open-Source Multi-Agent SDLC Harness Cuts AI Coding Costs](#item-10) ⭐️ 8.0/10
11. [Wind-Powered Ammonia Plant Operates Flexibly in Minnesota](#item-11) ⭐️ 7.0/10
12. [Paper Lengths and Review Bias Against Theoretical ML Research](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic unveils context engineering rules for Claude 5, draws criticism](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 8.0/10

Anthropic announced new rules for context engineering specifically for Claude 5, aiming to optimize how users structure prompts and system instructions for the model. This matters because context engineering is becoming a critical skill for getting reliable outputs from LLMs, and Anthropic's rules could shape best practices—but community members fear increased vendor lock-in and potential issues with Claude's automemory feature. The new rules reportedly emphasize structured templates and Anthropic-specific tooling, moving away from freeform .md files, which some users see as a lock-in strategy. Additionally, Claude 5's automemory has been criticized for making inappropriate contextual leaps that lead to unexpected behavior.

hackernews · mellosouls · Jul 25, 20:42 · [Discussion](https://news.ycombinator.com/item?id=49051361)

**Background**: Context engineering involves iteratively optimizing the instructions and context provided to an LLM to achieve desired results, going beyond simple prompt engineering. Anthropic's Claude models have a unique 'automemory' feature that allows the model to recall and use stored information across sessions, but this can sometimes lead to unpredictable outputs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.promptingguide.ai/guides/context-engineering-guide">Context Engineering Guide | Prompt Engineering Guide</a></li>
<li><a href="https://spring.io/blog/2026/04/07/spring-ai-agentic-patterns-6-memory-tools/">Spring AI Agentic Patterns (Part 6): AutoMemoryTools — Persistent Agent Memory Across Sessions</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some users advocate for explicit instruction languages rather than Anthropic's approach, while others report that Claude 5 makes more errors and ignores deliberate controls compared to previous versions. There is a strong desire for more control rather than less, with some users preferring GPT's stricter adherence to instructions.

**Tags**: `#Claude`, `#AI`, `#context engineering`, `#LLM`, `#Anthropic`

---

<a id="item-2"></a>
## [GM Backs Sodium-Ion Batteries for U.S. Grid Storage](https://spectrum.ieee.org/sodium-ion-battery-peak-energy) ⭐️ 8.0/10

General Motors has announced support for sodium-ion battery technology for large-scale grid storage in the United States, marking a strategic shift toward cheaper and more sustainable energy storage solutions. This move could reduce dependence on lithium, which is expensive and geographically concentrated, and accelerate the adoption of grid-scale storage critical for integrating renewable energy sources like solar and wind. Sodium-ion batteries offer a round-trip efficiency of 96% according to discussions, and they do not require cobalt, copper, or nickel, making them potentially cheaper and more environmentally friendly than lithium-ion batteries.

hackernews · rbanffy · Jul 25, 21:48 · [Discussion](https://news.ycombinator.com/item?id=49051947)

**Background**: Sodium-ion batteries use abundant sodium instead of lithium as charge carriers, with similar working principles to lithium-ion batteries. They gained interest in the 2010s due to lithium's high cost and environmental concerns, but are still behind lithium-ion in energy density and commercialization pace.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sodium-ion_batteries">Sodium-ion batteries</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about US manufacturing, with one user suggesting the batteries would just be Chinese hardware relabeled. Others discussed potential cost savings for HVAC in grid storage and interest in home sodium-ion batteries, while one noted that a promising US sodium-ion startup was sold for scrap due to lack of funding.

**Tags**: `#sodium-ion`, `#grid storage`, `#batteries`, `#GM`, `#energy`

---

<a id="item-3"></a>
## [DeepSeek pauses fundraising after compute gap comments leak](https://github.com/demo-zexuan/liang-wenfeng-investor-meeting-2026-7-22/blob/master/%E6%A2%81%E6%96%87%E9%94%8B%E6%8A%95%E8%B5%84%E8%80%85%E4%BA%A4%E6%B5%81%E4%BC%9A-%E6%96%87%E5%AD%97%E7%A8%BF_1_18_translate_20260723201651.pdf) ⭐️ 8.0/10

DeepSeek has paused its second fundraising round after leaked remarks from founder Liang Wenfeng about the US-China AI compute gap circulated online, according to Bloomberg. This pause signals uncertainty in the Chinese AI investment landscape and highlights the impact of geopolitical tensions on AI development funding, potentially affecting DeepSeek's ability to compete with well-funded US labs. The fundraising suspension was reported by Bloomberg, citing people familiar with the matter, and comes after speculation about Tencent's involvement; DeepSeek's open-weight models like DeepSeek-R1 are trained at a fraction of the cost of US counterparts.

hackernews · oliculipolicula · Jul 25, 23:32 · [Discussion](https://news.ycombinator.com/item?id=49052912)

**Background**: DeepSeek is a Chinese AI company founded in 2023 by Liang Wenfeng, previously funded by hedge fund High-Flyer. It gained attention in January 2025 with DeepSeek-R1, a model comparable to OpenAI's GPT-4 but trained at much lower cost. The US maintains a compute advantage due to export controls on advanced chips, but Chinese models are closing the performance gap.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://www.rand.org/pubs/commentary/2025/05/chinas-ai-models-are-closing-the-gap-but-americas-real.html">China's AI Models Are Closing the Gap—but America's Real Advantage Lies Elsewhere | RAND</a></li>
<li><a href="https://www.csis.org/analysis/securing-agi-laurel-export-controls-compute-gap-and-chinas-counterstrategy">Securing the AGI Laurel: Export Controls, the Compute Gap, and China’s Counterstrategy | CSIS</a></li>

</ul>
</details>

**Discussion**: Commenters debated the meaning of the pause: some clarified it's not due to leaked comments causing the pause, but rather the leak revealing the pause rationale. Others questioned the strategy of pursuing frontier models if Chinese models are more cost-efficient, and noted the difference in tone from US lab leaders.

**Tags**: `#deepseek`, `#ai-fundraising`, `#us-china-ai`, `#compute-gap`, `#ai-competition`

---

<a id="item-4"></a>
## [LLM with 28.9M parameters runs on $8 ESP32 microcontroller](https://github.com/slvDev/esp32-ai) ⭐️ 8.0/10

A developer successfully ran a 28.9 million parameter language model on an ESP32-S3 microcontroller costing around $8, demonstrating edge AI inference on ultra-low-cost hardware. This breakthrough significantly lowers the hardware barrier for deploying LLMs, enabling on-device AI in IoT and consumer devices without cloud connectivity. It could lead to new applications like offline voice assistants and smart sensors. The ESP32-S3 features 512KB of SRAM and up to 16MB of flash, with a RISC-V or Xtensa processor. The model uses per-layer embedding tricks to reduce memory usage, and the inference runs entirely on the microcontroller.

hackernews · boveyking · Jul 25, 18:59 · [Discussion](https://news.ycombinator.com/item?id=49050512)

**Background**: Edge AI inference involves running machine learning models directly on local devices instead of the cloud, enabling low latency and privacy. The ESP32 is a family of low-cost, low-power microcontrollers with integrated Wi-Fi and Bluetooth, widely used in IoT projects. Typically, microcontrollers have limited memory and compute, making LLM inference challenging.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ESP32">ESP32</a></li>
<li><a href="https://en.wikipedia.org/wiki/Edge_inference">Edge inference</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted the per-layer embedding trick and noted that viable TTS models of similar size exist, suggesting near-real-time speech synthesis on ESP32. Some questioned scalability to larger models on flash-backed CPUs, while others praised the ESP32-S3's capabilities compared to more expensive alternatives.

**Tags**: `#LLM`, `#edge AI`, `#microcontroller`, `#ESP32`, `#machine learning`

---

<a id="item-5"></a>
## [Debian Debates Three Proposals on LLM Contributions](https://www.debian.org/vote/2026/vote_002) ⭐️ 8.0/10

Debian has presented three proposals for a vote to regulate contributions created using large language models (LLMs) or generative AI, ranging from an outright ban to conditional acceptance. This debate sets a precedent for open-source governance on AI-generated code and content, as Debian is a major Linux distribution. The outcome could influence other community-driven projects. Proposal A bans all LLM-assisted contributions outright, while Proposal B allows them under strict conditions such as human review and licensing compliance. Proposal C takes a neutral stance, leaving decisions to individual maintainers.

hackernews · zdw · Jul 25, 19:44 · [Discussion](https://news.ycombinator.com/item?id=49050859)

**Background**: Debian is a volunteer-run Linux distribution known for its strict free software guidelines. The Debian Project holds general resolutions to decide major policy issues, and this vote is part of that process. LLMs like ChatGPT can generate code and documentation, raising questions about authorship, quality, and licensing.

**Discussion**: Commenters debate the nuances, with some arguing that LLMs are more than mere statistical models and others referencing Gentoo's ban as a precedent. There is also concern about whether existing Debian documentation already violates the stricter proposals.

**Tags**: `#debian`, `#open-source`, `#policy`, `#LLM`, `#AI`

---

<a id="item-6"></a>
## [Open-weight AI's Kubernetes moment](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

An article argues that open-weight AI models are poised to become the industry standard, similar to how Kubernetes became the dominant container orchestration platform, thereby democratizing AI infrastructure. This shift could lower barriers to AI development and deployment, enabling startups and smaller organizations to compete with tech giants and fostering innovation through community collaboration. The analogy suggests that just as Kubernetes became ubiquitous despite competing systems, open-weight models (with publicly released weights) may dominate over proprietary black-box AI, though they lack full open-source transparency.

hackernews · tknaup · Jul 25, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49048034)

**Background**: Open-weight AI refers to models whose internal parameters (weights) are publicly released, but without necessarily full open-source commitments such as training data or code. Kubernetes, originally developed by Google, is an open-source system for automating deployment, scaling, and management of containerized applications, and it has become the de facto standard in cloud-native computing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told – Open Source Initiative</a></li>

</ul>
</details>

**Discussion**: Commenters debate the technical feasibility of banning models by origin (e.g., Chinese models), noting weights are just numbers and hard to trace. Others discuss the bizarre pricing dynamics ('tokenomics') of proprietary APIs and suggest open-weight models provide a cost baseline. One commenter envisions companies collaborating on a shared open-weight model, similar to the Linux model.

**Tags**: `#AI`, `#open-weight`, `#Kubernetes`, `#industry trends`, `#open source`

---

<a id="item-7"></a>
## [Ruff v0.16.0 increases default rules from 59 to 413](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0 was released on July 23, 2026, increasing the default set of enabled linting rules from 59 to 413, potentially breaking existing CI pipelines. The tool now finds many more issues automatically, including syntax errors and immediate runtime errors. This change significantly raises the default strictness of Ruff, forcing Python developers to address many previously ignored issues. It may break CI pipelines across the ecosystem, but also improves code quality and catches severe errors earlier. Ruff's rule count grew from 708 to 968 since v0.1.0, yet many rules were not enabled by default. The v0.16.0 release includes an automatic fix mode that fixed 1,538 out of 1,618 errors in the sqlite-utils project when run with --fix --unsafe-fixes.

rss · Simon Willison · Jul 25, 22:44

**Background**: Ruff is an extremely fast Python linter developed by Astral, written in Rust, and designed to replace multiple tools like Flake8, isort, and Black. Astral was recently acquired by OpenAI, and Ruff is now widely used in the Python ecosystem for its speed and comprehensive rule set.

<details><summary>References</summary>
<ul>
<li><a href="https://astral.sh/ruff">Ruff , an extremely fast Python linter | Astral</a></li>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ ruff : An extremely fast Python linter and code...</a></li>
<li><a href="https://astral.sh/about">About | Astral</a></li>

</ul>
</details>

**Tags**: `#Ruff`, `#Python`, `#linting`, `#tooling`, `#Astral`

---

<a id="item-8"></a>
## [Anthropic Releases Claude Opus 5, a Proactive AI Model at Half the Cost of Fable 5](https://simonwillison.net/2026/Jul/24/introducing-claude-opus-5/#atom-everything) ⭐️ 8.0/10

Anthropic has released Claude Opus 5, a proactive model that approaches frontier-level intelligence while being priced at half the cost of Claude Fable 5. It is currently leading the Artificial Analysis leaderboard, surpassing even Fable 5. This release offers near-frontier intelligence at a significantly lower price point, making advanced AI capabilities more accessible. Its proactive nature and improved resistance to prompt injection could set new standards for AI safety and autonomy. Claude Opus 5 is priced the same as Opus 4.8 and offers a fast mode at double the base cost. It demonstrated proactive behavior by writing its own computer vision pipeline to reconstruct a 3D model from a drawing it could not directly view.

rss · Simon Willison · Jul 24, 23:48

**Background**: Frontier intelligence refers to AI models that perform at the cutting edge of capabilities, often matching or exceeding human performance on complex tasks. Proactive AI models can anticipate user needs and take actions without explicit prompts, unlike traditional reactive models that require specific instructions. Anthropic's Claude Opus 5 is designed to be such a proactive model, while also prioritizing safety by intentionally not training it on exploitation tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.alpha-sense.com/resources/research-articles/proactive-ai/">Proactive AI in 2026: Moving Beyond the Prompt</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-proactive-ai-agents-shifting-reactive-anticipatory">What Is Proactive AI? How Agents Are Shifting from Reactive to Anticipatory | MindStudio</a></li>
<li><a href="https://artificialanalysis.ai/leaderboards/models">LLM Leaderboard - Comparison of AI models from OpenAI, Anthropic...</a></li>

</ul>
</details>

**Discussion**: Boris Cherny highlighted that Opus 5 is Anthropic's least prompt-injectable model yet, based on evaluations and red teaming. This suggests significant improvements in safety against adversarial attacks, which is a crucial aspect for deploying AI in sensitive contexts.

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#Model Release`, `#LLM`

---

<a id="item-9"></a>
## [Compiler Turns Computation Graphs into Transformer Weights Without Training](https://www.reddit.com/r/MachineLearning/comments/1v5fxbe/i_built_a_compiler_that_turns_computation_graphs/) ⭐️ 8.0/10

The user physicsrob developed Torchwright, a compiler that takes Python computation graphs and produces the weights of a standard Phi-3 transformer, requiring no training. The resulting checkpoint loads in vanilla Hugging Face without custom code. This work demonstrates that transformers can be programmed algorithmically, separating expressible algorithms from learned ones, and enables hand-crafted weights for stock architectures, potentially advancing mechanistic interpretability and model design. It also allows researchers to explore what transformers can represent without the cost of training. Torchwright targets the Phi-3 architecture, a 3.8-billion-parameter small language model by Microsoft, and produces weights compatible with standard Hugging Face loading. The compiler builds on the RASP programming language and the Tracr compiler but improves by using ordinary Python and supporting stock architectures without custom code.

reddit · r/MachineLearning · /u/notforrob · Jul 24, 16:15

**Background**: RASP (Restricted Access Sequence Processing Language) is a programming language designed to simulate transformer computations at a discrete level, and Tracr is a compiler that translates RASP programs into actual transformer weights. However, RASP is not Python and Tracr targets custom architectures. Torchwright addresses these limitations by allowing computation graphs to be defined in standard Python and compiled directly to a stock architecture like Phi-3, enabling the weights to be loaded with vanilla Hugging Face without any custom code or 'trust_remote_code'.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2106.06981">[2106.06981] Thinking Like Transformers</a></li>
<li><a href="https://arxiv.org/pdf/2301.05062v1">Tracr : Compiled Transformers as a</a></li>
<li><a href="https://www.infoworld.com/article/2337210/microsoft-unveils-phi-3-family-of-small-language-models.html">Microsoft unveils Phi - 3 family of small language models | InfoWorld</a></li>

</ul>
</details>

**Tags**: `#transformer`, `#compiler`, `#machine learning`, `#weights`, `#no-training`

---

<a id="item-10"></a>
## [AutoDev Studio: Open-Source Multi-Agent SDLC Harness Cuts AI Coding Costs](https://www.reddit.com/r/MachineLearning/comments/1v59pal/i_built_an_opensource_multiagent_sdlc_harness/) ⭐️ 8.0/10

The developer released AutoDev Studio, an open-source multi-agent software development lifecycle (SDLC) harness that builds a persistent repository knowledge base using static analysis and embedding indexes, reducing task costs by 7–75% compared to a cold Claude Code run on large repositories up to 82k lines of code. This approach addresses a key inefficiency in current AI coding agents: repeatedly re-exploring the codebase for every task. By reusing a persistent knowledge base, it significantly reduces token usage and cost, making AI-assisted software development more accessible for large, complex projects. AutoDev Studio uses a multi-agent workflow with separate PM, Dev, QA, and Reviewer agents, and supports multiple model providers including Anthropic, OpenAI, Groq, and Ollama. It can run completely free using Groq's free tier and local embeddings, and it includes a Kanban board and cost tracking.

reddit · r/MachineLearning · /u/NeighborhoodOwn8510 · Jul 24, 12:15

**Background**: Multi-agent SDLC harnesses orchestrate specialized AI agents to handle different phases of software development, from requirements to code review. Persistent repository knowledge techniques aim to avoid redundant exploration by creating a reusable representation of the codebase. Tools like Agent Memory and Agentskill are earlier attempts in this direction.

<details><summary>References</summary>
<ul>
<li><a href="https://www.threadai.com/blog/an-inside-look-how-we-built-our-agentic-sdlc-harness">An Inside Look: How We Built Our Agentic SDLC Harness | Thread AI</a></li>
<li><a href="https://seylox.github.io/2026/03/05/blog-agents-meta-repo-pattern.html">In Which We Give Our AI Agent a Map (And It Stops Getting Lost) - Working around the limitations of my intelligence</a></li>
<li><a href="https://dev.to/airscript/turning-repository-knowledge-into-usable-agent-context-4pe4">Turning Repository Knowledge Into Usable Agent Context - DEV Community</a></li>

</ul>
</details>

**Tags**: `#AI coding`, `#multi-agent`, `#open-source`, `#software engineering`, `#benchmarks`

---

<a id="item-11"></a>
## [Wind-Powered Ammonia Plant Operates Flexibly in Minnesota](https://ammoniaenergy.org/articles/flexible-renewable-ammonia-demonstrator-now-operational-in-minnesota/) ⭐️ 7.0/10

A small-scale ammonia plant in Morris, Minnesota, powered entirely by wind energy, is now operational and demonstrates flexible intermittent production of green ammonia and fertilizer. This project demonstrates that renewable ammonia production is feasible at small scale with intermittent renewable power, offering a pathway to decarbonize fertilizer manufacturing and reduce agricultural carbon footprint. The plant is built for intermittent operation, shutting down when wind is unavailable. It uses water electrolysis to produce hydrogen and a small-scale Haber-Bosch process for ammonia synthesis, with ammonia stored in tanks.

hackernews · gritzko · Jul 25, 19:30 · [Discussion](https://news.ycombinator.com/item?id=49050735)

**Background**: Traditional ammonia production via the Haber-Bosch process relies on natural gas or coal for hydrogen, emitting large amounts of CO2. Green ammonia replaces fossil-derived hydrogen with hydrogen from renewable-powered electrolysis. A key challenge is that renewable sources like wind are intermittent, while conventional Haber-Bosch plants operate continuously. This demonstrator addresses that by enabling flexible, on/off operation to match wind availability, making green ammonia viable for distributed, farm-level production.

<details><summary>References</summary>
<ul>
<li><a href="https://gpaeurope.com/library/secure/optimizing-green-ammonia-operation-intermittent-mode">Optimizing Green Ammonia Operation in Intermittent Mode</a></li>
<li><a href="https://www.mdpi.com/2076-3298/11/4/71">Flexible Green Ammonia Production Plants: Small-Scale Simulations Based on Energy Aspects</a></li>
<li><a href="https://www.thyssenkrupp-uhde.com/en/products-and-technologies/fertilizer-technologies/ammonia-plants/green-ammonia">Green Ammonia</a></li>

</ul>
</details>

**Discussion**: Commenters generally view the project positively as a technical demonstration but question its cost-effectiveness at small scale. Some point out that much larger green ammonia projects exist globally, while others appreciate the value of fertilizer independence. The intermittent operation design is seen as a key innovation, but the lack of cost data leaves economic viability uncertain.

**Tags**: `#renewable energy`, `#ammonia production`, `#green hydrogen`, `#fertilizer`, `#industrial decarbonization`

---

<a id="item-12"></a>
## [Paper Lengths and Review Bias Against Theoretical ML Research](https://www.reddit.com/r/MachineLearning/comments/1v6gh43/paper_lengths_and_reasonable_assumptions_in_ml/) ⭐️ 6.0/10

A researcher shares personal observations that fixed paper lengths and unlimited appendices in top ML conferences may unfairly penalize theoretical papers, as reviewers increasingly cite mathematical difficulty or insufficient explanation as reasons for rejection. This discussion highlights a potential systemic bias in ML conference reviewing that could discourage theoretical contributions, which are essential for scientific rigor and long-term progress, and may push the field toward more empirical work. The author notes that many conferences have a rule that papers must be self-contained and reviewers are not expected to read appendices, yet theoretical papers often require prerequisite knowledge that cannot be fully explained within the main page limit.

reddit · r/MachineLearning · /u/OutsideSimple4854 · Jul 25, 18:48

**Background**: Machine learning conferences like NeurIPS and ICML typically impose strict page limits (e.g., 8 pages) for main papers and allow unlimited appendices, but reviewers are instructed to base decisions primarily on the main paper. Theoretical papers often rely on advanced mathematics, making it difficult to be both concise and self-contained. This tension between page limits and the need for rigorous explanation can lead to rejections based on perceived difficulty rather than scientific merit.

**Tags**: `#machine learning`, `#conferences`, `#theoretical ML`, `#research`, `#paper review`

---