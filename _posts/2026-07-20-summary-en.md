---
layout: default
title: "Horizon Summary: 2026-07-20 (EN)"
date: 2026-07-20
lang: en
---

> From 27 items, 16 important content pieces were selected

---

1. [SRE replaces $120k bowling scoring system with cheap ESP32s](#item-1) ⭐️ 9.0/10
2. [Alibaba Announces Qwen 3.8: 2.4T Parameter Open-Weights LLM](#item-2) ⭐️ 9.0/10
3. [Claude Code Now Uses Bun Written in Rust](#item-3) ⭐️ 8.0/10
4. [Lessons from Selling 2,500 MIDI Recorders: Hardware Isn't That Hard](#item-4) ⭐️ 8.0/10
5. [Sam Altman Leaked Email: OpenAI Planned Local GPT-3 Model](#item-5) ⭐️ 8.0/10
6. [AI Mania Eviscerates Global Decision-Making](#item-6) ⭐️ 8.0/10
7. [Anthropic makes Claude Fable 5 permanent on subscriptions](#item-7) ⭐️ 8.0/10
8. [Interactive hyperbolic tree visualization of GPT-2 token embeddings](#item-8) ⭐️ 8.0/10
9. [Interactive t-SNE Map of GPT-2 Token Embeddings](#item-9) ⭐️ 8.0/10
10. [Minecraft Java Edition Migrates to SDL3 for Better Cross-Platform Support](#item-10) ⭐️ 7.0/10
11. [SQLite Query Explainer: Interactive Browser Tool with Pyodide](#item-11) ⭐️ 7.0/10
12. [Kaggle DeepMind Prize Allegedly Awarded to 'AI Slop'](#item-12) ⭐️ 7.0/10
13. [GPT-2 Small Embedding Geometry: Discretized vs Continuous Neighbors](#item-13) ⭐️ 7.0/10
14. [Deep Learning Survey for scRNA-seq Analysis](#item-14) ⭐️ 7.0/10
15. [TabFM Studio: No-Code Spreadsheet Predictions with Google's Tabular Foundation Model](#item-15) ⭐️ 7.0/10
16. [Bananas sprout in UK garden after 15 years](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [SRE replaces $120k bowling scoring system with cheap ESP32s](https://news.ycombinator.com/item?id=48968606) ⭐️ 9.0/10

An SRE built a prototype bowling scoring system using ESP32 microcontrollers and a Raspberry Pi for about $200 per lane pair, replacing a proprietary system that cost $120,000. The system uses ESP-NOW mesh networking and Redis for event streaming. This demonstrates how modern low-cost embedded systems can replace expensive proprietary hardware in niche industries, potentially lowering barriers for small businesses and highlighting the power of open-source hardware and software for retrofitting legacy equipment. The system uses ESP32 nodes arranged in an ESP-NOW star-topology mesh with an RS485 wired fallback, reporting to a Raspberry Pi running Redis and a state machine. The author plans to open-source the project as OpenLaneLink once ready.

hackernews · section33 · Jul 19, 14:41

**Background**: ESP32 is a low-cost, low-power microcontroller with built-in Wi-Fi and Bluetooth, widely used in IoT projects. Traditional bowling scoring systems rely on expensive proprietary hardware with cameras and sensors; this project shows how commodity components can replicate complex functionality at a fraction of the cost.

<details><summary>References</summary>
<ul>
<li><a href="https://www.digikey.com/es/maker/blogs/2024/a-guide-for-the-esp32-microcontroller-series">A Guide for the ESP 32 Microcontroller Series</a></li>
<li><a href="https://mitsi.com/case-studies/bowling-pin-fall-tracker/">Pinspotters: The Bowling Tracker - Micro Technology Services, Inc.</a></li>

</ul>
</details>

**Discussion**: Community comments express strong interest and validation, with one commenter sharing a similar experience with mechanical bowling machines and another noting the potential for retrofitting old machine tools. There is excitement about adding features like LED chases and kiosk payments.

**Tags**: `#ESP32`, `#Bowling`, `#Retrofitting`, `#Embedded Systems`, `#Cost Reduction`

---

<a id="item-2"></a>
## [Alibaba Announces Qwen 3.8: 2.4T Parameter Open-Weights LLM](https://twitter.com/Alibaba_Qwen/status/2078759124914098291) ⭐️ 9.0/10

Alibaba announced Qwen 3.8, a 2.4 trillion parameter open-weights large language model, in direct response to Moonshot AI's recent Kimi K3 (2.8T parameters). The model is expected to be released on Hugging Face soon. This intensifies the competition in open-weights LLMs, providing developers with more powerful and accessible models. It also signals Alibaba's strong commitment to open-source AI, potentially accelerating innovation and lowering costs in the field. The model has 2.4 trillion parameters, making it one of the largest open-weights LLMs announced. Although smaller than Kimi K3's 2.8 trillion, it is expected to be competitive, with community members hoping for smaller variant releases suitable for local deployment.

hackernews · nh43215rgb · Jul 19, 08:44 · [Discussion](https://news.ycombinator.com/item?id=48966120)

**Background**: Large language models contain billions or trillions of parameters that determine their capacity to process and generate language. Open-weights models allow anyone to download and run them locally or fine-tune them, fostering innovation. Alibaba's Qwen series has been progressively increasing in size, from the first trillion-parameter Qwen3-Max-Preview in September 2025 to the current 2.4T models.

<details><summary>References</summary>
<ul>
<li><a href="https://officechai.com/ai/alibaba-qwen-3-8/">Alibaba Announces 2.4 Trillion-Parameter Open-Weight Qwen 3.8 ...</a></li>
<li><a href="https://openlm.ai/kimi-k3/">Kimi K3 | OpenLM.ai</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed but generally positive. Some celebrate the increasing competition and open availability, while others express frustration with previous Qwen models' performance (e.g., Qwen 3.7 Pro deemed unusable for software engineering). Many users hope for smaller model sizes to run locally on consumer hardware.

**Tags**: `#AI`, `#LLM`, `#open-source`, `#Alibaba`, `#Qwen`

---

<a id="item-3"></a>
## [Claude Code Now Uses Bun Written in Rust](https://simonwillison.net/2026/Jul/19/claude-code-in-bun-in-rust/#atom-everything) ⭐️ 8.0/10

Anthropic's Claude Code v2.1.181 and later versions use the Rust port of the Bun JavaScript runtime, achieving a 10% faster startup on Linux. This was verified by Simon Willison through binary inspection and confirmed by Bun's creator Jarred Sumner. This migration from Zig to Rust for a widely-used AI coding tool demonstrates the growing maturity and reliability of the Bun runtime. It also highlights the trend of leveraging Rust for performance and safety in production systems. The embedded Bun version in Claude Code appears as v1.4.0, which is a canary release not yet officially tagged on GitHub. Binary analysis reveals hundreds of .rs source files, confirming the Rust-based build.

rss · Simon Willison · Jul 19, 03:54 · [Discussion](https://news.ycombinator.com/item?id=48966569)

**Background**: Bun is a fast all-in-one JavaScript runtime initially written in Zig. In May 2025, Bun was acquired by Anthropic, and its creator Jarred Sumner announced a complete rewrite of Bun from Zig to Rust, aided by AI. Claude Code is Anthropic's agentic AI coding tool that helps developers understand codebases, edit files, and run commands.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.com/blog/bun-in-rust">Rewriting Bun in Rust | Bun Blog</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some appreciate the technical rationale for the rewrite, citing Rust's automatic memory management benefits. Others criticize the communication around the change and question why a terminal UI requires a JavaScript runtime, suggesting a native rewrite would be simpler. Concerns about Bun's governance and transparency were also raised.

**Tags**: `#Bun`, `#Rust`, `#Claude Code`, `#runtime`, `#rewrite`

---

<a id="item-4"></a>
## [Lessons from Selling 2,500 MIDI Recorders: Hardware Isn't That Hard](https://chipweinberger.com/articles/20260719-hardware-is-not-so-hard) ⭐️ 8.0/10

Chip Weinberger, creator of the JamCorder, shares insights from selling 2,500 MIDI recorders, arguing that hardware development difficulty is often overstated and depends on product complexity. This firsthand account provides valuable, practical lessons for aspiring hardware entrepreneurs, challenging the common perception that hardware is inherently difficult and highlighting that simple designs can succeed. The JamCorder is a simple device with only 25 components and an injection-molded clamshell case; it records MIDI directly to an SD card without requiring a companion app for data retrieval.

hackernews · chipweinberger · Jul 19, 10:34 · [Discussion](https://news.ycombinator.com/item?id=48966713)

**Background**: MIDI (Musical Instrument Digital Interface) is a technical standard that allows musical instruments and computers to communicate performance data like note pitches and velocities. The JamCorder is a portable MIDI recorder that captures live performances for later use.

**Discussion**: Commenters generally praised the product and insights, with one customer calling it 'a perfect product.' However, some argued that hardware difficulty scales with product complexity, and that simple products like the JamCorder are not representative of typical hardware challenges.

**Tags**: `#hardware`, `#entrepreneurship`, `#product development`, `#lessons learned`, `#MIDI`

---

<a id="item-5"></a>
## [Sam Altman Leaked Email: OpenAI Planned Local GPT-3 Model](https://simonwillison.net/2026/Jul/20/sam-altman/#atom-everything) ⭐️ 8.0/10

A leaked email from Sam Altman to OpenAI's board, dated October 1, 2022 and revealed in the Musk v. Altman lawsuit, outlines a plan to release a GPT-3-level language model that can run locally on consumer hardware to preempt competitors like Stability AI and hinder funding for rival efforts. This reveals strategic thinking behind OpenAI's open-source initiatives, showing a competitive rather than purely altruistic motive. It could shift public perception of OpenAI's open-source releases and influence how the AI community views corporate transparency. The proposed model would have 'approximate capability of GPT-3' and run locally on consumer hardware. The email explicitly states the goal is to 'discourage others from releasing similarly-powerful models' and 'make it harder for new efforts to get funded.'

rss · Simon Willison · Jul 20, 03:47

**Background**: GPT-3 is a large language model with 175 billion parameters, typically requiring cloud computing resources. Running a model locally on consumer hardware necessitates quantization and optimization. At the time, Stability AI, known for Stable Diffusion, was gaining attention. This email provides insight into OpenAI's internal competitive strategy regarding open-sourcing.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@paulhoke/the-complete-guide-to-running-large-language-models-locally-in-2026-hardware-tools-and-da9efb3170be">The Complete Guide to Running Large Language Models Locally ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stability_AI">Stability AI - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#openai`, `#sam-altman`, `#ai-ethics`, `#open-source`, `#competitive-strategy`

---

<a id="item-6"></a>
## [AI Mania Eviscerates Global Decision-Making](https://simonwillison.net/2026/Jul/19/ai-mania/#atom-everything) ⭐️ 8.0/10

Nik Suresh published an exposé detailing how irrational AI hype is leading to disastrous decision-making in large organizations, including cases where executives who never used AI produce AI-centric strategies and engineers fearfully rewrite codebases in trendy languages to justify their jobs. This critique highlights the real-world consequences of AI mania, such as wasted resources, eroded trust, and misalignment between technology adoption and actual business value, affecting engineers, executives, and customers across industries. The article includes an anecdote about a company with a token leaderboard (tracking AI token consumption) where an engineer considered rewriting a Go repository in Zig solely to appear productive, and another about executives at vendor companies afraid to contradict customer executives' unrealistic AI claims for fear of losing contracts.

rss · Simon Willison · Jul 19, 05:06

**Background**: A token leaderboard is a ranking system that tracks how many AI tokens (units of text processed) an individual or company consumes, often used internally to gamify AI usage. Zig is a relatively new systems programming language gaining attention for its performance and simplicity, but rewriting a mature Go codebase in Zig solely to appear productive is an extreme example of hype-driven engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://tokenleaderboard.org/">Token Leaderboard | AI Token Usage Rankings for Companies and Individuals</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Tags**: `#AI hype`, `#corporate decision-making`, `#software engineering`, `#critical analysis`

---

<a id="item-7"></a>
## [Anthropic makes Claude Fable 5 permanent on subscriptions](https://simonwillison.net/2026/Jul/18/claude-make-fable-5-permanent/#atom-everything) ⭐️ 8.0/10

Anthropic reversed its plan to remove Claude Fable 5 from subscription plans, announcing that starting July 20, Fable 5 will be included in Max and Team Premium plans at 50% of limits, and Pro and Team Standard users will receive a $100 credit for access via usage credits. This move ensures subscribers retain access to Anthropic's strongest model, preventing churn to competitors like OpenAI's GPT-5.6 Sol and Moonshot AI's Kimi 3, which had made the original removal plan untenable. The $20/month plan still does not include Fable 5; only Max ($100/$200 per month) and Team Premium subscriptions get the model. Anthropic's original removal plan was driven by compute capacity concerns, and they may now need to reduce training to free up GPUs for serving.

rss · Simon Willison · Jul 18, 06:00

**Background**: Claude Fable 5 is Anthropic's most advanced model, designed with strict safety guardrails for frontier research. Its removal was originally announced due to high compute costs. However, the launch of GPT-5.6 Sol and Kimi K3 created competitive pressure, as these models offered comparable or superior performance at lower cost.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 - Anthropic</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://www.kimi.com/en">Kimi AI with K3 | Built for Agentic Coding & Knowledge Work</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Claude`, `#Anthropic`, `#pricing`, `#competition`

---

<a id="item-8"></a>
## [Interactive hyperbolic tree visualization of GPT-2 token embeddings](https://www.reddit.com/r/MachineLearning/comments/1v0pv45/follow_up_gpt2s_vocabulary_as_a_hyperbolic_tree/) ⭐️ 8.0/10

A Reddit user created an interactive hyperbolic embedding of GPT-2's 32,070 token vocabulary in a Poincaré ball, explorable via Möbius translation. The visualization runs on mobile devices and allows users to rotate, zoom, and tap tokens to shift the space. This provides a novel way to understand the semantic structure of GPT-2's token embeddings, revealing a tree-like organization that is difficult to capture in flat space. It demonstrates the value of hyperbolic geometry for representing hierarchical data in machine learning. The layout uses raw GPT-2-small token embeddings without optimization or training, and the hyperbolic space naturally accommodates tree structures. The vocabulary forms a forest with one giant tree of about 2,300 tokens, hundreds of smaller families, and thousands of isolated tokens.

reddit · r/MachineLearning · /u/Limp-Contest-7309 · Jul 19, 12:54

**Background**: Hyperbolic geometry is a non-Euclidean geometry where space expands exponentially from the center, making it ideal for embedding tree structures. The Poincaré ball model represents hyperbolic space inside a unit ball, and Möbius translations are isometries that allow natural navigation. GPT-2 is a language model that uses a vocabulary of tokens; visualizing their embeddings helps understand semantic relationships.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Poincaré_ball_model">Poincaré ball model</a></li>
<li><a href="https://en.wikipedia.org/wiki/Möbius_transformation">Möbius transformation</a></li>

</ul>
</details>

**Discussion**: The community comments are not provided, but the project title references a previous reddit user's disappointment with a 2D projection, indicating the author addressed feedback. The technical execution and novel visualization likely received positive feedback.

**Tags**: `#GPT-2`, `#hyperbolic space`, `#token embeddings`, `#visualization`, `#NLP`

---

<a id="item-9"></a>
## [Interactive t-SNE Map of GPT-2 Token Embeddings](https://www.reddit.com/r/MachineLearning/comments/1v09muj/interactive_map_of_gpt2s_token_embedding_space/) ⭐️ 8.0/10

A developer released an interactive t-SNE map of GPT-2-small's token embedding space, allowing users to tap any token to see its nearest neighbors and walk the graph via a minimum spanning tree. This tool makes high-dimensional token embeddings intelligible and explorable for researchers, educators, and practitioners, offering an intuitive way to understand how GPT-2 organizes linguistic tokens without running the model. The map covers 32,070 alphabetic tokens from GPT-2-small's WTE layer, uses t-SNE on a compressed representation, and overlays a minimum spanning tree to show real nearest-kin relationships. It works on mobile with pinch-to-zoom and includes a search box.

reddit · r/MachineLearning · /u/Limp-Contest-7309 · Jul 18, 22:42

**Background**: Token embeddings convert discrete tokens (words, subwords) into dense numeric vectors that capture semantic meaning. t-SNE is a dimensionality reduction technique that projects high-dimensional data into 2D or 3D for visualization, preserving local structure. A minimum spanning tree (MST) connects all points with minimal total edge weight, here used to highlight nearest-neighbor links.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/T-distributed_stochastic_neighbor_embedding">t -distributed stochastic neighbor embedding - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Minimum_spanning_tree">Minimum spanning tree</a></li>
<li><a href="https://learncodecamp.net/token-embeddings/">Token Embeddings — what they are, why they matter, and how to ...</a></li>

</ul>
</details>

**Discussion**: The Reddit community praised the visualization's quality and mobile compatibility, with users noting it helps intuitively understand embedding geometry. Some discussed the choice of t-SNE over UMAP, while others asked about adding more tokens or context-dependent embeddings.

**Tags**: `#GPT-2`, `#token embeddings`, `#visualization`, `#t-SNE`, `#interactive`

---

<a id="item-10"></a>
## [Minecraft Java Edition Migrates to SDL3 for Better Cross-Platform Support](https://www.minecraft.net/en-us/article/minecraft-26-3-snapshot-4) ⭐️ 7.0/10

Minecraft Java Edition has adopted SDL3 (Simple DirectMedia Layer 3) for its input handling and windowing system, replacing the previous SDL2-based implementation. This change is part of the latest snapshot (26w04a) released on January 23, 2026. This migration improves cross-platform consistency and performance across Windows, macOS, Linux, and Wayland, benefiting millions of players. It also demonstrates the game's ongoing evolution toward a more modular engine, which can influence modding and future development. Known issues include crashes in exclusive fullscreen mode on Windows with multiple monitors and on Wayland when entering exclusive fullscreen. The SDL3 bindings for LWJGL were contributed by a member of the GTNH modpack team, highlighting community involvement.

hackernews · ObviouslyFlamer · Jul 19, 11:48 · [Discussion](https://news.ycombinator.com/item?id=48967256)

**Background**: Simple DirectMedia Layer (SDL) is a cross-platform library that abstracts hardware for multimedia applications, making it easier to support multiple operating systems. SDL3, released in January 2025, introduces new features and performance improvements over SDL2. Minecraft Java Edition uses LWJGL (Lightweight Java Game Library), which wraps SDL and other native libraries for Java.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Simple_DirectMedia_Layer">Simple DirectMedia Layer - Wikipedia</a></li>
<li><a href="https://wiki.libsdl.org/SDL3/FrontPage">SDL3/FrontPage - SDL Wiki</a></li>
<li><a href="https://glusoft.com/sdl3-tutorials/">Free SDL3 Tutorials - Glusoft</a></li>

</ul>
</details>

**Discussion**: Community members noted that the SDL3 bindings were contributed by a GTNH modpack team member, completing a cycle of vanilla-to-modded-to-vanilla contributions. Some expressed concern about the known fullscreen crashes, considering them blocking bugs that could have delayed the snapshot. There was also praise for the game's evolution toward a game engine.

**Tags**: `#Minecraft`, `#SDL3`, `#gamedev`, `#cross-platform`, `#updates`

---

<a id="item-11"></a>
## [SQLite Query Explainer: Interactive Browser Tool with Pyodide](https://simonwillison.net/2026/Jul/18/sqlite-query-explainer/#atom-everything) ⭐️ 7.0/10

Simon Willison built an interactive browser-based tool that runs SQLite in Python via Pyodide and WebAssembly to explain query plans, inspired by Julia Evans' blog post. It provides plain-English explanations for both EXPLAIN and EXPLAIN QUERY PLAN output. This tool lowers the barrier for developers to understand SQLite query plans, which are crucial for database performance tuning but often difficult to read. Running entirely in the browser with no server-side dependency makes it instantly accessible to anyone. The tool uses Pyodide to run Python's sqlite3 module inside the browser, executing queries via WebAssembly. It shows both the low-level EXPLAIN output and the more readable EXPLAIN QUERY PLAN, with added explanations. The author acknowledges his own limited expertise in SQLite query plans, so users should verify results.

rss · Simon Willison · Jul 18, 17:19

**Background**: SQLite query plans describe how the database engine executes a query, using operators like SEARCH and SCAN. EXPLAIN and EXPLAIN QUERY PLAN are built-in SQL commands that output low-level virtual machine instructions or a more readable plan tree. Pyodide is a Python distribution compiled to WebAssembly, enabling Python to run in the browser. WebAssembly is a binary instruction format that allows high-performance execution in web browsers, originally released in 2017.

<details><summary>References</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.2</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#query plan`, `#sql`, `#webassembly`, `#pyodide`

---

<a id="item-12"></a>
## [Kaggle DeepMind Prize Allegedly Awarded to 'AI Slop'](https://www.reddit.com/r/MachineLearning/comments/1uzyf66/did_blatant_ai_slop_just_win_a_25k_usd_deepmind/) ⭐️ 7.0/10

A Reddit post claims that the grand prize winner of a Google DeepMind-sponsored Kaggle competition is a low-quality submission full of unfounded claims and nonsensical code, alleging poor judging. This controversy raises serious questions about the integrity of high-stakes AI competitions and the rigor of peer review in benchmark design, potentially undermining trust in such contests. The competition, 'Measuring Progress Toward AGI - Cognitive Abilities,' asked participants to design cognitive-science-based benchmarks, and the winning submission was reportedly 10 times the requested format with no coherent methodology.

reddit · r/MachineLearning · /u/TheWerkmeister · Jul 18, 15:10

**Background**: Kaggle is a platform for data science competitions where companies host challenges with prizes. DeepMind, an AI research lab, sponsored this competition to incentivize novel AI benchmarks. Benchmarks are standardized tests used to evaluate AI model performance.

<details><summary>References</summary>
<ul>
<li><a href="https://benchlm.ai/benchmarks">AI Benchmarks : 321 LLM Evaluations Ranked (July 2026) | BenchLM. ai</a></li>
<li><a href="https://aimultiple.com/ai-benchmarks">200+ Leading AI Benchmarks</a></li>

</ul>
</details>

**Tags**: `#Kaggle`, `#DeepMind`, `#competition integrity`, `#AI benchmarks`, `#critical analysis`

---

<a id="item-13"></a>
## [GPT-2 Small Embedding Geometry: Discretized vs Continuous Neighbors](https://www.reddit.com/r/MachineLearning/comments/1v07xai/gpt2_smalls_embedding_geometry_around_trump/) ⭐️ 7.0/10

A visualization of GPT-2 Small's static token embeddings reveals that discretizing coordinates yields generic political neighbors for 'Trump', while continuous embeddings capture specific family members and rivals. This analysis highlights how different representations of the same embeddings can drastically alter nearest neighbor semantics, which is crucial for interpretability and understanding what models learn. The study uses t-SNE projection for visualization and compares nearest neighbors under two conditions: discretized (thresholded coordinates) vs continuous (original coordinates), without any attention or context.

reddit · r/MachineLearning · /u/Limp-Contest-7309 · Jul 18, 21:29

**Background**: Word embeddings are continuous vector representations of words learned by language models. Static embeddings, like those from GPT-2 Small's embedding table, assign a fixed vector per token, unlike contextual embeddings that change with context. t-SNE is a nonlinear dimensionality reduction technique used to visualize high-dimensional embeddings in 2D or 3D.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/1909.10724">Situating Sentence Embedders with Nearest Neighbor Overlap Lucy H. Lin⋆</a></li>
<li><a href="https://en.wikipedia.org/wiki/T-distributed_stochastic_neighbor_embedding">t-distributed stochastic neighbor embedding - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/pulse/static-vs-contextual-embeddings-vivek-palvia-moftc">Static vs Contextual Embeddings</a></li>

</ul>
</details>

**Tags**: `#gpt2`, `#embeddings`, `#token representation`, `#nearest neighbors`, `#interpretability`

---

<a id="item-14"></a>
## [Deep Learning Survey for scRNA-seq Analysis](https://www.reddit.com/r/MachineLearning/comments/1v06nc1/deep_learning_tackles_singlecell_analysis_a/) ⭐️ 7.0/10

A Reddit user has posted a comprehensive summary table of 25 deep learning methods for single-cell RNA-seq analysis, organized into 6 categories, based on a recent survey paper. This survey provides a structured overview of deep learning techniques in single-cell analysis, helping researchers quickly identify relevant methods for tasks such as cell clustering, gene imputation, and trajectory inference, thereby accelerating bioinformatics research. The table includes for each method its category, purpose, architecture, evaluation metrics, explanation, and specific novelty, covering both supervised and unsupervised approaches.

reddit · r/MachineLearning · /u/teraRockstar · Jul 18, 20:35

**Background**: Single-cell RNA sequencing (scRNA-seq) measures gene expression in individual cells, enabling the study of cellular heterogeneity. However, scRNA-seq data is high-dimensional, sparse, and noisy, posing challenges for traditional analysis methods. Deep learning models, such as autoencoders and generative adversarial networks, have been increasingly applied to tasks like data imputation, clustering, and visualization to overcome these challenges.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2210.12385">[2210.12385] Deep Learning in Single-Cell Analysis - arXiv.org</a></li>
<li><a href="https://dl.acm.org/doi/abs/10.1145/3641284">Deep Learning in Single-cell Analysis - ACM Digital Library</a></li>
<li><a href="https://dl.acm.org/doi/full/10.1145/3641284">Deep Learning in Single-cell Analysis - ACM Digital Library</a></li>

</ul>
</details>

**Tags**: `#deep learning`, `#scRNA-seq`, `#single-cell analysis`, `#bioinformatics`, `#survey`

---

<a id="item-15"></a>
## [TabFM Studio: No-Code Spreadsheet Predictions with Google's Tabular Foundation Model](https://www.reddit.com/r/MachineLearning/comments/1uzx1el/tabfm_studio_pointandclick_predictions_on/) ⭐️ 7.0/10

A new web app called TabFM Studio allows users to make predictions on spreadsheets using Google's TabFM tabular foundation model entirely without writing code, by simply uploading a CSV or Excel file and selecting the target column. This tool greatly lowers the barrier to using advanced tabular foundation models for non-programmers, enabling business analysts and domain experts to leverage state-of-the-art in-context learning for predictions directly in spreadsheets. The app runs entirely locally and currently supports only Google's TabFM model. It uses filled rows as in-context examples (few-shot learning) to predict missing target values in rows with empty cells.

reddit · r/MachineLearning · /u/Lckylke · Jul 18, 14:15

**Background**: Tabular foundation models like TabFM are pretrained on millions of diverse datasets and perform in-context learning, meaning they can make predictions for a new task by being given a few examples at inference time without additional fine-tuning. This is unlike traditional machine learning which requires training a model on a specific dataset. In-context learning was popularized by large language models and has now been extended to tabular data.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/">Introducing TabFM : A zero-shot foundation model for tabular data</a></li>
<li><a href="https://tabularfoundationmodels.com/">Tabular Foundation Models</a></li>
<li><a href="https://github.com/google-research/tabfm">GitHub - google -research/ tabfm : TabFM (Tabular Foundation Model)...</a></li>

</ul>
</details>

**Tags**: `#tabular foundation models`, `#no-code ML`, `#web app`, `#machine learning`, `#spreadsheets`

---

<a id="item-16"></a>
## [Bananas sprout in UK garden after 15 years](https://www.bbc.com/news/articles/cvg8edqq5g5o) ⭐️ 6.0/10

Banana plants have sprouted in a garden in Rayleigh, UK, after 15 years of growth, attributed to changing climate conditions. This event highlights the tangible effects of climate change on local ecosystems and gardening, showing that previously impossible crops can now grow in the UK. The banana variety is Musa Basjoo, which is not suitable for eating due to poor taste and texture; the plant typically flowers and dies before producing usable fruit.

hackernews · teleforce · Jul 19, 13:29 · [Discussion](https://news.ycombinator.com/item?id=48968063)

**Background**: Bananas are tropical plants that require warm temperatures and specific growing conditions. The UK's mild climate due to the Gulf Stream has been changing, allowing some tropical species to survive outdoors. However, fruiting remains challenging even with successful blooming.

**Discussion**: Commenters shared personal experiences of growing bananas in colder regions, noting that while plants bloom, they often die before producing ripe fruit. There was agreement that climate change is observable in gardens. One commenter humorously described the poor edibility of Musa Basjoo.

**Tags**: `#climate change`, `#banana`, `#gardening`, `#UK`, `#discussion`

---