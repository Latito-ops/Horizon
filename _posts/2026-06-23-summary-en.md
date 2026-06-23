---
layout: default
title: "Horizon Summary: 2026-06-23 (EN)"
date: 2026-06-23
lang: en
---

> From 32 items, 15 important content pieces were selected

---

1. [Steam Machine Launches with Fair Reservation System](#item-1) ⭐️ 9.0/10
2. [Moebius: 0.2B Parameter Model Challenges 10B-Level Performance](#item-2) ⭐️ 8.0/10
3. [Role Confusion Revealed as Root Cause of Prompt Injection](#item-3) ⭐️ 8.0/10
4. [Porting Moebius 0.2B image inpainting to browser with WebGPU](#item-4) ⭐️ 8.0/10
5. [New Benchmark Hides Juliet Cases to Test LLM Vulnerability Detection](#item-5) ⭐️ 8.0/10
6. [GLM-5.2 Local Inference: High Hardware Demands and Trade-offs](#item-6) ⭐️ 7.0/10
7. [Oak: A Git alternative built for AI agents](#item-7) ⭐️ 7.0/10
8. [Canada plans up to 10 nuclear reactors by 2040](#item-8) ⭐️ 7.0/10
9. [sqlite-utils 4.0rc1 adds migrations and nested transactions](#item-9) ⭐️ 7.0/10
10. [Cloudflare Launches Temporary Accounts for 60-Minute Deployments](#item-10) ⭐️ 7.0/10
11. [Hugging Face revives Papers with Code with new features](#item-11) ⭐️ 7.0/10
12. [MRU Update: Addressing Instability and Introducing Parallel Scan](#item-12) ⭐️ 7.0/10
13. [Seeking syntax-robust NLI for evaluating diffusion LLMs](#item-13) ⭐️ 6.0/10
14. [Improved DVD-JEPA demo shows JEPA's noise robustness](#item-14) ⭐️ 6.0/10
15. [Seeking Papers on EMA for LoRA Adapters in Self-Distillation](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Steam Machine Launches with Fair Reservation System](https://store.steampowered.com/news/group/45479024/view/685257114654870245) ⭐️ 9.0/10

Valve officially launched the Steam Machine gaming hardware today, featuring a randomized reservation system to combat bots and scalpers. The device is powered by a semi-custom AMD Zen 4 CPU and RDNA 4 graphics, offering over six times the performance of the Steam Deck. This launch marks Valve's return to dedicated gaming hardware with an open platform, emphasizing user freedom to install any OS or apps. It challenges traditional consoles by combining PC flexibility with a console-like experience, potentially reshaping the gaming hardware market. The Steam Machine uses a fair reservation system that accepts sign-ups over several days without rewarding early registrations. Pricing is directly tied to component costs, and the device is optimized for gaming but remains a fully open PC.

hackernews · theschwa · Jun 22, 17:09 · [Discussion](https://news.ycombinator.com/item?id=48632884)

**Background**: The Steam Machine is Valve's latest gaming hardware, following the Steam Deck handheld. Unlike traditional consoles, it runs SteamOS and allows users to install other operating systems or apps. The unit features a semi-custom AMD CPU and GPU, targeting high-end PC gaming in a living room form factor.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Steam_Machine">Steam Machine - Wikipedia</a></li>
<li><a href="https://www.lttlabs.com/articles/2026/06/22/the-newell-nucleus-steam-machine-ltt-companion-article">The Newell Nucleus: Steam Machine LTT Companion Article | LTT Labs</a></li>
<li><a href="https://store.steampowered.com/hardware/steammachine">Steam Machine</a></li>

</ul>
</details>

**Discussion**: Community comments praised the fair reservation system for reducing scalper advantage and highlighted the openness of the platform as a key selling point. Some users found the pricing and specs underwhelming but appreciated Valve's transparency. A humorous video clip on the store page also drew positive reactions.

**Tags**: `#Steam Machine`, `#Valve`, `#gaming hardware`, `#open platform`, `#product launch`

---

<a id="item-2"></a>
## [Moebius: 0.2B Parameter Model Challenges 10B-Level Performance](https://hustvl.github.io/Moebius/) ⭐️ 8.0/10

Moebius, a 0.2B parameter image inpainting model, claims to achieve performance comparable to 10B parameter models. A community contributor built a browser demo using ONNX, demonstrating the model's capabilities in real-time. This is significant because it suggests that with efficient architecture, small models can approach large model performance, potentially reducing computational costs for image inpainting tasks. It also sparked community debate about the validity of the performance claims. The model is limited to 512x512 output resolution, and some users observed visible artifacts in inpainted regions compared to the surroundings. The browser demo built by simonw requires a ~1.3GB download.

hackernews · DSemba · Jun 22, 13:53 · [Discussion](https://news.ycombinator.com/item?id=48630171)

**Background**: Image inpainting is a computer vision task that fills in missing or damaged parts of an image realistically. Moebius is a new model that aims to achieve high performance with very few parameters, using techniques like efficient transformers or convolutions. ONNX (Open Neural Network Exchange) is an open standard for representing machine learning models, enabling cross-platform deployment such as in a browser via ONNX Runtime.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ONNX">ONNX</a></li>

</ul>
</details>

**Discussion**: Simonw successfully ported the model to ONNX and created a browser demo, sharing code and a transcript. Lifthrasiir tested the model and found it impressive for its size but noted visible artifacts and limitations to 512x512, doubting it matches 10B models. Another user, chatmasta, asked for a definition of inpainting, indicating the term is not universally understood.

**Tags**: `#image inpainting`, `#small model`, `#performance claims`, `#ONNX`, `#web demo`

---

<a id="item-3"></a>
## [Role Confusion Revealed as Root Cause of Prompt Injection](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

Researchers have discovered that LLMs prioritize the stylistic sound of text over role tags, enabling prompt injection attacks; a technique called 'destyling' reduces attack success from 61% to 10% by rewriting text to look less like system or assistant roles. This work reveals a fundamental security flaw in LLMs that cannot be fixed with current defense methods, warning that injection defense will remain a 'perpetual whack-a-mole game' unless models achieve genuine role perception. The paper uses role probes to measure how LLMs internally perceive source, finding that role confusion predicts attack success before any token is generated; models like gpt-oss-20b can be jailbroken by appending text that mimics the style of internal thinking blocks.

rss · Simon Willison · Jun 22, 23:59

**Background**: Prompt injection attacks occur when an LLM is tricked into following instructions from untrusted user input, overriding its system instructions. Role tags like <system>, <user>, and <assistant> are used to mark different parts of the input, but this research shows that models infer authority from the style of the text rather than these tags, leading to role confusion.

<details><summary>References</summary>
<ul>
<li><a href="https://role-confusion.github.io/">Prompt Injection as Role Confusion</a></li>
<li><a href="https://arxiv.org/abs/2603.12277">[2603.12277] Prompt Injection as Role Confusion - arXiv.org Prompt Injection as Role Confusion - arXiv.org Prompt Injection as Role Confusion: Unmasking the Deeper Flaw ... [Paper Note] Prompt Injection as Role Confusion role-confusion/prompt-injection-as-role-confusion | DeepWiki Prompt Injection as Role Confusion - GitHub</a></li>
<li><a href="https://arxiv.org/html/2603.12277v5">Prompt Injection as Role Confusion - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#prompt injection`, `#LLM security`, `#AI safety`, `#role confusion`

---

<a id="item-4"></a>
## [Porting Moebius 0.2B image inpainting to browser with WebGPU](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison successfully ported the Moebius 0.2B lightweight image inpainting model to run entirely in a web browser using WebGPU, creating a working demo at simonw.github.io/moebius-web/. This demonstrates that image inpainting models can run efficiently in-browser without requiring dedicated GPU hardware, lowering the barrier for users to experiment with AI image editing tools directly from their browser. Willison used Claude Code to assist with the porting process, leveraging ONNX Runtime Web with the WebGPU backend to convert the PyTorch model, which originally required NVIDIA CUDA, into a browser-compatible format.

rss · Simon Willison · Jun 22, 23:43

**Background**: Moebius is a lightweight image inpainting framework with only 0.2 billion parameters, yet it claims performance comparable to 10-billion-parameter models. It uses a Latent Diffusion Model (LDM) with Latent Categories Guidance (LCG). The original implementation required PyTorch and NVIDIA CUDA, limiting its accessibility.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/22/porting-moebius/">Porting the Moebius 0.2B image inpainting model to run in the ...</a></li>
<li><a href="https://hustvl.github.io/Moebius/">Moebius: 0.2 B Lightweight Image Inpainting Framework with 10B ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebGPU">WebGPU</a></li>

</ul>
</details>

**Tags**: `#image inpainting`, `#WebGPU`, `#machine learning`, `#browser AI`, `#computer vision`

---

<a id="item-5"></a>
## [New Benchmark Hides Juliet Cases to Test LLM Vulnerability Detection](https://www.reddit.com/r/MachineLearning/comments/1ud0rft/nondeterministic_vulnerability_detection/) ⭐️ 8.0/10

A Reddit user proposes a non-deterministic vulnerability detection benchmark that disguises Juliet test cases to resemble real code and injects adversarial comments, aiming to evaluate LLM robustness in identifying CWEs. This benchmark addresses a critical gap in evaluating LLM-based vulnerability detection by removing the natural advantage LLMs have when viewing known test cases, and by testing the impact of adversarial comments, which can mislead models in real-world scenarios. The benchmark uses hundreds of CWEs from the Juliet test suite, hides them to avoid recognition, and adds accurate, misleading, or neutral comments via an LLM. It is about 80% complete and needs presentation polish, actual benchmarking of publish LLMs, and possible pruning of CWEs that may still be identified as Juliet code.

reddit · r/MachineLearning · /u/Psychological_Meat_6 · Jun 22, 23:34

**Background**: The Juliet test suite is a widely used set of synthetic C/C++ test cases with known vulnerabilities (CWEs) for evaluating static analysis tools. Recent research has explored adversarial comments that can mislead LLMs during code analysis, such as authority spoofing and technical deception. This benchmark combines both concepts to create a more realistic evaluation for LLM-based vulnerability detection.

<details><summary>References</summary>
<ul>
<li><a href="https://www.researchgate.net/figure/Experimental-results-for-vulnerability-discovery-on-the-Juliet-test-suite_fig3_352889408">Experimental results for vulnerability discovery on the Juliet test suite | Download Scientific Diagram</a></li>
<li><a href="https://arxiv.org/abs/2602.16741">[2602.16741] Can Adversarial Code Comments Fool AI Security Reviewers -- Large-Scale Empirical Study of Comment-Based Attacks and Defenses Against LLM Code Analysis</a></li>

</ul>
</details>

**Tags**: `#vulnerability detection`, `#LLM`, `#benchmarking`, `#cybersecurity`, `#adversarial robustness`

---

<a id="item-6"></a>
## [GLM-5.2 Local Inference: High Hardware Demands and Trade-offs](https://unsloth.ai/docs/models/glm-5.2) ⭐️ 7.0/10

A Hacker News discussion reveals that running the open-weight GLM-5.2 model locally requires at least 256GB of RAM and 24GB VRAM (for a single 3090 GPU), with real-world token generation speeds around 6 tok/s on a budget system using llama.cpp with MoE offloading. The model is a 685B-parameter Mixture-of-Experts model that sets new benchmarks but demands expensive hardware for reasonable performance. This discussion highlights the practical barriers to running state-of-the-art open-weight LLMs locally, which is crucial for privacy-sensitive users and developers wanting to avoid API costs. The hardware requirements for GLM-5.2 remain prohibitive for most individuals, contrasting with smaller models that run on consumer hardware, and underscore the ongoing need for better quantization and efficient inference techniques. Users report that with 512GB RAM and two 3090 GPUs running llama.cpp with -cmoe flag, they achieve ~6 tok/s on DDR4-2400 MHz, potentially increasing to ~9 tok/s with faster RAM. The model's prompt processing speed is significantly slower on CPU offloading, making it unusable without $50k+ in GPUs for acceptable prompt throughput. Quantization (e.g., Q4_K_XL) is required to fit the model into available memory.

hackernews · TechTechTech · Jun 22, 21:21 · [Discussion](https://news.ycombinator.com/item?id=48636377)

**Background**: GLM-5.2 is a 685B-parameter Mixture-of-Experts (MoE) model developed by Z.AI (previously Zhipu AI), released as open-weight. It has achieved top scores on design benchmarks and is competitive with leading proprietary models. Local inference of large LLMs often requires quantization—a technique that reduces numerical precision of weights to lower memory usage—and hardware like high-RAM workstations or clusters of GPUs to run at acceptable speeds. llama.cpp is a popular inference tool that supports MoE offloading across CPU and GPU.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/technology/comments/1uc5hjh/what_is_glm52_another_opensource_chinese_ai_model/">r/technology on Reddit: What is GLM-5.2? Another open-source Chinese AI model has Silicon Valley's attention.</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM-5.2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-glm-5-2-open-weight-model">What Is GLM 5.2? The Open-Weight Model Beating GPT 5.5 on Design Benchmarks | MindStudio</a></li>

</ul>
</details>

**Discussion**: Commenters share real-world benchmarks and hardware configurations, with some expressing regret for not investing in higher-end setups. One user notes that while 256GB RAM is the minimum, prompt processing is 20-50x slower on CPU-only setups, making the model impractical without heavy GPU investment. Another commenter is optimistic about future hardware like Nvidia GB10 clusters enabling easier local deployment.

**Tags**: `#GLM-5.2`, `#local inference`, `#LLM deployment`, `#hardware requirements`, `#quantization`

---

<a id="item-7"></a>
## [Oak: A Git alternative built for AI agents](https://oak.space/oak/oak) ⭐️ 7.0/10

Oak is a new open-source version control system designed specifically for AI agents, featuring virtual mounts that allow agents to work on repositories without downloading a full copy, and claiming up to 95% faster snapshots than Git. As AI agents become more integrated into software development, traditional version control systems like Git present bottlenecks in speed and context overhead. Oak aims to address these inefficiencies, potentially enabling agents to work in parallel on multiple tasks with reduced resource usage and faster iteration. Oak is still in early development, missing features like CI, issues, and comments, and currently only supports Linux and macOS (no Windows build). It is written in Rust and uses a Cargo workspace, with its own repository hosted on Oak itself, bootstrapped without Git backup.

hackernews · zdgeier · Jun 22, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48631726)

**Background**: Version control systems (VCS) like Git track changes to files over time, enabling collaboration and history management. AI agents often use Git for coding tasks, but they must clone entire repositories and maintain context, which can be slow and token-intensive. Oak introduces virtual mounts, a concept similar to Google's google3 workspace or Microsoft's VFS for Git, allowing on-demand file access without full cloning.

<details><summary>References</summary>
<ul>
<li><a href="https://oak.space/">Oak — Branch freely · oak</a></li>
<li><a href="https://github.com/mbrukman/oakdotspace-oak">GitHub - mbrukman/oakdotspace-oak: https://oak.space/oak/oak</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_version-control_software">List of version-control software - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion shows mixed sentiment: some users are skeptical about the need for a new VCS given the established Git ecosystem, while others are intrigued by the lazy mount approach and see potential for agent workflows. A commenter noted that Oak's virtual mounts are reminiscent of Google's internal system, suggesting room for such ideas even within Git.

**Tags**: `#version-control`, `#AI-agents`, `#git-alternative`

---

<a id="item-8"></a>
## [Canada plans up to 10 nuclear reactors by 2040](https://www.cbc.ca/news/politics/federal-nuclear-strategy-9.7244509) ⭐️ 7.0/10

Canada has announced a federal nuclear strategy aiming to build up to 10 nuclear reactors by 2040, leveraging its abundant uranium reserves and homegrown CANDU reactor technology. This plan could significantly reshape Canada's energy mix by providing reliable baseload power to complement renewables, reduce dependence on foreign uranium enrichment (especially from Russia), and position Canada as a global leader in nuclear technology exports. The strategy calls for construction to start on two new large-scale reactors by 2035, five more to be planned or under development by 2040, and at least one reactor to be under construction outside Ontario by 2035.

hackernews · geox · Jun 22, 19:06 · [Discussion](https://news.ycombinator.com/item?id=48634585)

**Background**: CANDU (Canada Deuterium Uranium) reactors are a Canadian-designed pressurized heavy-water reactor that uses natural uranium as fuel and heavy water as a neutron moderator, unlike most reactors that require enriched uranium. Canada possesses some of the largest uranium reserves in the world and has extensive experience with CANDU construction and refurbishment, such as at Darlington. The plan aims to provide stable baseload power to support the increasing share of intermittent solar and wind energy in provinces like Ontario.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CANDU_reactor">CANDU reactor - Wikipedia</a></li>
<li><a href="https://energyeducation.ca/encyclopedia/CANDU_reactor">CANDU reactor - Energy Education</a></li>

</ul>
</details>

**Discussion**: Comments generally support the plan but express skepticism about the timeline, noting that construction starting only by 2035 is too far away to be serious. Some highlight the strategic advantage of CANDU's use of natural uranium, which avoids reliance on Russian enriched uranium, while others question the lack of concrete details and urge a more aggressive schedule.

**Tags**: `#nuclear energy`, `#Canada`, `#energy policy`, `#CANDU`, `#infrastructure`

---

<a id="item-9"></a>
## [sqlite-utils 4.0rc1 adds migrations and nested transactions](https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/#atom-everything) ⭐️ 7.0/10

sqlite-utils 4.0rc1, the first release candidate of version 4.0, introduces built-in database migrations (ported from sqlite-migrate) and nested transactions via db.atomic(). This release also includes minor backwards-incompatible changes, prompting a major version bump. This update significantly enhances sqlite-utils for developers who rely on SQLite for data engineering and prototyping. The built-in migrations simplify schema evolution, while nested transactions improve error handling in complex workflows, making the library more robust for production use. Migrations support forward-only changes (no reverse migrations) and can be applied via Python API or CLI command sqlite-utils migrate. Nested transactions use SQLite's SAVEPOINT mechanism, allowing atomic blocks inside other transactions.

rss · Simon Willison · Jun 21, 23:35

**Background**: sqlite-utils is a Python library and CLI tool created by Simon Willison that provides high-level operations on SQLite databases, such as importing JSON and CSV, transforming tables, and running queries. Its popularity stems from simplifying common SQLite tasks for data analysis and application development.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>
<li><a href="https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/">sqlite-utils 4.0rc1 adds migrations and nested transactions</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#python`, `#database`, `#migrations`, `#cli`

---

<a id="item-10"></a>
## [Cloudflare Launches Temporary Accounts for 60-Minute Deployments](https://simonwillison.net/2026/Jun/21/temporary-cloudflare-accounts/#atom-everything) ⭐️ 7.0/10

Cloudflare has introduced temporary accounts that allow anyone to deploy a Workers project for 60 minutes using `npx wrangler deploy --temporary`, without signing up for an account. The feature is primarily aimed at AI agents but is available to all developers. This lowers the barrier to experimenting with Cloudflare Workers by eliminating the signup requirement, making it ideal for one-shot tasks, CI/CD pipelines, and AI agents. It reflects a growing trend toward ephemeral, frictionless developer experiences. Deployments receive a randomly generated project name and a unique workers.dev subdomain. Users can claim the account to extend the deployment beyond 60 minutes, via a claim link that expires in roughly 50 minutes.

rss · Simon Willison · Jun 21, 22:01

**Background**: Cloudflare Workers is a serverless computing platform that runs code on Cloudflare's global edge network. Wrangler is the official command-line tool for managing Workers projects. This new feature eliminates the need for prior account creation, streamlining the deployment process.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cloudflare.com/products/workers/">Cloudflare Workers - Global Serverless Functions Platform</a></li>
<li><a href="https://developers.cloudflare.com/workers/wrangler/">Wrangler · Cloudflare Workers docs</a></li>
<li><a href="https://developers.cloudflare.com/workers/">Overview · Cloudflare Workers docs</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (referenced in the article) likely contains reactions, but no specific comments are provided. The author Simon Willison notes the AI hook isn't necessary, implying the feature is broadly useful.

**Tags**: `#Cloudflare`, `#Workers`, `#serverless`, `#developer-tools`, `#ephemeral`

---

<a id="item-11"></a>
## [Hugging Face revives Papers with Code with new features](https://www.reddit.com/r/MachineLearning/comments/1ucm508/some_new_updates_to_papers_with_code_p/) ⭐️ 7.0/10

Hugging Face has added SOTA badges, a trending score that combines GitHub stars and Hugging Face artifact popularity, support for external (third-party) evaluations, and many new benchmarks to the revived Papers with Code platform. These updates make it easier for researchers to discover state-of-the-art papers and compare them across multiple evaluations, fostering collaboration and accelerating progress in machine learning research. The SOTA badge is displayed for papers ranking in the top 3 on a benchmark; the trending score now includes Hugging Face model, dataset, and Space velocity alongside GitHub stars; external evals enable viewing third-party benchmark results not introduced in the original paper.

reddit · r/MachineLearning · /u/NielsRogge · Jun 22, 14:29

**Background**: Papers with Code was originally a popular platform for linking academic papers to code implementations and benchmarks, but Meta shut it down in 2025. Hugging Face initiated a revival earlier in 2026, and this update brings back and enhances key features like SOTA badges and introduces a more comprehensive trending metric.

<details><summary>References</summary>
<ul>
<li><a href="https://paperswithcode.co/">Papers with Code</a></li>
<li><a href="https://www.linkedin.com/posts/niels-rogge-a3b7a3127_introducing-a-revival-of-paperswithcode-activity-7462137426585534464-3Vtl">Introducing a revival of PapersWithCode! One ... - LinkedIn</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#papers with code`, `#open source`, `#benchmarks`, `#hugging face`

---

<a id="item-12"></a>
## [MRU Update: Addressing Instability and Introducing Parallel Scan](https://www.reddit.com/r/MachineLearning/comments/1ubz5o8/an_update_on_matrix_recurrent_units_an_attention/) ⭐️ 7.0/10

The author presents improvements to their Matrix Recurrent Units (MRU) architecture, addressing training instability by experimenting with new methods to construct the input state matrix, and implementing an efficient parallel scan for hardware-friendly computation. This work explores an alternative to attention mechanisms for sequence modeling, offering a linear-time complexity approach. The findings on the importance of shear transformations over rotations could guide future designs of recurrent architectures. The author tested multiple input matrix construction methods, including orthogonal matrices via Cayley map and matrix exponential, LDU decomposition with determinant-one constraint, and QR factorization. The LDU method performed best, while forcing orthogonality led to poor performance, suggesting that shear transformations are critical.

reddit · r/MachineLearning · /u/mikayahlevi · Jun 21, 19:39

**Background**: Matrix Recurrent Units (MRU) are a novel linear-time sequence architecture that replaces attention by cumulatively multiplying input state matrices across the sequence dimension. The parallel scan algorithm exploits associativity to enable efficient computation on deep learning hardware. This update addresses earlier issues with training instability on larger datasets.

<details><summary>References</summary>
<ul>
<li><a href="https://towardsdatascience.com/the-math-behind-gated-recurrent-units-854d88aded65/">The Math Behind Gated Recurrent Units - Towards Data Science</a></li>
<li><a href="https://web.stanford.edu/~jurafsky/slp3/slides/rnnjan25.pdf">Simple Recurrent Networks (RNNs or Elman Nets) RNNs and LSTMs</a></li>
<li><a href="https://arxiv.org/pdf/2506.10918">Sequential-Parallel Duality in Prefix Scannable Models</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#recurrent neural networks`, `#sequence modeling`, `#attention alternatives`, `#linear-time architecture`

---

<a id="item-13"></a>
## [Seeking syntax-robust NLI for evaluating diffusion LLMs](https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/) ⭐️ 6.0/10

A Reddit user is requesting literature on syntax-robust Natural Language Inference (NLI) to evaluate the semantic correctness of text generated by diffusion language models, which often contain syntactic noise. This question identifies a gap in current evaluation methods for diffusion LLMs, which differ from autoregressive models. Developing syntax-robust NLI could improve assessment of these emerging models and guide future research. The user notes that autoregressive LLMs have been evaluated using NLI on sub-claims, but diffusion LLMs (except possibly LLaDA) struggle with syntactic correctness, complicating the use of NLI.

reddit · r/MachineLearning · /u/RepresentativeBee600 · Jun 22, 21:51

**Background**: Diffusion language models generate text by gradually denoising from random noise, enabling parallel generation but often causing syntactic errors. Natural Language Inference (NLI) determines if a hypothesis is entailed, contradicted, or neutral given a premise. Syntax-robust NLI would need to handle imperfect syntax while still assessing semantics.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/ProCreations/diffusion-language-model">Diffusion Language Models: The New Paradigm</a></li>
<li><a href="https://machinelearning.apple.com/research/latent-language-diffusion-model">Enhancing Paragraph Generation with a Latent Language Diffusion Model - Apple Machine Learning Research</a></li>
<li><a href="https://arxiv.org/abs/2502.09992">[2502.09992] Large Language Diffusion Models - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#NLI`, `#LLM`, `#diffusion models`, `#syntax robustness`, `#semantic evaluation`

---

<a id="item-14"></a>
## [Improved DVD-JEPA demo shows JEPA's noise robustness](https://www.reddit.com/r/MachineLearning/comments/1ubtf09/a_slightly_improved_dvdjepa_demo_p/) ⭐️ 6.0/10

A community fork of the original DVD-JEPA demo adds environment noise and a fair parameter-count comparison to a pixel-space baseline, more clearly illustrating JEPA's ability to ignore irrelevant details. This incremental improvement strengthens the empirical motivation for Joint Embedding Predictive Architectures (JEPA), a key self-supervised learning paradigm advocated by Yann LeCun, by directly demonstrating its advantage over pixel-based prediction. The demo uses roughly the same parameter count and compute budget for both the JEPA model and the pixel-space baseline to ensure fairness, and it removes the original web-demo and anomaly detection bits to focus on core JEPA principles.

reddit · r/MachineLearning · /u/Kirne · Jun 21, 15:49

**Background**: JEPA (Joint Embedding Predictive Architecture) learns by predicting masked-image representations in a latent space rather than reconstructing pixels, making it robust to unpredictable environmental details. The original demo lacked such noise and a fair baseline, which this improved version addresses.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@frinktyler1445/the-anatomy-of-jepa-the-architecture-behind-embedded-predictive-representation-learning-994bfa0bffe0">The Anatomy of JEPA: The Architecture Behind embedded Predictive Representation Learning | by Tyler Frink | Medium</a></li>
<li><a href="https://arxiv.org/abs/2301.08243">[2301.08243] Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture</a></li>
<li><a href="https://ai.meta.com/blog/yann-lecun-ai-model-i-jepa/">I-JEPA: The first AI model based on Yann LeCun’s vision for more human-like AI</a></li>

</ul>
</details>

**Tags**: `#JEPA`, `#representation learning`, `#self-supervised learning`, `#deep learning`

---

<a id="item-15"></a>
## [Seeking Papers on EMA for LoRA Adapters in Self-Distillation](https://www.reddit.com/r/MachineLearning/comments/1ubv0f5/ema_on_lora_r/) ⭐️ 6.0/10

A Reddit user asks for research papers that successfully use Exponential Moving Average (EMA) on LoRA adapters, where the EMA adapter acts as a self-teacher generating soft labels for the trainable adapter in an on-policy self-distillation setting. If successful, combining EMA with LoRA could enable efficient self-distillation in parameter-efficient fine-tuning, potentially improving model performance without the overhead of full fine-tuning. This could benefit applications with limited computational resources. The user references the On-Policy Self-Distillation (OPSD) paper but notes that OPSD uses full fine-tuning, not LoRA. The question implies interest in whether EMA on LoRA can produce a stable teacher for self-distillation, especially for low-rank adaptation (LoRA) models.

reddit · r/MachineLearning · /u/South-Conference-395 · Jun 21, 16:54

**Background**: Exponential Moving Average (EMA) is a technique that maintains a running average of model weights, often used to stabilize training or as a teacher in self-distillation. LoRA (Low-Rank Adaptation) is a parameter-efficient fine-tuning method that adds small trainable matrices to a frozen base model. Self-distillation is a process where a model learns from its own predictions, often with an EMA teacher. Combining EMA with LoRA could enable efficient on-policy self-distillation without full fine-tuning.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/huggingface/diffusers/issues/9998">EMA training for PEFT LoRAs · Issue #9998 · huggingface/diffusers</a></li>
<li><a href="https://github.com/huggingface/diffusers/issues/6505">[consistency distillation] LoRA scripts omits EMA update · Issue #6505 · huggingface/diffusers</a></li>
<li><a href="https://arxiv.org/abs/2601.18734">[2601.18734] Self-Distilled Reasoner: On-Policy Self-Distillation for Large Language Models</a></li>

</ul>
</details>

**Tags**: `#LoRA`, `#EMA`, `#knowledge-distillation`, `#fine-tuning`

---