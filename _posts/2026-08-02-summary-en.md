---
layout: default
title: "Horizon Summary: 2026-08-02 (EN)"
date: 2026-08-02
lang: en
---

> From 35 items, 17 important content pieces were selected

---

1. [ByteDance's Seedance 2.5 Boosts One-Take AI Video With Flexible Referencing](#item-1) ⭐️ 8.0/10
2. [Diátaxis: A Systematic Framework for Technical Documentation](#item-2) ⭐️ 8.0/10
3. [Lean Kernel Soundness Bug #14576 Postmortem Highlights Limits of Formal Verification](#item-3) ⭐️ 8.0/10
4. [Google's Actions Accelerated RSS Decline, Article Argues](#item-4) ⭐️ 8.0/10
5. [Ten advances in mathematics and theoretical computer science](#item-5) ⭐️ 8.0/10
6. [DeepSeek V4-Flash-0731: 304B-parameter model with enhanced agentic skills](#item-6) ⭐️ 8.0/10
7. [Stateless MCP 2.0 reinvigorates the protocol](#item-7) ⭐️ 8.0/10
8. [Reddit user trains encoder-only transformer to predict personal blood glucose](#item-8) ⭐️ 8.0/10
9. [Go Network Symmetry Study Shows Surprising Internal Structure](#item-9) ⭐️ 8.0/10
10. [VLM Benchmarks Reward Empty Reports While Erasing Clinical Terms in Chest X-Rays](#item-10) ⭐️ 8.0/10
11. [AI Financial Advice Surprises, But Good Prompts Are Key](#item-11) ⭐️ 7.0/10
12. [Simon Willison Releases llm-mcp-client 0.1a0](#item-12) ⭐️ 7.0/10
13. [Simon Willison on Oxide and Friends: Open Weight Revolution](#item-13) ⭐️ 7.0/10
14. [smevals: A Small Open-Source Eval Suite for Models and Prompts](#item-14) ⭐️ 7.0/10
15. [The Art of 64-bit Assembly Draws Praise and Debate Over AI-Generated Content](#item-15) ⭐️ 6.0/10
16. [Greg Brockman on Why People Dislike AI-Initiated Requests at Work](#item-16) ⭐️ 6.0/10
17. [Datasette Agent 0.4a0 Lets Tools Run in the Browser](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [ByteDance's Seedance 2.5 Boosts One-Take AI Video With Flexible Referencing](https://seed.bytedance.com/en/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5) ⭐️ 8.0/10

ByteDance has announced Seedance 2.5, its latest AI video generation model, which introduces one-take creation and flexible referencing for producing longer, high-quality videos. The release builds on the Seedance series' focus on multimodal input and stronger prompt following. Seedance 2.5 is significant because it targets two pain points in AI filmmaking: output length and creative control via references. It intensifies competition among video-generation models and may push rivals to add similar reference-and-control workflows. The model highlights one-take creation, meaning a complete video segment can be generated in a single pass, alongside flexible referencing that lets creators steer content using reference images or video. Community observations suggest the release page emphasizes text-to-video action and high-effect shots, while dialogue-driven or actor-reference scenarios receive less focus.

hackernews · njaremko · Aug 1, 20:45 · [Discussion](https://news.ycombinator.com/item?id=49138302)

**Background**: Seedance is ByteDance's family of AI video generation models. Seedance 2.0, the previous major version, is built on a unified multimodal audio-video joint generation architecture and accepts text, image, audio, and video inputs simultaneously—up to 9 images, 3 video clips, and 3 audio clips per job, with clip lengths from 4 to 15 seconds. Seedance 1.0 already emphasized multi-shot narratives and semantic understanding. 'One-take creation' in this context means generating a finished video clip in one pass rather than assembling multiple shots.

<details><summary>References</summary>
<ul>
<li><a href="https://seeddance.ai/seedance-2-0">Seedance 2.0 — Multimodal AI Video with</a></li>
<li><a href="https://seed.bytedance.com/en/models">Seed Models</a></li>

</ul>
</details>

**Discussion**: Commenters were largely impressed by output quality—one noted that Seedance videos were the first AI-generated footage that genuinely impressed them. Others raised strategic concerns, observing that ByteDance's focus on action and high-effect text-to-video aligns more with Chinese usage demand than Western filmmakers' desire for video-to-video and actor/dialogue control. Some users also asked practical questions about access and noted the high inference cost for creative workflows.

**Tags**: `#AI video generation`, `#ByteDance`, `#Seedance`, `#machine learning`, `#creative tools`

---

<a id="item-2"></a>
## [Diátaxis: A Systematic Framework for Technical Documentation](https://diataxis.fr/) ⭐️ 8.0/10

Diátaxis presents a systematic approach to organizing documentation into four types: tutorials, how-to guides, reference, and explanation. The framework is gaining traction as a standard methodology for software documentation, with an active community and ongoing translation efforts. This framework helps software teams create clearer, more maintainable documentation, directly improving developer experience and reducing long-term documentation drift. Its practical value is evidenced by a strong Hacker News discussion (236 points, 32 comments) where practitioners share real-world successes and caveats. Diátaxis distinguishes four user needs—learning, achieving goals, understanding, and obtaining information—each mapping to one documentation form. The framework also guides documentation process, not just content structure, and author DanieleProcida is working on translating the site into multiple languages.

hackernews · ryanseys · Aug 1, 20:33 · [Discussion](https://news.ycombinator.com/item?id=49138188)

**Background**: Diátaxis, whose name comes from the Ancient Greek dia ('across') and taxis ('arrangement'), is a documentation framework widely adopted in technical writing. It organizes documentation into four quadrants: tutorials (learning-oriented), how-to guides (goal-oriented), reference (information-oriented), and explanation (understanding-oriented). The framework has been used by organizations like Gatsby and Vonage to restructure their documentation. It is often compared to DITA and Information Mapping, but focuses more on matching content types to user needs.

<details><summary>References</summary>
<ul>
<li><a href="https://diataxis.fr/">Diátaxis</a></li>
<li><a href="https://idratherbewriting.com/blog/what-is-diataxis-documentation-framework">What is Diátaxis and should you be using it with your ...</a></li>
<li><a href="https://qiskit.github.io/qiskit_sphinx_theme/intro/diataxis.html">The Diátaxis Framework - Qiskit Docs Guide</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters generally praised Diátaxis; one user called it 'fantastic' for organizing a complex codebase handover, while the author promoted ongoing translation efforts. However, users also noted that documentation maintenance remains difficult, with tutorials and reference prone to drift, and one commenter humorously warned that reading the framework makes all docs look flawed. A practical tip from jamilbk was to read the entire website before undertaking a refactoring.

**Tags**: `#documentation`, `#technical writing`, `#software engineering`, `#diataxis`, `#developer experience`

---

<a id="item-3"></a>
## [Lean Kernel Soundness Bug #14576 Postmortem Highlights Limits of Formal Verification](https://leodemoura.github.io/blog/2026-8-1-postmortem-for-kernel-soundness-bug-14576/) ⭐️ 8.0/10

Lean creator Leonardo de Moura published a postmortem of kernel soundness bug #14576, explaining how the flaw was found and why independent verification still works as long as users run current versions of both checkers. Lean is a widely used proof assistant, so a kernel soundness bug directly affects trust in formal verification results built with it. The postmortem clarifies that verified results are extremely strong but not absolute guarantees, reinforcing the importance of keeping proof-checking tools up to date. The bug is identified as #14576, and the practical consequence is that independently checking proofs still works because exploiting it would require two distinct bugs in two separate implementations. However, users who rely on independent verification must use current versions of both the Lean kernel and the checking tool.

hackernews · juhopitk · Aug 1, 18:32 · [Discussion](https://news.ycombinator.com/item?id=49137060)

**Background**: A proof assistant uses a small, trusted kernel to check every inference step of a formal proof, so kernel soundness is the foundation of trust in the system. Lean is a dependently-typed proof assistant and programming language based on the calculus of inductive constructions; even mature proof assistants occasionally experience soundness bugs. Independent verification, such as checking a proof with a separately implemented checker, is a common way to increase confidence in machine-checked results.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Proof_assistant">Proof assistant - Wikipedia</a></li>
<li><a href="https://people.inf.ethz.ch/fukudak/lect/mssemi/reports/09_rep_PatrickSchnider.pdf">An Introduction to Proof Assistants - ETH Z</a></li>
<li><a href="https://dl.acm.org/doi/epdf/10.1145/3747511">McTT: A Verified Kernel for a Proof Assistant</a></li>

</ul>
</details>

**Discussion**: Commenters broadly agreed that soundness bugs in proof assistants are not surprising and that verified results should be viewed as strong but not absolute guarantees. Some noted the bug was presented as an exploit targeting two proof checkers and suggested broader fixes, while another argued alternative systems like Metamath make such bugs unlikely. One commenter asked whether any bug has allowed proving a genuinely new statement without enabling a direct proof of false, proposing a bounty on proving false to increase trust.

**Tags**: `#Lean`, `#formal verification`, `#soundness`, `#proof assistants`, `#type theory`

---

<a id="item-4"></a>
## [Google's Actions Accelerated RSS Decline, Article Argues](https://openrss.org/blog/how-google-helped-destroy-adoption-of-rss-feeds) ⭐️ 8.0/10

A 2023 article titled "How Google helped destroy adoption of RSS feeds" argues that Google's decisions—shutting down Google Reader in 2013 and de-prioritizing RSS across products—significantly accelerated RSS's decline. The article revisits this history and has sparked widespread commentary about the open web's trajectory. RSS is a cornerstone of the open, decentralized web, and its decline has contributed to today's walled-garden internet dominated by a few platforms. The article highlights how a single company's product decisions can reshape the entire web ecosystem, affecting users, publishers, and developers. The article specifically cites Google Reader's shutdown on July 1, 2013, and the removal of RSS support from other Google products as key turning points. It contends that Google's stated reason of declining usage was dubious, suggesting strategic priorities like promoting Google+ also played a role.

hackernews · pudgywalsh · Aug 1, 18:07 · [Discussion](https://news.ycombinator.com/item?id=49136821)

**Background**: RSS (Really Simple Syndication) is a web feed format that allows users to subscribe to website updates in a standardized XML format, which is then read through a news aggregator or feed reader. Google Reader was one of the most popular RSS readers; its shutdown in 2013 dealt a severe blow to RSS adoption, and the article argues that Google's broader deprioritization of RSS compounded the decline.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RSS_protocol">RSS protocol</a></li>
<li><a href="https://www.huffpost.com/entry/google-reader-shut-down_n_2876252">Google Reader To Shut Down July 1st, Sparking User... | HuffPost Life</a></li>

</ul>
</details>

**Discussion**: Commenters expressed nostalgia for the early internet and criticized today's ad-driven web, with one saying "Google Reader going away felt like the beginning of the end of the internet as I knew it." Others argued RSS is still alive and worth supporting, noting that adding RSS feeds is easy and has minimal resource cost.

**Tags**: `#RSS`, `#Google`, `#Open Web`, `#Web History`, `#Technology Critique`

---

<a id="item-5"></a>
## [Ten advances in mathematics and theoretical computer science](https://simonwillison.net/2026/Aug/1/ten-advances-in-mathematics/#atom-everything) ⭐️ 8.0/10

OpenAI reports its internal 'Astra' model solved ten long-standing mathematical problems for under $2,000 each, though the post notes no data on failed attempts.

rss · Simon Willison · Aug 1, 20:34

**Tags**: `#AI`, `#mathematics`, `#OpenAI`, `#research`, `#LLM`

---

<a id="item-6"></a>
## [DeepSeek V4-Flash-0731: 304B-parameter model with enhanced agentic skills](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek released V4-Flash-0731, a 304B-parameter open-weight model with 'substantially enhanced agentic capabilities'. Priced at $0.14 per million input tokens and $0.27 per million output tokens, Artificial Analysis ranks it ahead of MiniMax M3 (428B) and suggests it may currently be the best value-per-intelligence model on the market. This release matters because it pushes strong agentic performance into a much lower price tier, potentially resetting industry expectations for cost per unit of intelligence in the open-weight LLM market. Developers and enterprises building agentic applications on a budget could be the biggest beneficiaries. The model has 304B parameters and weighs about 167GB on Hugging Face. In Simon Willison's tests, the default reasoning level produced a disappointing image-generation result, but setting the reasoning effort to 'high' via OpenRouter yielded a much better output, showing that output quality is highly sensitive to the reasoning level configured.

rss · Simon Willison · Jul 31, 23:59

**Background**: DeepSeek is a Chinese AI lab known for releasing strong open-weight models such as V3 and R1. 'Agentic capabilities' refer to a model's ability to plan, use tools, and act autonomously in dynamic, open-ended environments rather than merely answering static questions. The Artificial Analysis Intelligence Index is a composite benchmark calculated as a weighted average of production benchmark scores, with agents, coding, general capability, and scientific reasoning each contributing 25%, and is used to compare model 'smartness' across the industry.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index | Artificial Analysis</a></li>
<li><a href="https://paperswithcode.co/paper/2601.12538">Agentic Reasoning for Large Language Models ... | Papers with Code</a></li>
<li><a href="https://ai-search.io/papers/agentic-reasoning-for-large-language-models">Agentic Reasoning for Large Language Models - AI for Dummies...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#LLM`, `#AI`, `#model release`, `#machine learning`

---

<a id="item-7"></a>
## [Stateless MCP 2.0 reinvigorates the protocol](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 8.0/10

MCP 2.0, the 2026-07-28 Model Context Protocol specification, introduces a stateless redesign that simplifies client and server implementations. Simon Willison built two new tools, mcp-explorer and datasette-mcp, to explore the updated protocol. The stateless MCP design significantly lowers implementation complexity, making the protocol more accessible for smaller models and more suitable for scalable web applications. This revival could accelerate AI agent tooling adoption after MCP was overshadowed by Claude Skills. The new stateless approach uses a single HTTP request with headers such as MCP-Protocol-Version, Mcp-Method, and Mcp-Name, eliminating the need for session IDs and server-side state. Legacy MCP required two requests: an initialize call to obtain a session ID, followed by the actual tool call.

rss · Simon Willison · Jul 31, 23:13

**Background**: MCP is an open standard introduced by Anthropic in November 2024 to standardize how AI systems integrate with external tools and data sources. It gained huge traction in 2025 but was later overshadowed by Claude Skills, which seemed more flexible for agent harnesses with terminal access. The stateless redesign is the most significant change since the protocol's launch, addressing complexity and scalability concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>
<li><a href="https://wpnews.pro/news/stateless-mcp-has-recaptured-my-interest-and-inspired-mcp-explorer-and-datasette">Stateless MCP has recaptured my interest (and inspired mcp -explorer...)</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#Model Context Protocol`, `#AI agents`, `#specification`, `#tools`

---

<a id="item-8"></a>
## [Reddit user trains encoder-only transformer to predict personal blood glucose](https://www.reddit.com/r/MachineLearning/comments/1vc1txc/i_have_trained_a_model_to_predict_my_blood_sugar_p/) ⭐️ 8.0/10

In a Reddit post, a developer (u/0xdeadf1sh) describes training encoder-only transformer models, from under 40K to 17M parameters, to forecast his personal blood glucose up to two hours ahead using past glucose, carbohydrates, and insulin data. He published the source code under the MIT license, along with trained weights and evaluation data. This is a notable example of a highly personalized AI health application built by an individual, not a lab, and it applies sophisticated techniques such as DILATE loss and uncertainty quantile prediction to a practical diabetes-management problem. If validated, open-source models like this could lower the barrier for DIY closed-loop insulin systems and CGM-based decision support. The architecture combines DILATE loss to fit the median glucose trajectory with pinball loss for uncertainty bands, merged via a Kendall-Gal approach, and all glucose values are transformed into Kovatchev risk space reparameterized to [40, 400] mg/dL. The largest model has 16 layers and 16 attention heads (~17M parameters); a limitation is that it currently requires announced meals and insulin to make predictions.

reddit · r/MachineLearning · /u/0xdeadf1sh · Jul 31, 20:09

**Background**: Continuous glucose monitors (CGMs) provide frequent blood glucose readings, and people with diabetes often manually track carbohydrate intake and insulin doses. Predicting future glucose levels is difficult because glucose dynamics are non-stationary and depend on meal timing, insulin action, and individual physiology. DILATE is a loss function for time-series forecasting that penalizes both shape error and temporal misalignment, making it suitable for predicting sudden changes. The OhioT1DM dataset, collected from people with type 1 diabetes, is commonly used as a benchmark for blood glucose prediction algorithms. Kovatchev's risk space is a log-transform that emphasizes clinically risky glucose ranges.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/1909.09020">Shape and Time Distortion Loss for Training Deep Time Series ... Shape and Time Distortion Loss for Training Deep Time Series ... Shape and Time Distortion Loss for Training Deep Time Series ... GitHub - vincent-leguen/DILATE: Code for our NeurIPS 2019 ... Re: Shape and Time Distortion Loss for Training Deep Time ... Deep Time Series Forecasting with Shape and Temporal Criteria DILATE: DIstortion Loss with shApe and tImE - GitHub</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC7881904/">The OhioT 1 DM Dataset for Blood Glucose Level Prediction : Update...</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12848927/">Glucose dysregulation and glycemic phenotyping in chronic migraine...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#transformers`, `#healthcare`, `#time-series`, `#blood glucose prediction`

---

<a id="item-9"></a>
## [Go Network Symmetry Study Shows Surprising Internal Structure](https://www.reddit.com/r/MachineLearning/comments/1vcrki2/how_symmetric_are_the_insides_of_a_go_network_r/) ⭐️ 8.0/10

The author of the open-source Go engine KataGo published a study examining whether neural networks learn orientation-independent internal representations of the Go board. Despite training with only stochastic eight-fold rotation/reflection augmentation, the networks appear to develop partially symmetric concepts, and one finding was unexpected. This research offers a rare look inside a superhuman Go model, an area where interpretability is still largely unexplored. Understanding how and why networks exploit symmetry could inform data augmentation strategies and architectural choices for other board-game or spatial AI systems. The write-up is intentionally accessible and was produced with heavy AI assistance under detailed human direction, with code linked from the study page. The author cautions that this is a small, single drop in the broader interpretability research bucket.

reddit · r/MachineLearning · /u/icosaplex · Aug 1, 16:18

**Background**: In Go, the board is fully symmetric under rotations and reflections, so the same position can be viewed in eight equivalent orientations. KataGo is a strong open-source Go engine trained by self-play and distributed computing, similar in spirit to AlphaZero. During training, each batch is randomly rotated and reflected to encourage the model not to depend on orientation, but the symmetry is never explicitly enforced. This study probes how much of that orientation independence the network actually internalizes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KataGo">KataGo</a></li>
<li><a href="https://grokipedia.com/page/KataGo">KataGo</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#interpretability`, `#symmetry`, `#Go`, `#KataGo`

---

<a id="item-10"></a>
## [VLM Benchmarks Reward Empty Reports While Erasing Clinical Terms in Chest X-Rays](https://www.reddit.com/r/MachineLearning/comments/1vcipzz/vlms_can_score_well_on_benchmarks_while_silently/) ⭐️ 8.0/10

Researchers discovered that current evaluation metrics for vision-language models (VLMs) in chest x-ray report generation reward repetitive templates and 'normal' reports lacking clinical terms. Their new framework explicitly measures the erasure of clinically meaningful terminology and the introduction of biased terms, as described in the paper 'Measuring What VLMs Don't Say' (arXiv:2603.01625). This matters because high benchmark scores may hide clinically useless or misleading radiology reports, threatening patient safety and trust in medical AI. It calls for more clinically-grounded evaluation metrics to ensure generated reports preserve precise terminology. The framework targets both term erasure (silent omission of rare but clinically meaningful words) and hallucinated bias (introduction of spurious associations). The authors argue that existing metrics like BLEU and CIDEr fail to capture these failures, making repeated 'normal' templates score highly.

reddit · r/MachineLearning · /u/ade17_in · Aug 1, 09:27

**Background**: Vision-language models combine computer vision and natural language processing to interpret medical images and generate textual reports. In radiology, these models often use encoder-decoder architectures and are evaluated with generic text-generation metrics, which reward lexical overlap rather than clinical correctness. Related work such as RaTEScore (2024) proposes entity-aware evaluation that emphasizes diagnostic outcomes and anatomy, while recent studies define 'erasure harms' as systematic omission of important terms in model outputs.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2403.02469">Vision - Language Models for Medical Report</a></li>
<li><a href="https://arxiv.org/pdf/2606.15815">On Defining Erasure Harms for NLP</a></li>
<li><a href="https://arxiv.org/html/2406.16845v1">RaTEScore: A Metric for Radiology Report Generation - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#VLM`, `#radiology`, `#evaluation metrics`, `#clinical NLP`, `#benchmarking`

---

<a id="item-11"></a>
## [AI Financial Advice Surprises, But Good Prompts Are Key](https://mitsloan.mit.edu/ideas-made-to-matter/ai-financial-advice-surprisingly-good-especially-if-you-ask-right-questions) ⭐️ 7.0/10

MIT Sloan research finds AI-generated financial advice can be unexpectedly effective, particularly when users craft detailed, well-structured questions. The study shows prompt quality significantly influences the usefulness of the recommendations. If AI can reliably provide quality financial guidance, it could democratize access to financial planning tools for millions of people who cannot afford human advisors. However, the dependence on user skill may reinforce existing financial literacy gaps. The research highlights that even small changes in prompt formulation can steer AI toward more accurate or flawed answers. Commenters also note that AI can mishandle nuanced rules, such as the five-year Roth IRA waiting period, showing limits for complex tax decisions.

hackernews · foxtrot8672 · Aug 1, 22:25 · [Discussion](https://news.ycombinator.com/item?id=49139102)

**Background**: Large language models (LLMs) are AI systems trained on vast amounts of text to understand and generate human-like language. Prompt engineering is the practice of structuring inputs to guide these models toward desired outputs, which is central to getting useful financial advice from AI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_engineering">Prompt engineering - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue the general public's financial illiteracy is a bigger issue than AI limitations, while others point out specific factual errors in the AI's advice, like Roth IRA rules. One user reports exceptional results when providing rich personal context, surpassing human professionals, but another questions whether the evaluations reflect real multi-turn usage.

**Tags**: `#AI`, `#finance`, `#financial advice`, `#LLM`, `#personal finance`

---

<a id="item-12"></a>
## [Simon Willison Releases llm-mcp-client 0.1a0](https://simonwillison.net/2026/Jul/31/llm-mcp-client/#atom-everything) ⭐️ 7.0/10

On July 31, 2026, Simon Willison released llm-mcp-client 0.1a0, an initial alpha library for building Model Context Protocol (MCP) clients. The release corresponds to his blog entry on stateless MCP and provides a Python package to simplify client-side MCP integration. As a prominent developer in the LLM space, Willison's library could become a reference implementation for building MCP clients, lowering the barrier for tool integration. It also signals practical adoption of the recently revised stateless MCP specification, potentially influencing the broader AI tooling ecosystem. The package is tagged 0.1a0, indicating an early alpha stage with potentially unstable APIs. It is designed around the stateless MCP approach that became a core feature in the 2026-07-28 protocol revision, and the accompanying blog entry explains the design rationale.

rss · Simon Willison · Jul 31, 23:03

**Background**: The Model Context Protocol (MCP) is an open standard introduced by Anthropic in November 2024 to standardize how AI systems connect to external tools and data sources. A stateless protocol is one where each request is independent and carries all necessary context, simplifying scaling and recovery. In July 2026, the MCP specification received a major revision that made a stateless core part of the protocol, and llm-mcp-client is built to support that new direction.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://en.wikipedia.org/wiki/Stateless_protocol">Stateless protocol</a></li>
<li><a href="https://blog.modelcontextprotocol.io/posts/2026-07-28-release-candidate/">The 2026-07-28 MCP Specification Release Candidate</a></li>

</ul>
</details>

**Tags**: `#llm`, `#model-context-protocol`, `#release`, `#tools`, `#mcp`

---

<a id="item-13"></a>
## [Simon Willison on Oxide and Friends: Open Weight Revolution](https://simonwillison.net/2026/Jul/31/oxide-and-friends/#atom-everything) ⭐️ 7.0/10

Simon Willison joined Bryan Cantrill and Adam Leventhal on the Oxide and Friends podcast to discuss the open weight model revolution, accidental cybersecurity attacks, and an industry open letter on American AI leadership. The conversation also revisited January 2026 predictions and added a new one: the Pope will say something about open models by year's end. The episode captures a pivotal moment where open weight models like Kimi K3 are matching proprietary frontier models, challenging the assumption that only closed labs can lead AI. It frames the ongoing industry debate about openness, security, and American AI leadership for a broad technical audience. Kimi K3 is a 2.8-trillion-parameter open model with a 1-million-token context window, described as the world's first open 3T-class model. The episode notes that DeepSeek V4 Flash and Anthropic's own cyber incident emerged just days after recording, illustrating how fast the field is moving.

rss · Simon Willison · Jul 31, 21:33

**Background**: An open-weight model is an AI model whose trained parameters (weights) are publicly released, allowing anyone to download, run, study, and modify it on their own hardware. This contrasts with proprietary frontier models that are only accessible through vendor APIs. Recent releases such as Kimi K3 from Moonshot AI and DeepSeek V4 Flash show open-weight models rapidly closing the gap with closed frontier systems.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#open weights`, `#AI`, `#podcast`, `#frontier models`, `#industry debate`

---

<a id="item-14"></a>
## [smevals: A Small Open-Source Eval Suite for Models and Prompts](https://simonwillison.net/2026/Jul/31/smevals/#atom-everything) ⭐️ 7.0/10

Simon Willison announced smevals, a new open-source evaluation suite developed with Prime Radiant, which lets users run small eval suites across model configurations and grade the results. The tool is available via `uvx smevals` and supports running, grading, serving, and building static HTML reports. smevals lowers the barrier to building and running custom model evaluations, making it easier for practitioners to compare models, prompts, and agent harnesses. It represents Willison's third iteration on evals tooling, and its integration with coding agents via simple commands could encourage more routine evaluation in AI workflows. An eval is defined as a directory of YAML files, and runs are kept separate from grading operations, which use configurable checks and custom checkers that can even call other models. The tool also includes a localhost web server for exploring results and a `smevals build` command to export static HTML reports.

rss · Simon Willison · Jul 31, 21:15

**Background**: Evaluation harnesses are infrastructure for running evaluations against AI models and routing results for analysis, and they are important both for benchmarking models and for testing production workflows. smevals is a lightweight, YAML-based framework that simplifies creating and running small eval suites, and it runs via uvx, a command runner provided by the uv Python package. This approach contrasts with larger harnesses like EleutherAI's lm-evaluation-harness, which focuses on standardized academic benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/prime-radiant-inc/smevals">GitHub - prime-radiant-inc/ smevals : A framework for running evals ...</a></li>
<li><a href="https://arize.com/blog/what-is-an-evaluation-harness/">What is an evaluation harness? Definition & guide - Arize AI</a></li>
<li><a href="https://github.com/EleutherAI/lm-evaluation-harness">GitHub - EleutherAI/lm-evaluation-harness: A framework for ... Building an Evaluation Harness for Production AI Agents: A 12 ... The evaluation harness: engineering the layer between your AI ... What Is an Evaluation Harness? How LLM Benchmarks Work GitHub - RyanAlberts/best-of-Agent-Harnesses: Curated ...</a></li>

</ul>
</details>

**Tags**: `#evals`, `#AI`, `#model evaluation`, `#open source`, `#tools`

---

<a id="item-15"></a>
## [The Art of 64-bit Assembly Draws Praise and Debate Over AI-Generated Content](https://nostarch.com/art-64-bit-assembly-v2) ⭐️ 6.0/10

A new edition of 'The Art of 64-bit Assembly' has been released by No Starch Press, sparking extensive community discussion on Hacker News. The nearly 800-page book covers x86-64 assembly programming using MASM, but its AI-generated opening passage and choice of tooling have drawn mixed reactions. The discussion underscores that assembly language remains relevant for low-level systems programming, operating systems, and performance-critical code even in an era of high-level languages and AI coding assistants. The controversy also highlights growing community unease about AI-generated content in technical books and about outdated tooling choices in otherwise valuable educational resources. Commenters noted the book is nearly 800 pages and uses Microsoft Macro Assembler (MASM), while experts compared MASM with GNU Assembler (GAS), pointing out GAS lacks features such as while loops and string-processing macros. One reader observed that the book begins with an AI-generated passage despite warning that AI can produce incomplete or bad results, leading to criticism about the publisher's editorial choices.

hackernews · 0x54MUR41 · Aug 1, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49134599)

**Background**: x86-64 is the 64-bit version of the x86 instruction set, used in most desktop and laptop processors, and x86-64 assembly is the human-readable representation of its machine code. Assembly languages allow precise control over hardware and are commonly used in real-time embedded systems, operating-system kernels, and device drivers, and compilers sometimes generate assembly as an intermediate step. Different assemblers, such as MASM and GAS, provide different macro and directive capabilities, which influences which tools developers prefer for learning or writing assembly.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/X86_assembly_language">X86 assembly language</a></li>
<li><a href="https://web.stanford.edu/class/cs107/guide/x86-64.html">CS107 Guide to x86-64 - Stanford University</a></li>
<li><a href="https://gpfault.net/posts/asm-tut-0.txt.html">Let's Learn x86-64 Assembly! Part 0 - Setup and First Steps CS107 Guide to x86-64 - Stanford University X86-64 playground Guide to x86 Assembly - University of Virginia GitHub - LilSuperUser/x86_64-asm-tutorials: x86_64 Assembly ... x86-64 assembly language reference - Brown University</a></li>

</ul>
</details>

**Discussion**: Community sentiment was mixed: some commenters dismissed the discussion as overly focused on meta-issues like the AI-generated marketing copy and tool choices, while others defended assembly as still highly valuable and fun to learn. Technical experts shared detailed comparisons of MASM and GAS, and one reader building a compiler asked for a Linux equivalent of the book. A recurring critique was disappointment with the AI-generated opening, with hopes that the author would replace it with their own words.

**Tags**: `#assembly`, `#books`, `#low-level programming`, `#x86-64`, `#education`

---

<a id="item-16"></a>
## [Greg Brockman on Why People Dislike AI-Initiated Requests at Work](https://simonwillison.net/2026/Aug/1/greg-brockman/#atom-everything) ⭐️ 6.0/10

Greg Brockman observed that many OpenAI employees connect ChatGPT to Slack, but coworkers strongly dislike when a colleague's ChatGPT contacts them asking for help, even though they would happily help the same colleague directly. He noted that this reinforces how much people value human relationships and want AI to give time back or enhance time together rather than become a layer separating people. This insight highlights a crucial social dynamic in human-AI interaction: AI should augment human connections, not mediate or replace them. It has practical implications for how AI assistants are designed for workplace collaboration, reminding developers and companies to prioritize human agency and relationship-preserving features. The observation comes from a tweet by Greg Brockman, President and Co-Founder of OpenAI, and was shared on Simon Willison's blog. The example involves ChatGPT integrated with Slack, raising broader questions about AI-initiated proactivity and the social norms surrounding requests for help.

rss · Simon Willison · Aug 1, 22:29

**Background**: As AI assistants become increasingly embedded in workplace tools like Slack, they can act on behalf of individual employees, including initiating conversations. This quote reflects a growing debate about AI autonomy versus human-centered design. Brockman's point indicates that even at an AI-focused company, people prefer direct human-to-human interaction for help and want AI to augment human time, not become a social intermediary.

**Tags**: `#AI`, `#OpenAI`, `#Human-AI Interaction`, `#AI Ethics`, `#Workplace`

---

<a id="item-17"></a>
## [Datasette Agent 0.4a0 Lets Tools Run in the Browser](https://simonwillison.net/2026/Jul/31/datasette-agent/#atom-everything) ⭐️ 6.0/10

Datasette-agent 0.4a0 adds a new await context.browser_task() mechanism that lets agent tools execute custom JavaScript directly in the user's browser. The release was announced by Simon Willison on July 31, 2026. This significantly expands what Datasette Agent plugins can do by moving tool execution from the server side to the browser, enabling interactive and client-side capabilities like debugging loops. It lowers the barrier for building rich AI-assisted features inside Datasette, though the alpha status means it is not yet production-ready. The new mechanism is implemented in pull request #33, and Simon Willison used it to add a debug loop to datasette-apps 0.2a0. Because this is an alpha release, the browser_task() API is likely to change before stabilization.

rss · Simon Willison · Jul 31, 14:14

**Background**: Datasette Agent is an LLM-powered AI assistant for Datasette that helps users explore, query, and chart data by writing and running SQL queries. Datasette itself is an open-source tool for publishing and exploring tabular data, and plugins extend its functionality. Previously, agent tools ran server-side; browser_task() creates a path for tools to run JavaScript in the user's browser, which is especially useful for building interactive HTML applications like those hosted by the Datasette Apps plugin.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/datasette/datasette-agent">GitHub - datasette/datasette-agent: An LLM-powered agent for ...</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-apps/">Host applications inside Datasette with Datasette ... - Datasette Blog</a></li>
<li><a href="https://simonwillison.net/2026/Jul/31/datasette-agent/">Release: datasette-agent 0.4a0 - simonwillison.net</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#llm-tool-use`, `#datasette-agent`, `#release`

---