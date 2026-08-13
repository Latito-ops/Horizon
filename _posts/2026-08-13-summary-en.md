---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 34 items, 21 important content pieces were selected

---

1. [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](#item-1) ⭐️ 9.0/10
2. [Qwen Releases Qwen3.8-2.4T-A95B, a 2.4T-Parameter MoE Model](#item-2) ⭐️ 9.0/10
3. [Researchers Recover Secret Chain-of-Thought Traces from Proprietary LLM APIs](#item-3) ⭐️ 9.0/10
4. [DeepSeek V4 Pro 0813](#item-4) ⭐️ 8.0/10
5. [HTML over WebSockets: Real-Time SPAs with Minimal JavaScript](#item-5) ⭐️ 8.0/10
6. [uBlock Origin Gives Up the Fight to Block Facebook Ads](#item-6) ⭐️ 8.0/10
7. [xAI Launches Grok 4.6, a New Frontier AI Model](#item-7) ⭐️ 8.0/10
8. [Why Tiny JPEGs Look Different in Chrome: Scaled Decoding Explained](#item-8) ⭐️ 8.0/10
9. [AI-assisted coding may create systems no developer understands, warns engineer](#item-9) ⭐️ 8.0/10
10. [There Are No Lossless Transformations of Natural-Language Text](#item-10) ⭐️ 8.0/10
11. [Adam's Coordinate-Wise Scaling Destroys Implicit Low-Rank Bias; Rotation-Invariant Optimizers Preserve It](#item-11) ⭐️ 8.0/10
12. [Decoupled Descent Training Tracks Test Error via AMP Onsager Corrections](#item-12) ⭐️ 8.0/10
13. [Zed launches Delta for multiplayer AI-agent coding](#item-13) ⭐️ 7.0/10
14. [Crowdsourced Webcam Page Tracks 2026 Solar Eclipse](#item-14) ⭐️ 7.0/10
15. [Honest CS Conference Ranking Sorts Venues by Travel Appeal](#item-15) ⭐️ 7.0/10
16. [Tim King, key AmigaDOS developer, has died](#item-16) ⭐️ 6.0/10
17. [Discovered Materials (YC P26) Uses AI Agents to Find Semiconductor Materials](#item-17) ⭐️ 6.0/10
18. [datasette-upload-dbs 0.5a0: formal API for database uploads and swaps](#item-18) ⭐️ 6.0/10
19. [AAAI 2027 Reviewer Questions Papers Without Code](#item-19) ⭐️ 6.0/10
20. [Developer Rebuilds Spiking Language Model NORD Around CPU-First Inference](#item-20) ⭐️ 6.0/10
21. [Seeking RL and Planning Guidance for Stochastic Merge Puzzle with Previewed Chance Events](#item-21) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 9.0/10

Tailscale traced repeated corruption of its control-plane SQLite database to a race condition in SQLite's WAL-reset logic, which the SQLite team estimates had existed for at least 16 years. They also funded an open-source VFS debugging shim that helped isolate the bug. This is a rare, deep root-cause analysis of a long-standing database bug that could affect any application using SQLite in WAL mode with certain checkpoint behavior. The company's decision to fund open-source debugging tooling also sets a positive example for ecosystem sustainability. The bug is triggered during checkpoints and can cause committed transactions to vanish from the database. A single-writer design does not protect against it because the race involves multiple database connections coordinating WAL resets. Tailscale's VFS shim is now available to help track down similar issues.

hackernews · ropbear · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**Background**: SQLite uses a write-ahead log (WAL) to provide crash safety and concurrency, and a special WAL-index file coordinates readers and writers. A subtle race in how the WAL is reset during checkpoints can leave the database inconsistent. SQLite is one of the most widely used embedded databases, so even a rarely triggered bug can affect many deployments.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL - Reset bug</a></li>
<li><a href="https://www.youngju.dev/blog/2026-07-16-sqlite-wal-reset-bug.en">The SQLite WAL - Reset Bug: A Data Corruption Race That Hid for 15...</a></li>
<li><a href="https://zeli.app/en/story/49272832">Tailscale Traces Database Corruption to 16y/o SQLite WAL - Reset Bug</a></li>

</ul>
</details>

**Discussion**: Commenters appreciated the clarity of the write-up and highlighted the interesting open-source funding model, while some initially puzzled over how a single-writer design could still race. Another comment noted the philosophical tension between SQLite's massive test suite and Dijkstra's saying that tests cannot prove the absence of bugs.

**Tags**: `#sqlite`, `#databases`, `#bug`, `#tailscale`, `#open-source`

---

<a id="item-2"></a>
## [Qwen Releases Qwen3.8-2.4T-A95B, a 2.4T-Parameter MoE Model](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Alibaba's Qwen team released Qwen3.8-2.4T-A95B, an open-weight mixture-of-experts model with 2.4 trillion total parameters and 95 billion active per token, along with an FP8 version. The model card claims frontier-level performance, which community members describe as between Opus 4.8 and Fable 5. This is one of the largest open-weight models ever released, bringing near-frontier capabilities to the open ecosystem and intensifying competition among Chinese AI labs. Its release will be felt by researchers and enterprises seeking to deploy frontier-grade models on their own infrastructure, though the massive memory requirements create a significant barrier to entry. The model has 512 routed experts with 10 active per token plus one shared expert, built on a 92-layer hybrid-attention backbone with a 256K context length. Initial releases are only in bf16 and FP8, so a 4-bit quantized version will require post-training quantization with substantial calibration data; the bf16 full model takes about 4.9TB of memory.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**Background**: Mixture-of-experts (MoE) is an architecture where a router selects only a small subset of specialized 'experts' for each token, allowing very large total parameter counts while keeping compute costs closer to a much smaller model. Quantization, such as FP8, reduces numeric precision to shrink memory footprint and speed up inference at the cost of some accuracy. These techniques matter because frontier models have grown too large for conventional single-GPU serving, making efficient deployment an active engineering challenge. Qwen is Alibaba's open-weight LLM family, and Qwen3.8-2.4T-A95B is the open-weight variant of the commercial Qwen3.8-Max.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/serve-qwen3-8-2-4t-a95b-a-2-4t-parameter-model-with-configurable-reasoning-on-nvidia-gb300-nvl72/">Serve Qwen3.8-2.4T-A95B, a 2.4T-Parameter Model, with Configurable Reasoning on NVIDIA GB300 NVL72 | NVIDIA Technical Blog</a></li>
<li><a href="https://recipes.vllm.ai/Qwen/Qwen3.8-2.4T-A95B">Qwen/Qwen3.8-2.4T-A95B — 2.4T / 95B active · MOE · 256K ctx</a></li>
<li><a href="https://localmodel.run/guides/mixture-of-experts">Mixture of experts (MoE) explained for local LLMs · localmodel.run</a></li>

</ul>
</details>

**Discussion**: Community comments are largely technical, focusing on serving difficulties: the model is larger than Kimi k3 at launch, and with no QAT'd 4-bit weights, someone with deep pockets will need to quantize it. Some express excitement that a 1-bit quant at ~397GB could put Opus 4.5-level performance on a high-end workstation, while others point out the open-weight version lacks vision input and the 1M context of Qwen3.8-Max. A few users question whether real-world performance matches the benchmark claims.

**Tags**: `#LLM`, `#Qwen`, `#MoE`, `#AI`, `#HuggingFace`

---

<a id="item-3"></a>
## [Researchers Recover Secret Chain-of-Thought Traces from Proprietary LLM APIs](https://simonwillison.net/2026/Aug/11/stealing-reasoning-traces/) ⭐️ 9.0/10

A new paper from stolen-thoughts.com reveals that encrypted chain-of-thought blocks from Anthropic, OpenAI, and Google APIs can be replayed into weaker sibling models and jailbroken, recovering the stronger model's private reasoning in plaintext. The attack was acknowledged by all providers and has reportedly been fixed since. This demonstrates a serious security flaw in how proprietary LLM APIs encrypt chain-of-thought reasoning, affecting Anthropic, OpenAI, and Google. It shows that encrypted reasoning traces are not safe from replay attacks, with major implications for AI privacy, safety, and intellectual property, as hidden reasoning can be extracted and used to distill model capabilities or find vulnerabilities. The vulnerability stems from all models in a family using the same encryption key, so a trace from a frontier model could be replayed into the weakest sibling. Claude Haiku 4.5 was exploited with a transcription prompt and a prefilled "<thinking-copy>" prefix; the providers have since patched the issue, while the removed prefix feature still worked on Haiku 4.5.

rss · Simon Willison · Aug 11, 22:40

**Background**: Chain-of-thought (CoT) reasoning is a technique where LLMs produce step-by-step intermediate reasoning before a final answer, improving performance on complex tasks. To protect proprietary secrets and prevent distillation, some API providers encrypt these intermediate reasoning tokens. A replay attack reuses captured messages in a different context to fool the system; jailbreaking uses carefully crafted prompts to bypass safety guardrails and make models reveal hidden information. Together, these allow attackers to decrypt hidden thinking traces.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.11903">[2201.11903] Chain - of - Thought Prompting Elicits Reasoning in ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Replay_attack">Replay attack - Wikipedia</a></li>
<li><a href="https://arxiv.org/pdf/2310.08419">Jailbreaking Black Box Large Language Models in</a></li>

</ul>
</details>

**Tags**: `#LLM security`, `#chain-of-thought`, `#AI safety`, `#proprietary APIs`, `#research`

---

<a id="item-4"></a>
## [DeepSeek V4 Pro 0813](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek V4 Pro 0813 is released, with early community testing showing strong performance and cost-effectiveness for development workloads.

hackernews · explosion-s · Aug 12, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49274600)

**Tags**: `#AI`, `#DeepSeek`, `#Large Language Models`, `#Machine Learning`

---

<a id="item-5"></a>
## [HTML over WebSockets: Real-Time SPAs with Minimal JavaScript](https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/) ⭐️ 8.0/10

The article presents HTML over WebSockets, a technique for building real-time single-page applications (SPAs) with barely any client-side JavaScript. It describes a bidirectional variant where the server generates HTML fragments and sends them over a WebSocket connection, while the client runs only a thin DOM-remoting script. This perspective challenges the conventional JavaScript-heavy SPA architecture and could simplify development by keeping rendering logic on the server. It also fuels an ongoing industry debate about when to use WebSockets versus Server-Sent Events (SSE) or REST, affecting how developers design real-time features. The article emphasizes a 'single language, no contracts, single rendering engine' approach. Critics note that for one-way server pushes, SSE is simpler and cheaper to operate, while WebSockets are only necessary for bidirectional low-latency communication, and alternatives like htmx or Blazor already implement similar patterns.

hackernews · redbell · Aug 12, 16:51 · [Discussion](https://news.ycombinator.com/item?id=49275335)

**Background**: A SPA (single-page application) traditionally loads an HTML page once and then updates the view using JavaScript, often fetching JSON from a REST API. Server-Sent Events (SSE) allows a server to push updates to the client over a single long-lived HTTP connection, while WebSockets provide a full-duplex persistent channel. HTML over WebSockets goes a step further by sending pre-rendered HTML fragments instead of JSON, so the client does not need a complex framework or state management. The concept is similar to how Phoenix LiveView, Blazor Server, or htmx work, and has roots in early prototypes like Chris McCord's Rails 'Sync'.

<details><summary>References</summary>
<ul>
<li><a href="https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/">HTML over WebSockets: real-time SPAs with barely any JavaScript | Andros Fenollosa</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events">Using server - sent events - Web APIs | MDN</a></li>
<li><a href="https://www.reddit.com/r/programming/comments/lsgimx/the_future_of_web_software_is_htmloverwebsockets/">r/programming on Reddit: The Future of Web Software Is HTML-over-WebSockets</a></li>

</ul>
</details>

**Discussion**: Commenters are split: some advocate SSE and Fetch for most use cases, arguing WebSockets add unnecessary complexity if only server push is needed. Others mention real-world examples like Blazor Server and htmx, and point out historical precedence with Chris McCord's earlier work, while one comment links to a critical response post.

**Tags**: `#WebSockets`, `#Real-time`, `#SPA`, `#JavaScript`, `#Server-rendered`

---

<a id="item-6"></a>
## [uBlock Origin Gives Up the Fight to Block Facebook Ads](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 8.0/10

uBlock Origin's volunteer developers have announced they will stop actively trying to block ads on Facebook, citing the platform's constantly changing anti-adblocking techniques. The team described Facebook as a 'disgusting anti-user site' in the announcement. This marks a significant defeat for one of the most popular ad blockers, affecting tens of millions of users who rely on uBlock Origin to keep Facebook's feed clean. It highlights how difficult it is for small open-source teams to keep up with large platforms' anti-adblocking measures, with broader implications for user privacy and the ad-blocking arms race. uBlock Origin is a free, open-source browser extension with over 29 million Chrome users and 10.6 million Firefox users as of June 2026. The decision only affects Facebook; the extension will continue to block ads on other sites, though Facebook itself warns that ad blockers may cause its site to malfunction.

hackernews · Markoff · Aug 12, 11:28 · [Discussion](https://news.ycombinator.com/item?id=49270726)

**Background**: uBlock Origin is a widely used content-filtering browser extension that blocks ads, trackers, and malicious URLs. Ad blockers work by comparing page elements against filter lists, but platforms like Facebook use obfuscation and rapidly changing markup to evade these lists, creating a constant cat-and-mouse game. The announcement was made on the uBlock Origin subreddit, where a team member explained why Facebook was especially difficult to keep blocking.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">UBlock Origin</a></li>
<li><a href="https://piunikaweb.com/2026/08/10/ublock-origin-facebook-ads-not-blocking/">Seeing ads on Facebook even with uBlock Origin? Here's why</a></li>

</ul>
</details>

**Discussion**: Commenters are largely supportive of the decision, with some predicting the arms race will eventually end in computer vision-based ad detection that draws boxes over ads. Others question why Facebook spends so much effort circumventing ad blockers when users with blockers installed are unlikely to click ads anyway, while a few argue that the only real solution is to leave Facebook altogether.

**Tags**: `#ad-blocking`, `#facebook-ads`, `#privacy`, `#ublock-origin`, `#web-platforms`

---

<a id="item-7"></a>
## [xAI Launches Grok 4.6, a New Frontier AI Model](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

On August 7, 2026, xAI launched Grok 4.6, a frontier AI model that it says delivers significant improvements over Grok 4.5 at the same price. Benchmark reports put it around 1753 ELO and claim it beats GPT-5.6-Sol on most benchmarks while costing about half as much as rival frontier models. Grok 4.6 strengthens xAI's position in the frontier AI race and puts competitive pressure on other major labs by offering strong performance at a lower price. For developers and enterprises, it provides a cost-effective alternative for demanding AI workloads, which could reshape pricing and model choice across the ecosystem. According to reports, Grok 4.6 is a 1.5-trillion-parameter model trained with improved supervised fine-tuning and reinforcement learning. It is available through xAI's API (including for code and other tasks) and is positioned as a significant step up from Grok 4.5 in handling more challenging tasks.

hackernews · iLuddite · Aug 12, 15:32 · [Discussion](https://news.ycombinator.com/item?id=49274027)

**Background**: Frontier AI models are the most advanced large-scale systems available at a given time, capable of matching or exceeding other models across a wide variety of tasks. Grok is xAI's series of large language models integrated into the X platform and offered via API. The launch of Grok 4.6 continues a rapid release cadence among major labs, with benchmarks and cost becoming key battlegrounds.

<details><summary>References</summary>
<ul>
<li><a href="https://www.basenor.com/blogs/news/xai-launches-grok-4-6-1753-elo-half-the-price-of-rival-frontier-models">xAI Launches Grok 4.6: 1753 ELO, Half the Price of Rival Frontier Models</a></li>
<li><a href="https://kie.ai/blog/what-is-grok-4-6">What Is Grok 4.6? xAI's 1.5T-Param Model Explained</a></li>
<li><a href="https://docs.x.ai/developers/models">Models - Docs - SpaceXAI</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed but generally engaged: some users praise Grok 4.6's speed, conciseness, and Fable-like intelligence, while others question how all major labs suddenly matched Fable within two months and suspect benchmark hacking or distillation. A notable complaint involves the API adding a default system prompt that overrides user instructions and refuses to discuss system prompts, which some find annoying.

**Tags**: `#AI models`, `#Grok`, `#xAI`, `#benchmarks`, `#machine learning`

---

<a id="item-8"></a>
## [Why Tiny JPEGs Look Different in Chrome: Scaled Decoding Explained](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

A developer found that tiny JPEGs render differently in Chrome than in Firefox, and traced it to Chrome's scaled decoding optimization. When downscaling JPEGs, Chrome uses partial IDCT scaling via libjpeg-turbo and decodes only low-frequency data, producing a slightly thicker or blurrier appearance. This matters because web developers and designers rely on consistent cross-browser rendering for icons and small images; a performance optimization silently changes visual output. The issue also affects Electron apps, since they embed Chromium, and highlights a broader trade-off between decoding speed and image fidelity. The optimization is specific to downscaled JPEG decoding: Chrome skips high-frequency DCT coefficients via libjpeg-turbo's scaled IDCT path, which changes edge rendering at small sizes. Commenters note the same problem occurs with PNGs, and Mozilla is tracking similar scaled-decompression work in Firefox bug 2033250; different scaling algorithms between browsers also contribute to visible differences.

hackernews · gutechh · Aug 12, 14:00 · [Discussion](https://news.ycombinator.com/item?id=49272549)

**Background**: JPEG compression works by transforming image blocks into DCT coefficients, where low-frequency coefficients carry most visual information and high-frequency coefficients carry detail. Decoding every coefficient at full resolution is expensive, so libjpeg-turbo offers a scaled decoding mode that computes only a subset, sacrificing some accuracy for speed. Browsers like Chrome and Firefox make different choices about when and how to use such optimizations, which is why the same JPEG can look different depending on the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://zeli.app/en/story/49272549">Chrome 's Clever JPEG Decoding Trick Makes Tiny Images Look... | Zeli</a></li>
<li><a href="https://issues.chromium.org/issues/381913638">Releative with 40946711: support scaled decode for... - Chromium</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters broadly confirmed the issue, with one noting the same problem appears in PNGs and that Chrome's optimization broke Electron app icons, forcing a delayed upgrade. Others debated whether Chrome's blurrier output or Firefox's sharper but ringing-prone output is preferable, and one commenter pointed out that the post only explains Chrome's side, asking whether Firefox does full rendering then scaling or a different partial method.

**Tags**: `#JPEG`, `#Chrome`, `#image scaling`, `#browser rendering`, `#web performance`

---

<a id="item-9"></a>
## [AI-assisted coding may create systems no developer understands, warns engineer](https://simonwillison.net/2026/Aug/12/florian-herrengt/) ⭐️ 8.0/10

Florian Herrengt's blog post, quoted on Simon Willison's site, warns that AI-driven development can produce convoluted, multi-layered systems that no single developer fully understands. The scenario depicts a team repeatedly asking AI tools like Claude to fix a bug without anyone grasping the data flow. As AI coding agents like Claude Fable 5 accelerate feature development, this raises urgent concerns about long-term maintainability and 'cognitive debt' in software projects. It also challenges the role of mid-level software engineers, who may lose the deep system understanding traditionally needed to debug and evolve complex systems. The quote specifically refers to 'Fable' as an AI that cannot figure out a recurring bug, and describes a developer saying 'Let me ask Claude' in response to a question about data origin. The post's title coins the phrase 'AI is removing the middle class of software engineering,' pointing to the erosion of mid-level engineering roles and tacit knowledge.

rss · Simon Willison · Aug 12, 15:08

**Background**: AI-assisted programming tools have evolved from simple autocomplete to autonomous agents that can build entire features or applications, such as Anthropic's Claude Fable 5, which handles complex multi-agent workflows in Claude Code. This shift means developers increasingly review generated code rather than write it line by line, reducing their familiarity with the system's internal logic. 'Cognitive debt' describes the accumulation of unexplained or poorly understood code, which becomes a growing maintenance burden as human comprehension lags behind machine-generated complexity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://workingnotworking.com/fable-ai-shift-from-prompting-to-full-software-building/">Fable AI Rapid Adoption Signals the Shift to Full Software Building</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#code quality`, `#developer experience`, `#future of work`

---

<a id="item-10"></a>
## [There Are No Lossless Transformations of Natural-Language Text](https://simonwillison.net/2026/Aug/11/there-are-no-lossless-transformations-of-natural-language-text/) ⭐️ 8.0/10

Sophie Alpert published an internal policy on acceptable use of AI writing by engineers, arguing that LLM rewrites of natural language are inherently lossy and that writers must stand behind every sentence. Simon Willison highlighted this policy as a valuable reference for responsible AI use. This matters because it provides practical guidance for engineering teams adopting AI writing tools, emphasizing authorial responsibility and the risk of information loss when AI rewrites text. It addresses a growing concern in the AI/ML and software engineering communities about the reliability and authenticity of AI-assisted communication. Alpert's policy states that every rewrite and rephrase changes meaning, especially when done by an entity without the writer's mental model. It also asserts that if a reviewer asks about a line, it's not acceptable to respond that AI wrote it and to ignore it.

rss · Simon Willison · Aug 11, 23:48

**Background**: The concept of lossless transformations originates from information theory, where a transformation is lossless if no information is lost in the process. Large language models (LLMs) are AI systems trained on vast amounts of text to generate, summarize, and translate language, but they lack the writer's specific intent and context, making their transformations potentially lossy. This contrast highlights the fundamental challenge of using AI for writing tasks that require precision and personal voice.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model</a></li>
<li><a href="https://diversedaily.com/exploring-absolute-information-conservation-a-comprehensive-analysis/">Exploring Absolute Information Conservation: A Comprehensive...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#writing`, `#engineering-practices`, `#ethics`

---

<a id="item-11"></a>
## [Adam's Coordinate-Wise Scaling Destroys Implicit Low-Rank Bias; Rotation-Invariant Optimizers Preserve It](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 8.0/10

A Reddit analysis reports that Adam's per-coordinate second-moment scaling removes the implicit low-rank bias that gradient descent exhibits in factored models, while rotation-invariant optimizers such as Muon and Shampoo preserve it. The author runs nine update rules on underdetermined matrix sensing and shows a one-parameter family from per-coordinate to shared-scalar Adam recovers the bias monotonically. This matters because it identifies a mechanistic property—coordinate-basis dependence—that separates optimizers that keep gradient descent's useful inductive bias from those that lose it. The result could guide optimizer choice and design for matrix recovery and deep linear networks, and it highlights Muon's mixed behavior as an open question. The experiments compare GD, shared-scalar Adam, Muon, and Shampoo (which keep the bias) against Adam, RMSProp, Lion, signum, and Adafactor (which lose it) at matched training loss. The author also notes that momentum is not covered by the theory, and that the 43-44% held-out error reduction on hyperspectral data shrinks considerably when each method selects its own learning rate.

reddit · r/MachineLearning · /u/EtherealGlyph · Aug 12, 16:39

**Background**: In factored models such as W = UV^T, the loss is invariant under rotations of the factors, and gradient descent respects this symmetry. Adam's per-coordinate second-moment scaling breaks rotation invariance because it depends on the basis in which the parameters are written. Implicit low-rank bias is a well-known phenomenon where certain optimizers prefer low-rank solutions in over-parameterized matrix factorization and deep linear networks. Muon is a structure-aware optimizer that orthogonalizes gradient updates and is used in models like Kimi K2; recent papers disagree about whether it exhibits a spectral simplicity bias.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/muon-optimizer">Muon optimizer</a></li>
<li><a href="https://arxiv.org/pdf/2011.13772">Gradient Descent for Deep Matrix Factorization</a></li>
<li><a href="https://en.papernotes.org/NeurIPS2025/optimization/understanding_adam_requires_better_rotation_dependent_assumptions/">[Paper Note] Understanding Adam Requires Better Rotation ...</a></li>

</ul>
</details>

**Tags**: `#optimization`, `#Adam`, `#implicit bias`, `#low-rank`, `#matrix sensing`

---

<a id="item-12"></a>
## [Decoupled Descent Training Tracks Test Error via AMP Onsager Corrections](https://www.reddit.com/r/MachineLearning/comments/1vlu1se/decoupled_descent_enforcing_exact_traintest_error/) ⭐️ 8.0/10

The paper introduces Decoupled Descent (DD), a neural-network training method that applies Onsager corrections from approximate message passing (AMP) to guarantee that, asymptotically, the training error equals the test error at every parameter iterate. The author also shares simulation results for a two-layer network on a high-dimensional XOR model, contrasting GD with DD. This matters because it offers a principled way to eliminate the train-test error gap that plagues gradient-based training, potentially enabling safer optimal stopping and hyperparameter tuning during neural-network training. It also builds a novel theoretical bridge between AMP-based high-dimensional statistics and optimization/generalization in deep learning. Decoupled Descent is framed as a theory-first result: it studies full-batch gradient descent on stylized Gaussian mixture models, and the guarantee is asymptotic rather than finite-sample. The author notes that the method is far from being ready for very large models and plans to release a PyTorch-compatible implementation in the future.

reddit · r/MachineLearning · /u/mlovik1 · Aug 11, 21:06

**Background**: Approximate message passing (AMP) is a class of iterative algorithms, originally developed for compressed sensing and high-dimensional regression, that solves high-dimensional statistical problems by reducing them to scalar denoising steps. A key element is the Onsager correction term, which cancels correlations that accumulate between iterations and enables exact tracking of error metrics via state evolution. The paper treats overfitting from full-batch gradient descent as 'data reuse bias,' caused by repeatedly using the same training data to update parameters, and uses AMP-style corrections to prevent this bias from separating train and test errors.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2008.11892">[2008.11892] Approximate Message Passing algorithms for ...</a></li>
<li><a href="https://www.emergentmind.com/topics/approximate-message-passing-amp-algorithms">Approximate Message Passing Algorithms - emergentmind.com</a></li>
<li><a href="https://arxiv.org/abs/2209.07074">[2209.07074] On the Reuse Bias in Off-Policy Reinforcement Learning</a></li>

</ul>
</details>

**Tags**: `#Machine Learning`, `#Approximate Message Passing`, `#Generalization`, `#Optimization`, `#Neural Networks`

---

<a id="item-13"></a>
## [Zed launches Delta for multiplayer AI-agent coding](https://zed.dev/blog/introducing-delta) ⭐️ 7.0/10

Zed announced Delta, a multiplayer environment for collaborative coding with AI agents, now in private beta. It turns agent conversations into shared documents that update in real time via DeltaDB. Delta could redefine how developers review and mentor each other by linking code to the exact conversation that produced it. It signals a broader shift toward making AI agents collaborative rather than solitary tools. Delta works with existing Git repositories, lets teammates comment on any code or conversation, and supports joining threads from a browser or via Claude Code. It builds on Zed's existing multiplayer architecture and is available in private beta.

hackernews · khy · Aug 12, 18:19 · [Discussion](https://news.ycombinator.com/item?id=49276574)

**Background**: Zed is a high-performance, open-source code editor written in Rust, first released publicly in 2024. Its native multiplayer editing already distinguishes it from older editors, and Delta extends that capability to AI agent interactions, aiming to close the gap between conversation and code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zed_(text_editor)">Zed (text editor) - Wikipedia</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-13-zed-introduces-delta-a-new-multiplayer-environment-for-collaborative-coding-with-ai-agents-and-real">Zed Delta: Multiplayer Coding Environment for AI Agents</a></li>
<li><a href="https://zeli.app/en/story/49276574">Zed launches Delta, a multiplayer coding environment with ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed feelings: some saw little value in multiplayer coding, calling it a 'solution in search of a problem,' while others highlighted mentoring junior engineers as a compelling use case. A separate thread criticized the verbose nature of AI-generated code summaries, and one user complained about the page's low-contrast design.

**Tags**: `#editor`, `#collaboration`, `#AI`, `#developer-tools`

---

<a id="item-14"></a>
## [Crowdsourced Webcam Page Tracks 2026 Solar Eclipse](https://jonty.github.io/2026_eclipse_webcams/) ⭐️ 7.0/10

Jonty has revived his crowdsourced webcam aggregation page for the 2026 solar eclipse, originally built in 2024 for the US eclipse. The page went live just before totality, with a friend's reminder prompting its return. This tool provides a live, community-driven way to watch the 2026 eclipse from multiple locations, especially for those unable to travel. It demonstrates how simple web tools can enhance public engagement with rare astronomical events. The page aggregates webcams across Iceland and Spain, and jonty notes that coordinating traffic to these cameras was unplanned. The project was built quickly in 2024, finished minutes before totality, and had been forgotten until a friend asked about it this morning.

hackernews · zoenolan · Aug 12, 11:53 · [Discussion](https://news.ycombinator.com/item?id=49270953)

**Background**: A solar eclipse occurs when the Moon passes between the Sun and Earth, temporarily blocking the Sun's light. Webcam aggregation pages collect live video feeds from multiple locations, allowing viewers to choose the best view or compare conditions. The 2026 eclipse is notable for its path across Iceland and Spain, where many enthusiasts travel to witness totality.

**Discussion**: The community response is enthusiastic and nostalgic. The author shares the backstory, while another commenter recounts traveling from Vancouver to Toronto for the 2024 eclipse and now being in Spain for the current one. Historical remarks about Thales' eclipse prediction add depth, and practical tips include webcam links and solar panel monitoring data.

**Tags**: `#eclipse`, `#webcams`, `#astronomy`, `#tools`

---

<a id="item-15"></a>
## [Honest CS Conference Ranking Sorts Venues by Travel Appeal](https://www.reddit.com/r/MachineLearning/comments/1vmbdk6/i_built_an_honest_cs_conference_ranking_sorted_by/) ⭐️ 7.0/10

A new website, honestcsrankings.org, ranks around 540 upcoming CORE-ranked CS conferences by destination quality instead of academic prestige, factoring in weather, safety, cost, accessibility, and city vibe. It also offers filters, an 'Upsets' tab for A* venues in poor destinations, distance-based sorting, and .ics calendar exports. This tool gives researchers a practical counterweight to traditional prestige-based rankings, helping them balance career value with personal experience when choosing conferences. It could shift how the academic community talks about conference attendance and travel decisions, for example by making destination quality a more explicit consideration. The ranking uses real climate data for the conference month, the Global Peace Index, and World Bank price levels. ICML/ICLR 2027 are absent because they are not yet announced, and COLM is missing because it has not been CORE-ranked; the long tail of smaller conferences is scraped from WikiCFP, so some errors are expected.

reddit · r/MachineLearning · /u/JohnAZoidberg77 · Aug 12, 11:23

**Background**: The CORE conference ranking, now part of the international ICORE collaboration, is a widely used measure of computing conference quality in many research communities. The Global Peace Index, produced by the Institute for Economics & Peace, ranks countries by peacefulness, while WikiCFP is a community-run wiki that collects calls for papers for science and technology conferences. Researchers commonly check venue location when deciding where to submit, but formal rankings rarely factor in destination attractiveness.

<details><summary>References</summary>
<ul>
<li><a href="https://portal.core.edu.au/conf-ranks/">portal. core .edu.au/conf- ranks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Global_Peace_Index">Global Peace Index</a></li>
<li><a href="http://www.wikicfp.com/cfp/servlet/event.showcfp?eventid=60382&copyownerid=1">WikiCFP : Call For Papers of Conferences, Workshops and Journals</a></li>

</ul>
</details>

**Tags**: `#CS conferences`, `#academic tools`, `#ranking`, `#travel`, `#research productivity`

---

<a id="item-16"></a>
## [Tim King, key AmigaDOS developer, has died](https://amiga-news.de/en/news/AN-2026-08-00070-EN.html) ⭐️ 6.0/10

Tim King, one of the key minds behind the AmigaDOS operating system, has passed away, as reported by amiga-news.de. His death has prompted reflection on his role in the development of the Amiga's command-line environment. Tim King's death is significant for retrocomputing and software history, as AmigaDOS was a core component of the AmigaOS platform. His work helped shape the command-line experience that influenced many later users and developers. AmigaDOS is the disk operating system of AmigaOS, providing file systems, file and directory manipulation, the command-line interface, and file redirection. Its early structure came directly from TRIPOS, with Tim King's work at MetaComCo bringing that technology to the Amiga.

hackernews · doener · Aug 12, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49272655)

**Background**: The Amiga is a family of personal computers produced by Commodore from 1985 until the company's bankruptcy in 1994, known for advanced graphics, sound, and multitasking. AmigaOS includes the Workbench graphical desktop and AmigaDOS as its underlying disk operating system. Tim King's work on AmigaDOS placed him firmly inside the technical history of the Commodore Amiga, specifically in one of the operating system's core components.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AmigaDOS">AmigaDOS - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AmigaOS">AmigaOS - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amiga">Amiga - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed gratitude and shared personal stories about how Tim King and AmigaDOS influenced their careers and interest in command-line interfaces. Several noted that AmigaDOS was their gateway to later using Linux CLI, while one remembered him as the friendly founder of UK Online. Another commenter shared a link to an October 2021 interview with King.

**Tags**: `#Amiga`, `#AmigaDOS`, `#Retrocomputing`, `#Obituary`, `#Software History`

---

<a id="item-17"></a>
## [Discovered Materials (YC P26) Uses AI Agents to Find Semiconductor Materials](https://discoveredmaterials.com/research/) ⭐️ 6.0/10

Startup Discovered Materials, from Y Combinator's P26 batch, launched AI agents that computationally discover new semiconductor materials, and released hundreds of discovered materials plus a benchmark at discoveredmaterials.com/research. They report that frontier models from Anthropic, OpenAI, and Kimi can find dynamically stable, promising materials in an 8-hour run. This matters because chip heat dissipation is becoming a critical bottleneck: GPUs' TDP is roughly doubling each generation, and data centers consume enormous power and water for cooling. If AI agents can shrink the expensive, years-long 'lab-to-fab' timeline, they could accelerate adoption of advanced packaging and better thermal materials in semiconductors. The founders say computational discovery is the 'easy part'; synthesis recipes from models are still weak, so they validate candidates in the lab. During their YC batch, they simulated, synthesized, and tested thermal interface materials that reportedly match performance of trade-secret materials from major chemical companies, and their benchmark also documents odd model behaviors such as Claude reward hacking and GPT-5.6 'losing its mind' after around 50M tokens.

hackernews · advaith08 · Aug 12, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49269090)

**Background**: Semiconductor chips generate heat proportional to their power consumption; TDP (Thermal Design Power) is the maximum heat a cooling system must handle. High Bandwidth Memory (HBM) stacks DRAM dies vertically and connects them with through-silicon vias, enabling 3D packaging, but dielectric materials like SiO2 trap heat between logic and memory. Bringing a new material into a semiconductor fab historically takes years and hundreds of millions of dollars, a hurdle known as the 'lab-to-fab valley of death.'

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Thermal_design_power">Thermal design power - Wikipedia</a></li>
<li><a href="https://blogs.sw.siemens.com/semiconductor-packaging/2025/06/05/chip-packaging-basics-to-advanced-3d-ic/">Chip Packaging: Engineer’s Guide to 2.5D and 3D IC</a></li>

</ul>
</details>

**Discussion**: Commenters were cautiously optimistic but skeptical. One questioned whether 'novel' compounds are actually novel given training-set contamination and suggested blind-test validation; another noted that similar AI-for-materials efforts have lacked impact but praised this post for addressing feasibility. A researcher said closing the computational-experimental loop is the main challenge and wished them luck, while others found the quoted GPT-5.6 output amusing.

**Tags**: `#AI`, `#materials science`, `#semiconductors`, `#startup`, `#deep tech`

---

<a id="item-18"></a>
## [datasette-upload-dbs 0.5a0: formal API for database uploads and swaps](https://simonwillison.net/2026/Aug/11/datasette-upload-dbs/) ⭐️ 6.0/10

datasette-upload-dbs 0.5a0 introduces a formalized REST API endpoint (/-/upload-dbs) that allows authenticated users to upload a new SQLite database or atomically replace an existing one via curl or HTTP clients. This update makes it practical to build fresh databases in environments like GitHub Actions and deploy them to production seamlessly, replacing old data without downtime. Atomic swaps reduce the risk of serving corrupted or incomplete databases. The new API endpoint accepts a multipart POST with the database file and a target name, requiring an API token for authentication. The uploaded database is verified before the atomic swap, ensuring the /name path serves the new data only after successful validation.

rss · Simon Willison · Aug 11, 20:35

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases through a web interface. This plugin extends a hosted Datasette instance by letting users upload new database files and swap them in atomically — meaning the replacement is an all-or-nothing operation that avoids exposing incomplete data to readers. The new API formalizes a programmatic way to trigger that process, which was previously only available through the plugin's interface.

<details><summary>References</summary>
<ul>
<li><a href="https://arpitbhayani.me/blogs/atomicity/">Decoding Atomicity - The A in ACID</a></li>

</ul>
</details>

**Tags**: `#Datasette`, `#SQLite`, `#API`, `#plugin`, `#database`

---

<a id="item-19"></a>
## [AAAI 2027 Reviewer Questions Papers Without Code](https://www.reddit.com/r/MachineLearning/comments/1vlqjby/aaai_2027_review_no_code_submission_d/) ⭐️ 6.0/10

A reviewer for AAAI 2027 posted on Reddit expressing surprise at the large number of submissions lacking code implementations. They are considering whether to factor missing code into their initial scores and asked for community opinions. This discussion highlights reproducibility concerns in machine learning research and could shape how reviewers treat code submission. If reviewers penalize missing code, authors may be more motivated to release code, potentially improving research transparency. The reviewer notes they always submit code and publish it on ArXiv after the review process, and mentions that AI assistants could quickly generate empirical papers with fake results. They are unsure whether the lack of code is common across all review batches or specific to their assigned papers.

reddit · r/MachineLearning · /u/wontonut · Aug 11, 18:58

**Background**: AAAI is a major artificial intelligence conference that has been explicit about emphasizing reproducibility. The Reddit post reflects an ongoing debate in the machine learning community about whether code submission should be a required part of the review process.

**Tags**: `#reproducibility`, `#AAAI`, `#peer review`, `#code submission`, `#machine learning`

---

<a id="item-20"></a>
## [Developer Rebuilds Spiking Language Model NORD Around CPU-First Inference](https://www.reddit.com/r/MachineLearning/comments/1vlrajq/continued_development_of_the_model_based_on_the/) ⭐️ 6.0/10

After a six-month hiatus, the developer of Project NORD announced NORD 5.5 'Flash,' a rebuild of their spiking language model designed for CPU-first inference. The new architecture replaces the artificial spike-time dimension with the actual token sequence as the time axis and removes quadratic attention from the main inference path. This project demonstrates a niche but interesting alternative to Transformer-based language models, potentially enabling low-power, CPU-only inference for long sequences. If successful, it could contribute to the broader research on spiking neural networks and efficient language model architectures. The design includes strictly causal processing, causal convolution-style token mixing, token-time LIF/event dynamics, a top-1 sparse MoE with a shared expert, and persistent recurrent memory banks. The developer also plans to benchmark NORD 5.0 against 5.5 on CPU tokens/sec, RAM usage, perplexity, and long-context behavior.

reddit · r/MachineLearning · /u/zemondza · Aug 11, 19:25

**Background**: Spiking neural networks (SNNs) are brain-inspired models that communicate via discrete spikes, offering potential energy efficiency and sparse computation. Transformers, which dominate NLP, have a quadratic attention bottleneck that limits long-context scaling; alternatives like linear attention, RWKV, and state-space models aim to address this. NORD 5.5 combines SNN principles with recurrent memory and sparse MoE to explore a CPU-first, event-driven architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2510.05364v1">The End of Transformers? On Challenging Attention and the ...</a></li>
<li><a href="https://github.com/gtausa197-svg/-Project-Nord-Spiking-Neural-Network-Language-Model">GitHub - gtausa197-svg/-Project-Nord- Spiking - Neural - Network ...</a></li>

</ul>
</details>

**Tags**: `#spiking neural networks`, `#language model`, `#CPU inference`, `#architecture`

---

<a id="item-21"></a>
## [Seeking RL and Planning Guidance for Stochastic Merge Puzzle with Previewed Chance Events](https://www.reddit.com/r/MachineLearning/comments/1vlfavg/planningrl_for_a_stochastic_singleplayer_merge/) ⭐️ 6.0/10

A developer shared a detailed spec of a stochastic single-player merge puzzle and asked the community for algorithms, papers, and implementations for planning and reinforcement learning. The game resembles 2048 with afterstates and previewed chance events, but adds 30 actions, stack constraints, and a long-horizon throughput objective. This is a well-posed challenge at the intersection of afterstate RL, stochastic planning, and resource-constrained search, so it can inform game-AI design for 2048-like titles and real-time planning systems. Responses could also clarify how previewed randomness changes the trade-off between learned value estimates and lookahead in small, exact simulators. The board has six stacks of height at most seven; an action moves the complete contiguous run of equal top tiles from one source column to another, triggering merges. Every fourth action is preceded by a preview of six random tiles that arrive next, and the stated objectives are maximizing 9s per game and per 30-minute session.

reddit · r/MachineLearning · /u/CaiwenGong · Aug 11, 11:53

**Background**: In reinforcement learning, an afterstate is the deterministic result of taking an action before the environment's stochastic outcome is applied; value functions over afterstates can be much easier to learn than over full state-action pairs. This concept is emphasized in standard references such as Sutton and Barto's textbook. Stochastic games introduce chance events, and when such events are previewed, the player can plan almost as if the next transition were deterministic, reducing variance and improving search efficiency. Merge puzzles like 2048 combine smooth spatial reasoning with combinatorial action choices, making them a common testbed for game AI and planning algorithms.

<details><summary>References</summary>
<ul>
<li><a href="http://www.incompleteideas.net/book/the-book-2nd.html">Sutton & Barto Book: Reinforcement Learning : An Introduction</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stochastic_game">Stochastic game - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#reinforcement-learning`, `#planning`, `#game-ai`, `#stochastic-optimization`, `#merge-puzzle`

---