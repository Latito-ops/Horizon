---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 37 items, 18 important content pieces were selected

---

1. [Firefox compiled to WebAssembly runs inside another browser](#item-1) ⭐️ 9.0/10
2. [Inkling: Open-weights 975B MoE multimodal model from Thinking Machines Lab](#item-2) ⭐️ 9.0/10
3. [First atmosphere detected on rocky exoplanet in habitable zone](#item-3) ⭐️ 8.0/10
4. [Practical Tips for Running SQLite in Production](#item-4) ⭐️ 8.0/10
5. [Moonshot AI Releases Kimi K3, 2.8T Parameter Open-Weight Model](#item-5) ⭐️ 8.0/10
6. [GPT-5.6 Codex Bug Deletes Files in Full Access Mode](#item-6) ⭐️ 8.0/10
7. [Linus Torvalds: Linux is not anti-AI](#item-7) ⭐️ 8.0/10
8. [EU AI Act OpenRAG: Structured Corpus with BGE-M3 Embeddings](#item-8) ⭐️ 8.0/10
9. [Kaiser Nurses Critique AI and Surveillance Impacts](#item-9) ⭐️ 7.0/10
10. [Recurse Center Founder Thanks HN for 15 Years](#item-10) ⭐️ 7.0/10
11. [Zilog Z80 Celebrates 50th Anniversary with Community Nostalgia](#item-11) ⭐️ 7.0/10
12. [Stereo2Spatial: Open-Source Model Converts Stereo Music to Spatial Audio](#item-12) ⭐️ 7.0/10
13. [Prism Bug Leaks Paper During Compilation](#item-13) ⭐️ 7.0/10
14. [DABSN: A New Recurrent Language Model Seeks Collaborators](#item-14) ⭐️ 7.0/10
15. [ExTernD: Expanded-Rank Ternary Decomposition for LLM PTQ](#item-15) ⭐️ 7.0/10
16. [LLM Cliché Highlighter Tool](#item-16) ⭐️ 6.0/10
17. [Mermaid to ASCII Art Tool with WebAssembly and Color Support](#item-17) ⭐️ 6.0/10
18. [Rethinking AI Memory: From Facts to Reasoning Patterns](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Firefox compiled to WebAssembly runs inside another browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter has compiled the full Firefox/Gecko browser to WebAssembly using AI-assisted programming, allowing it to run inside another browser with all network traffic proxied via WebSocket using the Wisp protocol. This groundbreaking demonstration proves that even complex native applications like a full web browser can be compiled to WebAssembly, opening up new possibilities for browser-based emulation, sandboxing, and streaming of entire operating systems. The WebAssembly binary is 233MB (gecko.wasm) plus 18MB compressed assets, and the project reportedly consumed an estimated $25,000 in AI tokens but cost much less due to a subscription plan. All network requests flow through Puter's server via the Wisp protocol, with end-to-end encryption verified for HTTPS traffic.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (WASM) is a low-level binary instruction format that runs near-native speed in modern browsers, originally designed for performance-critical tasks. Compiling a full browser like Firefox to WASM is an enormous engineering challenge due to the large codebase and network requirements; Puter chose the single-process Gecko engine to simplify the port.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>
<li><a href="https://puter.com/app/puter-browser">Puter Browser</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion noted that the project's servers had to be scaled up to handle the traffic spike, highlighting both the technical interest and the practical challenges of such a demo. Overall sentiment was very positive, with amazement at the scale of the achievement.

**Tags**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Emulation`, `#WASM`

---

<a id="item-2"></a>
## [Inkling: Open-weights 975B MoE multimodal model from Thinking Machines Lab](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, a 975B total parameter (41B active) mixture-of-experts multimodal model under Apache-2.0 license, trained on 45 trillion tokens of text, images, audio, and video. As a large-scale open-weights model from a US lab, Inkling strengthens the open-source AI ecosystem and provides a strong base for fine-tuning, especially through their Tinker platform. It offers a competitive alternative to models from China and other open-weight initiatives. Inkling is not a frontier model but a strong base model for customization. The lab also plans to release Inkling-Small (276B total, 12B active) but it is still in testing. The model card and training data documentation are minimal, which may raise transparency concerns.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) is an architecture that activates only a subset of parameters per token, enabling large total parameter counts with efficient inference. Open-weights models release only the trained weights, not full training code or data, distinguishing them from fully open-source models. This release is part of a trend of increasingly large open-weights models from both US and Chinese labs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/mixture-of-experts-architecture-reshaping-how-frontier-ai-lbvrc">Mixture - of - Experts : the architecture reshaping how frontier AI...</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you've been told - Open Source Initiative</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#MoE`, `#multimodal`, `#machine learning`

---

<a id="item-3"></a>
## [First atmosphere detected on rocky exoplanet in habitable zone](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

JWST has detected an atmosphere on LHS 1140b, a rocky exoplanet located 48 light-years away in the habitable zone of its red dwarf star. This marks the first time an atmosphere has been confirmed on a rocky world in a habitable zone. This discovery is significant because it opens the door to studying atmospheres of potentially habitable rocky exoplanets, which is crucial for assessing habitability and searching for biosignatures. It also provides insights into planetary formation and evolution around red dwarfs. LHS 1140b is about 5.6 times Earth's mass and 70% larger in radius, placing it in the super-Earth category. The detection was made via transmission spectroscopy as the planet transits its star, and the community debate centers on whether it is truly Earth-like or a mini-Neptune with a thick atmosphere.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: Red dwarfs like LHS 1140 are smaller and cooler than the Sun, meaning their habitable zones are much closer. This proximity increases stellar activity and the risk of atmospheric stripping. Mini-Neptunes are planets with thick hydrogen-helium atmospheres, intermediate in size between Earth and Neptune.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mini-Neptune">Mini - Neptune - Wikipedia</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - Science@NASA</a></li>

</ul>
</details>

**Discussion**: Commenters debated whether LHS 1140b is Earth-like or a mini-Neptune, with one referencing an arXiv paper that rules out mini-Neptune via JWST emission spectroscopy. Others discussed implications for the Fermi paradox and proposed using solar lens telescopes for future observations.

**Tags**: `#exoplanets`, `#astronomy`, `#astrobiology`, `#JWST`, `#LHS 1140b`

---

<a id="item-4"></a>
## [Practical Tips for Running SQLite in Production](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 8.0/10

Julia Evans published a blog post sharing practical tips for running SQLite, including using the .expert command for index recommendations, backup strategies with compressed dumps, and batch deletion techniques. SQLite is widely used but often misconfigured in production; these tips help developers avoid common issues like slow queries and backup failures, improving reliability and performance. The .expert mode automatically suggests indexes based on SQL queries, and backup strategies include piping .dump to zstd with the --rsyncable flag for efficient incremental syncing. Deleting in batches or preloading rowids can mitigate locking issues.

hackernews · surprisetalk · Jul 17, 17:45 · [Discussion](https://news.ycombinator.com/item?id=48950122)

**Background**: SQLite is a self-contained, serverless SQL database engine that stores data in a single file. The .expert command is a CLI feature that analyzes queries and recommends indexes to improve performance. Write-Ahead Logging (WAL) mode allows concurrent reads during writes, making backups less disruptive.

**Discussion**: Community comments highlighted the .expert feature for index recommendations, a tool for scoped S3 credentials, and a backup pipeline using zstd with rsyncable compression. One user shared batch delete strategies, noting that SELECT preloading does not block writers.

**Tags**: `#SQLite`, `#databases`, `#backups`, `#SQL`, `#production`

---

<a id="item-5"></a>
## [Moonshot AI Releases Kimi K3, 2.8T Parameter Open-Weight Model](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 8.0/10

Moonshot AI announced Kimi K3, a 2.8 trillion parameter open-weight model, available via API and web with open weights promised by July 27, 2026. This is the largest open-weight model to date, surpassing DeepSeek's 1.6T model, and its high pricing signals a shift in the open model market; the pelican benchmark also reveals tokenization quirks like an 85-token hidden prompt. K3 uses 21% fewer output tokens than K2.6, costs $3/$15 per million input/output tokens, and leads the Frontend Code Arena; the pelican test showed an 85-token hidden system prompt due to tokenizer quirks.

rss · Simon Willison · Jul 16, 20:19 · [Discussion](https://news.ycombinator.com/item?id=48947717)

**Background**: The pelican benchmark is an informal test where Simon Willison asks LLMs to generate an SVG of a pelican riding a bicycle, used to compare model output quality and tokenization behavior. Moonshot AI is a Chinese AI lab that previously released Kimi K2.6.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/pelican-bicycle">GitHub - simonw/pelican-bicycle: LLM benchmark: Generate an SVG of a ...</a></li>
<li><a href="https://huggingface.co/spaces/victor/pelican-benchmark">Pelican Benchmark - a Hugging Face Space by victor</a></li>

</ul>
</details>

**Discussion**: Commenters questioned whether the pelican test is in the training set due to its popularity, noted the 85-token hidden prompt, and proposed more rigorous benchmarks like SWE-bench with pelican interruptions. Some also suggested running multiple tests per model for consistency.

**Tags**: `#AI`, `#LLM`, `#benchmarks`, `#open source`, `#model release`

---

<a id="item-6"></a>
## [GPT-5.6 Codex Bug Deletes Files in Full Access Mode](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

A bug in GPT-5.6's Codex tool causes accidental deletion of files when the model attempts to override the $HOME environment variable in full access mode without sandboxing protections. This highlights a critical safety risk in AI coding agents, particularly when granting elevated permissions, and underscores the need for sandboxing and auto-review safeguards. The bug occurs when full access mode is enabled, Codex runs without sandboxing and auto-review, the model tries to set a temporary directory via $HOME override, but mistakenly deletes $HOME instead.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is an AI coding agent from OpenAI that can execute commands on a user's machine. Full access mode allows Codex to perform actions without step-by-step approval, while sandboxing and auto-review modes provide safety layers. The $HOME environment variable typically points to the user's home directory, and its accidental deletion can cause significant data loss.

<details><summary>References</summary>
<ul>
<li><a href="https://vladimirsiedykh.com/blog/codex-cli-approval-modes-2025">Codex CLI approval modes explained: auto vs read only vs...</a></li>
<li><a href="https://alignment.openai.com/auto-review/">Auto-review of agent actions without synchronous human oversight</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>

</ul>
</details>

**Tags**: `#codex`, `#gpt`, `#ai-safety`, `#file-deletion`, `#coding-agents`

---

<a id="item-7"></a>
## [Linus Torvalds: Linux is not anti-AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds publicly declared on the Linux Media mailing list that Linux is not an anti-AI project, stating that AI tools are clearly useful and challenging dissenting developers to fork or leave. As Linux's creator and top maintainer, Torvalds' authoritative endorsement of AI tools may shift the open-source community's stance on AI adoption, influencing thousands of contributors and downstream projects. The statement was posted in a thread on the Linux Media mailing list (lore.kernel.org) and references AI as a tool whose utility is no longer in question, while acknowledging other open questions about AI's economy.

rss · Simon Willison · Jul 16, 13:26

**Background**: Linus Torvalds is the creator and long-time maintainer of the Linux kernel, the core of countless operating systems. In recent years, the use of AI tools like GitHub Copilot in open-source development has sparked debate, with some developers opposing AI-generated code due to licensing or ethical concerns. Torvalds' direct intervention signals a strong pro-AI direction for the Linux project.

**Tags**: `#linux`, `#linus torvalds`, `#ai`, `#open source`, `#kernel development`

---

<a id="item-8"></a>
## [EU AI Act OpenRAG: Structured Corpus with BGE-M3 Embeddings](https://www.reddit.com/r/MachineLearning/comments/1uytlac/eu_ai_act_openrag_933_legally_structured_chunks/) ⭐️ 8.0/10

The author released EU AI Act OpenRAG, a downloadable SQLite corpus containing 933 legally structured chunks of the EU AI Act, each with a normalized 1024-dimensional BGE-M3 embedding. Retrieval evaluations show improved performance over baseline, with article recall@20 of 0.541 vs 0.449 and QA hit@10 of 0.927 vs 0.898. This resource provides a high-quality, legally-grounded corpus for developing and evaluating RAG systems in the legal domain, particularly for EU AI Act compliance. Its structured chunking and embedding approach could improve legal NLP tasks like article retrieval and question answering. The corpus chunks are based on the regulation's legal structure (articles, recitals, definitions, annex points) rather than sliding windows, and include EUR-Lex links and application-date metadata. The author published evaluation results, limitations, and methodology transparently, encouraging technical feedback.

reddit · r/MachineLearning · /u/Automatic-Forever-63 · Jul 17, 08:18

**Background**: The EU AI Act (Regulation 2024/1689) is a landmark European law regulating artificial intelligence. Retrieval-Augmented Generation (RAG) systems combine retrieval of relevant documents with a language model to generate answers. BGE-M3 is a multilingual embedding model supporting dense, sparse, and multi-vector retrieval. EUR-Lex is the official EU law database.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/BAAI/bge-m3">BAAI/bge-m3 · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/EUR-Lex">EUR - Lex - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2603.09435">AI Act Evaluation Benchmark: An Open, Transparent, and Reproducible ...</a></li>

</ul>
</details>

**Tags**: `#AI Act`, `#legal-NLP`, `#RAG`, `#embeddings`, `#corpus`

---

<a id="item-9"></a>
## [Kaiser Nurses Critique AI and Surveillance Impacts](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

Nurses at Kaiser Permanente report that AI tools and workplace surveillance are exacerbating job stress and compromising patient care, though some find value in medical LLMs. This debate highlights tensions between efficiency-driven technology and frontline care quality, potentially influencing how healthcare systems adopt AI and monitoring. The article centers on complaints about call center metrics and pressure to ration care, which some commenters say are misattributed to AI, while a pilot AI empathy tool was discontinued in 2024.

hackernews · gnabgib · Jul 17, 22:26 · [Discussion](https://news.ycombinator.com/item?id=48952880)

**Background**: Large language models (LLMs) are increasingly used in healthcare for tasks like summarizing notes and translating, aiming to reduce documentation burden. However, workplace surveillance technologies, such as location-tracking badges, have been criticized for increasing pressure on staff.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ai21.com/knowledge/llms-in-healthcare/">LLMs in Healthcare: Applications, Examples, & Benefits | AI21</a></li>
<li><a href="https://ssir.org/articles/entry/the_long_shadow_of_workplace_surveillance">How Workplace Surveillance Technology Harms Workers</a></li>
<li><a href="https://www.sfgate.com/news/bayarea/article/kaiser-nurses-technology-22344290.php">Kaiser nurses say technology is making jobs — and patient care...</a></li>

</ul>
</details>

**Discussion**: Commenters express mixed views: some clarify that the real issues are metrics and rationing, not AI, while others note that nurses find value in LLM tools for translation and note-taking. A nurse's personal anecdote highlights time savings and reduced stress.

**Tags**: `#AI in healthcare`, `#workplace surveillance`, `#nursing`, `#LLM tools`, `#ethics`

---

<a id="item-10"></a>
## [Recurse Center Founder Thanks HN for 15 Years](https://news.ycombinator.com/item?id=48949551) ⭐️ 7.0/10

The founder of Recurse Center publicly thanked Hacker News for its role in supporting the programming retreat over 15 years, noting that HN has been the second largest source of applicants after word of mouth. This reflection highlights the enduring impact of a community-driven programming retreat that has positively affected over 3,000 participants, and underscores the value of non-traditional, passion-driven projects in the tech ecosystem. The Recurse Center is a free, self-directed programming retreat founded by YC alumni after a failed startup idea, funded by a built-in recruiting agency where companies pay to hire alumni, without deducting from participants' salaries.

hackernews · nicholasjbs · Jul 17, 16:57

**Background**: The Recurse Center (formerly Hacker School) started in 2010 as a free, self-directed programming retreat where participants work on projects, contribute to open source, and help each other grow. It has no teachers or curriculum; instead, it emphasizes peer learning and a supportive environment. An initial HN post in 2012 helped it gain traction beyond the founders' personal networks.

**Discussion**: Comments express profound gratitude and personal transformation from former participants, who share fond memories of their time at RC and strongly recommend applying. Some discuss the unique free pricing model and social rules. Overall sentiment is overwhelmingly positive and nostalgic.

**Tags**: `#recurse-center`, `#hacker-news`, `#community`, `#programming-retreat`, `#milestone`

---

<a id="item-11"></a>
## [Zilog Z80 Celebrates 50th Anniversary with Community Nostalgia](https://goliath32.com/blog/z80.html) ⭐️ 7.0/10

The Zilog Z80 microprocessor, first released in July 1976, celebrated its 50th anniversary, with community members sharing memories and technical insights. The Z80 was a foundational component in early personal computers, game consoles, and embedded systems, influencing generations of programmers and engineers. The Z80 was designed by Federico Faggin and introduced in July 1976. It was binary compatible with Intel 8080 but added new registers and instructions, and it was used in systems like TRS-80, ZX Spectrum, and many arcade games.

hackernews · st_goliath · Jul 17, 19:41 · [Discussion](https://news.ycombinator.com/item?id=48951461)

**Background**: The Z80 is an 8-bit microprocessor known for its role in the personal computing revolution of the late 1970s and early 1980s. Its design allowed for easier system integration and greater performance than its predecessor, the Intel 8080, leading to widespread adoption in home computers and gaming consoles.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zilog_Z80">Zilog Z80</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zilog">Zilog - Wikipedia</a></li>
<li><a href="https://grokipedia.com/page/Zilog_Z80">Zilog Z80</a></li>

</ul>
</details>

**Discussion**: Commenters shared nostalgic experiences: one user recalled building a Z80 kit to learn digital electronics, another reflected on learning assembly from a ZX-81 manual, and a third expressed affection for the processor despite struggling with assembly language as a child.

**Tags**: `#Z80`, `#CPU`, `#history`, `#retrocomputing`, `#vintage tech`

---

<a id="item-12"></a>
## [Stereo2Spatial: Open-Source Model Converts Stereo Music to Spatial Audio](https://www.reddit.com/r/MachineLearning/comments/1uzevbg/stereo2spatial_convert_stereo_music_tracks_to/) ⭐️ 7.0/10

The author released Stereo2Spatial, a flow-matching diffusion model that converts stereo music tracks into spatialized binaural mixes, with both latent and waveform versions available under Apache 2.0 license. This tool democratizes access to high-quality spatial audio conversion, enabling creators and listeners to experience immersive sound without requiring specialized equipment or manual mixing, potentially accelerating adoption of spatial audio in music. The waveform version uses amplitude lifting from the WavFlow paper to stabilize training, and includes optional mix-style conditioning for controllable outputs; the latent version operates on EAR-VAE latent space but encountered quality bottlenecks.

reddit · r/MachineLearning · /u/kittenkrazy · Jul 17, 22:55

**Background**: Spatial audio (e.g., 7.1.4 surround) creates a three-dimensional sound field, while binaural audio simulates this for headphones using head-related transfer functions. Flow-matching diffusion is a generative model that learns to transform noise into data by matching probability flows. Variational Autoencoders (VAEs) learn compressed latent representations of audio. The model was trained on 7,669 tracks for 20 days on two A6000 GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Eps-Acoustic-Revolution-Lab/EAR_VAE">GitHub - Eps-Acoustic-Revolution-Lab/EAR_VAE: This is the ...</a></li>
<li><a href="https://arxiv.org/abs/2509.14912">[2509.14912] Back to Ear: Perceptually Driven High Fidelity ... ϵar-VAE Demo earlab/EAR_VAE at main - Hugging Face EAR_VAE/docs/index.html at main · Eps-Acoustic ... - GitHub Back to Ear: Perceptually Driven High Fidelity Music ...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#audio processing`, `#spatial audio`, `#diffusion models`, `#VAE`

---

<a id="item-13"></a>
## [Prism Bug Leaks Paper During Compilation](https://www.reddit.com/r/MachineLearning/comments/1uz75qt/prism_accidentally_leaked_d/) ⭐️ 7.0/10

A bug on the Prism platform caused someone else's paper to be returned during compilation, resulting in an accidental paper leak. The platform was taken down within 10 minutes of being flagged. This incident underscores serious privacy risks in collaborative ML platforms, where leaked papers can compromise double-blind review or intellectual property. The quick response shows good practice, but users remain concerned about their own papers' security. The bug was first reported on Twitter, and Prism's website was taken down within 10 minutes. Users are worried that their own papers may have been exposed as well.

reddit · r/MachineLearning · /u/Few-Monitor5103 · Jul 17, 17:59

**Background**: Prism is a platform used in the machine learning community for compiling papers, likely for tools like LaTeX or formatting. Accidental leaks during compilation can expose unpublished work, which is critical during blind review processes.

**Tags**: `#machine learning`, `#privacy`, `#paper leak`, `#Prism`, `#bug`

---

<a id="item-14"></a>
## [DABSN: A New Recurrent Language Model Seeks Collaborators](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 7.0/10

The author introduces DABSN, a novel recurrent architecture, and releases a preprint with open-source code (PyTorch, C++, Triton). A 24M parameter language model trained on 1B tokens shows promising results, and the author seeks collaborators for scaling and independent evaluation. DABSN could challenge the dominance of transformers in language modeling, especially for long-context tasks, by offering efficient recurrent computation. Open collaboration may accelerate its validation and adoption. The architecture was evaluated on benchmarks including MQAR, Copy, Key-Value retrieval, and A5/60. The codebase includes custom Triton kernels for GPU efficiency. The author trained a 24M parameter model with a GPT-2 tokenizer on 1B tokens.

reddit · r/MachineLearning · /u/BleedingXiko · Jul 16, 19:17

**Background**: Recurrent neural networks (RNNs) were once dominant for sequence modeling but were overshadowed by transformers. Recently, state-space models (e.g., Mamba) and other recurrent variants have regained interest for their linear-time inference. MQAR (Multi-Query Associative Recall) benchmarks a model's ability to perform multiple associative lookups from context. Triton is a Python-based language for writing efficient GPU kernels.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/multi-query-associative-recall-mqar">MQAR: Multi-Query Associative Recall - emergentmind.com</a></li>
<li><a href="https://triton-lang.org/main/">Welcome to Triton ’s documentation! — Triton documentation</a></li>

</ul>
</details>

**Tags**: `#recurrent neural networks`, `#language modeling`, `#deep learning`, `#open source`, `#collaboration`

---

<a id="item-15"></a>
## [ExTernD: Expanded-Rank Ternary Decomposition for LLM PTQ](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 7.0/10

Researchers propose ExTernD, a post-training ternary decomposition method that expands the inner rank of weight matrix factorization beyond full rank, enabling accuracy that approaches any target quantization level with only a modest increase in VRAM. This addresses a fundamental limitation of fixed-size ternary quantization in large language models (LLMs), offering a path to extremely low-bit quantization (e.g., 2-bit equivalent) without catastrophic accuracy loss, which could dramatically reduce memory and inference costs for LLM deployment. ExTernD decomposes each weight matrix A into B·diag(D)·C, where B and C are ternary matrices with entries in {-1, 0, +1}, and D is a real scale vector. The inner rank k is set to mu*min(m,n) with mu>1, allowing components beyond full rank to correct quantization errors. The method uses Shannon entropy to fairly compare bits-per-weight with other methods.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Post-training quantization (PTQ) reduces model size and speeds up inference by converting pre-trained weights into lower-precision formats without retraining. Ternary quantization restricts weights to -1, 0, +1, offering extreme compression but often causing accuracy drops. ExTernD builds on matrix factorization approaches like SVD but uses ternary factors and an expanded rank to better preserve accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.13511">[2607.13511] ExTernD: Expanded-Rank Ternary Decomposition ...</a></li>
<li><a href="https://arxiv.org/html/2607.13511v1">ExTernD: Expanded-Rank Ternary Decomposition Ternary LLM PTQ ...</a></li>

</ul>
</details>

**Tags**: `#LLM quantization`, `#ternary decomposition`, `#post-training quantization`, `#model compression`, `#machine learning`

---

<a id="item-16"></a>
## [LLM Cliché Highlighter Tool](https://simonwillison.net/2026/Jul/17/llm-cliche-highlighter/#atom-everything) ⭐️ 6.0/10

Simon Willison created a web tool that highlights ten common clichés found in LLM-generated writing, built using AI-assisted vibe coding via Fable 5. This tool helps readers and content curators quickly identify AI writing patterns, promoting more critical consumption of AI-generated content and potentially reducing the spread of generic, cliché-ridden text. The highlighter can load and analyze any URL via Jina AI's reader service, and it currently flags 11 patterns (including 'is real and', 'worth naming') with a clear match count per sentence.

rss · Simon Willison · Jul 17, 12:11

**Background**: LLMs often reuse formulaic phrases and clichés, making their output recognizable. Vibe coding is a term coined by Andrej Karpathy in 2025, describing development where AI generates code from natural language prompts, often accepted without thorough review.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>
<li><a href="https://jina.ai/about-us/">About Jina AI</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#AI detection`, `#writing`, `#clichés`, `#tools`

---

<a id="item-17"></a>
## [Mermaid to ASCII Art Tool with WebAssembly and Color Support](https://simonwillison.net/2026/Jul/16/mermaid-ascii/#atom-everything) ⭐️ 6.0/10

Simon Willison compiled the Go library AlexanderGrooff/mermaid-ascii to WebAssembly, creating a browser-based tool that converts Mermaid diagrams into colorful ASCII art. This tool makes Mermaid diagrams accessible in plain-text environments like terminals or code comments, while the WebAssembly approach allows complex Go-based rendering to run efficiently in the browser without a server. The Go library supports colors in ASCII output, which the earlier Rust-based implementation lacked, and the WebAssembly compilation enables interactive adjustments like padding and box padding.

rss · Simon Willison · Jul 16, 14:57

**Background**: Mermaid is an open-source JavaScript-based diagramming tool that generates diagrams from text descriptions. WebAssembly (Wasm) is a portable binary format that allows high-performance code from languages like Go or Rust to run in web browsers, enabling serverless execution.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mermaid_(software)">Mermaid (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>

</ul>
</details>

**Tags**: `#mermaid`, `#ascii-art`, `#webassembly`, `#developer-tools`

---

<a id="item-18"></a>
## [Rethinking AI Memory: From Facts to Reasoning Patterns](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 6.0/10

A Reddit post proposes that AI memory systems should evolve from storing descriptive facts to inferring higher-level reasoning patterns such as explanatory frameworks and reasoning styles. This would transform persistent context from a collection of notes into an evolving model of how a user understands problems. This conceptual shift could influence future AI architectures to focus on modeling user reasoning styles, enabling more personalized and adaptive AI interactions. It challenges the prevailing emphasis on factual recall in current memory systems. The post contrasts descriptive memory (e.g., 'user likes economics') with inferential memory (e.g., 'user explains economics via incentives'). It questions whether such representations can emerge naturally from sufficiently capable AI systems or require fundamentally different architectures than today's retrieval and summarization methods.

reddit · r/MachineLearning · /u/Boris_Ljevar · Jul 16, 16:00

**Background**: Current AI agents maintain persistent context through saved memories, conversation summaries, user preferences, and project notes, which are primarily descriptive. Frameworks like Mem0, Zep, and Letta aim to improve this with richer context. The post suggests a further evolution: instead of just remembering facts, systems could infer higher-level patterns such as explanatory frameworks and reasoning styles, effectively building an evolving model of how a user interprets problems.

<details><summary>References</summary>
<ul>
<li><a href="https://vectorize.io/articles/best-ai-agent-memory-systems">Best AI Agent Memory Systems in 2026: 8 Frameworks Compared</a></li>
<li><a href="https://aiagentmemory.org/articles/ai-memory-frameworks/">AI Memory Frameworks: Building Persistent Recall for …</a></li>

</ul>
</details>

**Tags**: `#AI memory`, `#persistent context`, `#machine learning`, `#reasoning patterns`, `#abstraction`

---