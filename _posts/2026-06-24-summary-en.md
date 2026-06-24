---
layout: default
title: "Horizon Summary: 2026-06-24 (EN)"
date: 2026-06-24
lang: en
---

> From 35 items, 22 important content pieces were selected

---

1. [Rhombus 1.0 Released: A Macro-Extensible Language on Racket](#item-1) ⭐️ 8.0/10
2. [Swift Package Index joins Apple](#item-2) ⭐️ 8.0/10
3. [Meta Pauses Employee-Tracking Program After Data Leak](#item-3) ⭐️ 8.0/10
4. [Datasette 1.0a35 Adds Table Create/Alter with JSON APIs](#item-4) ⭐️ 8.0/10
5. [Prompt Injection as Role Confusion](#item-5) ⭐️ 8.0/10
6. [Porting Moebius 0.2B inpainting model to browser with Claude Code](#item-6) ⭐️ 8.0/10
7. [DeepSWE: A Contamination-Free Benchmark for Frontier Coding Models](#item-7) ⭐️ 8.0/10
8. [Vulnerability Reports Lose Their Luster to LLM-Generated Spam](#item-8) ⭐️ 7.0/10
9. [FUTO Swipe – Open swipe typing model](#item-9) ⭐️ 7.0/10
10. [Open-Source WYSIWYG TikZ Editor Built by AI](#item-10) ⭐️ 7.0/10
11. [Vitamin D Supplementation: Mostly Overhyped, But Real for the Severely Deficient](#item-11) ⭐️ 7.0/10
12. [ML Security Testing Lags Behind Software Standards](#item-12) ⭐️ 7.0/10
13. [Non-deterministic Vulnerability Detection Benchmark System](#item-13) ⭐️ 7.0/10
14. [uv 0.11.24 adds CPython 3.15b3 and relocatable environments](#item-14) ⭐️ 6.0/10
15. [Jerry's Map: Six Decades of Imaginary Cartography](#item-15) ⭐️ 6.0/10
16. [Tribute to Tony Krueger, inventor of red/green squiggly spell-check underlines](#item-16) ⭐️ 6.0/10
17. [Kevin Mitnick Gifts Dream Car to Man Who Helped Imprison Him](#item-17) ⭐️ 6.0/10
18. [OPFS + Pyodide test harness for persistent SQLite in browser](#item-18) ⭐️ 6.0/10
19. [Engineer seeks advice on picking cloud GPU providers for LLM inference](#item-19) ⭐️ 6.0/10
20. [Hugging Face revives Papers with Code with new features](#item-20) ⭐️ 6.0/10
21. [Seeking Robust NLI for Diffusion LLM Syntax](#item-21) ⭐️ 6.0/10
22. [Potential Mistake Found in ICLR 2026 Blog Post](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Rhombus 1.0 Released: A Macro-Extensible Language on Racket](https://blog.racket-lang.org/2026/06/rhombus-v1.0.html) ⭐️ 8.0/10

The Rhombus language, built on Racket, has reached version 1.0, introducing a powerful `...` macro operator that enables pattern matching and map-like operations on nested data structures. Rhombus 1.0 marks a significant milestone for the Racket ecosystem, offering a conventional syntax with the full power of Racket's macro system, potentially lowering the barrier for new users and expanding the language's reach. The `...` operator is not a built-in feature but a macro, showcasing Rhombus's macro extensibility; it can differentiate between binding and expression contexts, enabling context-specific behaviors.

hackernews · Decabytes · Jun 22, 17:50 · [Discussion](https://news.ycombinator.com/item?id=48633473)

**Background**: Racket is a Lisp-family language known for its powerful hygienic macro system but uses S-expressions (parentheses), which can be a barrier. Rhombus was initially called 'Racket2' and aims to provide a more conventional syntax while preserving macro capabilities. The `...` macro operator is a key example of how Rhombus allows custom syntax extensions.

<details><summary>References</summary>
<ul>
<li><a href="https://beautifulracket.com/appendix/thoughts-on-rhombus.html">Beautiful Racket: Thoughts on Rhombus (formerly known as Racket2)</a></li>
<li><a href="https://github.com/racket/rhombus">GitHub - racket/rhombus: Rhombus programming language · GitHub</a></li>
<li><a href="https://news.ycombinator.com/item?id=48633473">Rhombus Language 1.0 - Hacker News</a></li>

</ul>
</details>

**Discussion**: Community members praised the `...` operator for its generality and power, with some noting it feels like a splat operator but is more flexible. Others expressed a preference for S-expressions, and there was interest in talks about Rhombus at conferences.

**Tags**: `#Rhombus`, `#Racket`, `#Programming Languages`, `#Macros`, `#Language Design`

---

<a id="item-2"></a>
## [Swift Package Index joins Apple](https://swiftpackageindex.com/blog/swift-package-index-joins-apple) ⭐️ 8.0/10

Apple has acquired the Swift Package Index (SPI), the community-maintained package registry for Swift, and the SPI team joins Apple while promising to keep the project open source. This acquisition places a key community resource under Apple's control, raising hopes for improved Swift Package Manager integration but also concerns about Apple's track record with open source and potential new restrictions on package indexing. SPI currently indexes metadata from over 11,000 Swift packages and is the default package search tool for Swift.org. Apple explicitly mentions developer identity as a future direction, causing skepticism among some community members.

hackernews · JDevlieghere · Jun 23, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48648779)

**Background**: The Swift Package Manager (SPM) is Apple's tool for managing Swift code distribution and dependencies. The Swift Package Index (SPI) was created by the community to provide a searchable index of Swift packages, filling a gap left by the lack of an official package registry. SPI has been widely used by Swift developers to discover and evaluate packages.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5mac.com/2026/06/23/swift-package-index-joins-apple-pledges-to-remain-open-source/">Swift Package Index joins Apple, pledges to remain open source</a></li>
<li><a href="https://swiftpackageindex.com/">Swift Package Index</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some congratulated the SPI team (e.g., dragon-hn), while others expressed skepticism about Apple's stewardship (e.g., jshier). A few noted confusion with similar sites, and one commenter plans to build a competitor due to SPI's GitHub-only limitation.

**Tags**: `#swift`, `#apple`, `#package-manager`, `#open-source`, `#acquisition`

---

<a id="item-3"></a>
## [Meta Pauses Employee-Tracking Program After Data Leak](https://www.wired.com/story/meta-pauses-employee-tracking-program-following-internal-security-breach/) ⭐️ 8.0/10

Meta has paused its controversial employee-tracking program, which monitored keystrokes and other activities for AI training, after an internal data leak exposed sensitive employee information to the entire company. This incident highlights the privacy risks of workplace surveillance and raises questions about Meta's handling of sensitive data, especially as it trains AI on employee behavior. It also fuels criticism of Meta's culture and its broader impact on trust. The leaked data included plain-text private conversations and performance information from the tracking program, which involved full screen recording. Meta had intended to anonymize the data but failed to do so, leading to the leak.

hackernews · 1vuio0pswjnm7 · Jun 24, 00:28 · [Discussion](https://news.ycombinator.com/item?id=48653575)

**Background**: Meta's employee-tracking program was part of an initiative to train AI agents by recording employee interactions with their laptops. Such programs are controversial due to privacy concerns, and this leak demonstrates the risks of collecting sensitive data without proper safeguards.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wired.com/story/meta-accidentally-let-employees-access-each-others-keystroke-data/">Meta Exposed Data Internally From Its Controversial Employee-Tracking Program | WIRED</a></li>
<li><a href="https://www.businessinsider.com/meta-ai-training-data-leak-exposed-employee-activity-across-company-2026-6">Meta pauses an AI training program that tracks employees' keystrokes after an internal leak</a></li>
<li><a href="https://www.reddit.com/r/technology/comments/1uczyyq/meta_pauses_employeetracking_program_following/">Meta Pauses Employee-Tracking Program Following Internal Data Leak | The move comes after the company left potentially sensitive data from the initiative exposed internally - Reddit</a></li>

</ul>
</details>

**Discussion**: Commenters were overwhelmingly critical, with many expressing distrust in Meta and citing the incident as evidence of the company's disregard for privacy and ethics. Some noted that even rule-abiding employees could be penalized based on interpreted 'working to rule' behavior. Others pointed out the irony of Meta using surveillance that leaked data, undermining its own security posture.

**Tags**: `#Meta`, `#surveillance`, `#privacy`, `#data leak`, `#employee tracking`

---

<a id="item-4"></a>
## [Datasette 1.0a35 Adds Table Create/Alter with JSON APIs](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a35 introduces a 'Create table' interface and an 'Alter table' interface, each backed by dedicated JSON API endpoints for programmatic table manipulation. The release also includes comprehensive template context documentation that is considered a stable API for custom templates. These new features significantly enhance Datasette's utility as a database management tool, allowing users to create and alter SQLite tables through both a UI and a JSON API. This paves the way for the stable 1.0 release and makes Datasette more powerful for developers and data publishers. The 'Create table' JSON API supports defining columns, primary keys, custom types, NOT NULL constraints, literal and expression defaults, and single-column foreign keys. The 'Alter table' API can add, rename, reorder, and drop columns, change column types, defaults, constraints, primary keys, foreign keys, and rename the table, and also includes a drop table button.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases, providing a web interface and JSON API for data interaction. SQLite is a widely-used embedded database engine. The JSON API allows programmatic access to databases, and this release adds endpoints for schema modification, which was previously limited to manual SQL or external tools.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/stable/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="http://datasette.io/blog/2026/api-extras">Datasette 1.0a33 with JSON extras in the API - Datasette Blog</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#database`, `#JSON API`, `#open source`

---

<a id="item-5"></a>
## [Prompt Injection as Role Confusion](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

Research by Charles Ye, Jasmine Cui, and Dylan Hadfield-Menell shows that LLMs prioritize the style of role tags over their actual content, enabling new prompt injection attacks. They found that 'destyling' input text reduces attack success from 61% to 10%. This reveals a fundamental vulnerability in LLM security, as models cannot reliably distinguish trusted instructions from untrusted user input based on role tags alone. It underscores that prompt injection defense will remain a challenging cat-and-mouse game without genuine role perception. The paper introduces 'role confusion' where models interpret text based on stylistic resemblance to internal thought blocks (e.g., <think>, <assistant>) rather than explicit labels. The attack success rate drops dramatically from 61% to 10% when the style is altered while preserving semantic meaning.

rss · Simon Willison · Jun 22, 23:59

**Background**: Prompt injection attacks exploit the way LLMs process instructions, where malicious input can override system prompts. Role tags like <system> and <user> are supposed to separate contexts, but this research shows that models rely on stylistic cues — the 'sound' of text — more than the tags themselves. This insight explains why simple formatting changes can bypass safety measures.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.12277">[2603.12277] Prompt Injection as Role Confusion</a></li>

</ul>
</details>

**Tags**: `#prompt injection`, `#AI safety`, `#LLM security`, `#jailbreaks`

---

<a id="item-6"></a>
## [Porting Moebius 0.2B inpainting model to browser with Claude Code](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison ported the Moebius 0.2B lightweight image inpainting model to run in the browser via WebGPU, using Claude Code as an AI coding assistant. A live demo is available at simonw.github.io/moebius-web/. This showcases that small AI models can achieve practical performance in the browser via WebGPU, enabling image editing without cloud dependencies. It also demonstrates how AI coding agents like Claude Code can accelerate complex porting tasks. The original Moebius model required PyTorch and NVIDIA CUDA, but Simon used ONNX Runtime Web with the WebGPU backend for browser inference. The demo allows users to upload images, mask areas, and run inpainting entirely locally.

rss · Simon Willison · Jun 22, 23:43

**Background**: Image inpainting is the task of filling missing or removed regions of an image with plausible content. Moebius is a 0.2 billion parameter model that claims performance comparable to 10B+ models like FLUX.1-Fill-Dev, with over 15x speedup. WebGPU is a web standard for low-level GPU access, enabling compute-heavy workloads like AI inference in browsers. Claude Code is Anthropic's AI assistant for software development.

<details><summary>References</summary>
<ul>
<li><a href="https://hustvl.github.io/Moebius/">Moebius Project Page</a></li>
<li><a href="https://simonwillison.net/2026/Jun/22/porting-moebius/">Porting the Moebius 0.2B image inpainting model to run in the browser with Claude Code</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebGPU">WebGPU</a></li>

</ul>
</details>

**Tags**: `#image inpainting`, `#WebGPU`, `#browser AI`, `#model porting`, `#machine learning`

---

<a id="item-7"></a>
## [DeepSWE: A Contamination-Free Benchmark for Frontier Coding Models](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE is a new open-source benchmark for evaluating frontier coding models, featuring contamination-free tasks written from scratch, high diversity across 91 repositories and 5 languages, real-world complexity, and hand-written verifiers. This benchmark addresses key weaknesses in existing code generation evaluations, particularly data contamination, by ensuring no model has seen the solutions during pretraining, which could lead to more reliable assessments of AI coding capabilities. DeepSWE prompts are about half the length of SWE-bench Pro's, yet solutions require 5.5x more code and ~2x more output tokens, and its hand-written verifiers test software behavior rather than implementation details.

reddit · r/MachineLearning · /u/we_are_mammals · Jun 24, 02:03

**Background**: Existing benchmarks like SWE-bench evaluate AI models on real-world GitHub issues, but they can suffer from data contamination where models may have seen similar tasks during training. Contamination-free benchmarks such as LiveCodeBench collect new problems over time to avoid this issue. DeepSWE builds on this approach by creating entirely new tasks from scratch.

<details><summary>References</summary>
<ul>
<li><a href="https://epoch.ai/benchmarks/swe-bench-verified">SWE-bench Verified | Epoch AI</a></li>
<li><a href="https://www.swebench.com/">SWE-bench Leaderboards</a></li>
<li><a href="https://livecodebench.github.io/">LiveCodeBench: Holistic and Contamination Free Evaluation of Large Language Models for Code</a></li>

</ul>
</details>

**Tags**: `#benchmark`, `#code generation`, `#AI`, `#software engineering`, `#evaluation`

---

<a id="item-8"></a>
## [Vulnerability Reports Lose Their Luster to LLM-Generated Spam](https://words.filippo.io/vuln-reports/) ⭐️ 7.0/10

An influx of low-quality, LLM-generated vulnerability reports and spam is making genuine security disclosures harder to distinguish, according to a recent article by Filippo Valsorda. This trend threatens the credibility of vulnerability reporting, potentially causing real issues to be ignored and increasing the burden on maintainers, while also highlighting the need for better automated detection tools. Valsorda notes that half of unsolicited reports are LLM-generated or extortion attempts, and even authentic researchers face skepticism; the situation is driven by the low cost of LLM usage compared to human effort.

hackernews · goranmoomin · Jun 23, 23:42 · [Discussion](https://news.ycombinator.com/item?id=48653216)

**Background**: Vulnerability reporting is a process where security researchers or automated tools find and disclose security flaws to software maintainers. Traditionally, these reports were rare and valuable. However, with the rise of LLMs, automated tools can now generate many more reports, including false positives and spam, overwhelming maintainers and reducing the signal-to-noise ratio.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/huhusmang/Awesome-LLMs-for-Vulnerability-Detection">GitHub - huhusmang/Awesome-LLMs-for-Vulnerability-Detection: The community's most comprehensive, continuously-updated index of research on Large Language Models for software vulnerability detection — papers across function-level, repository-level, agentic, and smart-contract detection, plus datasets, benchmarks, and surveys.</a></li>
<li><a href="https://claroty.com/team82/research/hands-free-what-llm-driven-vulnerability-research-looks-like">Hands Free: What LLM Driven Vulnerability Research Looks Like | Claroty</a></li>
<li><a href="https://vulnrepo.com/">VULNRΞPO - Vulnerability Report Generator & Repository</a></li>

</ul>
</details>

**Discussion**: Comments reflect a mix of frustration and cautious optimism. Some users report receiving frequent spam reports, while others believe LLMs will eventually help fix bugs and reduce false positives, leading to a more secure ecosystem.

**Tags**: `#security`, `#vulnerability reporting`, `#LLM`, `#spam`, `#software engineering`

---

<a id="item-9"></a>
## [FUTO Swipe – Open swipe typing model](https://swipe.futo.tech/) ⭐️ 7.0/10

FUTO Swipe is a new open-source swipe typing model and algorithm suite released by FUTO, designed to improve accuracy and reduce word overlap for mobile keyboards. It is now available for use in FUTO Keyboard and welcomes community adoption. This matters because high-quality swipe typing has long been locked behind proprietary, privacy-invasive keyboard apps. FUTO Swipe provides a free, open alternative that could enable swipe typing on more platforms and empower users with greater control over their typing data. The model is trained using community-contributed swipe data and supports multiple languages and keyboard layouts. It specifically targets the 'word overlap' problem where similar swipe paths yield ambiguous results, which is a common pain point in swipe typing.

hackernews · futohq · Jun 23, 17:50 · [Discussion](https://news.ycombinator.com/item?id=48648619)

**Background**: Swipe typing (also called gesture typing) lets users input words by sliding their finger across a keyboard without lifting it. Traditional high-quality swipe models, like those in Gboard, are proprietary and often require network connectivity or collect user data. FUTO Swipe is open-source, allowing developers to integrate it into any keyboard app while preserving user privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://swipe.futo.tech/">FUTO Swipe</a></li>
<li><a href="https://news.ycombinator.com/item?id=48648619">FUTO Swipe – A new swipe typing model | Hacker News</a></li>
<li><a href="https://swipe.futo.org/">FUTO Keyboard Swipe Training</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, with users reporting that the new swipe model feels competitive with Gboard. Some users note minor issues like random capitalization and lack of context-aware suggestions, but overall sentiment is that it's a significant improvement over previous open-source keyboards.

**Tags**: `#mobile keyboard`, `#swipe typing`, `#HCI`, `#user experience`, `#input method`

---

<a id="item-10"></a>
## [Open-Source WYSIWYG TikZ Editor Built by AI](https://tikz.dev/editor/) ⭐️ 7.0/10

An open-source WYSIWYG TikZ editor has been released that simultaneously shows TikZ source code and rendered figure, allowing visual editing by dragging and resizing while keeping both views in sync. The editor was built almost entirely by the AI coding agent Codex. This addresses a long-standing pain point for LaTeX users who manually code TikZ figures, potentially saving significant time and reducing the learning curve. It also demonstrates a new capability for AI coding agents to build complex, niche software that would be tedious for humans. The editor parses TikZ code and tracks source locations of each object, enabling coordinate overrides without altering formatting. A noted limitation is that generated code uses absolute coordinates, whereas TikZ often benefits from relative positioning.

hackernews · DominikPeters · Jun 23, 14:24 · [Discussion](https://news.ycombinator.com/item?id=48645437)

**Background**: TikZ is a powerful LaTeX package for creating vector graphics within documents, but it requires manual coordinate coding and recompilation to see results. WYSIWYG editors for LaTeX figures have been rare due to the complexity of parsing TikZ. This project was built largely by the AI Codex, costing about $500 in ChatGPT subscription fees for 700M tokens used.

<details><summary>References</summary>
<ul>
<li><a href="https://www.overleaf.com/learn/latex/TikZ_package">TikZ package - Overleaf, Online LaTeX Editor</a></li>
<li><a href="https://www.overleaf.com/learn/latex/LaTeX_Graphics_using_TikZ:_A_Tutorial_for_Beginners_(Part_1)—Basic_Drawing">LaTeX Graphics using TikZ: A Tutorial for Beginners (Part 1)—Basic Drawing - Overleaf, Online LaTeX Editor</a></li>

</ul>
</details>

**Discussion**: Community feedback praised the UI and concept but criticized the generated code for heavily using absolute coordinates. The creator shared cost details of using Codex, and users referenced similar tools like quiver.app and CircuitTikZ integrations.

**Tags**: `#LaTeX`, `#TikZ`, `#WYSIWYG`, `#open-source`, `#editor`

---

<a id="item-11"></a>
## [Vitamin D Supplementation: Mostly Overhyped, But Real for the Severely Deficient](https://dynomight.net/vitamin-d/) ⭐️ 7.0/10

A skeptical deep-dive analysis of vitamin D studies argues that the strongest evidence for supplementation benefits is limited to severely deficient individuals, while claims of widespread benefits for the general population are exaggerated. This challenges mainstream health advice that recommends universal vitamin D supplementation, potentially shifting public health guidance toward targeted use for those with confirmed deficiency. The analysis highlights that many studies fail to account for participants' baseline vitamin D levels, and that sunlight's benefits extend beyond mere vitamin D production, making oral supplementation a poor substitute.

hackernews · surprisetalk · Jun 23, 16:30 · [Discussion](https://news.ycombinator.com/item?id=48647486)

**Background**: Vitamin D is a fat-soluble vitamin crucial for calcium absorption and bone health, often synthesized through skin exposure to sunlight. Deficiencies are common in northern latitudes, leading to widespread supplementation recommendations. However, randomized controlled trials have produced mixed results on non-bone health benefits, fueling ongoing scientific debate.

**Discussion**: Commenters largely praised the article's balanced approach, with some sharing personal anecdotes of mood and immune improvements after taking vitamin D. Others emphasized the multifactorial health benefits of sunlight beyond vitamin D. One commenter noted methodological issues in NHANES deficiency surveys due to seasonal and latitudinal data collection constraints.

**Tags**: `#health`, `#vitamin D`, `#science`, `#nutrition`, `#analysis`

---

<a id="item-12"></a>
## [ML Security Testing Lags Behind Software Standards](https://www.reddit.com/r/MachineLearning/comments/1uddtws/are_model_security_risks_extraction_poisoning/) ⭐️ 7.0/10

A Reddit post by user Xorphian highlights that many ML teams deploy models to production without conducting adversarial security testing, unlike standard software that undergoes rigorous security reviews. This oversight exposes organizations to model extraction and poisoning attacks, which can lead to intellectual property theft and compromised model integrity, underscoring the urgent need for security practices in ML production comparable to traditional software. Model extraction attacks involve adversaries stealing model behavior by systematically querying the API, while model poisoning attacks manipulate training data or parameters to alter model behavior. The post invites industry practitioners to share whether such testing is actually performed in their workplaces.

reddit · r/MachineLearning · /u/Xorphian · Jun 23, 10:52

**Background**: Adversarial machine learning is the study of attacks and defenses on ML models. Model extraction attacks allow an attacker with query access to steal a model's functionality by building a replica. Model poisoning attacks inject malicious data during training to alter model outputs. Despite these risks, adversarial testing before deployment is not yet standard practice in many ML teams.

<details><summary>References</summary>
<ul>
<li><a href="https://www.praetorian.com/blog/stealing-ai-models-through-the-api-a-practical-model-extraction-attack/">Stealing AI Models Through the API: A Practical Model Extraction Attack | Praetorian</a></li>
<li><a href="https://owasp.org/www-project-machine-learning-security-top-10/docs/ML10_2023-Model_Poisoning">OWASP Machine Learning Security Top Ten 2023 | ML10:2023 Model Poisoning | OWASP Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Adversarial_machine_learning">Adversarial machine learning - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#model security`, `#adversarial testing`, `#ML production`, `#AI safety`, `#software security`

---

<a id="item-13"></a>
## [Non-deterministic Vulnerability Detection Benchmark System](https://www.reddit.com/r/MachineLearning/comments/1ud0rft/nondeterministic_vulnerability_detection/) ⭐️ 7.0/10

A work-in-progress benchmark that modifies Juliet test cases to appear as real code and injects various comment sentiments to evaluate LLM vulnerability detection robustness. This benchmark addresses a known limitation of LLM-based vulnerability detection by hiding known patterns and testing sensitivity to comment sentiment, which is crucial for real-world deployment. The benchmark uses Juliet test cases covering hundreds of CWEs, modifies them to resemble real codebases, and injects LLM-generated comments with accurate, misleading, or neutral sentiments.

reddit · r/MachineLearning · /u/Psychological_Meat_6 · Jun 22, 23:34

**Background**: Juliet test cases are a standard benchmark for vulnerability detection, containing examples of common weakness enumerations (CWEs). LLMs have been shown to be effective at detecting vulnerabilities but can be fooled by simple modifications or misleading comments. This benchmark aims to create a more realistic evaluation by obscuring the origin of test cases and introducing sentiment bias.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/find-sec-bugs/juliet-test-suite">GitHub - find-sec-bugs/juliet-test-suite: :microscope: A collection of test cases in the Java language. It contains examples for 112 different CWEs. · GitHub</a></li>
<li><a href="https://www.castsoftware.com/pulse/juliet-and-owasp-benchmark-results-how-cast-tests">Juliet and OWASP Benchmark Results: How CAST Tests Against 2 Most Important Application Security Standards in 2019</a></li>

</ul>
</details>

**Tags**: `#vulnerability detection`, `#benchmark`, `#LLM`, `#security`, `#machine learning`

---

<a id="item-14"></a>
## [uv 0.11.24 adds CPython 3.15b3 and relocatable environments](https://github.com/astral-sh/uv/releases/tag/0.11.24) ⭐️ 6.0/10

uv 0.11.24 adds support for CPython 3.15.0b3 and introduces a preview feature for relocatable project environments, along with performance improvements and bug fixes. This release keeps uv aligned with the latest Python beta, enabling early testing, while the relocatable environments preview addresses a long-standing need for portable Python setups. Performance optimizations like the compact index further solidify uv's reputation as a fast package manager. The relocatable environments feature is opt-in under the preview flag, and only project environments are affected. This release also fixes bugs related to archive ID collisions and transparent Python upgrades in project environments.

github · github-actions[bot] · Jun 23, 21:16

**Background**: uv is a fast, modern Python package manager written in Rust, designed as a drop-in replacement for pip and pip-tools. Relocatable environments allow Python virtual environments to be moved or copied to different paths without breaking, which is useful for deployment and CI scenarios. The compact index for lazy version maps reduces memory usage when resolving dependencies. The 'exclude-newer' option, which was made disableable in this release, helps create reproducible environments by ignoring packages published after a specified date.

<details><summary>References</summary>
<ul>
<li><a href="https://relenv.readthedocs.io/en/v0.4.1/">Relenv - Build and use relocatable Python environments</a></li>
<li><a href="https://pydevtools.com/handbook/how-to/how-to-use-exclude-newer-for-reproducible-python-environments/">Use uv --exclude-newer for Reproducible Installs | pydevtools</a></li>

</ul>
</details>

**Tags**: `#Python`, `#package management`, `#uv`, `#release`

---

<a id="item-15"></a>
## [Jerry's Map: Six Decades of Imaginary Cartography](http://www.jerrysmap.com/the-map) ⭐️ 6.0/10

Since 1963, artist Jerry has been continuously drawing and expanding a map of an imaginary land, using a custom card deck to determine the features of each new map tile. This project exemplifies outsider art and the power of generative creative constraints, inspiring discussions about creativity, systems, and long-term artistic commitment. The process involves drawing a card that dictates whether the next tile includes a river, mountain, city, or other feature; the map has grown to cover many sheets and is viewable online.

hackernews · turtleyacht · Jun 23, 18:40 · [Discussion](https://news.ycombinator.com/item?id=48649435)

**Background**: Jerry's Map is a long-running outsider art project. Outsider art refers to art created outside the boundaries of official culture, often by self-taught individuals. Jerry uses a system of cards to guide his creative decisions, ensuring both structure and spontaneity. The project has gained a following for its meditative and evolving nature.

**Discussion**: Commenters share personal experiences of similar map-drawing in childhood, appreciate the card-driven creative process, and link to a video and interactive version. Some note its connection to outsider art and games like Dwarf Fortress.

**Tags**: `#art`, `#map`, `#creative process`, `#outsider art`, `#Hacker News`

---

<a id="item-16"></a>
## [Tribute to Tony Krueger, inventor of red/green squiggly spell-check underlines](https://devblogs.microsoft.com/oldnewthing/20260622-00/?p=112451) ⭐️ 6.0/10

Raymond Chen's article pays tribute to Tony Krueger, who introduced the now-ubiquitous red and green squiggly underlines for real-time spell-checking in word processors. This seemingly small UX innovation fundamentally changed how people interact with text, making error detection instant and non-intrusive. It became a standard feature in virtually every modern word processor, influencing decades of software design. The article notes that Tony Krueger ported the spell-check feature to Microsoft Word, and the squiggly underline concept may have originated from earlier programs like ProWrite on the Amiga, which used a red squiggly line for misspelled words.

hackernews · saikatsg · Jun 23, 18:10 · [Discussion](https://news.ycombinator.com/item?id=48648959)

**Background**: Before real-time spell-checking, users had to manually run a separate spell-check process after writing. The squiggly underline provides immediate visual feedback without interrupting the typing flow. The red underline typically indicates spelling errors, while green indicates grammar issues.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Spell_checker">Spell checker - Wikipedia</a></li>
<li><a href="https://support.microsoft.com/en-us/office/check-spelling-and-grammar-in-office-5cdeced7-d81d-47de-9096-efd0ee909227">Check spelling and grammar in Office | Microsoft Support</a></li>

</ul>
</details>

**Discussion**: Commenters shared mixed sentiments: some praised the innovation's impact, while others noted that multi-language environments make squiggles less useful due to incorrect language detection. One commenter pointed out a circular citation issue between Chen's article and Wikipedia.

**Tags**: `#computing history`, `#spell check`, `#Raymond Chen`, `#ux`

---

<a id="item-17"></a>
## [Kevin Mitnick Gifts Dream Car to Man Who Helped Imprison Him](https://www.thedrive.com/news/this-man-was-gifted-his-dream-car-by-the-notorious-hacker-he-put-in-prison) ⭐️ 6.0/10

Kevin Mitnick, the once notorious hacker, gifted his dream car to Shawn Nunley, the man who assisted in his capture and imprisonment, as a gesture of friendship formed years later. This story illustrates the unexpected personal connections that can emerge from high-profile cases, humanizing both a legendary hacker and the person who helped catch him, and highlighting Mitnick's post-prison transformation into a security consultant. Shawn Nunley worked for a telecommunications company and played a key role in tracing Mitnick's phone activity, leading to his 1995 arrest. Mitnick later became a security consultant and writer before his death in July 2023.

hackernews · mauvehaus · Jun 22, 18:03 · [Discussion](https://news.ycombinator.com/item?id=48633643)

**Background**: Kevin Mitnick was one of the most wanted computer hackers in the 1990s, known for breaking into major companies' systems. He was captured with help from Shawn Nunley, leading to a five-year prison sentence. After his release, Mitnick reinvented himself as a security consultant, author, and keynote speaker, and he and Nunley eventually became friends.

**Discussion**: Community comments note Mitnick's consulting work sometimes lacked technical depth, focusing on physical security rather than common flaws like SQL injection. However, many express admiration for his influence on hackers like George Hotz, and appreciation for the humanity shown in his later friendship with Nunley. Some also lament that Mitnick and Shimomura never reconciled.

**Tags**: `#Kevin Mitnick`, `#hacker culture`, `#cybersecurity history`, `#human interest`

---

<a id="item-18"></a>
## [OPFS + Pyodide test harness for persistent SQLite in browser](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison created a test harness that combines the Origin Private File System (OPFS) with Pyodide to explore whether Datasette Lite can edit persistent SQLite files stored on the user's computer entirely within the browser. This experiment could enable fully client-side, persistent data editing for Python web applications running via WebAssembly, reducing reliance on server backends and improving offline capabilities for tools like Datasette Lite. The test harness uses the OPFS API, which provides a high-performance, origin-private virtual file system not visible to the user, and Pyodide, a WebAssembly-based Python distribution for the browser.

rss · Simon Willison · Jun 23, 18:58

**Background**: Pyodide is a Python distribution for the browser and Node.js based on WebAssembly, allowing Python code to run in the browser. The Origin Private File System (OPFS) is part of the File System API, providing a sandboxed, origin-specific storage area that is optimized for performance. Datasette Lite is a version of the Datasette data exploration tool that runs entirely in the browser via Pyodide.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN</a></li>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.0</a></li>

</ul>
</details>

**Tags**: `#browsers`, `#pyodide`, `#webassembly`, `#datasette-lite`, `#opfs`

---

<a id="item-19"></a>
## [Engineer seeks advice on picking cloud GPU providers for LLM inference](https://www.reddit.com/r/MachineLearning/comments/1udfovh/whats_your_biggest_pain_point_when_choosing/) ⭐️ 6.0/10

A Reddit user, an ML engineer, posted a discussion asking the community about the methods and pain points they encounter when comparing cloud GPU providers for LLM inference. This discussion highlights the practical challenges many ML practitioners face in selecting cost-effective and reliable GPU resources, which directly impacts development and deployment costs for LLM applications. The engineer mentions currently using spreadsheets to manually compare metrics like $/hr, $/token, throughput, and reliability, and asks if there are tools or resources they might be missing.

reddit · r/MachineLearning · /u/Technomadlyf · Jun 23, 12:24

**Tags**: `#cloud GPU`, `#LLM inference`, `#cost comparison`, `#ML engineering`, `#discussion`

---

<a id="item-20"></a>
## [Hugging Face revives Papers with Code with new features](https://www.reddit.com/r/MachineLearning/comments/1ucm508/some_new_updates_to_papers_with_code_p/) ⭐️ 6.0/10

Niels from Hugging Face announced new features for Papers with Code, including SOTA badges for top-3 benchmark scores, a trending score that combines GitHub stars and Hugging Face activity, support for external evals, and additional benchmarks/tasks. These enhancements improve discoverability of SOTA models and trending research, helping the community build on each other's work. It marks a significant revival of Papers with Code after Meta shut it down in July 2025, now integrated with Hugging Face's ecosystem. The trending score now accounts for both GitHub star velocity and Hugging Face artifacts (models, datasets, spaces). SOTA badges are displayed whenever a paper ranks in the top 3 of a benchmark, and external evals allow third-party benchmark results to appear alongside a paper's own results.

reddit · r/MachineLearning · /u/NielsRogge · Jun 22, 14:29

**Background**: Papers with Code was a widely-used platform that indexed machine learning papers, linked them to code, and tracked SOTA results on benchmarks. Meta shut it down in July 2025, redirecting the domain to Hugging Face Trending Papers. Hugging Face is now reviving it as paperswithcode.co, adding features that leverage the Hugging Face Hub, such as models and datasets. The new features aim to make research discovery more reproducible and community-driven.

<details><summary>References</summary>
<ul>
<li><a href="https://www.codesota.com/papers-with-code">Papers With Code Alternative: SOTA Leaderboards and Archived Data | CodeSOTA | CodeSOTA</a></li>
<li><a href="https://posttrainbench.com/">PostTrainBench</a></li>
<li><a href="https://arxiv.org/abs/2603.08640">[2603.08640] PostTrainBench: Can LLM Agents Automate LLM Post-Training?</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#papers with code`, `#open source`, `#SOTA`, `#huggingface`

---

<a id="item-21"></a>
## [Seeking Robust NLI for Diffusion LLM Syntax](https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/) ⭐️ 6.0/10

A Reddit user asks for literature on syntax-robust Natural Language Inference (NLI) to evaluate semantic correctness of imperfectly generated text from diffusion large language models (LLMs). This highlights a gap in evaluating diffusion LLMs, which often produce syntactically noisy text, complicating standard NLI usage. Addressing this could improve reliability of LLM evaluation frameworks. The user specifically mentions diffusion LLMs like LLaDA and the challenge of syntactic noise in applying NLI to gauge correctness. They seek the state-of-the-art on syntax-robust NLI.

reddit · r/MachineLearning · /u/RepresentativeBee600 · Jun 22, 21:51

**Background**: Autoregressive LLMs generate text token by token, while diffusion LLMs (e.g., LLaDA) generate text by gradually denoising a random sequence, leading to potential syntactic errors. NLI is a task that determines whether a hypothesis is entailed, contradicted, or neutral given a premise, used to evaluate LLM output. Standard NLI models are sensitive to syntactic variations, making them less robust for diffusion LLM outputs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reddit.com/r/MachineLearning/comments/1ucy7p3/syntactically_robust_nli_for_semantics_of/">Syntactically robust NLI for semantics of imperfectly generated text? [R] - Reddit</a></li>
<li><a href="https://github.com/ML-GSAI/LLaDA">GitHub - ML-GSAI/LLaDA: Official PyTorch implementation for "Large Language Diffusion Models" · GitHub</a></li>
<li><a href="https://aclanthology.org/2023.iwcs-1.29.pdf">[PDF] AMR4NLI: Interpretable and robust NLI measures from semantic graph - ACL Anthology</a></li>

</ul>
</details>

**Tags**: `#NLI`, `#LLM evaluation`, `#diffusion LLMs`, `#syntax robustness`, `#semantics`

---

<a id="item-22"></a>
## [Potential Mistake Found in ICLR 2026 Blog Post](https://www.reddit.com/r/MachineLearning/comments/1ud9i2g/found_a_potential_mistake_in_an_iclr_2026/) ⭐️ 6.0/10

A Reddit user reported a potential mistake in an ICLR 2026 blog post, creating a GitHub issue and contacting the authors without response for weeks. This highlights the importance of community peer review in preprint and blog post venues, especially for top conferences like ICLR. The specific mistake is detailed in GitHub issue #218 of the iclr-blogposts/2026 repository, but the user seeks validation before the issue escalates.

reddit · r/MachineLearning · /u/metalwhaledev · Jun 23, 06:39

**Background**: ICLR (International Conference on Learning Representations) is a top machine learning conference that publishes blog post submissions alongside traditional papers. The ICLR blogpost track allows researchers to present new ideas or critiques in a more accessible format. Community-driven error detection is a common practice in open science.

**Tags**: `#ICLR`, `#machine learning`, `#blog post review`, `#community inquiry`

---