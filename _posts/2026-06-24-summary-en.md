---
layout: default
title: "Horizon Summary: 2026-06-24 (EN)"
date: 2026-06-24
lang: en
---

> From 32 items, 15 important content pieces were selected

---

1. [John Carmack: Quake Mistakes Ruined id Software](#item-1) ⭐️ 8.0/10
2. [Bunny DNS Goes Free, Eliminates Query Fees](#item-2) ⭐️ 8.0/10
3. [Krea 2: State-of-the-Art Open-Weight 12B Image Model Released](#item-3) ⭐️ 8.0/10
4. [Datasette 1.0a35 adds table creation and alteration JSON APIs](#item-4) ⭐️ 8.0/10
5. [Prompt Injection as Role Confusion: New Research Paper](#item-5) ⭐️ 8.0/10
6. [Moebius Inpainting Model Ported to Browser with WebGPU](#item-6) ⭐️ 8.0/10
7. [DeepSWE: A Contamination-Free Coding Benchmark](#item-7) ⭐️ 8.0/10
8. [LLM Inference Pricing Comparison Reveals Surprising Caching Costs](#item-8) ⭐️ 8.0/10
9. [RubyLLM 1.0: Unified Ruby Framework for Major AI Providers](#item-9) ⭐️ 7.0/10
10. [Nub: All-in-One Toolkit for Node.js](#item-10) ⭐️ 7.0/10
11. [Founding a GmbH in Germany: €9600, 152 Days of Bureaucracy](#item-11) ⭐️ 7.0/10
12. [Curated OCR Benchmarks and Models at Papers with Code](#item-12) ⭐️ 7.0/10
13. [Non-deterministic Vulnerability Detection Benchmark Using Juliet Cases](#item-13) ⭐️ 7.0/10
14. [OPFS + Pyodide Test Harness for Persistent SQLite Editing](#item-14) ⭐️ 6.0/10
15. [ML model security testing in production: a gap](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [John Carmack: Quake Mistakes Ruined id Software](https://twitter.com/ID_AA_Carmack/status/2069799283369345247) ⭐️ 8.0/10

John Carmack tweeted that pushing everyone too hard during Quake's development caused burnout and ultimately ruined id Software, reflecting that maturing companies need more slack. This reflection offers valuable lessons on startup intensity and company culture, relevant to software engineering and management, especially for teams transitioning from startup to mature organization. Carmack noted that running people constantly at startup intensity wears them out, and he apologized to Sandy Petersen, whose perspective on the matter appears in interviews. Quake is considered an iconic game, but the development process took a lasting toll on the company.

hackernews · shadowtree · Jun 24, 15:56 · [Discussion](https://news.ycombinator.com/item?id=48661825)

**Background**: id Software, founded in 1991, revolutionized first-person shooters with games like Wolfenstein 3D, Doom, and Quake. John Carmack was the lead programmer, known for pushing technical boundaries. The company's intense work culture was typical of startups but became unsustainable as it matured.

**Discussion**: Comments generally agree with Carmack's wisdom, with ChrisMarshallNY calling it valuable for many companies. Starkparker referenced Sandy Petersen's interviews. Rustyhancock argued Quake was worth the cost. Tejohnso noted that Quake III Arena seemed unaffected but Doom 3 lacked the same energy.

**Tags**: `#game development`, `#startup culture`, `#software engineering`, `#burnout`, `#John Carmack`

---

<a id="item-2"></a>
## [Bunny DNS Goes Free, Eliminates Query Fees](https://bunny.net/blog/were-making-bunny-dns-free/) ⭐️ 8.0/10

Bunny.net announced that its DNS service is now free, removing all DNS query fees and providing free DNS hosting for up to 500 domains per account. This move significantly lowers the barrier for website owners, especially those in the EU seeking alternatives to US-based providers like Cloudflare, by offering a competitive free tier with no query limits. Free DNS hosting includes up to 500 domains, unlimited DNS queries, and access to advanced features such as smart records and health monitoring without requiring enterprise plans.

hackernews · dabinat · Jun 24, 08:50 · [Discussion](https://news.ycombinator.com/item?id=48657030)

**Background**: DNS (Domain Name System) translates domain names into IP addresses, and DNS hosting services typically charge based on the number of queries. Many providers impose query limits or bill for overages. Bunny.net, known for its CDN and edge services, previously charged for DNS queries. This move makes Bunny DNS fully free, competing with other free DNS providers.

<details><summary>References</summary>
<ul>
<li><a href="https://bunny.net/dns/">Bunny DNS | The #1 Scriptable DNS Platform | bunny.net</a></li>
<li><a href="https://dn.org/the-economics-of-dns-costs-of-hosting-and-query-traffic/">The Economics of DNS Costs of Hosting and Query Traffic</a></li>

</ul>
</details>

**Discussion**: Overall sentiment is positive, with users praising the EU-based alternative to Cloudflare. Some express concerns about unexpected charges from bot traffic, noting that Bunny's billing safeguards only apply to CDN products. Others applaud the company's organic growth approach without investor pressure.

**Tags**: `#DNS`, `#CDN`, `#free service`, `#EU tech`

---

<a id="item-3"></a>
## [Krea 2: State-of-the-Art Open-Weight 12B Image Model Released](https://www.krea.ai/blog/krea-2-technical-report) ⭐️ 8.0/10

Krea has released the open weights and a detailed technical report for their Krea 2 model, a 12-billion-parameter text-to-image diffusion model that achieves state-of-the-art results. This release provides the AI community with a high-quality, open-weights image generation model that enables customization and research, challenging the dominance of proprietary systems and fostering transparency. The report covers data curation, captioning, model architecture, post-training, RL pipelines, prompt expansion, style references, and infrastructure; two versions are released: the standard Krea 2 and a distilled Turbo variant.

hackernews · mattnewton · Jun 23, 15:31 · [Discussion](https://news.ycombinator.com/item?id=48646659)

**Background**: Open-weights AI models allow users to access and modify the trained parameters, offering transparency and control over the model's behavior. Text-to-image models generate images from textual descriptions, and diffusion models are a leading approach. This release contributes to the growing ecosystem of open generative AI.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/open-models/">Open models by OpenAI</a></li>
<li><a href="https://www.oracle.com/artificial-intelligence/ai-open-weights-models/">“Open-weights” AI models offer transparency and control.</a></li>
<li><a href="https://openai.com/global-affairs/open-weights-and-ai-for-all/">Open weights and AI for all | OpenAI</a></li>

</ul>
</details>

**Discussion**: The community appreciates the detailed write-up and the model's versatility across many styles, though some commenters note that newer agentic composition models may already surpass it. There is also excitement about the Turbo variant being readily available in GGUF format.

**Tags**: `#open-weights`, `#text-to-image`, `#AI model`, `#technical report`, `#diffusion`

---

<a id="item-4"></a>
## [Datasette 1.0a35 adds table creation and alteration JSON APIs](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a35 introduces new web interfaces and JSON APIs for creating and altering SQLite tables, including support for columns, primary keys, constraints, and foreign keys. The release also adds stable template context documentation for custom templates. This release significantly enhances Datasette's programmatic schema management capabilities, allowing users to create and alter tables via API without manual SQL. It extends Datasette's utility as a data exploration and publishing platform for SQLite databases. The create table API is available at /<database>/-/create, and the alter table API at /<database>/<table>/-/alter. The alter API supports renaming, reordering, and dropping columns, as well as changing primary keys and foreign keys. The template context documentation is generated from dataclass definitions and treated as a stable API until Datasette 2.0.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring, publishing, and analyzing SQLite databases. It provides a web interface and a JSON API for querying and browsing data. Previously, schema modifications like creating or altering tables required direct SQL commands or external tools, limiting automation. With this release, Datasette gains built-in, API-driven schema management, making it easier to integrate into data pipelines.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://docs.datasette.io/en/stable/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://tools4all.ai/trends/datasette-10a35-introduces-table-creation-and-alteration-apis">Datasette 1.0a35 introduces table creation and alteration APIs</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#open-source`, `#data`, `#JSON API`, `#release`

---

<a id="item-5"></a>
## [Prompt Injection as Role Confusion: New Research Paper](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

A new research paper titled 'Prompt Injection as Role Confusion' confirms that LLMs cannot reliably distinguish privileged text from user input, and that models are more influenced by the style of text than its actual role tag. The paper demonstrates that 'destyling' text can reduce attack success rates from 61% to 10%. This research highlights a fundamental limitation in current language model security, suggesting that prompt injection defense is a 'perpetual whack-a-mole game' until models achieve genuine role perception. The finding that style matters more than role tags exposes a new vector for jailbreaks and undermines existing mitigation strategies. The paper introduces the concept of role confusion, showing that models like gpt-oss-20b can be tricked by mimicking the writing style of internal thinking blocks. 'Destyling'—rewriting text to look less like a role tag format—dramatically reduces attack success, yet the content remains semantically identical to a human reader.

rss · Simon Willison · Jun 22, 23:59

**Background**: Prompt injection is a vulnerability where attackers embed malicious instructions in user input that the model treats as system commands. Traditionally, developers use role tags like <system> and <user> to separate privileged instructions from user data, but this defense is brittle because both inputs are natural language. This paper formalizes the problem as 'role confusion,' where the model's perception of a text's source is influenced more by stylistic cues than by the explicit role tag.

<details><summary>References</summary>
<ul>
<li><a href="https://role-confusion.github.io/">Prompt Injection as Role Confusion</a></li>
<li><a href="https://github.com/role-confusion/prompt-injection-as-role-confusion">GitHub - role-confusion/prompt-injection-as-role-confusion: Prompt Injection as Role Confusion · GitHub</a></li>
<li><a href="https://genai.owasp.org/llmrisk/llm01-prompt-injection/">LLM01:2025 Prompt Injection - OWASP Gen AI Security Project</a></li>

</ul>
</details>

**Tags**: `#prompt injection`, `#LLM security`, `#AI safety`, `#role confusion`, `#jailbreaks`

---

<a id="item-6"></a>
## [Moebius Inpainting Model Ported to Browser with WebGPU](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison successfully ported the lightweight Moebius 0.2B image inpainting model to run entirely in a web browser using WebGPU, and released a working demo. This shows that advanced deep learning models like inpainting can run client-side without server dependencies, enabling privacy-preserving and offline-capable applications. It also lowers the barrier for using high-quality image editing directly in the browser. The port uses ONNX Runtime Web with the WebGPU backend, replacing the original PyTorch and CUDA. The demo lets users upload an image, mark regions to remove, and run inpainting entirely in-browser.

rss · Simon Willison · Jun 22, 23:43

**Background**: Image inpainting fills missing parts of an image plausibly. The Moebius model achieves high quality with only 0.2 billion parameters, making it suitable for client-side deployment. WebGPU is a modern web API for GPU compute, and ONNX Runtime Web runs ML models in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/22/porting-moebius/">Porting the Moebius 0.2B image inpainting model to run in the browser with Claude Code</a></li>
<li><a href="https://hustvl.github.io/Moebius/">Moebius Project Page</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebGPU_API">WebGPU API - Web APIs | MDN - MDN Web Docs</a></li>

</ul>
</details>

**Discussion**: On Hacker News and the blog, community members showed interest and discussed weight precision (FP32) and potential FP16 optimization. The overall sentiment was positive, with appreciation for the port and the detailed walkthrough.

**Tags**: `#inpainting`, `#WebGPU`, `#browser ML`, `#image generation`, `#model porting`

---

<a id="item-7"></a>
## [DeepSWE: A Contamination-Free Coding Benchmark](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE, a new open-source benchmark for frontier coding agents, was released, featuring tasks written from scratch across 91 repositories in 5 languages to ensure contamination-free evaluation. Existing benchmarks like SWE-bench may suffer from data contamination, where models have seen solutions during pretraining; DeepSWE provides a more realistic and reliable measure of coding agent performance in real-world software engineering tasks. DeepSWE tasks require 5.5x more code changes and ~2x output tokens compared to SWE-bench Pro prompts, and verifiers test software behavior rather than implementation details, increasing complexity and reliability.

reddit · r/MachineLearning · /u/we_are_mammals · Jun 24, 02:03

**Background**: Benchmark contamination occurs when LLMs are trained on data that includes test set solutions, inflating performance scores. SWE-bench and its variants are widely used but may not fully guard against this. DeepSWE addresses this by writing tasks from scratch, ensuring no model has seen the solution during pretraining, and by increasing task diversity and complexity to better reflect real-world software engineering challenges.

<details><summary>References</summary>
<ul>
<li><a href="https://labs.scale.com/leaderboard/swe_bench_pro_public">SWE-Bench Pro Leaderboard AI Coding Benchmark (Public Dataset) | Scale</a></li>
<li><a href="https://arxiv.org/html/2605.19999v1">LLM Benchmark Datasets Should Be Contamination-Resistant</a></li>

</ul>
</details>

**Tags**: `#benchmark`, `#AI coding`, `#software engineering`, `#machine learning`, `#open-source`

---

<a id="item-8"></a>
## [LLM Inference Pricing Comparison Reveals Surprising Caching Costs](https://www.reddit.com/r/MachineLearning/comments/1ueavxn/i_compiled_llm_inference_pricing_across_7/) ⭐️ 8.0/10

A Reddit user compiled a side-by-side comparison of LLM inference pricing across seven providers, including OpenRouter, DeepSeek, Together AI, Fireworks, and Groq, revealing that cached input costs vary dramatically, with cache hits being tens of times cheaper than misses for models like DeepSeek V4 Pro. This comparison is practically valuable for developers and companies optimizing LLM costs, as caching policies can have a greater impact on total cost than headline token prices, especially for agents, RAG pipelines, and multi-turn conversations. The spreadsheet includes input/output token pricing, context windows, and cached input pricing where available, but notes that real throughput, cold-start times, and precision (FP16 vs FP8) are not yet compared.

reddit · r/MachineLearning · /u/Technomadlyf · Jun 24, 11:28

**Background**: Prompt caching is a technique that reuses previously computed results for repeated portions of input prompts, significantly reducing latency and cost. DeepSeek is a Chinese AI company known for low-cost, high-performance open-weight models; its DeepSeek V4 Pro model is one example where caching costs vary widely across providers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/prompt-caching">What is Prompt Caching? - IBM</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_LLM">DeepSeek LLM</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion (78 comments) reflects strong interest in practical pricing insights, with users sharing additional metrics like throughput and reliability concerns, and some questioning the accuracy of caching prices from certain providers.

**Tags**: `#LLM pricing`, `#inference optimization`, `#caching`, `#cloud AI costs`, `#practical ML`

---

<a id="item-9"></a>
## [RubyLLM 1.0: Unified Ruby Framework for Major AI Providers](https://rubyllm.com/) ⭐️ 7.0/10

RubyLLM 1.0 was released as a unified Ruby framework that provides a beautiful, expressive API for all major AI providers, enabling developers to build chatbots, AI agents, RAG applications, and multimodal workflows with minimal code. This framework fills a critical gap in the Ruby ecosystem, which previously lacked a polished, unified AI library comparable to Python's LangChain or Vercel's AI SDK, potentially accelerating AI adoption in Ruby and Rails applications. Despite its elegant design, users report issues such as unreliable caching (e.g., with xAI's completions API returning incorrect thought signatures) and difficulty in achieving true trace observability, with retry patterns sometimes deleting underlying model history.

hackernews · doener · Jun 24, 14:41 · [Discussion](https://news.ycombinator.com/item?id=48660711)

**Background**: Ruby is a dynamic language popular for web development, especially with Ruby on Rails, but has lacked a comprehensive AI framework. RubyLLM aims to provide a unified, developer-friendly API across providers like OpenAI, Anthropic, and Google, similar to how Vercel's AI SDK works in the JavaScript ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://rubyllm.com/">RubyLLM | One beautiful Ruby framework for all major AI providers. Chat ...</a></li>
<li><a href="https://github.com/crmne/ruby_llm">GitHub - crmne/ruby_llm: One delightful Ruby framework for every major ...</a></li>
<li><a href="https://dev.to/crmne/introducing-rubyllm-10-a-beautiful-way-to-work-with-ai-5p0">Introducing RubyLLM 1.0: A Beautiful Way to Work with AI</a></li>

</ul>
</details>

**Discussion**: Community feedback is largely positive, with users praising its elegance and production-readiness. Some appreciate the issue tracker's feature request process that prevents scope creep. However, caveats include cache unreliability and observability challenges, though overall it is seen as an excellent library.

**Tags**: `#ruby`, `#AI framework`, `#LLM`, `#developer tools`, `#open source`

---

<a id="item-10"></a>
## [Nub: All-in-One Toolkit for Node.js](https://github.com/nubjs/nub) ⭐️ 7.0/10

Nub is a new toolkit that adds transpilation, module resolution, and polyfills to Node.js via a preload hook, enabling a Bun-like developer experience without replacing Node itself. It enhances Node.js developer productivity by providing TypeScript execution, faster package management, and built-in version switching, bridging the gap between Node.js and modern runtimes like Bun. Nub is written in Rust and uses an oxc-powered transpiler packaged as a Node-API add-on. It registers a module resolution hook and injects polyfills for APIs like Worker and Temporal, all purely additive without modifying Node's engine.

hackernews · colinmcd · Jun 24, 14:14 · [Discussion](https://news.ycombinator.com/item?id=48660267)

**Background**: Node.js is a popular JavaScript runtime but lacks built-in TypeScript support and efficient module resolution. Bun and Deno offer all-in-one experiences with these features. Nub adds similar capabilities to Node.js via a --require preload hook, combining Node's stability with modern tooling.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/nubjs/nub">GitHub - nubjs/nub: The all-in-one Node.js toolkit</a></li>
<li><a href="https://nubjs.com/">Nub — an all-in-one toolkit for Node.js</a></li>
<li><a href="https://nubjs.com/docs">Introduction — Nub</a></li>

</ul>
</details>

**Discussion**: The community response is positive. The creator highlighted the additive approach, and users praised embracing existing Node infrastructure rather than rewriting. One user reported zero issues after migrating a monorepo, while another inquired about TypeScript resolution compatibility.

**Tags**: `#typescript`, `#nodejs`, `#transpiler`, `#tooling`, `#polyfills`

---

<a id="item-11"></a>
## [Founding a GmbH in Germany: €9600, 152 Days of Bureaucracy](https://paolino.me/founding-a-company-in-germany/) ⭐️ 7.0/10

A tech entrepreneur recounts the costly and slow process of founding a GmbH in Germany, spending €9600 and 152 days without being able to send an invoice. This highlights bureaucratic inefficiencies that burden entrepreneurs in Germany, potentially discouraging startup formation and innovation. The process involves a minimum share capital of €25,000 for a GmbH, and the author criticizes the mandatory notary fees and long registration times.

hackernews · earcar · Jun 24, 12:31 · [Discussion](https://news.ycombinator.com/item?id=48658718)

**Background**: A GmbH (Gesellschaft mit beschränkter Haftung) is the German equivalent of a limited liability company, popular for liability protection. It requires a minimum capital of €25,000 and a notarized incorporation process.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GmbH">GmbH - Wikipedia</a></li>
<li><a href="https://www.investopedia.com/terms/g/gmbh.asp">GmbH: Definition, Requirements, and Comparison to LLCs</a></li>
<li><a href="https://stripe.com/resources/more/start-gmbh-germany">Incorporating a limited liability company (GmbH) in Germany | Stripe</a></li>

</ul>
</details>

**Discussion**: Commenters discuss alternatives like the UG (mini-GmbH) with lower capital, but note that the 'UG' label may signal lack of seriousness. Others debate the necessity of the €25,000 minimum and double taxation issues.

**Tags**: `#entrepreneurship`, `#Germany`, `#bureaucracy`, `#startup`, `#regulatory`

---

<a id="item-12"></a>
## [Curated OCR Benchmarks and Models at Papers with Code](https://www.reddit.com/r/MachineLearning/comments/1ueiam6/find_the_best_opensource_ocr_models_in_one_place/) ⭐️ 7.0/10

A new curated page on Papers with Code lists major OCR benchmarks and top open-source models, featuring recent releases like Baidu's Unlimited OCR (3B parameters with Reference Sliding Window Attention) and Mistral OCR v4 (API-based). This centralized resource helps practitioners quickly identify the best OCR models for powering Retrieval-Augmented Generation (RAG) and agentic AI workflows, which convert messy PDFs into structured Markdown for chatbots and enterprise applications. Recommended benchmarks include OlmOCRBench by Ai2 and OmniDocBench by Shanghai AI Laboratory; top recommended models are Chandra OCR 2 (open-source, self-hostable) and Mistral OCR v4 (API). Baidu's Unlimited OCR introduces Reference Sliding Window Attention (R-SWA) to handle long sequences efficiently.

reddit · r/MachineLearning · /u/NielsRogge · Jun 24, 16:26

**Background**: Optical Character Recognition (OCR) digitizes scanned documents and PDFs into machine-readable text. The rise of agentic RAG, which combines AI agents with retrieval-augmented generation, demands robust OCR to convert diverse document formats into clean Markdown for downstream AI consumption. Papers with Code revived its platform to host this task-specific hub.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/reference-sliding-window-attention-r-swa">Reference Sliding Window Attention (R-SWA)</a></li>
<li><a href="https://arxiv.org/abs/2512.10411">[2512.10411] SWAA: Sliding Window Attention Adaptation for ... Unlimited OCR Works - arXiv.org SWA Chapter 4 Guide | Sebastian Raschka, PhD Sliding Window Attention - GeeksforGeeks Sliding Window Attention (SWA) | Sebastian Raschka, PhD Sliding Window Attention: A Comprehensive Guide for 2025</a></li>
<li><a href="https://www.ibm.com/think/topics/agentic-rag">What is Agentic RAG? | IBM</a></li>

</ul>
</details>

**Tags**: `#OCR`, `#Machine Learning`, `#Open Source`, `#RAG`, `#Benchmarks`

---

<a id="item-13"></a>
## [Non-deterministic Vulnerability Detection Benchmark Using Juliet Cases](https://www.reddit.com/r/MachineLearning/comments/1ud0rft/nondeterministic_vulnerability_detection/) ⭐️ 7.0/10

A new benchmark system transforms Juliet test cases to look like real-world code and injects misleading or neutral comments to test LLMs' ability to detect vulnerabilities, aiming to prevent overfitting to known CWE patterns. This addresses a critical gap in LLM-based vulnerability detection by evaluating resilience to comment manipulation and obfuscation, potentially leading to more robust security tools. The benchmark is about 80% complete and currently covers several hundred CWEs, with code snippets sized to fill input context. Remaining work includes presentation, benchmarking published LLMs, and pruning CWEs that might be recognized as Juliet code.

reddit · r/MachineLearning · /u/Psychological_Meat_6 · Jun 22, 23:34

**Background**: The Juliet test suite is a synthetic collection of Java test cases covering 112 common weaknesses (CWEs) used for vulnerability detection research. LLMs often perform well on these test cases but may overfit to the synthetic patterns, failing on real-world code. This benchmark transforms them to reduce such advantages and adds comment manipulation to test natural language influence.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/find-sec-bugs/juliet-test-suite">GitHub - find-sec-bugs/juliet-test-suite: :microscope: A collection of test cases in the Java language. It contains examples for 112 different CWEs. · GitHub</a></li>
<li><a href="https://www.researchgate.net/figure/Experimental-results-for-vulnerability-discovery-on-the-Juliet-test-suite_fig3_352889408">Experimental results for vulnerability discovery on the Juliet test suite | Download Scientific Diagram</a></li>

</ul>
</details>

**Tags**: `#vulnerability detection`, `#LLM benchmarking`, `#cybersecurity`, `#code analysis`, `#non-deterministic`

---

<a id="item-14"></a>
## [OPFS + Pyodide Test Harness for Persistent SQLite Editing](https://simonwillison.net/2026/Jun/23/opfs-pyodide/#atom-everything) ⭐️ 6.0/10

Simon Willison released a test harness that uses the Origin Private File System (OPFS) with Pyodide to explore editing persistent SQLite files directly in the browser. This tool demonstrates a path for running full Python applications like Datasette Lite entirely in the browser with persistent local storage, potentially enabling powerful offline data analysis tools. The harness is a playground UI built by Claude Code for web, allowing users to test OPFS support across different browsers. It addresses a key limitation of Datasette Lite — the inability to persist data across sessions.

rss · Simon Willison · Jun 23, 18:58

**Background**: The Origin Private File System (OPFS) is a browser storage API that provides a private, sandboxed filesystem for web applications, optimized for performance. Pyodide is a port of CPython to WebAssembly, enabling Python to run in the browser. Datasette Lite is a browser-based version of the Datasette data exploration tool, which currently runs entirely in memory.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/File_System_API/Origin_private_file_system">Origin private file system - Web APIs | MDN</a></li>
<li><a href="https://web.dev/articles/origin-private-file-system">The origin private file system | Articles | web.dev</a></li>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.0</a></li>

</ul>
</details>

**Tags**: `#webassembly`, `#pyodide`, `#opfs`, `#browser-storage`, `#datasette-lite`

---

<a id="item-15"></a>
## [ML model security testing in production: a gap](https://www.reddit.com/r/MachineLearning/comments/1uddtws/are_model_security_risks_extraction_poisoning/) ⭐️ 6.0/10

A Reddit post highlights that many ML teams skip adversarial testing like extraction and poisoning before deploying models, raising concerns about a security review gap compared to traditional software. This matters because deployed ML models without security testing are vulnerable to attacks that can steal intellectual property (extraction) or degrade model integrity (poisoning), posing risks to business and user trust. Model extraction attacks aim to replicate a model's functionality via query APIs, while data poisoning attacks manipulate training data to alter model behavior; both are well-studied but rarely addressed in production pipelines.

reddit · r/MachineLearning · /u/Xorphian · Jun 23, 10:52

**Background**: Model security risks like extraction and poisoning are critical threats in machine learning. Extraction attacks allow adversaries to steal a model by observing its outputs, while poisoning attacks inject malicious data during training to cause misbehavior. Despite extensive academic research, industry adoption of defenses remains low, especially in production.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2502.16065v1">A Survey of Model Extraction Attacks and Defenses in ...</a></li>

</ul>
</details>

**Tags**: `#model security`, `#adversarial testing`, `#ML production`, `#security review`

---