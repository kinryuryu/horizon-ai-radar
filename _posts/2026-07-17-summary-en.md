---
layout: default
title: "Horizon Summary: 2026-07-17 (EN)"
date: 2026-07-17
lang: en
---

> From 53 items, 20 important content pieces were selected

---

1. [Firefox Compiled to WebAssembly Runs Inside Browser](#item-1) ⭐️ 9.0/10
2. [Inkling: Open-weights 975B MoE model from Thinking Machines Lab](#item-2) ⭐️ 9.0/10
3. [xAI open-sources Grok Build after privacy backlash](#item-3) ⭐️ 9.0/10
4. [Kimi K3: Largest Open Model with Opus 4.8-Class Performance](#item-4) ⭐️ 9.0/10
5. [Hugging Face Discloses July 2026 Security Incident](#item-5) ⭐️ 9.0/10
6. [New arXiv Book on Mathematics of Data Science](#item-6) ⭐️ 8.0/10
7. [Roc Compiler Team's Rust-to-Zig Rewrite Experience](#item-7) ⭐️ 8.0/10
8. [OTA Update Breaks Android Auto, Sparking Quality Debate](#item-8) ⭐️ 8.0/10
9. [GPT-Red: Self-Play Red Teaming for AI Safety](#item-9) ⭐️ 8.0/10
10. [DeepMind and Isomorphic Labs unveil bioresilience approach](#item-10) ⭐️ 8.0/10
11. [GPT-5.6 Codex Bug Can Delete Files in Full Access Mode](#item-11) ⭐️ 8.0/10
12. [Linus Torvalds Endorses AI in Linux Kernel](#item-12) ⭐️ 8.0/10
13. [Claude Tricked into Leaking Private Data via web_fetch Loophole](#item-13) ⭐️ 8.0/10
14. [Lila Sciences: Labs as Data Centers for AI Discovery](#item-14) ⭐️ 8.0/10
15. [NVIDIA Nemotron-3 Embed Tops RTEB, Boosts Agentic Retrieval](#item-15) ⭐️ 8.0/10
16. [Newer AI Models Maintain Scaling Law Advantages](#item-16) ⭐️ 8.0/10
17. [Model Routing: Simple in Theory, Hard in Practice](#item-17) ⭐️ 8.0/10
18. [QLoRA default learning rate 2e-4 is wrong for small datasets](#item-18) ⭐️ 8.0/10
19. [ExTernD: Ternary LLM PTQ with Accuracy Approaching Any Level](#item-19) ⭐️ 8.0/10
20. [PnP-CoSMo: Plug-and-Play Multi-Contrast MRI via Content/Style Modeling](#item-20) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Firefox Compiled to WebAssembly Runs Inside Browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter has compiled the full Firefox browser to WebAssembly, allowing it to run inside another browser like Chrome. The project used an estimated $25,000 worth of Claude Opus and Fable tokens for AI-assisted development. This is a groundbreaking technical achievement that demonstrates the possibility of running a full browser inside another browser, potentially enabling new forms of virtualization and cross-platform compatibility. It also showcases the power of AI-assisted programming in tackling complex engineering challenges. The demo uses the Wisp protocol to proxy all network traffic through Puter's server, as WebAssembly code cannot open arbitrary network connections. The project claims end-to-end encryption, and inspection confirmed that HTTPS traffic remains encrypted while HTTP traffic is visible.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (WASM) is a binary instruction format that allows code written in languages like C++ to run in web browsers at near-native speed. Compiling a full browser engine like Firefox's Gecko to WASM is extremely challenging due to the complexity of browser internals and the need to handle network access, which browsers restrict for security reasons.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus">Claude Opus</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was highly positive, with many expressing amazement at the technical feat. Some commenters noted the high server costs and the clever use of AI tools, while others discussed the potential security implications and the clever use of the Wisp protocol for networking.

**Tags**: `#WebAssembly`, `#Firefox`, `#Browser`, `#Virtualization`, `#AI-assisted development`

---

<a id="item-2"></a>
## [Inkling: Open-weights 975B MoE model from Thinking Machines Lab](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 9.0/10

Thinking Machines Lab, founded by Mira Murati, released Inkling, an open-weights Mixture-of-Experts multimodal model with 975B total parameters and 41B active parameters, under the Apache-2.0 license. Inkling strengthens the US open-weights AI ecosystem, offering a competitive alternative to Chinese open models and enabling fine-tuning via the Tinker platform, which could accelerate custom AI development. The model card and training data documentation are sparse, with minimal details about data sources. A smaller variant, Inkling-Small (276B total, 12B active), is still in testing and will be released later.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) models use multiple specialized sub-networks (experts) and activate only a subset per input, enabling larger total parameters with lower computational cost. Open-weights models release trained parameters publicly, allowing download and fine-tuning, but may not include full training code or data. The Apache-2.0 license permits free use, modification, and distribution.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#Mira Murati`

---

<a id="item-3"></a>
## [xAI open-sources Grok Build after privacy backlash](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 9.0/10

xAI released the entire Grok Build codebase under the Apache 2.0 license after users discovered the CLI tool uploaded entire directories to Google Cloud buckets, including sensitive files like SSH keys and password databases. This incident highlights serious privacy risks in AI-powered developer tools and the importance of transparency; open-sourcing the code is a step toward rebuilding trust, but the initial design flaw raises questions about data handling practices in the industry. The codebase contains 844,530 lines of Rust, with only about 3% vendored, and includes a self-contained Mermaid diagram renderer using Unicode box-drawing. xAI deleted all previously retained user data and disabled default data retention.

rss · Simon Willison · Jul 15, 23:59

**Background**: Grok Build is a CLI tool from xAI that uses AI models to assist with coding tasks. The Apache 2.0 license is a permissive open-source license that allows users to freely use, modify, and distribute the software. Google Cloud buckets are cloud storage containers used to store data objects.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/superagent-ai/grok-cli">GitHub - superagent-ai/grok-cli: An open-source coding agent for the Grok API · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apache_License">Apache License</a></li>
<li><a href="https://docs.cloud.google.com/storage/docs/buckets">About Cloud Storage buckets | Google Cloud Documentation</a></li>

</ul>
</details>

**Discussion**: The community reacted with outrage when the upload behavior was discovered, with one user reporting that running the tool in their home directory uploaded SSH keys, password manager databases, and personal files. xAI's response—deleting retained data and open-sourcing the code—was seen as a necessary but belated step to regain trust.

**Tags**: `#security`, `#open source`, `#AI`, `#privacy`, `#xAI`

---

<a id="item-4"></a>
## [Kimi K3: Largest Open Model with Opus 4.8-Class Performance](https://www.latent.space/p/ainews-kimi-k3-28t-a50b-the-largest) ⭐️ 9.0/10

Kimi released K3, the largest open model ever with 2.8 trillion parameters, claiming Opus 4.8-class performance at Sonnet 5 pricing. This marks a significant milestone in open AI, offering frontier-level performance at a lower cost, potentially accelerating AI commoditization and competition. K3 uses a hybrid linear attention mechanism called Kimi Delta Attention and Attention Residuals, supports a 1M token context window, and is priced at $3/$15 per million tokens (cache $0.3).

rss · Latent Space · Jul 17, 01:46

**Background**: Open models are AI models with publicly available weights, allowing anyone to use, modify, or study them. Opus 4.8 is Anthropic's latest frontier model, while Sonnet 5 is a more affordable model from Anthropic. Kimi K3 aims to bridge the gap between open and closed models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://artificialanalysis.ai/models/kimi-k3">Kimi K 3 - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K 3 - Kimi API Platform</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the model's high cost for a Chinese open-weight model but note it's justified if truly competitive. Some see Chinese labs driving AI commoditization, while others question the payoff of such massive investments.

**Tags**: `#AI`, `#open models`, `#Kimi K3`, `#large language models`, `#machine learning`

---

<a id="item-5"></a>
## [Hugging Face Discloses July 2026 Security Incident](https://huggingface.co/blog/security-incident-july-2026) ⭐️ 9.0/10

Hugging Face published a blog post disclosing a security incident that occurred in July 2026, detailing the nature of the breach and the steps taken to address it. As a major AI/ML platform hosting models and datasets, a security incident at Hugging Face could compromise user trust and affect the broader AI community. This disclosure is critical for users to assess risks and take protective actions. The blog post outlines the incident timeline, affected systems, and remediation measures, but specific technical details such as the attack vector or data exposed are not provided in the summary.

rss · Hugging Face Blog · Jul 16, 00:00

**Background**: Hugging Face is a popular platform for sharing machine learning models and datasets, used by researchers and developers worldwide. Security incidents on such platforms can lead to unauthorized access to proprietary models or sensitive data, making transparency important for maintaining community trust.

**Tags**: `#security`, `#incident disclosure`, `#Hugging Face`, `#AI/ML`

---

<a id="item-6"></a>
## [New arXiv Book on Mathematics of Data Science](https://arxiv.org/abs/2607.11938) ⭐️ 8.0/10

A new book titled 'Mathematics of Data Science' has been posted on arXiv, focusing on high-dimensional intuition and its role in modern data science and machine learning. This resource addresses a critical gap by building intuition for high-dimensional spaces, which is essential for understanding modern ML algorithms like stochastic gradient descent and high-dimensional models. The book emphasizes how everyday intuition breaks down in high dimensions, covering concepts like spikiness and volume, and connects these to practical model fitting and optimization.

hackernews · Anon84 · Jul 16, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48939896)

**Background**: In data science and machine learning, data often lives in high-dimensional spaces (hundreds or thousands of features). The 'curse of dimensionality' causes phenomena like data sparsity and distance metric breakdown, making it crucial to develop new intuitions beyond our 3D experience.

<details><summary>References</summary>
<ul>
<li><a href="https://towardsdatascience.com/intuitions-in-high-dimensional-spaces-c22f0441ce19/">Intuitions in high-dimensional spaces - Towards Data Science</a></li>
<li><a href="https://en.wikipedia.org/wiki/Curse_of_dimensionality">Curse of dimensionality</a></li>
<li><a href="https://www.mathstacy.com/2025/09/weirdness-of-high-dimensions.html">Weirdness of High Dimensions - mathstacy.com</a></li>

</ul>
</details>

**Discussion**: Commenters praised the book's focus on high-dimensional intuition, noting it helps students understand fundamental concepts like stochastic gradient descent. One commenter also discussed the overloaded term 'data science' and the value of building intuition for decision-making.

**Tags**: `#data science`, `#mathematics`, `#high-dimensional`, `#machine learning`, `#education`

---

<a id="item-7"></a>
## [Roc Compiler Team's Rust-to-Zig Rewrite Experience](https://rtfeldman.com/rust-to-zig) ⭐️ 8.0/10

The Roc compiler team published a detailed blog post about their ongoing rewrite from Rust to Zig, highlighting Zig's superior memory control and cross-compilation capabilities while acknowledging Rust's safety advantages. This rewrite demonstrates real-world trade-offs between Rust and Zig for systems programming, particularly for compilers, and may influence language choices in the systems programming community. The post notes that for compilers emitting machine code, memory-unsafe operations are often necessary, and Zig's explicit memory control and fast incremental builds are key motivators for the switch.

hackernews · jorangreef · Jul 16, 11:39 · [Discussion](https://news.ycombinator.com/item?id=48933149)

**Background**: Roc is a fast, friendly functional language whose compiler is being rewritten. Rust is known for memory safety without garbage collection, while Zig offers manual memory management and seamless cross-compilation. The rewrite highlights the different philosophies of the two languages.

<details><summary>References</summary>
<ul>
<li><a href="https://www.roc-lang.org/">The Roc Programming Language</a></li>
<li><a href="https://zig.guide/build-system/cross-compilation/">Cross-compilation - zig.guide</a></li>
<li><a href="https://piembsystech.com/memory-management-in-zig-programming-language/">Memory Management in Zig Programming Language</a></li>

</ul>
</details>

**Discussion**: Steve Klabnik questioned the claim that memory-unsafe operations are a big part of compiler work, arguing that only hot patching requires unsafe code, not regular compilation. Other commenters debated Zig's incremental build speed and the feasibility of achieving similar features in Rust.

**Tags**: `#Rust`, `#Zig`, `#compilers`, `#programming languages`, `#systems programming`

---

<a id="item-8"></a>
## [OTA Update Breaks Android Auto, Sparking Quality Debate](https://imdanielkendall.com/the-great-software-regress-how-move-fast-and-break-things-broke-our-lives/) ⭐️ 8.0/10

A car owner reports that an over-the-air (OTA) update broke Android Auto functionality, highlighting a growing trend of automotive software updates introducing new bugs rather than fixing them. This incident underscores systemic issues in automotive software quality, where users bear the cost of broken updates, potentially eroding trust in car brands and impacting sales decisions. The author's personal account describes Android Auto ceasing to work after an OTA update, with no explanation or fix provided. Similar issues have been reported with Kia EV9 updates breaking CarPlay.

hackernews · Expletive4138 · Jul 16, 22:29 · [Discussion](https://news.ycombinator.com/item?id=48941129)

**Background**: OTA updates allow car manufacturers to remotely update vehicle software, adding features or fixing issues without a dealership visit. Android Auto is a Google platform that mirrors smartphone apps on a car's infotainment display. As cars become more software-defined, the risk of updates introducing regressions increases.

<details><summary>References</summary>
<ul>
<li><a href="https://www.consumerreports.org/cars/car-maintenance/ota-car-software-updates-are-they-safe-how-they-work-a4081157745/">OTA Car Software Updates: Are They Safe and How Do They Work? via @ConsumerReports</a></li>
<li><a href="https://en.wikipedia.org/wiki/Android_Auto">Android Auto</a></li>

</ul>
</details>

**Discussion**: Commenters widely agree that users are effectively unpaid QA testers, with one noting that the cost of shipping broken software has shifted from manufacturers to consumers. Others argue that automotive software should be more conservative, avoiding unnecessary digitalization of hardware functions.

**Tags**: `#automotive software`, `#software quality`, `#OTA updates`, `#agile development`, `#user experience`

---

<a id="item-9"></a>
## [GPT-Red: Self-Play Red Teaming for AI Safety](https://openai.com/index/unlocking-self-improvement-gpt-red) ⭐️ 8.0/10

OpenAI has introduced GPT-Red, an automated red teaming system that uses self-play to improve AI safety, alignment, and robustness against prompt injection attacks. This development automates a critical safety evaluation process, potentially reducing the need for human red teamers and enabling continuous improvement of AI models against evolving threats like prompt injection. GPT-Red works by having one instance of the model act as an attacker to find vulnerabilities, while another instance acts as a defender, in a self-play zero-sum game. It has reportedly outperformed human red teamers on prompt injection tests.

rss · OpenAI News · Jul 15, 10:00

**Background**: Red teaming is a security practice where testers simulate attacks to find weaknesses. In AI, prompt injection attacks involve inserting malicious instructions into inputs to hijack a model's behavior. Self-play is a reinforcement learning technique where an agent improves by playing against itself, and has been applied to AI safety by having models generate and defend against attacks in a loop.

<details><summary>References</summary>
<ul>
<li><a href="https://www.technologyreview.com/2026/07/15/1140514/meet-gpt-red-an-llm-super-hacker-openai-built-to-make-its-models-safer/">Meet GPT-Red: an LLM super-hacker OpenAI built to make its models safer | MIT Technology Review</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/07/16/openai-gpt-red-prompt-injection-test/">GPT-Red beat human red teamers on a prompt injection test - Help Net Security</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#red teaming`, `#self-play`, `#alignment`, `#prompt injection`

---

<a id="item-10"></a>
## [DeepMind and Isomorphic Labs unveil bioresilience approach](https://deepmind.google/blog/our-approach-to-bioresilience/) ⭐️ 8.0/10

Google DeepMind and Isomorphic Labs have announced their joint approach to bioresilience, leveraging AI models to enhance the adaptability of biological systems to environmental and anthropogenic changes. This initiative could revolutionize healthcare and biological research by using AI to predict and mitigate biological threats, potentially leading to new treatments and improved ecosystem resilience. The approach builds on DeepMind's AlphaFold technology, which accurately predicts protein structures, and aims to apply AI to broader biological resilience challenges. No specific models or timelines were disclosed in the announcement.

rss · Google DeepMind Blog · Jul 16, 09:30

**Background**: Bioresilience refers to the ability of biological systems—from genes to ecosystems—to resist and recover from perturbations. Isomorphic Labs, a spin-off from DeepMind, focuses on AI-driven drug discovery. This joint effort signals a strategic expansion from drug discovery to broader biological adaptation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bioresilience">Bioresilience - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Isomorphic_Labs">Isomorphic Labs</a></li>
<li><a href="https://www.isomorphiclabs.com/">Reimagining Drug Discovery Process with AI - Isomorphic Labs</a></li>

</ul>
</details>

**Tags**: `#AI`, `#bioresilience`, `#DeepMind`, `#Isomorphic Labs`, `#healthcare`

---

<a id="item-11"></a>
## [GPT-5.6 Codex Bug Can Delete Files in Full Access Mode](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

Thibault Sottiaux from OpenAI reported that GPT-5.6 Codex can unexpectedly delete files when full access mode is enabled without sandboxing, due to a mistake in overriding the $HOME environment variable. This bug highlights critical safety risks in AI coding agents with full system access, emphasizing the need for sandboxing and auto-review features to prevent destructive actions. The bug occurs when Codex attempts to override $HOME to define a temporary directory but mistakenly deletes $HOME instead. The issue is most common when full access mode is enabled and sandboxing or auto review is disabled.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is an AI coding agent that can autonomously read, write, and execute code. Full access mode gives it unrestricted system permissions, while sandboxing isolates its operations to prevent harm. The $HOME environment variable points to the user's home directory, and overriding it incorrectly can lead to unintended file deletions.

<details><summary>References</summary>
<ul>
<li><a href="https://explainx.ai/blog/openai-codex-gpt-5-6-home-deletion-full-access-july-2026">Codex GPT - 5 . 6 $HOME Deletion — Full Access | explainx.ai</a></li>
<li><a href="https://amux.io/guides/ai-agent-sandboxing/">AI Agent Sandboxing in 2026: Docker, E2B, Firecracker... — amux</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#AI safety`, `#bug`

---

<a id="item-12"></a>
## [Linus Torvalds Endorses AI in Linux Kernel](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds, the creator and top maintainer of Linux, publicly declared that Linux is not an anti-AI project and that AI is a clearly useful tool, warning that those who disagree can fork the project or leave. This authoritative stance from the top Linux maintainer signals a strong endorsement of AI integration in the kernel, potentially influencing the open-source community's acceptance of AI tools and shaping future development practices. Torvalds made the statement on the Linux Media Mailing List, emphasizing that AI's usefulness is no longer in question, though he acknowledged other open questions about AI's economic impact.

rss · Simon Willison · Jul 16, 13:26

**Background**: The Linux kernel is a massive open-source project with thousands of contributors. AI tools, such as large language models, have been increasingly used in software development for tasks like code generation and bug detection, but have also faced resistance from some developers concerned about quality, ethics, or job displacement.

**Tags**: `#Linux`, `#AI`, `#Open Source`, `#Linus Torvalds`

---

<a id="item-13"></a>
## [Claude Tricked into Leaking Private Data via web_fetch Loophole](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Researcher Ayush Paul discovered a loophole in Claude's web_fetch tool that allowed an attacker to exfiltrate private user data, such as name, city, and employer, by tricking the model into following nested links from a honeypot site. This attack bypasses Anthropic's security design for web_fetch, which was intended to prevent data exfiltration, highlighting a critical vulnerability in LLM agent safety that could affect all users of Claude. The attack worked because web_fetch was allowed to visit URLs embedded in previously fetched pages, enabling a chain of requests that exfiltrated data. Anthropic had already identified the issue internally and closed the hole by removing the ability to follow links from fetched content.

rss · Simon Willison · Jul 15, 14:21

**Background**: The 'lethal trifecta' describes a dangerous combination in LLM agents: access to private data, ability to communicate externally, and exposure to untrusted content. Claude's web_fetch tool was designed to only fetch URLs provided by the user or from its web_search tool, but the loophole allowed following links from fetched pages, enabling prompt injection attacks.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and...</a></li>
<li><a href="https://ellmer.tidyverse.org/reference/claude_tool_web_fetch.html">Claude web fetch tool — claude _ tool _ web _ fetch • ellmer</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#data exfiltration`, `#Claude`, `#vulnerability`, `#LLM security`

---

<a id="item-14"></a>
## [Lila Sciences: Labs as Data Centers for AI Discovery](https://www.latent.space/p/the-lab-of-the-future-should-feel) ⭐️ 8.0/10

Lila Sciences proposes transforming scientific laboratories into data centers that generate training data for AI-driven discovery, rather than relying on internet data. This approach could unlock a vast, untapped source of high-quality training data for AI, accelerating breakthroughs in medicine, materials, and sustainability. Lila Sciences aims to build autonomous labs that use AI to design, conduct, observe, and redesign experiments, effectively treating the lab as a data generation engine.

rss · Latent Space · Jul 16, 13:30

**Background**: Traditional AI training relies heavily on internet data, which is finite and noisy. Lila Sciences believes that scientific experimentation can produce structured, high-value data that is more suitable for training AI models to make novel discoveries.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lila.ai/">LILA | Scientific Superintelligence</a></li>
<li><a href="https://www.lila.ai/about">About | LILA | The World's First Operating System for Science</a></li>

</ul>
</details>

**Tags**: `#AI`, `#scientific discovery`, `#automation`, `#data infrastructure`, `#lab automation`

---

<a id="item-15"></a>
## [NVIDIA Nemotron-3 Embed Tops RTEB, Boosts Agentic Retrieval](https://huggingface.co/blog/nvidia/nemotron-3-embed-wins-rteb) ⭐️ 8.0/10

NVIDIA's Nemotron-3 Embed model achieved the #1 overall score on the Retrieval Text Embedding Benchmark (RTEB), a new benchmark focused on realistic retrieval tasks. This marks a significant advancement in agentic retrieval capabilities for AI systems. This achievement sets a new standard for embedding models in retrieval-augmented generation (RAG) and agentic AI, where accurate and efficient retrieval is critical. It validates NVIDIA's approach to building specialized models for agentic workflows, potentially influencing future model development and enterprise AI deployments. The Nemotron-3 Embed model is a 1B-parameter text embedding model optimized for retrieval and semantic similarity, with strong multilingual and cross-lingual capabilities. It is designed as a foundational component for RAG systems and is available via NVIDIA NIM.

rss · Hugging Face Blog · Jul 16, 16:01

**Background**: Embedding models convert text into numerical vectors that capture semantic meaning, enabling efficient similarity search in retrieval systems. RTEB is a new benchmark that evaluates retrieval accuracy of embedding models and rerankers, focusing on realistic use cases. Agentic retrieval extends traditional RAG by allowing AI agents to dynamically plan, execute, and refine searches as part of a broader decision-making process.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/nvidia/nemotron-3-embed-wins-rteb">NVIDIA Nemotron 3 Embed Ranks #1 Overall on RTEB, Advancing ...</a></li>
<li><a href="https://build.nvidia.com/nvidia/nemotron-3-embed-1b/modelcard">nemotron-3-embed-1b Model by NVIDIA | NVIDIA NIM</a></li>
<li><a href="https://huggingface.co/blog/rteb">Introducing RTEB : A New Standard for Retrieval Evaluation</a></li>

</ul>
</details>

**Discussion**: The Hugging Face blog post has garnered positive attention from the community, with many praising the model's performance and the introduction of RTEB as a more realistic benchmark. Some commenters discussed the implications for RAG systems and the importance of multilingual support.

**Tags**: `#NVIDIA`, `#embeddings`, `#retrieval`, `#AI`, `#benchmark`

---

<a id="item-16"></a>
## [Newer AI Models Maintain Scaling Law Advantages](https://huggingface.co/blog/Dharma-AI/newer-models-same-advantages) ⭐️ 8.0/10

An analysis on Hugging Face shows that newer AI models continue to exhibit similar performance advantages over their predecessors, reinforcing the validity of neural scaling laws. This finding confirms that scaling up model size, data, and compute remains a reliable path to improved performance, guiding resource allocation for AI development. The analysis compares multiple generations of models across various benchmarks, showing consistent improvements that align with power-law scaling relationships.

rss · Hugging Face Blog · Jul 16, 11:49

**Background**: Neural scaling laws are empirical relationships that describe how model performance improves with increases in parameters, dataset size, and compute. These laws often follow a power-law form, where gains diminish but remain predictable. The analysis in the blog post tests whether newer models still obey these laws.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neural_scaling_law">Neural scaling law - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/artificial-intelligence/scaling-laws-in-ai/">Scaling Laws in AI - GeeksforGeeks</a></li>

</ul>
</details>

**Tags**: `#AI`, `#machine learning`, `#model scaling`, `#performance analysis`

---

<a id="item-17"></a>
## [Model Routing: Simple in Theory, Hard in Practice](https://huggingface.co/blog/ibm-research/model-routing-is-simple-until-it-isnt) ⭐️ 8.0/10

IBM Research published a detailed blog post on Hugging Face explaining why model routing for large language models (LLMs) is deceptively complex, with simple approaches failing in production due to trade-offs in cost, latency, and quality. As organizations deploy multiple LLMs, efficient routing is critical to balance performance and cost. This analysis provides practical insights for engineers building production-grade routing systems, highlighting pitfalls that naive implementations encounter. The post discusses challenges such as dynamic model availability, varying query complexity, and the need for continuous evaluation. It contrasts simple heuristics (e.g., always use the cheapest model) with learned routers that adapt over time.

rss · Hugging Face Blog · Jul 15, 17:27

**Background**: Model routing selects which LLM to use for each query, aiming to minimize cost while maintaining quality. Early approaches used fixed rules or thresholds, but real-world conditions—like model updates, cost changes, and diverse user requests—require more adaptive strategies. Libraries like RouteLLM and LLMRouter have emerged to address these needs.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ulab-uiuc/LLMRouter">LLMRouter: An Open-Source Library for LLM Routing - GitHub</a></li>
<li><a href="https://github.com/lm-sys/RouteLLM">GitHub - lm-sys/RouteLLM: A framework for serving and ...</a></li>
<li><a href="https://arxiv.org/abs/2502.08773">Universal Model Routing for Efficient LLM Inference GitHub - lm-sys/RouteLLM: A framework for serving and ... Model router for Microsoft Foundry concepts - Microsoft Foundry A Developer’s Guide to Model Routing - Medium [2603.04445] Dynamic Model Routing and Cascading for ... Best LLM routers and model routing platforms in 2026 Images</a></li>

</ul>
</details>

**Tags**: `#model routing`, `#LLM`, `#AI deployment`, `#systems design`, `#IBM Research`

---

<a id="item-18"></a>
## [QLoRA default learning rate 2e-4 is wrong for small datasets](https://www.reddit.com/r/MachineLearning/comments/1uy1z8b/the_qlora_2e4_default_is_wrong_under_10k_samples/) ⭐️ 8.0/10

A Reddit user argues that the widely used default learning rate of 2e-4 for QLoRA fine-tuning causes overfitting on datasets with fewer than 10,000 samples, and that reducing it to 1e-4 with more epochs significantly improves evaluation performance. This challenges a commonly accepted hyperparameter default in the LLM fine-tuning community, potentially saving practitioners weeks of debugging and improving model quality for small-scale fine-tuning tasks. The default 2e-4 originates from the Alpaca dataset (52k samples), but for datasets under 10k samples, the model overfits within the first epoch. The user recommends starting at 1e-4 or lower for datasets under 10k, and tuning for datasets between 10k and 30k.

reddit · r/MachineLearning · /u/Pretty-Ad774 · Jul 16, 12:50

**Background**: QLoRA is a parameter-efficient fine-tuning method that combines quantization and Low-Rank Adaptation (LoRA) to reduce memory usage. The learning rate is a critical hyperparameter; a value too high can cause overfitting on small datasets. Many tutorials and libraries default to 2e-4 based on the original QLoRA paper's Alpaca experiments.

<details><summary>References</summary>
<ul>
<li><a href="https://lightning.ai/pages/community/lora-insights/">Finetuning LLMs with LoRA and QLoRA : Insights from... - Lightning AI</a></li>
<li><a href="https://github.com/artidoro/qlora">GitHub - artidoro/ qlora : QLoRA : Efficient Finetuning of Quantized LLMs</a></li>
<li><a href="https://medium.com/@matteo28/qlora-fine-tuning-with-unsloth-a-complete-guide-8652c9c7edb3">QLoRA Fine-Tuning with Unsloth | Medium</a></li>

</ul>
</details>

**Discussion**: The Reddit post received strong engagement, with many users sharing similar experiences and confirming the finding. Some suggested using learning rate schedulers or lower ranks for small datasets, while others debated the exact threshold and the role of dataset quality.

**Tags**: `#QLoRA`, `#fine-tuning`, `#hyperparameters`, `#machine learning`, `#LLM`

---

<a id="item-19"></a>
## [ExTernD: Ternary LLM PTQ with Accuracy Approaching Any Level](https://www.reddit.com/r/MachineLearning/comments/1uy2zb3/externd_expandedrank_ternary_decomposition/) ⭐️ 8.0/10

ExTernD (Expanded-rank Ternary Decomposition) is proposed as a post-training quantization method for LLMs that decomposes each weight matrix into two ternary matrices and a diagonal scaling matrix, allowing the inner rank to be arbitrarily large to overcome accuracy limitations of fixed-size ternary quantization. This approach enables ternary quantization to achieve accuracy approaching any quantization level while using only slightly more VRAM than current methods, potentially making ternary LLMs more practical for deployment. The decomposition uses expanded-rank matrices, meaning the inner rank can be arbitrarily large, and the author claims the accuracy can be arbitrarily small. The method requires slightly more VRAM than existing quantization techniques.

reddit · r/MachineLearning · /u/LMTLS5 · Jul 16, 13:31

**Background**: Post-training quantization (PTQ) reduces the precision of LLM weights to lower bit-widths (e.g., ternary: -1, 0, +1) to improve inference speed and memory efficiency. Previous ternary PTQ methods used fixed-size matrices, which limited accuracy. ExTernD addresses this by decomposing the matrix into a product of two ternary matrices and a scaling diagonal, allowing flexible rank.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.13511">[2607.13511] ExTernD : Expanded-Rank Ternary Decomposition ...</a></li>
<li><a href="https://arxiv.org/html/2607.13511">ExTernD: Expanded - Rank Ternary Decomposition Ternary LLM PTQ...</a></li>
<li><a href="https://github.com/ozzzp/ternary_decompose">GitHub - ozzzp/ ternary _ decompose : Code of papers [ Ternary ...]</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion likely involves technical debate about the effectiveness and trade-offs of the method, but no specific comments are provided.

**Tags**: `#LLM`, `#quantization`, `#ternary`, `#PTQ`, `#decomposition`

---

<a id="item-20"></a>
## [PnP-CoSMo: Plug-and-Play Multi-Contrast MRI via Content/Style Modeling](https://www.reddit.com/r/MachineLearning/comments/1uy2h66/pnpcosmo_a_multicontrast_mri_reconstruction/) ⭐️ 8.0/10

PnP-CoSMo introduces a plug-and-play framework for multi-contrast MRI reconstruction that explicitly models contrast-invariant content and contrast-specific style, achieving state-of-the-art performance without requiring raw k-space training data. This work addresses a major data bottleneck in MRI reconstruction by eliminating the need for raw k-space data, and its generalizability across contrasts and forward operators could accelerate clinical adoption of deep learning-based MRI. The framework consists of two stages: first, a content/style model is learned from purely image-domain data; second, the frozen model serves as a prior in iterative reconstruction. The method is published in Medical Image Analysis with open code.

reddit · r/MachineLearning · /u/void_gear · Jul 16, 13:10

**Background**: Multi-contrast MRI acquires images with different tissue contrasts (e.g., T1-weighted, T2-weighted) to aid diagnosis, but long scan times often require undersampling and reconstruction. Traditional deep learning methods need paired raw k-space data, which is scarce and hard to obtain. Plug-and-play frameworks separate the denoising prior from the reconstruction algorithm, allowing flexible integration of learned models.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2509.04888">[2509.04888] INR meets Multi-Contrast MRI Reconstruction Deep unregistered multi-contrast MRI reconstruction Multi-Contrast MRI Reconstruction Based on Frequency Domain ... A plug-and-play method for guided multi-contrast MRI ... Prior-Guided Image Reconstruction for Accelerated Multi ... [2409.14113] Accelerated Multi-Contrast MRI Reconstruction ... INR Meets Multi-contrast MRI Reconstruction - Springer</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0730725X21000795">Deep unregistered multi-contrast MRI reconstruction</a></li>
<li><a href="https://arxiv.org/html/2502.20619">Style Content Decomposition-based Data Augmentation for ...</a></li>

</ul>
</details>

**Tags**: `#MRI reconstruction`, `#deep learning`, `#medical imaging`, `#plug-and-play`, `#content/style modeling`

---