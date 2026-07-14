---
layout: default
title: "Horizon Summary: 2026-07-14 (EN)"
date: 2026-07-14
lang: en
---

> From 28 items, 14 important content pieces were selected

---

1. [Datasette code-frequency chart shows AI's impact on development velocity](#item-1) ⭐️ 8.0/10
2. [Chain of Thought as scaling trap; latent reasoning as next wave](#item-2) ⭐️ 8.0/10
3. [GPUHedge slashes serverless GPU cold start latency by 74%](#item-3) ⭐️ 8.0/10
4. [Build and Ship Mac/iOS Apps Without Ever Opening Xcode](#item-4) ⭐️ 7.0/10
5. [Apple's SpeechAnalyzer API Benchmarked Against Whisper](#item-5) ⭐️ 7.0/10
6. [California bill targets infinite scroll as addictive design](#item-6) ⭐️ 7.0/10
7. [Sega CD Silpheed: Art & Engineering Analysis](#item-7) ⭐️ 7.0/10
8. [DOOMQL: SQLite as Game Engine for a Doom-like Game](#item-8) ⭐️ 7.0/10
9. [LLM Agents Should Never Be Directly Responsible Individuals](#item-9) ⭐️ 7.0/10
10. [Anthropic Extends Claude Fable 5 Access Amid Compute Constraints](#item-10) ⭐️ 7.0/10
11. [Open-source tool filters arXiv papers by personal research interests](#item-11) ⭐️ 7.0/10
12. [J-Space Entropy Tested as Error Predictor on Qwen3-4B](#item-12) ⭐️ 7.0/10
13. [Zer0Fit MCP Server Wraps Google TabFM and TimesFM for Zero-Shot ML](#item-13) ⭐️ 7.0/10
14. [Prompt-Engineering Paper at ICML Stirs Debate on Rigor](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Datasette code-frequency chart shows AI's impact on development velocity](https://simonwillison.net/2026/Jul/13/datasette-code-frequency/#atom-everything) ⭐️ 8.0/10

Simon Willison published a blog post analyzing the GitHub code frequency chart for his project Datasette, highlighting a dramatic spike in code additions and deletions in 2026 corresponding to his use of advanced AI coding agents like Opus 4.8, GPT-5.5, Fable 5, and GPT-5.6 Sol. This provides empirical evidence that AI-assisted coding tools can dramatically increase developer output, as seen in the largest spike of 37,022 additions and 9,528 deletions in a single week. It sparks discussion on how AI is transforming software engineering productivity. The chart shows green addition bars and red deletion bars per week from 2018 to 2026, with the biggest spike of 37,022 additions and -9,528 deletions in 2026. Other notable spikes include 14,638 additions in late 2025 and a deletion spike of -10,658 in mid-2020.

rss · Simon Willison · Jul 13, 21:45

**Background**: GitHub code frequency charts visualize the volume of code changes over time, showing additions and deletions per week. Simon Willison is the creator of Datasette, an open-source tool for exploring and publishing data. The chart illustrates how AI coding agents, which can generate and modify code autonomously, have amplified his development pace.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2604.16323">Beyond the ‘Diff’: Addressing Agentic Entropy in Agentic Software ...</a></li>
<li><a href="https://cursor.com/">Cursor: AI coding agent</a></li>

</ul>
</details>

**Tags**: `#AI-assisted coding`, `#software development`, `#GitHub`, `#Datasette`, `#productivity`

---

<a id="item-2"></a>
## [Chain of Thought as scaling trap; latent reasoning as next wave](https://www.reddit.com/r/MachineLearning/comments/1uviru5/chain_of_thought_is_a_scaling_trap_the_next_wave/) ⭐️ 8.0/10

A Reddit post argues that Chain of Thought reasoning is a scaling trap due to faithfulness and cost issues, and proposes latent reasoning methods like Coconut, HRM, and RecursiveMAS as the next wave, while also discussing the interpretability challenge and the need for outer loop governance. This critique challenges the dominant Chain of Thought paradigm in LLM reasoning, highlighting its fundamental limitations and pointing toward emerging latent reasoning architectures that could reduce cost and improve scalability, but also raise new governance concerns for high-stakes applications. Latent reasoning methods such as Coconut use continuous latent space for tree-like search, HRM separates slow planning from fast execution, and RecursiveMAS enables recursive multi-agent collaboration via latent embeddings; however, these methods create a black box that may require an outer governance layer with DAG-based verification and deterministic checks.

reddit · r/MachineLearning · /u/meowsterpieces · Jul 13, 17:50

**Background**: Chain of Thought (CoT) is a prompting technique that improves LLM reasoning by generating intermediate steps in text, but it suffers from faithfulness issues where the text does not reflect the model's actual computation, and cost issues from longer token sequences. Latent reasoning methods aim to perform reasoning in hidden states instead of text, potentially reducing cost and enabling deeper recursion, but they sacrifice interpretability. The post frames CoT as an interface artifact rather than a scalable reasoning path.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2412.06769">Training Large Language Models to Reason in a Continuous Latent ...</a></li>
<li><a href="https://arxiv.org/abs/2506.21734">[2506.21734] Hierarchical Reasoning Model</a></li>
<li><a href="https://arxiv.org/abs/2604.25917">[2604.25917] Recursive Multi-Agent Systems - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#chain-of-thought`, `#latent reasoning`, `#LLM scaling`, `#faithfulness`, `#reasoning architectures`

---

<a id="item-3"></a>
## [GPUHedge slashes serverless GPU cold start latency by 74%](https://www.reddit.com/r/MachineLearning/comments/1uvlb6h/gpuhedge_hedging_serverless_gpu_providers/) ⭐️ 8.0/10

GPUHedge is an open-source library that reduces serverless GPU cold start p95 latency from 117 seconds to 30 seconds by speculatively executing requests across multiple providers and cancelling slower ones. Cold start latency is a critical bottleneck for serverless GPU inference, especially for large AI models. GPUHedge's hedging approach offers a practical solution that significantly improves user experience and reduces costs, potentially making serverless GPU more viable for production workloads. In a benchmark using RunPod as primary and Cerebrium as backup with a 10-second hedge trigger, GPUHedge reduced p95 latency from 116.6s to 29.4s, eliminated all requests over 60 seconds, and lowered modeled active-compute cost from $0.0114 to $0.0083 per request. The project is in alpha and Apache 2.0 licensed.

reddit · r/MachineLearning · /u/Putrid_Construction3 · Jul 13, 19:20

**Background**: Serverless GPU providers load AI models on demand, leading to cold start delays that can exceed a minute for large models. Hedging is a technique used in distributed systems where redundant requests are sent and the first successful response is used, with others cancelled. GPUHedge applies this concept across multiple GPU providers, using policy engines to decide when to launch backups.

<details><summary>References</summary>
<ul>
<li><a href="https://www.beam.cloud/blog/top-serverless-gpu-providers">The Top Serverless GPU Providers in 2025, Ranked by Cold Start</a></li>
<li><a href="https://www.spheron.network/blog/gpu-cold-start-llm-inference-2026/">GPU Cold Start on Serverless LLM Inference: 4 Fixes That Actually Work ...</a></li>

</ul>
</details>

**Tags**: `#serverless GPU`, `#cold start`, `#latency optimization`, `#hedging`, `#AI inference`

---

<a id="item-4"></a>
## [Build and Ship Mac/iOS Apps Without Ever Opening Xcode](https://scottwillsey.com/building-and-shipping-mac-and-ios-apps-without-ever-opening-xcode/) ⭐️ 7.0/10

A developer shares a workflow using command-line tools and automation (e.g., xcodebuild, fastlane) to build, sign, notarize, and distribute Mac and iOS apps without ever launching the Xcode GUI. This approach enables integration with CI/CD pipelines, LLM-based coding agents, and custom automation scripts, potentially reducing manual GUI dependencies for Apple developers. It also raises security concerns as it may require running agents with elevated privileges. The workflow typically uses xcodebuild for building, codesign for signing, and altool or notarytool for notarization. Community members also mention alternative projects like xtool (cross-platform iOS building from Linux) and Axiom (LLM-oriented Apple development tools).

hackernews · speckx · Jul 13, 18:22 · [Discussion](https://news.ycombinator.com/item?id=48896665)

**Background**: Xcode is Apple's integrated development environment (IDE) for macOS and iOS app development. Command-line tools like xcodebuild have long existed but are often underutilized by developers. Automation tools like fastlane further streamline the build, test, and deployment process. The recent rise of AI coding agents has renewed interest in GUI-free workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/library/archive/technotes/tn2339/_index.html">Technical Note TN2339: Building from the Command Line with Xcode FAQ</a></li>
<li><a href="https://fastlane.tools/">fastlane - App automation done right</a></li>
<li><a href="https://www.tricentis.com/learn/xcodebuild-ios-command-line-ci-cd">How to build iOS apps from the command line with xcodebuild</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights security risks: one commenter worries about running agents without sandboxing, citing a past incident where xAI uploaded a user's home directory including SSH keys. Others share alternative tools like xtool for cross-platform iOS development from Linux and Axiom for LLM-friendly Apple development.

**Tags**: `#iOS development`, `#macOS development`, `#Xcode`, `#automation`, `#developer tools`

---

<a id="item-5"></a>
## [Apple's SpeechAnalyzer API Benchmarked Against Whisper](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 7.0/10

Apple released the on-device SpeechAnalyzer API in April 2024, and benchmark tests show it is faster than OpenAI's Whisper Small model but with a slight accuracy trade-off. This API could shift the speech recognition landscape by enabling real-time, private on-device transcription without cloud costs, potentially disrupting third-party transcription services that rely on cloud APIs. SpeechAnalyzer supports streaming transcription, providing immediate feedback as users speak, unlike many models that require full audio before returning text. It operates entirely on-device, ensuring user privacy and eliminating per-call fees.

hackernews · get-inscribe · Jul 13, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48894752)

**Background**: Speech recognition systems convert spoken language into text. OpenAI's Whisper is a widely used open-source model known for robustness, but it typically runs on servers. Apple's previous speech APIs were on-device but less capable. SpeechAnalyzer is a new module in iOS 26's Speech framework that improves speed and introduces streaming.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/speech/speechanalyzer">SpeechAnalyzer | Apple Developer Documentation</a></li>
<li><a href="https://digitechbytes.com/emerging-consumer-tech-explained/apple-s-new-speechanalyzer-api-benchmarked-against-whisper-and-its-predecessor/">Apple's New SpeechAnalyzer API, Benchmarked Against Whisper And Its ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Whisper_(speech_recognition_system)">Whisper (speech recognition system) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Whisper may not be the state-of-the-art benchmark; models like Nvidia's Nemotron and Parakeet, Mistral's Voxtral, and Cohere Transcribe are more current. Others praised SpeechAnalyzer's streaming support as a major UX improvement and speculated that Apple might build a native recorder app, threatening paid Whisper wrappers.

**Tags**: `#Apple`, `#Speech Recognition`, `#API`, `#Whisper`, `#Benchmark`

---

<a id="item-6"></a>
## [California bill targets infinite scroll as addictive design](https://www.sfgate.com/politics/article/meta-social-media-teenagers-22337724.php) ⭐️ 7.0/10

A proposed California law seeks to restrict addictive features in social media, such as infinite scroll, requiring platforms to disclose and limit design elements that maximize user engagement at the expense of well-being. If passed, this law could reshape UI design standards across the tech industry, forcing companies to replace infinite scroll with pagination or other less addictive patterns, potentially reducing excessive screen time and protecting vulnerable users like teenagers. The bill specifically targets 'addictive feeds' that use infinite scroll or autoplay, and would require platforms to provide a non-addictive version by default for minors. The law has sparked debate on where to draw the line between good user experience and manipulative design.

hackernews · Stratoscope · Jul 13, 18:53 · [Discussion](https://news.ycombinator.com/item?id=48897104)

**Background**: Infinite scrolling is a web design technique that automatically loads new content as the user scrolls down, eliminating the need for pagination. Critics argue that this pattern, along with other addictive design elements like autoplay videos and pull-to-refresh, exploits psychological vulnerabilities to keep users engaged longer than intended, contributing to mental health issues.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Infinite_scrolling">Infinite scrolling</a></li>
<li><a href="https://en.wikipedia.org/wiki/Addiction_by_Design">Addiction by Design</a></li>

</ul>
</details>

**Discussion**: Comments debate the boundary between addictive features and good UX, with some arguing that infinite scroll is clearly unnecessary and designed to keep users on apps longer, while others worry about overregulation. A prominent suggestion is to ban targeted advertising as the root cause of addictive design.

**Tags**: `#social media regulation`, `#infinite scroll`, `#UX design`, `#tech policy`, `#addictive design`

---

<a id="item-7"></a>
## [Sega CD Silpheed: Art & Engineering Analysis](https://fabiensanglard.net/silpheed/index.html) ⭐️ 7.0/10

Fabien Sanglard published a detailed technical analysis of the Sega CD game Silpheed, explaining how it used full-motion video (FMV) tricks to simulate 3D graphics on limited hardware. This analysis highlights the engineering ingenuity behind retro game development, showing how developers pushed the Sega CD beyond its capabilities. It offers valuable lessons for modern game optimization and nostalgic appreciation. The article details how Silpheed pre-rendered 3D sequences into FMV and synced player input with video playback, creating an illusion of real-time 3D. It also notes the game's use of the Sega CD's extra memory for smooth playback.

hackernews · ibobev · Jul 13, 14:52 · [Discussion](https://news.ycombinator.com/item?id=48893639)

**Background**: The Sega CD (Mega-CD) was an add-on for the Sega Genesis that used CD-ROMs for larger storage, enabling full-motion video (FMV) games. However, it lacked 3D rendering hardware, so developers often used FMV tricks to create 3D-like visuals. Silpheed is a notable example that combined FMV with gameplay to appear polygonal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fmvworld.com/console_segacd.html">Games for Sega CD | FMV Games List - FMV World</a></li>
<li><a href="https://segadoes.com/2017/11/08/5-fmv-sega-cd-games-that-dont-suck/">5 FMV Sega CD Games that Don't Suck! - Sega Does</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article and shared additional insights, such as demo scene achievements on the Mega Drive (e.g., Overdrive 2) and similar FMV tricks in other games. Some noted Silpheed's impressive visuals but criticized its weak gameplay. A few pointed out this was a repost of an older article.

**Tags**: `#retro gaming`, `#Sega CD`, `#game development`, `#technical deep-dive`, `#optimization`

---

<a id="item-8"></a>
## [DOOMQL: SQLite as Game Engine for a Doom-like Game](https://simonwillison.net/2026/Jul/13/doomql/#atom-everything) ⭐️ 7.0/10

Peter Gostev built DOOMQL, a Doom-like game where SQLite handles all game logic including movement, collision, enemy AI, and rendering via a recursive CTE ray tracer, using Python and GPT-5.6 Sol. This project showcases a novel and creative use of SQLite as a full game engine, demonstrating that a relational database can handle real-time rendering and game state management. It highlights the versatility of SQLite and inspires experimentation with database-driven applications beyond traditional use cases. The game is implemented as a Python terminal script that creates a SQLite database holding all game state, and includes a massive SQL query implementing a full ray tracer using a recursive CTE. Users can also view the game live in a Datasette app that queries the same database for a minimap and pixel display.

rss · Simon Willison · Jul 13, 22:34

**Background**: SQLite is a lightweight, embedded relational database management system widely used for local storage in applications. Recursive Common Table Expressions (CTEs) are a SQL feature that allows queries to refer to themselves, enabling complex computations like ray tracing within a database. GPT-5.6 Sol is OpenAI's latest flagship model, described as its best coding model.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#Doom`, `#game engine`, `#Python`, `#experimental`

---

<a id="item-9"></a>
## [LLM Agents Should Never Be Directly Responsible Individuals](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 7.0/10

Simon Willison defines Directly Responsible Individuals (DRI) via the GitLab handbook and argues that LLM-powered agents should never serve as DRIs because accountability is uniquely human. This opinion piece connects a key software engineering accountability concept to the rapid rise of AI agents, raising important ethical and management questions about who bears responsibility for AI-driven outcomes. The term DRI originated at Apple and is defined in the GitLab handbook as the person ultimately accountable for a project's success or failure. Willison references a 1979 IBM training slide stating that a computer can never be held accountable and thus must never make a management decision.

rss · Simon Willison · Jul 12, 23:57

**Background**: Directly Responsible Individual (DRI) is a concept popularized by Apple to assign clear ownership and accountability for a project or initiative. In software engineering, the DRI has final decision-making authority and is answerable for outcomes. LLM-powered agents are AI systems that can autonomously perform tasks, but they lack human moral and legal accountability.

<details><summary>References</summary>
<ul>
<li><a href="https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals/">Directly Responsible Individuals (DRI) - The GitLab Handbook</a></li>

</ul>
</details>

**Tags**: `#DRI`, `#accountability`, `#AI agents`, `#software engineering`, `#GitLab`

---

<a id="item-10"></a>
## [Anthropic Extends Claude Fable 5 Access Amid Compute Constraints](https://simonwillison.net/2026/Jul/12/bump/#atom-everything) ⭐️ 7.0/10

Anthropic has once again extended access to its most capable model, Claude Fable 5, on paid plans through July 19, citing compute constraints, while OpenAI removed usage limits for GPT-5.6 Sol and reports 6 million active users. This highlights the competitive pressure on Anthropic to ensure consistent access to its best models, as users may migrate to OpenAI's GPT-5.6 Sol due to availability uncertainty. The compute constraint issue affects pricing and accessibility for developers and enterprises relying on frontier AI models. Claude Fable 5 users on Max plans can use up to half their weekly limit on Fable 5, and then continue with usage credits or switch models. Meanwhile, OpenAI's GPT-5.6 Sol is described as more efficient, using fewer tokens and costing about one-third less than Fable 5 on coding benchmarks.

rss · Simon Willison · Jul 12, 21:20

**Background**: Claude Fable 5 is Anthropic's most capable generally available model, designed for ambitious, long-running, asynchronous tasks. GPT-5.6 Sol is OpenAI's latest model, particularly strong in coding and cybersecurity. Compute constraints refer to the limited availability of computing resources needed to serve these large models, which can necessitate usage caps or price adjustments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT - 5 . 6 - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#GPT-5`, `#compute constraints`

---

<a id="item-11"></a>
## [Open-source tool filters arXiv papers by personal research interests](https://www.reddit.com/r/MachineLearning/comments/1uvcdf7/hundreds_of_papers_hit_arxiv_every_day_and_maybe/) ⭐️ 7.0/10

A developer released Research Radar, an open-source tool that daily fetches new arXiv papers, scores their abstracts against a user-defined research interests file, and generates detailed summaries for top-scoring papers. This tool addresses the common problem of information overload for researchers, saving time by surfacing only relevant papers from the hundreds posted daily on arXiv. The tool uses a two-stage model pipeline: a cheap model for batch scoring abstracts and a strong model for deep reading of top papers, with a model-agnostic backend supporting local models via Ollama/vLLM.

reddit · r/MachineLearning · /u/usedtobreath · Jul 13, 13:59

**Background**: arXiv is an open-access repository of scientific preprints in fields like physics, computer science, and mathematics, with about 24,000 new submissions per month. Researchers often spend significant time scanning daily listings to find relevant papers, and existing newsletters or recommendation systems may not tailor to individual interests.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv_(identifier)">ArXiv (identifier)</a></li>
<li><a href="https://info.arxiv.org/help/rss.html">RSS Feeds - arXiv info</a></li>

</ul>
</details>

**Tags**: `#arXiv`, `#research tools`, `#machine learning`, `#NLP`, `#open source`

---

<a id="item-12"></a>
## [J-Space Entropy Tested as Error Predictor on Qwen3-4B](https://www.reddit.com/r/MachineLearning/comments/1uv5l75/evaluating_jspace_entropy_as_an_error_predictor/) ⭐️ 7.0/10

A study evaluates J-space (workspace) entropy as an error predictor on Qwen3-4B across ~11,400 examples from seven datasets, finding it complements output confidence for factual recall but fails on internalized misconceptions and is highly task-dependent. This work provides a nuanced empirical test of J-space entropy, a proposed interpretability signal, showing it is not a general-purpose hallucination detector but may serve as a complementary routing signal for confidently incorrect factual answers. It highlights the importance of cross-model validation and task-specific calibration. The study uses Qwen3-4B on TriviaQA, PopQA, NQ-Open, TruthfulQA, HotpotQA, GSM8K, and CommonSenseQA. Key findings: workspace entropy can improve error-routing precision at low review budgets for highly confident factual answers, but fails on TruthfulQA (internalized misconceptions) and is task-dependent; multiple-choice formatting weakens the signal.

reddit · r/MachineLearning · /u/dasjomsyeet · Jul 13, 08:27

**Background**: J-space (Jacobian lens workspace) is an interpretability technique from Anthropic that reads out internal activations in language models to reveal what they are disposed to say. Entropy in this workspace was hypothesized to indicate uncertain or hallucinated outputs. The Jacobian lens uses the Jacobian of logits with respect to activations to inspect verbalizable representations inside the model.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/global-workspace">A global workspace in language models \ Anthropic</a></li>
<li><a href="https://github.com/anthropics/jacobian-lens">GitHub - anthropics/ jacobian - lens : Companion code for the global...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#interpretability`, `#error detection`, `#language models`, `#entropy`

---

<a id="item-13"></a>
## [Zer0Fit MCP Server Wraps Google TabFM and TimesFM for Zero-Shot ML](https://www.reddit.com/r/MachineLearning/comments/1uue8cc/zer0fit_i_took_googles_new_tabfm_timesfm_ml/) ⭐️ 7.0/10

A grad student released Zer0Fit, an open-source MCP server that wraps Google's TabFM and TimesFM foundation models, enabling zero-shot classification, regression, and time-series forecasting through a chat interface like Open WebUI. It achieves 94.7% accuracy on Iris classification and an R2 of 0.91 on California housing regression without any fine-tuning. This project lowers the barrier to applying advanced ML models by integrating them into the MCP ecosystem, allowing LLM agents to perform ML tasks without training or tuning. It demonstrates a practical use of Google's new tabular and time-series foundation models in an accessible, containerized tool. Zer0Fit runs in a single Docker container, requires about 16GB VRAM (CUDA-only via PyTorch), and dynamically loads/unloads models with a 5-minute TTL. It currently supports CSV input; future support for XLS, XLSX, JSON, and JSONL is planned.

reddit · r/MachineLearning · /u/Porespellar · Jul 12, 12:32

**Background**: TabFM and TimesFM are foundation models from Google Research for tabular data classification/regression and time-series forecasting, respectively. They are designed for zero-shot inference, meaning they can make predictions on new datasets without task-specific training. The Model Context Protocol (MCP) is an open standard that connects AI models with external tools and data sources, often used with LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/introducing-tabfm-a-zero-shot-foundation-model-for-tabular-data/">Introducing TabFM : A zero-shot foundation model for tabular data</a></li>
<li><a href="https://github.com/google-research/timesfm">GitHub - google -research/ timesfm : TimesFM ( Time Series...)</a></li>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#TimesFM`, `#TabFM`, `#zero-shot learning`, `#ML engineering`

---

<a id="item-14"></a>
## [Prompt-Engineering Paper at ICML Stirs Debate on Rigor](https://www.reddit.com/r/MachineLearning/comments/1uv1xb3/promptengineering_paper_accepted_to_icml_r/) ⭐️ 6.0/10

A paper titled 'Verbalized Sampling: How to Mitigate Mode Collapse and Unlock LLM Diversity' was accepted to ICML. It introduces a simple prompt-engineering strategy to increase output diversity, but critics argue it lacks theoretical rigor and may not belong at a top-tier venue. This highlights a growing tension in the machine learning community between empirical prompt-engineering work and traditional theoretical research. The acceptance at ICML signals a potential shift in what is considered publishable at top conferences, affecting researchers, reviewers, and the direction of the field. The paper tackles mode collapse—a phenomenon where LLMs produce repetitive outputs after alignment. Verbalized Sampling works by prompting the model to first generate a distribution over possible responses before sampling, a training-free method. The debate centers on whether such prompt-engineering tricks require rigorous theoretical justification for acceptance at ICML.

reddit · r/MachineLearning · /u/Mean_Revolution1490 · Jul 13, 05:00

**Background**: Mode collapse in LLMs refers to the reduction in output diversity after RLHF alignment. Prompt engineering involves crafting input prompts to steer model behavior without updating weights. ICML is a premier venue for machine learning research, traditionally emphasizing theoretical contributions and rigorous empirical validation.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@JacksonAAaron/verbalized-sampling-the-ai-strategy-solving-repetition-bias-and-boring-chatbots-82ba5a8a8198">Verbalized Sampling : The AI Strategy Fixing Slop | Medium</a></li>
<li><a href="https://www.emergentmind.com/topics/semantic-mode-collapse">Semantic Mode Collapse in Generative Models</a></li>
<li><a href="https://arxiv.org/html/2510.01171">Verbalized Sampling: How to Mitigate Mode Collapse and Unlock LLM...</a></li>

</ul>
</details>

**Discussion**: The Reddit thread expresses mixed opinions. Some agree that prompt-engineering work should be in less technical venues, while others argue that such empirical innovations are part of 'modern machine learning' and deserve recognition. There is also discussion about the lack of theoretical analysis and whether the paper's contribution is significant enough.

**Tags**: `#prompt-engineering`, `#ICML`, `#machine-learning`, `#research-standards`, `#LLM`

---