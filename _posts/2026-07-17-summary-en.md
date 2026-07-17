---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 39 items, 29 important content pieces were selected

---

1. [Firefox in WebAssembly: Browser Inside Browser](#item-1) ⭐️ 10.0/10
2. [Kimi K3: 2.8 Trillion Parameter Open-Weight Model Announced](#item-2) ⭐️ 9.0/10
3. [Prompt Injection Attack Exfiltrates Claude User Memories](#item-3) ⭐️ 9.0/10
4. [Schema Harness Claims 99% on ARC-AGI-3 Without Weight Changes](#item-4) ⭐️ 9.0/10
5. [LM Studio Bionic: AI Agent for Open Models](#item-5) ⭐️ 8.0/10
6. [Rust-to-Zig Rewrite: Progress and Rationale](#item-6) ⭐️ 8.0/10
7. [GPT-5.6 Codex Bug Can Delete User Files](#item-7) ⭐️ 8.0/10
8. [Thinking Machines Lab Releases Inkling, a Large Open-Weights MoE Model](#item-8) ⭐️ 8.0/10
9. [xAI open-sources Grok Build after CLI privacy backlash](#item-9) ⭐️ 8.0/10
10. [ExTernD: Expanded-Rank Ternary Decomposition for LLM Quantization](#item-10) ⭐️ 8.0/10
11. [PnP-CoSMo: Plug-and-Play Multi-Contrast MRI Reconstruction](#item-11) ⭐️ 8.0/10
12. [Hadamard Product Technique Disentangles Convolutional Neurons](#item-12) ⭐️ 8.0/10
13. [Microsoft Comic Chat Open-Sourced](#item-13) ⭐️ 7.0/10
14. [Google Rebrands NotebookLM as Gemini Notebook](#item-14) ⭐️ 7.0/10
15. [Community Highlights Math Foundations in Data Science](#item-15) ⭐️ 7.0/10
16. [Detecting LLM-Generated Text with Classical Machine Learning](#item-16) ⭐️ 7.0/10
17. [Immersive Linear Algebra Book Revives Interest in Interactive Education](#item-17) ⭐️ 7.0/10
18. [Turn Golf Courses into Parks to Offset Water Use](#item-18) ⭐️ 7.0/10
19. [Linus Torvalds Declares Linux Not Anti-AI](#item-19) ⭐️ 7.0/10
20. [DABSN Recurrent Architecture Seeks Collaborators for Scaling](#item-20) ⭐️ 7.0/10
21. [Rethinking AI Memory: From Facts to Reasoning Patterns](#item-21) ⭐️ 7.0/10
22. [QLoRA 2e-4 Default Learning Rate Overfits Small Datasets](#item-22) ⭐️ 7.0/10
23. [Reddit Seeks Devil's Advocate on JEPA for Robot Learning](#item-23) ⭐️ 7.0/10
24. [170x PyTorch slowdown on T4 vs A100 baffles user](#item-24) ⭐️ 7.0/10
25. [uv 0.11.29 adds JSON tree, CUDA 13.2 support](#item-25) ⭐️ 6.0/10
26. [Decoy Font Tricks AI but Not Robust](#item-26) ⭐️ 6.0/10
27. [Mermaid to ASCII art with WebAssembly and color support](#item-27) ⭐️ 6.0/10
28. [Mermaid diagrams rendered as Unicode box art via WebAssembly](#item-28) ⭐️ 6.0/10
29. [Seeking Python Tools for Multi-Objective Surrogate-Based Optimization on Meta-Analysis Data](#item-29) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Firefox in WebAssembly: Browser Inside Browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 10.0/10

Puter has successfully compiled Firefox to WebAssembly, allowing a full Firefox browser instance to run inside another browser like Chrome. The project used AI assistance from Claude Opus and Fable tokens to achieve this, and employed the Wisp protocol for network proxying. This demonstrates the extreme portability of complex applications via WebAssembly, potentially revolutionizing software deployment and access. It also showcases the viability of AI-assisted compilation for large-scale projects. Firefox's Gecko engine was chosen for its strong single-process support, and the WebAssembly binary is 233MB. Network traffic is proxied through Puter's server using the Wisp protocol over a WebSocket, with end-to-end encryption for HTTPS connections.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (Wasm) is a binary instruction format that enables near-native execution in web browsers. Running a full browser inside another is technically challenging due to networking and resource constraints. The Wisp protocol is a low-overhead protocol for multiplexing multiple TCP/UDP sockets over a single WebSocket connection, essential for proxying network requests from within the Wasm environment.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wire_protocol">Wire protocol</a></li>

</ul>
</details>

**Tags**: `#WebAssembly`, `#Firefox`, `#browser`, `#virtualization`, `#cross-platform`

---

<a id="item-2"></a>
## [Kimi K3: 2.8 Trillion Parameter Open-Weight Model Announced](https://simonwillison.net/2026/Jul/16/kimi-k3/#atom-everything) ⭐️ 9.0/10

Moonshot AI announced Kimi K3, a 2.8 trillion parameter open-weight model that outperforms most proprietary models on benchmarks and will be publicly released by July 27, 2026. Kimi K3 represents a significant leap in open-weight model capabilities, rivaling top proprietary models like Claude Opus 4.8 and GPT-5.5, which could accelerate AI research and commoditize intelligence. With 2.8 trillion parameters, Kimi K3 is priced at $3 per million input tokens and $15 per million output tokens, making it the most expensive Chinese open-weight model to date, comparable to Anthropic's Claude Sonnet series.

rss · Simon Willison · Jul 16, 20:19

**Background**: Open-weight models release their trained parameters publicly, allowing anyone to download and run them on their own hardware. The 'pelican riding a bicycle' test is an informal benchmark created by developer Simon Willison to evaluate LLMs' ability to generate SVG code from a simple prompt. Kimi K3 passed this test for 25 cents.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark) — Grokipedia</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Discussion**: Comments note that the pelican test cost 25 cents, making it the most expensive through a Chinese model. Some discuss the commoditization of intelligence by Chinese labs, while others note the high pricing compared to other open-weight models.

**Tags**: `#AI`, `#large language models`, `#open source`, `#Moonshot AI`, `#benchmarks`

---

<a id="item-3"></a>
## [Prompt Injection Attack Exfiltrates Claude User Memories](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 9.0/10

Researcher Ayush Paul demonstrated a prompt injection attack that exploits Claude's web_fetch tool to exfiltrate user memories, bypassing Anthropic's URL restrictions. The attack uses a honeypot website that tricks Claude into following nested links to send private data to an attacker-controlled server. This vulnerability is critical because it demonstrates a practical data exfiltration attack on a widely-used AI assistant, Claude, despite Anthropic's security safeguards. It highlights the ongoing challenge of protecting AI agents with access to private data and external tools from prompt injection attacks. The attack exploited a loophole where web_fetch could navigate to URLs embedded in previously fetched pages. The attacker created a honeypot site that only responded to Claude-User agents, instructing the model to browse alphabetically and append user answers to malicious URLs. Anthropic had already internally identified the issue and removed the ability to follow links from fetched content.

rss · Simon Willison · Jul 15, 14:21

**Background**: Claude's web_fetch tool allows the model to retrieve content from URLs specified in the conversation. However, AI agents face a "lethal trifecta" risk when they combine private data (like user memories), untrusted content (from web pages), and exfiltration capabilities (like URL fetching). Anthropic attempted to mitigate this by restricting web_fetch to only navigate URLs provided by the user or from its web_search tool, but the honeypot attack bypassed that by using links from fetched pages.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>
<li><a href="https://docs.claude.com/en/docs/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Docs</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/memory-tool">Memory tool - Claude Platform Docs</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#prompt injection`, `#data exfiltration`, `#vulnerability`, `#Anthropic`

---

<a id="item-4"></a>
## [Schema Harness Claims 99% on ARC-AGI-3 Without Weight Changes](https://www.reddit.com/r/MachineLearning/comments/1uyf8oo/new_fable5opus48_harness_called_schema_claims_99/) ⭐️ 9.0/10

A new AI harness called Schema achieves 99% accuracy on the ARC-AGI-3 public benchmark using Claude Opus 4.8 and Fable 5, and 95.35% using GPT-5.6 Sol, all without modifying model weights. This result is significant because it demonstrates that large performance gains on challenging reasoning benchmarks can come from process-level innovations (the harness) rather than larger or retrained models. It attracts attention from the ARC Prize president, indicating community validation and potential to reshape AI agent development. The harness uses a fixed fallback rule: Opus 4.8 and Sol xhigh run first; games scoring below 80 are rerun with Fable 5 and Sol max, retaining the higher per-game score. Schema does not change model weights but alters how observations are turned into models, how predictions are tested, and how plans are executed and revised.

reddit · r/MachineLearning · /u/we_are_mammals · Jul 16, 21:02

**Background**: ARC-AGI-3 is an interactive reasoning benchmark designed to measure human-like intelligence in AI agents by requiring them to explore novel environments, infer goals, and plan in turn-based settings. A harness is the scaffolding (context delivery, tool interfaces, planning artifacts, verification loops, and memory systems) that surrounds an AI agent and determines its success on real tasks, separate from the model itself.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://github.com/ai-boost/awesome-harness-engineering">ai-boost/awesome-harness-engineering - GitHub</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">[2603.24621] ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence</a></li>

</ul>
</details>

**Tags**: `#ARC-AGI`, `#AI reasoning`, `#harness`, `#Claude Opus`, `#GPT-5`

---

<a id="item-5"></a>
## [LM Studio Bionic: AI Agent for Open Models](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 8.0/10

LM Studio has launched Bionic, a new Mac app that serves as an AI agent for open models, enabling coding, research, and complex document manipulation tasks using local or cloud-based open models. This release marks a significant step in making local AI agents practical for real work, combining the privacy and cost benefits of open models with a polished user interface, potentially shifting users away from cloud-only solutions. Bionic supports both local models and switching to open-source models in the cloud via LM Studio Secure Cloud, with automatic checkpointing for every change made in 'Work' projects.

hackernews · minimaxir · Jul 16, 20:18 · [Discussion](https://news.ycombinator.com/item?id=48939662)

**Background**: LM Studio is a popular desktop application for running local large language models (LLMs) on personal computers. Bionic extends its capability from chat to agentic tasks like coding and document editing, leveraging open models that have recently crossed an inflection point in quality (e.g., Kimi K2.6, GLM 5.2).

<details><summary>References</summary>
<ul>
<li><a href="https://9to5mac.com/2026/07/16/lm-studio-expands-beyond-chat-with-bionic-a-new-ai-agent-app-for-open-models/">LM Studio launches Bionic, a new AI agent app for open models - 9to5Mac</a></li>
<li><a href="https://lmstudio.ai/blog/introducing-lm-studio-bionic">Introducing LM Studio Bionic: the AI agent for open models | LM Studio Blog | LM Studio</a></li>
<li><a href="https://x.com/yagilb/status/2077840161241456649?lang=en">yags on X: "Today we're introducing Bionic - LM Studio's agent, made for open models. A few months ago open models have crossed an inflection point with Kimi K2.6, and recently with GLM 5.2. LM Studio Bionic is built for this moment. Using open models is a viable and obvious decision for" / X</a></li>

</ul>
</details>

**Discussion**: The founder Yagil engaged directly, offering credits for testing with specific models. User feedback was positive, with one user praising the familiar UI and good results with Qwen3.6 35B, while noting some rough edges. Concerns were raised about the shift to a cloud-based business model and why to choose Bionic over other harnesses.

**Tags**: `#AI agents`, `#open-source models`, `#local LLM`, `#coding`, `#product launch`

---

<a id="item-6"></a>
## [Rust-to-Zig Rewrite: Progress and Rationale](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

A blog post details the ongoing rewrite of a compiler from Rust to Zig, highlighting improvements in incremental build performance and memory control. This decision underscores the trade-offs between memory safety and low-level control in systems programming, potentially influencing future language choices for performance-critical projects. The rewrite targets a compiler that emits machine code, where Zig's manual memory management and fast incremental builds are key advantages. The author notes that compilers often require unsafe operations for tasks like binary patching.

hackernews · jorangreef · Jul 16, 11:39 · [Discussion](https://news.ycombinator.com/item?id=48933149)

**Background**: Rust and Zig are both modern systems programming languages, but Rust prioritizes memory safety through its ownership model, while Zig offers more direct control with manual memory management. Compilers, especially those emitting machine code, often need low-level operations that can be difficult to express safely in Rust.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://ziglang.org/">Home Zig Programming Language</a></li>

</ul>
</details>

**Discussion**: Community comments include skepticism about the necessity of unsafe operations in compilers, questions about Zig's runtime memory safety checks, and debates on build speed comparisons. Overall, the discussion is technically engaged and highlights differing perspectives on language trade-offs.

**Tags**: `#Rust`, `#Zig`, `#Compiler`, `#Programming Languages`, `#Systems Programming`

---

<a id="item-7"></a>
## [GPT-5.6 Codex Bug Can Delete User Files](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

OpenAI employee Thibault Sottiaux reported that GPT-5.6 Codex can accidentally delete user files when full access mode is enabled without sandboxing protections and the model mistakenly deletes the $HOME directory instead of a temporary directory. This bug raises serious safety concerns for AI coding agents, as it can cause irreversible data loss and erodes trust in AI-assisted development tools. It underscores the need for robust sandboxing and review mechanisms before granting file system access to AI agents. The bug occurs specifically when full access mode is enabled without sandboxing or auto-review, and the model attempts to override the $HOME environment variable to define a temporary directory but mistakenly deletes $HOME instead. OpenAI has investigated the reports and identified the root cause.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is an AI coding agent developed by OpenAI for software engineering tasks such as writing code and fixing bugs. Sandboxing is a security technique that isolates code execution to prevent unintended system access. When full access mode is enabled without sandboxing, the AI has unrestricted file system permissions, making mistakes like this possible.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Codex_(AI_agent)">OpenAI Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://www.luiscardoso.dev/blog/sandboxes-for-ai">A field guide to sandboxes for AI - luiscardoso.dev</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#gpt-5.6`

---

<a id="item-8"></a>
## [Thinking Machines Lab Releases Inkling, a Large Open-Weights MoE Model](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

Mira Murati's Thinking Machines Lab released Inkling, an open-weights Mixture-of-Experts multimodal model with 975B total parameters (41B active), trained on 45 trillion tokens of text, images, audio, and video, under the Apache-2.0 license. Inkling strengthens the US open-weights ecosystem by providing a competitive alternative to Chinese open models and other contenders like NVIDIA Nemotron and Gemma 4, offering a strong base for fine-tuning via its Tinker platform. The model is not a frontier model but designed as a base for customization; a smaller Inkling-Small (276B total, 12B active) is still in testing. The accompanying model card and training data documentation are notably sparse.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) is an architecture that activates only a subset of parameters per input, enabling large model capacity with lower inference cost. Open-weights models allow anyone to download, run, and fine-tune them, fostering transparency and customization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Tags**: `#open-weights`, `#AI`, `#mixture-of-experts`, `#multimodal`, `#large language model`

---

<a id="item-9"></a>
## [xAI open-sources Grok Build after CLI privacy backlash](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 8.0/10

xAI faced severe backlash after its Grok CLI tool was discovered to upload entire directories to the cloud, and responded by open-sourcing the entire Grok Build codebase under the Apache 2.0 license. This incident highlights critical privacy risks in AI-powered coding tools, and the open-sourcing move is a rare step to rebuild trust that could set a precedent for transparency in the industry. The open-source repository contains 844,530 lines of Rust code (only ~3% vendored), includes a Mermaid diagram renderer for terminals, and features tool implementations inspired by Codex and OpenCode.

rss · Simon Willison · Jul 15, 23:59

**Background**: Grok Build is xAI's terminal-based AI coding agent that can edit files, run commands, and manage tasks. CLI tools that access local files must handle data uploads carefully; the incident revealed a default behavior of uploading entire directories, which users perceived as a major privacy violation.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xai-org/grok-build">GitHub - xai-org/grok-build: SpaceXAI's coding agent harness ...</a></li>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>

</ul>
</details>

**Discussion**: The community reacted with outrage, with one user reporting that running the tool in their home directory uploaded SSH keys and password databases. The open-sourcing was seen as a positive step, but skepticism remains about whether data was truly deleted and whether the move is sufficient to restore trust.

**Tags**: `#AI`, `#open source`, `#privacy`, `#CLI`, `#xAI`

---

<a id="item-10"></a>
## [ExTernD: Expanded-Rank Ternary Decomposition for LLM Quantization](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

ExTernD proposes a novel post-training quantization method that decomposes each weight matrix into two ternary matrices and a diagonal scaling matrix, allowing the inner rank to be expanded arbitrarily to improve accuracy. This method challenges the assumption that ternary quantization inherently degrades accuracy, showing that with decomposition it can approach full-precision performance, offering a practical trade-off between model compression and accuracy with minimal VRAM overhead. The decomposition uses two ternary matrices and a diagonal scaling matrix, where the inner rank can be increased beyond fixed limits, allowing ExTernD to achieve accuracy comparable to any quantization level while only moderately increasing VRAM usage compared to existing methods.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Large language models (LLMs) are memory-intensive; quantization reduces memory by using lower precision. Ternary quantization (weights -1, 0, +1) is an extreme form that typically suffers from accuracy loss due to limited representational capacity. ExTernD addresses this by decomposing each weight matrix into a product of two ternary matrices and a diagonal scaling matrix, allowing the inner dimension to be expanded to capture more information.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2607.13511v1">ExTernD: Expanded-Rank Ternary Decomposition Ternary LLM PTQ ...</a></li>
<li><a href="https://arxiv.org/abs/2406.07177">[2406.07177] TernaryLLM: Ternarized Large Language Model</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#quantization`, `#ternary`, `#post-training`, `#efficient ML`

---

<a id="item-11"></a>
## [PnP-CoSMo: Plug-and-Play Multi-Contrast MRI Reconstruction](https://www.reddit.com/r/MachineLearning/comments/1uy2h66/pnpcosmo_a_multicontrast_mri_reconstruction/) ⭐️ 8.0/10

PnP-CoSMo, a plug-and-play framework for multi-contrast MRI reconstruction, was published in Medical Image Analysis. It learns content and style models from image-domain data only, eliminating the need for raw k-space data. This work addresses a major bottleneck in ML-based MRI reconstruction by removing the requirement for raw k-space training data, which is often difficult to obtain. It achieves state-of-the-art results and generalizes across different MR contrasts and forward operators, potentially accelerating clinical adoption. PnP-CoSMo operates in two stages: first learning a content/style model from image data, then freezing it as a prior in iterative reconstruction. It is designed to work across various contrasts and forward operators without retraining, offering a built-in explanatory framework.

reddit · r/MachineLearning · /u/void_gear · Jul 16, 13:10

**Background**: In MRI, data is acquired in the spatial frequency domain (k-space), and reconstruction typically requires converting this raw data into images. Plug-and-play reconstruction uses a pretrained denoiser as a prior within iterative algorithms, allowing reuse across tasks without retraining. Content/style modeling separates invariant structural content from contrast-specific style, enabling multi-contrast fusion.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/K-space_in_magnetic_resonance_imaging">k-space in magnetic resonance imaging - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2508.01441">[2508.01441] Viscosity Stabilized Plug - and - Play Reconstruction</a></li>

</ul>
</details>

**Tags**: `#MRI`, `#Deep Learning`, `#Medical Imaging`, `#Image Reconstruction`, `#Plug-and-Play`

---

<a id="item-12"></a>
## [Hadamard Product Technique Disentangles Convolutional Neurons](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

A novel method uses the Hadamard product of receptive field and weights to visualize patterns detected by a convolutional neuron, revealing monosemantic clusters for concepts like cars and cats. This work advances mechanistic interpretability by providing a simple yet powerful tool to analyze individual neurons, potentially enabling better understanding of how vision models perceive concepts. The analysis was performed on a 1x1 convolutional neuron in InceptionV1, and the technique also uncovered low-valued clusters (e.g., letters) where positive and negative weights cancel out.

reddit · r/MachineLearning · /u/narang_27 · Jul 15, 06:59

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by understanding their internal circuits. Monosemantic neurons respond to a single concept, while polysemantic neurons respond to multiple. The Hadamard product is an element-wise multiplication of matrices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_product_(matrices)">Hadamard product (matrices) - Wikipedia</a></li>
<li><a href="https://www.lesswrong.com/posts/8uMA6vwitdwqs5AH4/monosemanticity-and-quantization">Monosemanticity & Quantization — LessWrong</a></li>

</ul>
</details>

**Discussion**: The author notes that starting with convolutions received less attention, and expresses hope for feedback. No comments are provided in the content, so community sentiment is unknown.

**Tags**: `#mechanistic interpretability`, `#convolutional neural networks`, `#neuron analysis`, `#computer vision`

---

<a id="item-13"></a>
## [Microsoft Comic Chat Open-Sourced](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 7.0/10

On July 16, 2026, Microsoft open-sourced Comic Chat, the graphical IRC client that turns text conversations into comic panels, along with its source code on GitHub. This release preserves a piece of internet history and allows developers to study and remix a pioneering graphical chat experience that influenced early online communities and even introduced the Comic Sans font to the world. Comic Chat was developed by Microsoft researcher David Kurlander and first released with Internet Explorer 3.0 in 1996; it later became Microsoft Chat and was bundled with Windows 98. The open-source release includes the original code and is available under an MIT license.

hackernews · jervant · Jul 16, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48936426)

**Background**: Comic Chat is a graphical IRC client that automatically visualizes conversations as comic strips with characters, speech bubbles, and expressions. IRC (Internet Relay Chat) is a text-based chat protocol popular in the 1990s and early 2000s for group communication. The client used a custom extension to the IRC protocol to convey character appearance and emotions, distinguishing it from purely text-based clients.

<details><summary>References</summary>
<ul>
<li><a href="https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/">Microsoft Comic Chat is now open source</a></li>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Comic_Chat">Microsoft Comic Chat</a></li>
<li><a href="https://en.wikipedia.org/wiki/IRC">IRC - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community responded enthusiastically, with many sharing personal stories about Comic Chat's influence. Robert Standefer, who helped make the release happen, recounted the six-year effort, while others recalled its inspiration for their own projects or noted its quirky place in internet culture.

**Tags**: `#open source`, `#microsoft`, `#irc`, `#nostalgia`, `#community engagement`

---

<a id="item-14"></a>
## [Google Rebrands NotebookLM as Gemini Notebook](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook/) ⭐️ 7.0/10

Google has rebranded NotebookLM to Gemini Notebook, integrating the AI note-taking tool more deeply into its Gemini ecosystem. The change reflects a broader strategy to unify AI products under the Gemini brand. This rebranding signals Google's commitment to consolidating its AI offerings, potentially improving cross-product integration and user experience. It may also affect how users perceive and adopt the tool, as Gemini Notebook becomes a core part of Google's AI suite. NotebookLM was known for features like Audio Overviews, which generate podcast-like discussions from uploaded content. The new name aligns it with Google's Gemini models, which power the tool's AI capabilities.

hackernews · xnx · Jul 16, 16:08 · [Discussion](https://news.ycombinator.com/item?id=48936451)

**Background**: NotebookLM is a research and note-taking tool that uses retrieval-augmented generation (RAG) to help users interact with their documents. It was developed by Google Labs and gained popularity for its AI-generated podcast summaries. The rebranding to Gemini Notebook reflects a broader trend of Google unifying its AI products under the Gemini brand, similar to how other products like Bard were renamed to Gemini.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NotebookLM">NotebookLM</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions. Some users note the novelty of NotebookLM's audio features has worn off, and they prefer alternatives like ChatGPT Live for audio learning. Others ask about comparisons between different AI notebooks, such as Microsoft Copilot's notebook. There is also speculation about internal team dynamics at Google driving the rebranding.

**Tags**: `#Google`, `#Gemini`, `#NotebookLM`, `#Rebranding`, `#AI`

---

<a id="item-15"></a>
## [Community Highlights Math Foundations in Data Science](https://arxiv.org/abs/2607.11938) ⭐️ 7.0/10

A community discussion on an arXiv preprint titled 'Mathematics of Data Science' emphasizes that mathematical foundations, particularly high-dimensional geometry and statistics, are critical for modern data science practice. The discussion argues that understanding these concepts is essential for building intuition and making sound decisions from data. This discussion underscores a growing recognition that data science requires deep mathematical understanding, not just tool proficiency. It matters because as data science evolves, practitioners with strong fundamentals can better avoid pitfalls and create more reliable models, affecting job roles and industry standards. Commenters specifically note that high-dimensional intuition often breaks down—for example, volumes behave counterintuitively—which directly impacts optimization and model training. One commenter identifies statistics as the absolute top priority skill for data scientists today.

hackernews · Anon84 · Jul 16, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48939896)

**Background**: High-dimensional geometry studies geometric properties in spaces with many dimensions, where phenomena like the concentration of measure occur. High-dimensional statistics deals with datasets where the number of features is large relative to the sample size, requiring specialized techniques. These mathematical areas are foundational for understanding modern machine learning algorithms like stochastic gradient descent.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High-dimensional_statistics">High-dimensional statistics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Higher-dimensional_geometry">Higher-dimensional geometry</a></li>
<li><a href="https://www.cs.princeton.edu/courses/archive/fall14/cos521/lecnotes/lec11.pdf">Lecture 11: High Dimensional Geometry , Curse of</a></li>

</ul>
</details>

**Discussion**: The community comments reflect strong agreement on the importance of mathematical foundations. User 'wosk' shares their teaching experience emphasizing high-dimensional intuition breakdown, while 'astro1234' argues that statistics is the number one priority skill. The overall sentiment is that building mathematical intuition is difficult but crucial for effective data science.

**Tags**: `#data science`, `#mathematics`, `#high-dimensional`, `#statistics`, `#intuition`

---

<a id="item-16"></a>
## [Detecting LLM-Generated Text with Classical Machine Learning](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 7.0/10

The blog post explores using classical machine learning techniques, such as logistic regression and random forests, to detect whether a text was generated by a large language model (LLM). The author presents a classifier trained on features like n-grams and sentence length. As LLMs become widespread, detecting their output is crucial for content moderation and academic integrity. This approach offers a lightweight alternative to deep learning detectors, potentially enabling real-time detection in browsers or low-resource environments. The classifier uses features such as n-grams, sentence length, and punctuation patterns, and achieves moderate accuracy on a benchmark dataset. However, the author acknowledges that like all such detectors, it can be evaded by adversarial prompts or human editing.

hackernews · uneven9434 · Jul 16, 16:41 · [Discussion](https://news.ycombinator.com/item?id=48936880)

**Background**: Classical machine learning refers to algorithms like logistic regression, decision trees, and support vector machines that rely on hand-engineered features rather than neural networks. Unlike deep learning, these methods are often faster to train and require less computational power, making them suitable for deployment on consumer devices. The blog post contrasts this with typical LLM detection methods that use neural networks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/machine-learning/classic-and-adaptive-machines/">Classic and Adaptive machines - GeeksforGeeks</a></li>
<li><a href="https://link.springer.com/protocol/10.1007/978-1-0716-3195-9_2">Classic Machine Learning Methods | Springer Nature Link</a></li>

</ul>
</details>

**Discussion**: The community discussion reveals skepticism about the long-term viability of LLM detection, with some commenters comparing it to 'tarot card reading.' A notable alternative proposed is 'effort detection'—gauging the amount of human effort in writing rather than detecting AI origins. Others suggest a browser extension for real-time detection, and one commenter notes that human detectors remain the best.

**Tags**: `#LLM detection`, `#machine learning`, `#AI-generated text`, `#classical ML`, `#content moderation`

---

<a id="item-17"></a>
## [Immersive Linear Algebra Book Revives Interest in Interactive Education](https://immersivemath.com/ila/) ⭐️ 7.0/10

A 2015 interactive linear algebra book with fully interactive figures has gained renewed attention online, praised for its clean presentation and potential to enhance math education. This book demonstrates how interactive visuals can simplify abstract mathematical concepts, potentially transforming textbook design and improving student comprehension in STEM fields. Authored by J. Ström, K. Åström, and T. Akenine-Möller, it is claimed as the world's first linear algebra book with fully interactive figures, available online at immersivemath.com.

hackernews · srean · Jul 16, 15:32 · [Discussion](https://news.ycombinator.com/item?id=48935951)

**Background**: Traditional linear algebra textbooks rely on static diagrams, which can make abstract concepts like vector spaces and transformations difficult to grasp. Interactive figures allow students to manipulate mathematical objects in real time, providing intuitive understanding. This book represents an early example of embedding interactive visualizations directly into a digital textbook.

<details><summary>References</summary>
<ul>
<li><a href="http://immersivemath.com/ila/index.html">Immersive Math</a></li>
<li><a href="https://www.lth.se/fileadmin/lth/genombrottet/LUkonf2015/41_Stro__m_etal.pdf">Immersive Linear Algebra - LTH, Lunds Tekniska Högskola</a></li>

</ul>
</details>

**Discussion**: Commenters enthusiastically praised the book, with one lamenting its absence during their own studies and expressing desire for similar books in statistics and robotics. Others noted that modern AI tools like LLMs make creating such interactive content easier, hinting at a future where textbooks become more dynamic.

**Tags**: `#linear algebra`, `#interactive learning`, `#education`, `#mathematics`

---

<a id="item-18"></a>
## [Turn Golf Courses into Parks to Offset Water Use](https://simonwillison.net/2026/Jul/17/spot-birds-not-golf/#atom-everything) ⭐️ 7.0/10

Simon Willison proposes that hyperscalers like Google could offset their data center water consumption by purchasing and converting golf courses into public parks, backed by calculations comparing water usage. This idea links AI data center water usage to golf course consumption with concrete numbers, highlighting a potential sustainability trade-off that could influence tech policy and environmental discussions. Google used 10.9 billion gallons of water in 2025, about 30 million gallons per day. Coachella Valley has 120 golf courses each using ~800 acre-feet per year (~750,000 gallons per day), so buying up 40 courses would offset Google's daily water use.

rss · Simon Willison · Jul 17, 02:58

**Background**: A hyperscaler is a large-scale cloud service provider that operates vast, distributed infrastructure. Data centers, especially those supporting AI workloads, consume significant amounts of water for cooling, raising environmental concerns. Golf courses are known for high water usage, often in arid regions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyperscale_computing">Hyperscale computing - Wikipedia</a></li>
<li><a href="https://www.eesi.org/articles/view/data-centers-and-water-consumption">Data Centers and Water Consumption | Article | EESI</a></li>

</ul>
</details>

**Tags**: `#ai`, `#water usage`, `#data centers`, `#environment`, `#sustainability`

---

<a id="item-19"></a>
## [Linus Torvalds Declares Linux Not Anti-AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 7.0/10

Linus Torvalds, the creator of Linux, explicitly stated on the Linux Media Mailing List that Linux is not an anti-AI project and that AI is a clearly useful tool, asserting his authority as top-level maintainer. This definitive stance from Torvalds sets a strong community norm, potentially influencing Linux kernel contributors and the broader open-source ecosystem to embrace AI tools rather than reject them. Torvalds noted that while there are still questions about AI's economy, its usefulness is no longer in doubt, and those who disagree can fork the project or walk away.

rss · Simon Willison · Jul 16, 13:26

**Background**: The Linux kernel is one of the largest open-source projects, with Torvalds as its benevolent dictator for life (BDFL). Recently, some open-source communities have expressed strong anti-AI sentiment, particularly around training models on their code. Torvalds' statement directly counters that trend within the Linux community.

**Tags**: `#linux`, `#ai`, `#open-source`, `#linus-torvalds`, `#kernel`

---

<a id="item-20"></a>
## [DABSN Recurrent Architecture Seeks Collaborators for Scaling](https://www.reddit.com/r/MachineLearning/comments/1uycffg/seeking_collaborators_for_scaling_and_independent/) ⭐️ 7.0/10

The author of DABSN (Dynamic Adaptive Bias State Network) has released a preprint and open-source code, and is seeking collaborators to scale and independently evaluate the architecture. If validated, DABSN could offer an efficient recurrent alternative to transformers for language modeling, potentially reducing computational costs while maintaining performance. The architecture was tested on reasoning, memory, and long-sequence benchmarks including MQAR and A5/60, and a 24M parameter language model was trained on 1B tokens with a GPT-2 tokenizer.

reddit · r/MachineLearning · /u/BleedingXiko · Jul 16, 19:17

**Background**: Recurrent architectures like LSTMs and GRUs were dominant before transformers, but struggle with long-range dependencies. Recently, new recurrent models like Mamba and the MQAR benchmark have revived interest in alternatives to the transformer architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2312.04927">[2312.04927] Zoology: Measuring and Improving Recall in ... GitHub - HazyResearch/zoology: Understand and test language ... GitHub - howard-hou/Visual-MQAR: Understand and test multi ... MQAR: Multi-Query Associative Recall - emergentmind.com Zoology (Blogpost 1): Measuring and Improving Recall in ... Published as a workshop paper at SCOPE - ICLR 2025 - OpenReview Understanding Input Selectivity in Mamba: Impact on ...</a></li>
<li><a href="https://github.com/HazyResearch/zoology">GitHub - HazyResearch/zoology: Understand and test language ... GitHub - howard-hou/Visual-MQAR: Understand and test multi ... MQAR: Multi-Query Associative Recall - emergentmind.com Zoology (Blogpost 1): Measuring and Improving Recall in ... Published as a workshop paper at SCOPE - ICLR 2025 - OpenReview Understanding Input Selectivity in Mamba: Impact on ...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#recurrent neural networks`, `#language models`, `#open source`

---

<a id="item-21"></a>
## [Rethinking AI Memory: From Facts to Reasoning Patterns](https://www.reddit.com/r/MachineLearning/comments/1uy6yht/are_current_ai_memory_architectures_optimizing/) ⭐️ 7.0/10

A Reddit post speculates that future AI memory systems should evolve from storing descriptive facts about users to inferring higher-level reasoning patterns, such as explanatory frameworks and characteristic reasoning styles. This challenges current designs of persistent context in AI, which primarily store factual user information, and suggests a paradigm shift towards modeling how users think, potentially leading to more personalized and insightful AI interactions. The post distinguishes current descriptive memory (e.g., user interests) from proposed inferential memory (e.g., how a user explains economic outcomes through incentives), and questions whether such higher-level patterns can emerge naturally or require fundamentally different architectures.

reddit · r/MachineLearning · /u/Boris_Ljevar · Jul 16, 16:00

**Background**: Current AI systems use persistent context mechanisms like conversation summaries and user preferences to maintain memory across sessions, which are primarily descriptive. Products like Mem0 provide drop-in memory infrastructure that stores factual user information. The post argues that future systems might instead model how users reason, similar to explanatory learning frameworks that use symbolic explanations.

<details><summary>References</summary>
<ul>
<li><a href="https://mem0.ai/">Mem0 - AI Memory Layer for your Agents & Apps | Persistent Context</a></li>
<li><a href="https://sverhulst.medium.com/the-context-loop-04d473545909">The Context Loop. How AI Remembers Us, and Shapes... | Medium</a></li>

</ul>
</details>

**Tags**: `#AI memory`, `#persistent context`, `#machine learning`, `#reasoning patterns`

---

<a id="item-22"></a>
## [QLoRA 2e-4 Default Learning Rate Overfits Small Datasets](https://www.reddit.com/r/MachineLearning/comments/1uy1z8b/the_qlora_2e4_default_is_wrong_under_10k_samples/) ⭐️ 7.0/10

A Reddit user argues that the widely-used default QLoRA learning rate of 2e-4 is too high for datasets with fewer than 10,000 samples, causing overfitting. They recommend starting at 1e-4 and increasing the number of epochs instead. This practical finding could save many fine-tuning practitioners weeks of debugging, as the default learning rate is often copied from tutorials without adjustment. Small dataset fine-tuning is common in domain adaptation, and this advice may improve model quality significantly. The original QLoRA paper and tools like Unsloth use 2e-4 as a starting point based on the 52k-sample Alpaca dataset, but this does not transfer well to smaller datasets. The user suggests a rule of thumb: above 30k samples, 2e-4 is fine; under 10k, start at 1e-4 or lower and add epochs.

reddit · r/MachineLearning · /u/Pretty-Ad774 · Jul 16, 12:50

**Background**: QLoRA (Quantized Low-Rank Adaptation) is an efficient fine-tuning method that reduces memory usage by updating a small set of parameters while keeping the base model quantized. The learning rate is a critical hyperparameter: too high causes overfitting on small datasets, too low leads to slow convergence. The default 2e-4 originates from the original QLoRA paper's experiments on the 52k-instruction Alpaca dataset. However, many practitioners work with custom datasets of 5-10k samples, where this default is suboptimal.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/datasets/tatsu-lab/alpaca">tatsu-lab/alpaca · Datasets at Hugging Face</a></li>
<li><a href="https://www.heulistic.com/blog/learning-rate-qlora-fine-tuning">What Learning Rate to Use for QLoRA Fine-Tuning</a></li>
<li><a href="https://medium.com/@matteo28/qlora-fine-tuning-with-unsloth-a-complete-guide-8652c9c7edb3">QLoRA Fine-Tuning with Unsloth | Medium</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#fine-tuning`, `#QLoRA`, `#hyperparameters`, `#overfitting`

---

<a id="item-23"></a>
## [Reddit Seeks Devil's Advocate on JEPA for Robot Learning](https://www.reddit.com/r/MachineLearning/comments/1uxcryc/looking_for_jepa_devil_advocates_r/) ⭐️ 7.0/10

A Reddit user in r/MachineLearning is asking for critical viewpoints on JEPA (Joint Embedding Predictive Architecture) models, specifically for use as world models in robot learning, suspecting that Yann LeCun's claims may be overhyped. This discussion is important because JEPA is a prominent research direction for building world models that could lead to more human-like AI, especially in robotics. Hearings from skeptics helps the community validate or challenge LeCun's strong claims against LLMs and RL. The user has read recent JEPA papers and finds the approach promising, but is concerned that LeCun dismisses LLMs and RL while promoting JEPA as the only next big thing. They are seeking concrete red flags and downsides compared to other world model approaches.

reddit · r/MachineLearning · /u/Amazing-Coat5160 · Jul 15, 17:34

**Background**: JEPA (Joint Embedding Predictive Architecture) is a family of models proposed by Yann LeCun that learn to predict abstract representations of data rather than raw pixels, aiming to capture the underlying structure of the world. It is a candidate for world models in robotics, which are models that predict future sensory states given actions. LeCun has been critical of autoregressive LLMs and reinforcement learning, arguing that JEPA-style architectures are more aligned with how humans learn and reason.

<details><summary>References</summary>
<ul>
<li><a href="https://rohitbandaru.github.io/blog/JEPA-Deep-Dive/">Deep Dive into Yann LeCun’s JEPA | Rohit Bandaru</a></li>
<li><a href="https://arxiv.org/abs/2605.00080">World Model for Robot Learning: A Comprehensive Survey Robotics World Modeling World Model for Robot Learning: A Comprehensive Survey World models for robotics - Harvard AI and Robotics Lab 1X World Model | From Video to Action: A New Way Robots Learn Pretrained to Imagine, Fine-Tuned to Act: The Rise of World ... World Model for Robot Learning: A Comprehensive Survey</a></li>

</ul>
</details>

**Tags**: `#JEPA`, `#world models`, `#robot learning`, `#Yann LeCun`, `#deep learning`

---

<a id="item-24"></a>
## [170x PyTorch slowdown on T4 vs A100 baffles user](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 7.0/10

A user reports a 170× slowdown running a PyTorch point-tracking model on an NVIDIA T4 GPU compared to an A100, with the T4 taking ~85 seconds per half-video versus ~0.5 seconds on the A100. This extreme performance gap is beyond what typical hardware generational differences would suggest, and diagnosing it could reveal critical insights into optimizing deep learning models for deployment on diverse GPU architectures. The model uses pure FP32 precision, builds 4D correlation volumes for dense matching, and includes transformer layers; GPU utilization is 99% on T4, and the issue reproduces on two independent T4 machines.

reddit · r/MachineLearning · /u/Future-Structure-296 · Jul 15, 13:44

**Background**: The NVIDIA T4 (Turing) and A100 (Ampere) differ significantly: the A100 has much higher memory bandwidth, more FP32 compute units, and supports advanced features like sparse matmul. 4D correlation volumes are memory-intensive operations that involve computing similarity scores across spatial and temporal dimensions. Running such operations in FP32 on a T4, which has relatively limited FP32 throughput and memory bandwidth, can exacerbate the performance gap.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/changh95/visual-slam-roadmap/blob/main/level-05-deep-learning/sea-raft.md">visual-slam-roadmap/level-05- deep - learning /sea-raft.md at main...</a></li>
<li><a href="https://arxiv.org/pdf/2510.20951">Generative Point Tracking with Flow Matching - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#PyTorch`, `#GPU performance`, `#debugging`, `#deep learning`

---

<a id="item-25"></a>
## [uv 0.11.29 adds JSON tree, CUDA 13.2 support](https://github.com/astral-sh/uv/releases/tag/0.11.29) ⭐️ 6.0/10

uv 0.11.29 was released on July 15, 2026, adding JSON output to the `uv tree` command and CUDA 13.2 as a supported PyTorch backend. It also includes performance improvements, bug fixes, and preview features for OSV audit. JSON output in `uv tree` enables programmatic consumption of dependency trees, improving CI/CD integration and tooling. CUDA 13.2 support ensures compatibility with the latest NVIDIA GPU computing toolkit for PyTorch users. The JSON output option can be invoked via `uv tree --format json`, providing structured data. CUDA 13.2 support is part of uv's PyTorch backend integration, following NVIDIA's March 2026 release of CUDA 13.2 with enhanced tile support.

github · github-actions[bot] · Jul 15, 18:44

**Background**: uv is a fast Python package manager and resolver developed by Astral Software, written in Rust. The `uv tree` command displays project dependencies in a hierarchical tree format, useful for debugging. CUDA is NVIDIA's parallel computing platform for GPU acceleration; CUDA 13.2 is the latest version with new Python features and tile support. OSV (Open Source Vulnerabilities) audit helps find known vulnerabilities in dependencies.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/reference/cli/">Commands | uv - Astral</a></li>
<li><a href="https://developer.nvidia.com/blog/cuda-13-2-introduces-enhanced-cuda-tile-support-and-new-python-features/">CUDA 13.2 Introduces Enhanced CUDA Tile Support and New ...</a></li>
<li><a href="https://dev.to/curioustore_48788631d0e2e/uv-audit-vs-pip-audit-and-a-gate-narrower-than-it-looks-30nf">uv audit vs pip- audit , and a gate narrower than it... - DEV Community</a></li>

</ul>
</details>

**Tags**: `#uv`, `#python`, `#package-manager`, `#release`

---

<a id="item-26"></a>
## [Decoy Font Tricks AI but Not Robust](https://www.mixfont.com/experiments/decoy-font) ⭐️ 6.0/10

A font called Decoy Font has been released that displays different text to human readers and to AI/OCR systems by embedding hidden letters within the visible glyphs using subtle pixel-level variations. This experiment highlights the vulnerability of current AI vision models to adversarial typography, but also underscores the ease with which such tricks can be bypassed, questioning their practical utility for security. The font works by combining each letter with a decoy letter, so that the intended message is perceived by humans while OCR or AI reads the decoy. However, community tests show that resizing the image or prompting AI to look for hidden text often reveals the true message.

hackernews · ray__ · Jul 16, 16:18 · [Discussion](https://news.ycombinator.com/item?id=48936584)

**Background**: Adversarial typography is a technique where fonts or text are designed to be misread by machine learning models while remaining legible to humans. This often exploits the way OCR and vision models process pixel-level details differently from human perception. The Decoy Font is a recent example of such an approach, intentionally embedding a secondary message that is only visible when the text is analyzed at different resolutions or with specific prompting.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mixfont.com/experiments/decoy-font">Decoy Font: A TTF font that hides what you type - mixfont.com</a></li>

</ul>
</details>

**Discussion**: Comments generally agree that the font is a cool experiment but not practically useful for stopping AI. Users demonstrated that AI models like GPT-4o can identify the hidden text when asked, and others noted that simple image processing could bypass the effect. There was also some debate about whether the technique is novel or just a variation of existing adversarial examples.

**Tags**: `#font`, `#AI`, `#OCR`, `#adversarial`, `#design`

---

<a id="item-27"></a>
## [Mermaid to ASCII art with WebAssembly and color support](https://simonwillison.net/2026/Jul/16/mermaid-ascii/#atom-everything) ⭐️ 6.0/10

Simon Willison compiled the Go-based mermaid-ascii library to WebAssembly, creating a browser tool that converts Mermaid diagrams to ASCII art with color support, and compared it to a prior Rust-based version. This demonstrates practical use of WebAssembly to run Go code in the browser, enabling client-side rendering of diagrams without server dependencies, and enhances accessibility of Mermaid diagrams by offering colored ASCII output for terminals or text-based environments. The Go library (AlexanderGrooff/mermaid-ascii) supports ANSI color codes, while the earlier Rust version did not. The tool runs entirely in the browser via WebAssembly and includes a web interface for editing and copying the ASCII output.

rss · Simon Willison · Jul 16, 14:57

**Background**: Mermaid is a popular open-source tool that uses a text-based syntax to generate diagrams like flowcharts and sequence diagrams. WebAssembly allows code written in languages like Go and Rust to run in web browsers at near-native performance. ASCII art rendering converts graphical diagrams into text characters, useful for environments without graphical display support.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/AlexanderGrooff/mermaid-ascii">GitHub - AlexanderGrooff/ mermaid - ascii : Render Mermaid graphs...</a></li>
<li><a href="https://tools.simonwillison.net/mermaid-ascii">Mermaid to ASCII art ( mermaid - ascii )</a></li>
<li><a href="https://mermaid.js.org/intro/syntax-reference.html">Diagram Syntax | Mermaid</a></li>

</ul>
</details>

**Tags**: `#mermaid`, `#ascii-art`, `#webassembly`, `#go`, `#rust`

---

<a id="item-28"></a>
## [Mermaid diagrams rendered as Unicode box art via WebAssembly](https://simonwillison.net/2026/Jul/16/grok-mermaid/#atom-everything) ⭐️ 6.0/10

Simon Willison created a browser-based tool that converts Mermaid diagram code into Unicode box art using a Rust-based WebAssembly module extracted from Grok's open-source CLI codebase. This tool makes Mermaid diagram rendering accessible directly in the terminal or any text environment without needing a graphical viewer, benefiting developers who work in terminal-centric workflows or need accessibility-friendly diagram output. The tool is hosted at tools.simonwillison.net and was built using Claude Code for Web (Fable 5) with a prompt to compile the Rust mermaid.rs component to WebAssembly. It includes controls for max width, copy as text, and copy link to diagram.

rss · Simon Willison · Jul 16, 00:33

**Background**: Mermaid is an open-source JavaScript library that allows users to create diagrams and flowcharts using a simple markdown-like syntax. Unicode box art uses box-drawing characters from the Unicode standard to create text-based graphical elements. WebAssembly enables high-performance code written in languages like Rust to run in web browsers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Box-drawing_characters">Box-drawing characters - Wikipedia</a></li>
<li><a href="https://mermaid.live/">Online FlowChart & Diagrams Editor - Mermaid Live Editor</a></li>

</ul>
</details>

**Tags**: `#Mermaid`, `#Unicode`, `#WebAssembly`, `#Rust`, `#Developer Tools`

---

<a id="item-29"></a>
## [Seeking Python Tools for Multi-Objective Surrogate-Based Optimization on Meta-Analysis Data](https://www.reddit.com/r/MachineLearning/comments/1uxty9v/best_current_tools_for_multiobjective/) ⭐️ 6.0/10

A user on Reddit asks for the best current Python tools for multi-objective surrogate-based optimization (MOSBO) applied to physiological data from a meta-analysis of approximately 40 studies, with a need for hierarchical modeling and continuous optimization under constraints. This question highlights the growing need for accessible, Colab-compatible optimization workflows in applied fields like physiology, where practitioners often lack deep programming expertise but require sophisticated multi-objective optimization from heterogeneous data. The user specifically mentions candidates such as PyMC for hierarchical modeling, pymoo/pysamoo for surrogate-assisted optimization, and SMT for surrogates, and notes constraints like physiological plausibility and the need for fine-grained continuous outputs rather than discrete study parameters.

reddit · r/MachineLearning · /u/BleakReason · Jul 16, 05:43

**Background**: Multi-objective surrogate-based optimization (MOSBO) combines surrogate models (e.g., Gaussian processes) to approximate expensive objective functions with multi-objective optimization algorithms (e.g., NSGA-II). Tools like pysamoo extend the pymoo framework to handle expensive evaluations. The user's meta-analysis context adds complexity due to hierarchical structure and domain-specific constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://anyoptimization.com/projects/pysamoo/">pysamoo: Surrogate-Assisted Multi-objective Optimization</a></li>
<li><a href="https://smt.readthedocs.io/">SMT : Surrogate Modeling Toolbox — SMT 2.14.2.dev1+g0d3602a74...</a></li>

</ul>
</details>

**Tags**: `#multi-objective optimization`, `#surrogate-based optimization`, `#hierarchical modeling`, `#meta-analysis`, `#Python tools`

---