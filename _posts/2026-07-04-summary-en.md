---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 54 items, 20 important content pieces were selected

---

1. [Mistral Releases Leanstral 1.5 for Lean 4](#item-1) ⭐️ 8.0/10
2. [AMD MI355X beats Blackwell on GLM5.2 inference at 2x lower cost](#item-2) ⭐️ 8.0/10
3. [SearXNG: A Free, Privacy-Respecting Metasearch Engine](#item-3) ⭐️ 8.0/10
4. [EU Parliament Member Hacked with Pegasus Spyware](#item-4) ⭐️ 8.0/10
5. [Wordgard: New Rich-Text Editor from ProseMirror Creator](#item-5) ⭐️ 8.0/10
6. [Ubicloud Advocates Strict Memory Overcommit for PostgreSQL](#item-6) ⭐️ 8.0/10
7. [Open Source AI Gap Map Launched](#item-7) ⭐️ 8.0/10
8. [Chrome DevTools MCP Server Enables AI Agents to Control Browser](#item-8) ⭐️ 8.0/10
9. [Anthropic Python SDK v0.116.0 Adds Beta Header for Agent Memory](#item-9) ⭐️ 7.0/10
10. [Guide to Running SOTA LLMs Locally Sparks Cost Debate](#item-10) ⭐️ 7.0/10
11. [Factories Are Just Rooms: A Philosophical Reflection](#item-11) ⭐️ 7.0/10
12. [Starlink Bridges Digital Divide in Africa](#item-12) ⭐️ 7.0/10
13. [FreeBSD Memory Reporting: Heuristics vs. Reality](#item-13) ⭐️ 7.0/10
14. [Google DeepMind and A24 announce first-of-its-kind research partnership](#item-14) ⭐️ 7.0/10
15. [Course Creator Reports 50%+ Revenue Drop Due to AI](#item-15) ⭐️ 7.0/10
16. [Simon Willison uses DSPy to optimize Datasette Agent prompts](#item-16) ⭐️ 7.0/10
17. [Understand to Participate: Key to AI Collaboration](#item-17) ⭐️ 7.0/10
18. [Vercel's Eve: A New Kind of Software Agent Framework](#item-18) ⭐️ 7.0/10
19. [Adobe Experiments with Self-Assembling Websites](#item-19) ⭐️ 7.0/10
20. [Skill Engineering vs. One-Shot AI Design](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Mistral Releases Leanstral 1.5 for Lean 4](https://mistral.ai/news/leanstral-1-5/) ⭐️ 8.0/10

Mistral has released Leanstral 1.5, a fine-tuned large language model specialized for theorem proving in Lean 4, which improves proof generation and bug finding capabilities. This model advances the use of LLMs in formal verification, a critical area for ensuring software correctness, and could make Lean 4 more accessible to developers and mathematicians. Leanstral 1.5 is fine-tuned from Mistral's base model and demonstrates improved performance on Lean 4 proof generation compared to earlier models, though some community members question the novelty of its bug-finding claims.

hackernews · programLyrique · Jul 3, 22:33 · [Discussion](https://news.ycombinator.com/item?id=48780801)

**Background**: Lean 4 is an interactive theorem prover and functional programming language used for formal verification. Fine-tuning an LLM on Lean 4 code and proofs aims to automate parts of the theorem proving process, reducing manual effort.

<details><summary>References</summary>
<ul>
<li><a href="https://lean-lang.org/theorem_proving_in_lean4/">Theorem Proving in Lean 4</a></li>
<li><a href="https://octagono.org/blog/lean-four/">Lean 4 : Theorem Proving Meets General-Purpose... — octagono</a></li>
<li><a href="https://benchlm.ai/models/leanstral">Leanstral Benchmarks: Data Coming Soon | BenchLM.ai</a></li>

</ul>
</details>

**Discussion**: Community comments highlight skepticism about the bug-finding example, noting that the overflow bug was already reported a week prior, and question the comparison baseline using older models. Some also discuss the choice of Lean 4 over other formal verification tools.

**Tags**: `#formal verification`, `#LLM`, `#Lean 4`, `#Mistral`, `#theorem proving`

---

<a id="item-2"></a>
## [AMD MI355X beats Blackwell on GLM5.2 inference at 2x lower cost](https://www.wafer.ai/blog/glm52-amd) ⭐️ 8.0/10

AMD's MI355X GPU achieves 2626 tokens per second per node on the GLM5.2 model, delivering over 2x lower cost compared to Nvidia's Blackwell architecture. This performance claim positions AMD as a viable alternative to Nvidia for AI inference, potentially reducing costs and supply chain dependency for data centers, especially outside the US. The reported throughput is an aggregate value, not actual per-request latency, and relies on assumptions like 60% cache hit rate and quantized model weights (mxfp4 instead of fp8), which may cause accuracy degradation.

hackernews · latchkey · Jul 3, 21:49 · [Discussion](https://news.ycombinator.com/item?id=48780417)

**Background**: GLM5.2 is Z.ai's flagship model for coding and agentic tasks, released in June 2026. The AMD MI355X is a new AI GPU with 288GB HBM3E memory and 8TB/s bandwidth, optimized for inference. Nvidia's Blackwell architecture is the previous generation, not specifically optimized for inference, while the upcoming Rubin is said to be 5x faster.

<details><summary>References</summary>
<ul>
<li><a href="https://ollama.com/library/glm-5.2">GLM - 5 . 2 is Z.ai’s flagship model for the era of long-horizon tasks.</a></li>
<li><a href="https://d33gy59ovltp76.cloudfront.net/news/amd-unveils-puzzling-new-mi355x-ai-gpu-as-it-acknowledges-there-won-t-be-any-ai-apu-for-now">AMD unveils puzzling new MI 355 X AI GPU as it</a></li>

</ul>
</details>

**Discussion**: Community comments highlight concerns about accuracy degradation when switching from fp8 to mxfp4, the reliance on a 60% cache hit assumption, and that the 2600 tok/s is an aggregate not actual throughput. Some users also request performance per watt metrics and note that Blackwell was not optimized for inference.

**Tags**: `#AMD`, `#GPU`, `#inference`, `#cost comparison`, `#GLM`

---

<a id="item-3"></a>
## [SearXNG: A Free, Privacy-Respecting Metasearch Engine](https://github.com/searxng/searxng) ⭐️ 8.0/10

SearXNG is a free and open-source metasearch engine that aggregates results from up to 280 search services without tracking or profiling users. It supports JSON output, making it suitable for integration with RAG systems and local AI models. SearXNG provides a privacy-focused alternative to centralized search engines, enabling users and developers to build custom search experiences. Its JSON API and compatibility with RAG pipelines make it a valuable tool for AI agents and local model search. SearXNG is a fork of the discontinued Searx and can be self-hosted via Docker. While it offers strong privacy, users may experience slower results and occasional CAPTCHA blocks from upstream search engines like DuckDuckGo or Brave.

hackernews · theanonymousone · Jul 3, 20:15 · [Discussion](https://news.ycombinator.com/item?id=48779454)

**Background**: A metasearch engine aggregates results from multiple search engines without maintaining its own index. SearXNG is a free, open-source metasearch engine that prioritizes user privacy by not collecting personal data. RAG (Retrieval-Augmented Generation) is a technique that enhances LLMs by retrieving external information, and SearXNG can serve as a privacy-preserving search backend for such systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SearXNG">SearXNG</a></li>
<li><a href="https://docs.searxng.org/">SearXNG Documentation (2026.7.3+21773bbb2)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Metasearch_engine">Metasearch engine</a></li>

</ul>
</details>

**Discussion**: Community members praise SearXNG for daily use and RAG applications, but note speed trade-offs and occasional blocks. The original Searx creator has moved on to a new project, Hister, which indexes full page content for offline previews. Some users recommend using the Brave Search API for reliability.

**Tags**: `#search engine`, `#privacy`, `#open source`, `#metasearch`, `#RAG`

---

<a id="item-4"></a>
## [EU Parliament Member Hacked with Pegasus Spyware](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

Citizen Lab investigation found that Stelios Kouloglou, a member of the European Parliament, had his iPhone infected with Pegasus spyware on multiple occasions in 2022 and 2023. This incident reveals state-sponsored espionage targeting EU parliament members, undermining democratic institutions and raising serious concerns about the misuse of commercial spyware in Europe. The first infection occurred around October 21, 2022, and subsequent infections on March 6-7, 2023, overlapping with a Pegasus campaign targeting exiled journalists and activists in Europe.

hackernews · ledoge · Jul 3, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48779683)

**Background**: Pegasus is a spyware developed by Israeli company NSO Group, capable of remotely compromising mobile devices. Citizen Lab is a research lab at the University of Toronto that investigates digital threats. The European Parliament has been investigating spyware abuses, including the Greek Predatorgate scandal.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>
<li><a href="https://citizenlab.ca/">The Citizen Lab - The Citizen Lab</a></li>

</ul>
</details>

**Discussion**: Comments highlight the Greek Predatorgate scandal and question whether the attack was by a member state rather than an external actor. Some users note that several European countries have abused Pegasus, with Israel cutting ties with some. Others criticize the lack of separation between work and personal devices for EU parliament members.

**Tags**: `#cybersecurity`, `#spyware`, `#espionage`, `#Pegasus`, `#European Parliament`

---

<a id="item-5"></a>
## [Wordgard: New Rich-Text Editor from ProseMirror Creator](https://wordgard.net/) ⭐️ 8.0/10

Wordgard is a new in-browser rich-text editor released by the creator of ProseMirror, offering a fresh approach with shared concepts but no direct upgrade path from ProseMirror. This release is significant because it comes from a highly respected developer in the rich-text editor ecosystem, potentially offering a simpler or more modern alternative to ProseMirror for new projects. Wordgard shares many concepts with ProseMirror but is not backward-compatible, meaning switching from ProseMirror requires significant rework. The editor features a clean design by artist Kamil Stankiewicz.

hackernews · indy · Jul 3, 08:50 · [Discussion](https://news.ycombinator.com/item?id=48772573)

**Background**: ProseMirror is a battle-tested, open-source rich-text editor framework widely used as the foundation for editors like Tiptap. It offers top-tier performance but has a steep learning curve. Wordgard aims to provide a fresh take on in-browser editing while retaining some of ProseMirror's core ideas.

<details><summary>References</summary>
<ul>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**Discussion**: The community is excited about Wordgard's design and potential, with some users noting the lack of an upgrade path from ProseMirror as a concern. Others appreciate the visual design and find the technical approach validating for their own work.

**Tags**: `#rich-text-editor`, `#prosemirror`, `#web-development`, `#open-source`, `#javascript`

---

<a id="item-6"></a>
## [Ubicloud Advocates Strict Memory Overcommit for PostgreSQL](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud published a blog post explaining why they use strict memory overcommit (vm.overcommit_memory=2) for PostgreSQL to prevent the OOM killer from terminating database processes, detailing trade-offs and configuration guidance. This is significant because PostgreSQL is notoriously vulnerable to the Linux OOM killer under default memory overcommit settings, and the article provides a practical, battle-tested configuration that can improve production database stability. Strict overcommit (mode 2) causes memory allocation requests that exceed the commit limit to fail immediately with ENOMEM, preventing the system from entering a state where the OOM killer must intervene. However, caution is needed because mode 2 can prevent fork() calls if the commit limit is set too low, potentially breaking application startup.

hackernews · furkansahin · Jul 3, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48774509)

**Background**: Linux memory overcommit allows processes to allocate more virtual memory than physical RAM, relying on the fact that not all allocated memory is used simultaneously. The OOM killer is a kernel mechanism that terminates processes when the system runs out of memory, which can kill PostgreSQL and cause data loss or corruption. PostgreSQL is especially sensitive because it uses shared memory and forking for connections.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit">PostgreSQL and the OOM Killer: Why We Use Strict Memory Overcommit</a></li>
<li><a href="https://en.wikipedia.org/wiki/Memory_overcommitment">Memory overcommitment - Wikipedia</a></li>
<li><a href="https://www.percona.com/blog/out-of-memory-killer-or-savior/">How to Adjust Linux Out-Of-Memory Killer Settings for PostgreSQL</a></li>

</ul>
</details>

**Discussion**: Commenters generally agreed with the technical content but urged caution: one noted that mode 2 can prevent forks if overcommit ratios are adjusted, and recommended thorough testing. Another shared experience of instability when using mode 2 with a Go backend that allocates large virtual memory. Ubicloud's Ozgun acknowledged the article's strong tone and noted that strict overcommit may not suit all scenarios.

**Tags**: `#PostgreSQL`, `#Linux`, `#memory management`, `#OOM killer`, `#database administration`

---

<a id="item-7"></a>
## [Open Source AI Gap Map Launched](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

Current AI, a non-profit founded at the AI Action Summit in Paris in February 2025, launched the Open Source AI Gap Map v0.1, indexing 421 open source AI products including 266 tools, 85 models, 50 datasets, and 20 hardware projects from 228 organizations. This map provides the first comprehensive, structured overview of the open source AI ecosystem, helping researchers and practitioners identify gaps and opportunities. The underlying data is released under an MIT license, enabling further analysis and community contributions. The map organizes products into 14 categories across 3 layers: model components, product/UX, and infrastructure. Additionally, 24,400 uncategorized artifacts are tracked but not scored until researched and cited.

rss · Simon Willison · Jul 3, 22:04

**Background**: Current AI is a global non-profit partnership backed by $400 million in committed capital, aiming to build a public option for AI. The Gap Map builds on work from experts at Columbia Convening, MOF, Hugging Face, and others to map the open source AI stack and identify missing components.

<details><summary>References</summary>
<ul>
<li><a href="https://map.currentai.org/">Current AI – Open Source AI Gap Map</a></li>

</ul>
</details>

**Tags**: `#open source`, `#AI`, `#ecosystem`, `#mapping`, `#non-profit`

---

<a id="item-8"></a>
## [Chrome DevTools MCP Server Enables AI Agents to Control Browser](https://github.com/ChromeDevTools/chrome-devtools-mcp) ⭐️ 8.0/10

The Chrome DevTools team has released an official MCP server that allows AI coding agents to inspect, debug, and control a live Chrome browser via the Model Context Protocol. This bridges AI coding assistants with real browser debugging capabilities, potentially revolutionizing automated testing, web development, and performance analysis workflows. The server is written in TypeScript and currently in public preview, supporting tools like element inspection, console logging, and network monitoring.

ossinsight · ChromeDevTools · Jul 4, 02:03

**Background**: The Model Context Protocol (MCP) is an open standard developed by Anthropic for connecting AI agents to external tools and data sources. An MCP server exposes specific capabilities (tools/resources) that AI agents can invoke. This Chrome DevTools MCP server implements that protocol, enabling AI assistants like Claude, Cursor, or Gemini to directly interact with a browser's DevTools.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ChromeDevTools/chrome-devtools-mcp">GitHub - ChromeDevTools/chrome-devtools-mcp: Chrome DevTools for coding agents · GitHub</a></li>
<li><a href="https://developer.chrome.com/blog/chrome-devtools-mcp">Chrome DevTools (MCP) for your AI agent | Blog | Chrome for Developers</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Chrome DevTools`, `#MCP`, `#AI agents`, `#TypeScript`, `#developer tools`

---

<a id="item-9"></a>
## [Anthropic Python SDK v0.116.0 Adds Beta Header for Agent Memory](https://github.com/anthropics/anthropic-sdk-python/releases/tag/v0.116.0) ⭐️ 7.0/10

Anthropic released version 0.116.0 of its Python SDK on July 2, 2026, which adds a beta header 'agent-memory-2026-07-22' for accessing the experimental agent memory API. This release enables developers to experiment with long-term agent memory, a key frontier in AI agent development, allowing agents to retain context across sessions and improve continuity. The beta header must be included in API requests to opt into the experimental agent memory feature, which is subject to change and may be removed in future releases.

github · stainless-app[bot] · Jul 2, 19:07

**Background**: Beta headers in APIs allow developers to access experimental features before they become stable. Agent memory enables AI agents to remember information across multiple interactions, which is crucial for building persistent, context-aware assistants. Anthropic's 'Dreaming' initiative and similar efforts by OpenAI and LangGraph highlight the industry's focus on long-term memory.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/api/beta-headers">Beta headers - Claude Platform Docs</a></li>
<li><a href="https://andrew.ooo/answers/anthropic-dreaming-vs-langgraph-memory-vs-openai-memory-may-2026/">Anthropic Dreaming vs LangGraph Memory vs... — andrew.ooo</a></li>

</ul>
</details>

**Tags**: `#anthropic`, `#sdk`, `#python`, `#agent-memory`

---

<a id="item-10"></a>
## [Guide to Running SOTA LLMs Locally Sparks Cost Debate](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob published a guide on GitHub detailing how to build expensive local setups for running state-of-the-art LLMs, including a ~$50K configuration with 4x GPUs at $12K each. This guide highlights the extreme cost and hardware requirements for local SOTA LLM inference, sparking debate on whether it's worth it compared to cloud API subscriptions like Claude Opus at $200/month. The guide suggests a REAP-pruned, quantized version of GLM-5.2 with ~594B parameters, but community members note that even with quantization, the actual cost may exceed $50K and performance may degrade outside benchmarks.

hackernews · livestyle · Jul 3, 15:03 · [Discussion](https://news.ycombinator.com/item?id=48775921)

**Background**: Running large language models locally requires powerful GPUs with high VRAM and memory bandwidth. Quantization techniques reduce model size but can impact quality. Cloud APIs offer a cheaper alternative for most users, but local setups provide privacy and control.

<details><summary>References</summary>
<ul>
<li><a href="https://unsloth.ai/docs/models/qwen3.5">Qwen3.5 - How to Run Locally | Unsloth Documentation</a></li>
<li><a href="https://www.geeksforgeeks.org/deep-learning/recommended-hardware-for-running-llms-locally/">Recommended Hardware for Running LLMs Locally - GeeksforGeeks</a></li>
<li><a href="https://www.ikangai.com/the-complete-guide-to-running-llms-locally-hardware-software-and-performance-essentials/">The Complete Guide to Running LLMs Locally: Hardware, Software, and Performance Essentials</a></li>

</ul>
</details>

**Discussion**: Community comments are largely critical: users point out that the $40K budget actually exceeds $50K, and that $50K could pay for 16.8 years of Claude Opus subscription. Some suggest mid-range options like 128GB unified memory for running DeepSeek V4 flash, while others warn about quantization artifacts and model backdoor risks.

**Tags**: `#LLM`, `#local inference`, `#hardware`, `#cost analysis`, `#deep learning`

---

<a id="item-11"></a>
## [Factories Are Just Rooms: A Philosophical Reflection](https://interconnected.org/home/2026/07/03/factories) ⭐️ 7.0/10

An essay on interconnected.org argues that factories are fundamentally just rooms where people make things, challenging the mystique around manufacturing. Community comments add real-world experiences and critiques, deepening the discussion. This perspective demystifies manufacturing, encouraging more people to consider starting small-scale production. It also sparks debate about the social and economic constructs that surround factory work. The essay scores 7.0/10 with 196 points and 76 comments, indicating high engagement. Commenters share personal experiences running small factories and critique the 'just a room' idea as oversimplified.

hackernews · arbesman · Jul 3, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48776035)

**Background**: The essay reflects on the nature of factories, suggesting that the physical space is less important than the people and processes within. This idea resonates with the maker movement and small-scale manufacturing trends.

**Discussion**: Commenters like ChuckMcM note how far society has drifted from a 'you can do that' mindset, while rm445 shares a cautionary tale of a company that treated its factory as 'just a room' and struggled. simonbarker87 fondly recalls running a small factory, and legitster argues that fast-food kitchens are efficient factories.

**Tags**: `#manufacturing`, `#philosophy of work`, `#making`, `#industrial design`, `#community discussion`

---

<a id="item-12"></a>
## [Starlink Bridges Digital Divide in Africa](https://www.economist.com/middle-east-and-africa/2026/07/02/africans-are-turning-to-starlink) ⭐️ 7.0/10

Africans are increasingly adopting Starlink satellite internet to gain connectivity in areas lacking traditional broadband infrastructure, as reported by The Economist in July 2026. This trend could significantly reduce the digital divide in Africa and other underserved regions, enabling access to education, healthcare, and economic opportunities. It mirrors the earlier leapfrogging of mobile phones over landlines in the continent. Starlink provides broadband internet via a low Earth orbit satellite constellation, with speeds up to 220 Mbps and a portable terminal that can run on a small battery pack. Users in rural America and remote areas like the Utah desert report reliable connectivity where no other options exist.

hackernews · bookofjoe · Jul 3, 21:08 · [Discussion](https://news.ycombinator.com/item?id=48779977)

**Background**: The digital divide refers to the gap between those with access to modern information technology and those without. Starlink, a subsidiary of SpaceX, operates a constellation of thousands of satellites to deliver internet globally, particularly targeting rural and remote areas where laying fiber or cable is impractical.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Starlink">Starlink - Wikipedia</a></li>
<li><a href="https://starlink.com/technology">Starlink | Technology</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_divide">Digital divide - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters share personal experiences: a former Starlink engineer expresses pride in bringing internet to the unserved; users in rural America and remote Utah describe Starlink as a game-changer, providing fast, affordable connectivity where only slow, expensive options existed before. The discussion draws parallels to Africa's rapid mobile phone adoption.

**Tags**: `#Starlink`, `#digital divide`, `#satellite internet`, `#rural connectivity`, `#Africa`

---

<a id="item-13"></a>
## [FreeBSD Memory Reporting: Heuristics vs. Reality](https://crocidb.com/post/freebsd-ate-my-ram/) ⭐️ 7.0/10

A detailed investigation reveals that FreeBSD's memory reporting tools use different heuristics, causing confusion about actual memory usage, and the author's fixes have been merged upstream. This matters because accurate memory reporting is critical for system administrators and developers to monitor and optimize system performance, and the merged fixes will improve consistency across tools. The post explains that tools like fastfetch and htop use different heuristics to categorize memory as free, inactive, or cached, leading to discrepancies. The author's patches standardize the reporting logic in the kernel.

hackernews · theanonymousone · Jul 3, 19:08 · [Discussion](https://news.ycombinator.com/item?id=48778757)

**Background**: FreeBSD uses a virtual memory system where kernel structures and filesystem caches (like ZFS ARC) consume memory. Unlike Linux, FreeBSD does not map all physical memory into kernel virtual memory, and tools rely on heuristics to report usage, which can be misleading.

<details><summary>References</summary>
<ul>
<li><a href="https://crocidb.com/post/freebsd-ate-my-ram/">FreeBSD ate my ram! - Bruno Croci</a></li>
<li><a href="https://docs.freebsd.org/en/books/arch-handbook/vm/">Chapter 7. Virtual Memory System | FreeBSD Documentation Portal</a></li>
<li><a href="https://forums.freebsd.org/threads/understanding-memory-management.84695/">Understanding memory management | The FreeBSD Forums</a></li>

</ul>
</details>

**Discussion**: Commenters appreciated the deep dive, with one noting a related 'htop explained' post. A user questioned the need for heuristics, while another praised the author for getting fixes merged.

**Tags**: `#FreeBSD`, `#memory management`, `#operating systems`, `#kernel`

---

<a id="item-14"></a>
## [Google DeepMind and A24 announce first-of-its-kind research partnership](https://deepmind.google/blog/google-deepmind-and-a24-announce-first-of-its-kind-research-partnership/) ⭐️ 7.0/10

Google DeepMind and independent film studio A24 have announced a first-of-its-kind research partnership to explore the application of AI in film and storytelling. This partnership signals a growing trend of AI integration into creative industries, potentially transforming how films are made and stories are told. The partnership is described as 'first-of-its-kind' but specific details about projects or technologies have not been disclosed.

rss · Google DeepMind Blog · Jul 3, 14:25

**Background**: Google DeepMind is a leading AI research lab known for breakthroughs like AlphaGo and Gemini. A24 is a prestigious independent film studio known for critically acclaimed films such as 'Moonlight' and 'Everything Everywhere All at Once'.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/A24">A24 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_DeepMind">Google DeepMind - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#research partnership`, `#entertainment`, `#DeepMind`, `#A24`

---

<a id="item-15"></a>
## [Course Creator Reports 50%+ Revenue Drop Due to AI](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

Josh W. Comeau, a prominent course creator, reported that his new course launch sold only one-third of typical copies, and his existing courses saw revenue decline by over 50% compared to last year, attributing the drop to AI-driven job uncertainty and LLMs replacing paid learning resources. This firsthand account provides concrete evidence of AI's disruptive impact on the developer education market, signaling a structural shift that threatens the livelihoods of independent educators and content creators. Comeau noted that multiple course creators have corroborated the same trend: revenue down 50%+, fewer engagements, and learners switching to LLMs that consume creators' work without consent or compensation.

rss · Simon Willison · Jul 3, 21:25

**Background**: Josh W. Comeau is a well-known developer educator who creates interactive courses on front-end development topics like CSS and React. The online course market has grown significantly in recent years, but the rise of large language models (LLMs) like ChatGPT now offers free or low-cost alternatives for learning, while AI-related job fears reduce willingness to invest in new skills.

**Tags**: `#AI impact`, `#developer education`, `#online courses`, `#LLMs`, `#industry trends`

---

<a id="item-16"></a>
## [Simon Willison uses DSPy to optimize Datasette Agent prompts](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison used the DSPy framework to evaluate and improve the SQL system prompts of Datasette Agent, an AI assistant for Datasette. He ran an asynchronous research task via Claude Code, which tested using GPT-4.1 mini and nano models and identified several promising optimization directions. This demonstrates a practical application of DSPy for prompt optimization in real-world AI tools, showing how systematic evaluation can improve LLM-based agents. It highlights the growing trend of using optimization frameworks to replace manual prompt engineering, potentially leading to more reliable and efficient AI systems. One key finding was that the schema listing only included table names, and the advice to avoid calling describe_table when information is already available led to column-name guessing and error-retry loops. The proposed improvement was to either include column names in the prompt's schema listing or soften that advice.

rss · Simon Willison · Jul 2, 18:25

**Background**: DSPy is a framework for programming—rather than prompting—language models, enabling algorithmic optimization of prompts and model weights. Datasette Agent is an open-source AI assistant for Datasette, a tool for exploring and publishing data in SQLite databases. Prompt optimization aims to improve LLM performance by systematically refining system prompts, which is crucial for building reliable AI agents.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp/dspy: DSPy: The framework for programming—not prompting—language models</a></li>
<li><a href="https://github.com/datasette/datasette-agent">GitHub - datasette/datasette-agent: An LLM-powered agent for Datasette · GitHub</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-agent/">Datasette Agent, an extensible AI assistant for Datasette - Datasette Blog</a></li>

</ul>
</details>

**Tags**: `#DSPy`, `#prompt engineering`, `#LLM optimization`, `#Datasette Agent`, `#SQL`

---

<a id="item-17"></a>
## [Understand to Participate: Key to AI Collaboration](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 7.0/10

Geoffrey Litt introduced the concept 'Understand to participate' at the AIE conference, arguing that developers must deeply understand code changes made by AI agents to avoid cognitive debt and remain active collaborators. This framing addresses a critical challenge in AI-assisted development: as AI agents generate larger code changes, developers risk losing understanding, leading to cognitive debt. The concept promotes a mindset where understanding is essential for effective participation, impacting how teams adopt AI tools. Litt emphasized that developers need a rich set of concepts in mind to think creatively and fluently about moving a project forward. He also published a thread version of his talk on Twitter, and the full talk is available on YouTube.

rss · Simon Willison · Jul 2, 17:07

**Background**: Cognitive debt is a term gaining traction in software engineering, referring to the erosion of shared understanding across a system over time, leading to inadequate mental models for reasoning about changes. As AI coding agents become more capable, developers face the risk of accumulating cognitive debt by not fully understanding AI-generated code.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/2/understand-to-participate/">Understand to participate | Simon Willison’s Weblog</a></li>
<li><a href="https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck.html">Understanding is the new bottleneck</a></li>
<li><a href="https://margaretstorey.com/blog/2026/02/09/cognitive-debt/">How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#cognitive debt`, `#coding agents`, `#software engineering`

---

<a id="item-18"></a>
## [Vercel's Eve: A New Kind of Software Agent Framework](https://www.latent.space/p/vercel-agents-new-software) ⭐️ 7.0/10

Vercel's Chief of Software, Andrew Qu, introduced 'eve', an open-source agent framework that treats an agent as a directory with instructions in Markdown and tools in TypeScript, and discussed why agents represent a new software category requiring skills, sandboxes, and agent-readable websites. This matters because Vercel, a major platform company, is defining a new paradigm for building and deploying AI agents, potentially influencing how developers create agent-based applications and how websites are optimized for AI consumption. Eve is open-source, supports durable execution for long-running agents, and compiles the agent directory into deployable workflows; it also connects to various channels. The framework emphasizes 'agent-readable websites' with structured instructions for AI agents.

rss · Latent Space · Jul 3, 00:08

**Background**: AI agents are autonomous programs that perform tasks on behalf of users, often requiring access to tools and the web. Traditional websites are designed for human readers, but agent-readable websites include explicit instructions and structured data to help AI agents understand and interact with them. Skills are reusable capabilities that agents can invoke, and sandboxes provide secure, isolated environments for agents to execute code safely.

<details><summary>References</summary>
<ul>
<li><a href="https://vercel.com/eve">eve – The Agent Framework - Vercel</a></li>
<li><a href="https://vercel.com/kb/guide/agent-readability-spec">Agent Readability : A Specification for AI-Optimized Websites</a></li>
<li><a href="https://dev.to/davekurian/vercel-launches-eve-an-open-source-framework-simplifying-ai-agent-development-57oi">Vercel launches eve , an open-source framework simplifying AI agent ...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Vercel`, `#software architecture`, `#web development`, `#agent frameworks`

---

<a id="item-19"></a>
## [Adobe Experiments with Self-Assembling Websites](https://www.latent.space/p/the-website-of-the-future) ⭐️ 7.0/10

Adobe is experimenting with 'agentic sites' that dynamically generate pages tailored to each visitor's intent, as discussed by Carlos Sanchez at AIEWF. This concept could revolutionize web development and user experience by making websites adaptive and personalized, potentially reducing the need for static page design. The agentic sites use AI to understand user intent and assemble content in real time, moving beyond traditional static or template-based pages.

rss · Latent Space · Jul 2, 21:25

**Background**: The agentic web is an emerging phase of the internet where AI agents act on behalf of users, not just serving information but taking actions and making decisions. Adobe's experiment aligns with this trend, hinting at a future where websites are built dynamically for each visitor.

<details><summary>References</summary>
<ul>
<li><a href="https://cyclr.com/resources/ai/what-is-the-agentic-web">What is the agentic web? | Cyclr</a></li>

</ul>
</details>

**Tags**: `#agentic web`, `#web development`, `#user experience`, `#AI`, `#Adobe`

---

<a id="item-20"></a>
## [Skill Engineering vs. One-Shot AI Design](https://www.latent.space/p/skill-engineering-design) ⭐️ 7.0/10

Paul Bakaus introduces 'skill engineering' as a human-in-the-loop approach to AI agent design, arguing against fully autonomous one-shot AI systems. This challenges the prevailing trend of fully autonomous AI agents, emphasizing the need for human judgment and reusable skill packages in reliable AI workflows. Skill engineering involves creating reusable capability packages that agents can discover, apply, and improve across tasks, contrasting with one-shot prompts that lack adaptability.

rss · Latent Space · Jul 2, 14:36

**Background**: Prompt engineering focuses on crafting single prompts for LLMs, but as agents become more complex, skill engineering emerges to build structured, reusable instructions. 'Loopmaxxing' refers to designing resilient loops with LLMs at their core, a term derived from internet culture.

<details><summary>References</summary>
<ul>
<li><a href="https://www.turingpost.com/p/from-prompt-engineering-to-skill-engineering">From Prompt Engineering to Skill Engineering</a></li>
<li><a href="https://www.teamday.ai/ai/glossary/skill-engineering">Skill Engineering - AI Glossary - TeamDay. ai</a></li>
<li><a href="https://turnkeydatacenter.ai/blog/loopmaxxing-infinite-ai-agents-fixed-cost-infrastructure/">Loopmaxxing : Why Infinite AI Agents Demand... - turnkeydatacenter.ai</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#human-in-the-loop`, `#skill engineering`, `#AI design`

---