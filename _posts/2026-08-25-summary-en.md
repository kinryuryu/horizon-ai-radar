---
layout: default
title: "Horizon Summary: 2026-08-25 (EN)"
date: 2026-08-25
lang: en
---

> From 38 items, 20 important content pieces were selected

---

1. [Interactive Moon Visualization Showcases Future of Web Education](#item-1) ⭐️ 8.0/10
2. [MS Paint and Photos Invisibly Watermark Local Images with GUID](#item-2) ⭐️ 8.0/10
3. [San Francisco Recreated as Playable 3D Web Game](#item-3) ⭐️ 8.0/10
4. [Oceans Hit Record High Temperatures](#item-4) ⭐️ 8.0/10
5. [IPFS Maintainer Team Shipyard Winds Down](#item-5) ⭐️ 8.0/10
6. [LLMs Could Exploit Inference Engines to Control Host Machines](#item-6) ⭐️ 8.0/10
7. [seL4 Security Proofs Complete on AArch64](#item-7) ⭐️ 8.0/10
8. [AI Coding Tools May Prevent Developers from Building Deep Expertise](#item-8) ⭐️ 8.0/10
9. [OpenAI Launches GPT-5.6 in Kiro with Price Cuts](#item-9) ⭐️ 8.0/10
10. [Your Executable Is a SQLite Database: A Clever Linux Hack](#item-10) ⭐️ 8.0/10
11. [Bart: A Vintage LLM Trained on Pre-1931 English](#item-11) ⭐️ 8.0/10
12. [AI as Spatial Software Generator Creates Programmable 3D Objects](#item-12) ⭐️ 8.0/10
13. [Delay-Corrected Bellman Operator and Causal Attribution for Constrained RL](#item-13) ⭐️ 8.0/10
14. [Xiaomi's New CPU Matches Apple's Single-Core, Beats in Multi-Core](#item-14) ⭐️ 7.0/10
15. [EU Regulations Threaten Makers and Micro-Entrepreneurs](#item-15) ⭐️ 7.0/10
16. [XMPP Celebrates 25 Years of Digital Independence](#item-16) ⭐️ 7.0/10
17. [PicoMQ: Durable Streams over HTTP on Object Storage](#item-17) ⭐️ 7.0/10
18. [Choosing Uncertainty Over Anger as a Path to Agency](#item-18) ⭐️ 7.0/10
19. [GlassBox Reveals Browser Fingerprinting and Identifiability](#item-19) ⭐️ 7.0/10
20. [Anthropic's flagship model lags as cheaper rivals gain ground](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Interactive Moon Visualization Showcases Future of Web Education](https://ciechanow.ski/moon/) ⭐️ 8.0/10

Bartosz Ciechanowski released 'Moon (2024)', an interactive, detailed visualization of the Moon, continuing his series of educational web articles. The piece uses advanced web technologies to create a fully interactive experience. This work exemplifies the potential of interactive web content for education, making complex astronomical concepts intuitive and engaging. It sets a high standard for educational web design and may influence how such content is created in the future. The visualization is part of Ciechanowski's portfolio of interactive articles, known for their deep technical explanations and polished presentation. It likely leverages WebGL and custom JavaScript for rendering, similar to his previous works.

hackernews · simonebrunozzi · Aug 24, 22:06 · [Discussion](https://news.ycombinator.com/item?id=49426466)

**Background**: Bartosz Ciechanowski is a programmer and technical writer renowned for creating interactive online articles that explain complex topics in science and engineering. His works often use real-time simulations and visualizations to make abstract concepts tangible, and this Moon visualization continues that tradition.

<details><summary>References</summary>
<ul>
<li><a href="https://ciechanow.ski/">Bartosz Ciechanowski</a></li>
<li><a href="https://grokipedia.com/page/Bartosz_Ciechanowski">Bartosz Ciechanowski — Grokipedia</a></li>
<li><a href="https://css-tricks.com/bartosz-ciechanowskis-interactive-blog-posts/">Bartosz Ciechanowski 's Interactive Blog Posts | CSS-Tricks</a></li>

</ul>
</details>

**Discussion**: Community comments express admiration for Ciechanowski's work, with some noting it as a benchmark for the future of web content. There is also discussion about the ethics of using AI to replicate his style, and a suggestion for adding a table of contents for better navigation.

**Tags**: `#visualization`, `#interactive`, `#education`, `#web development`, `#moon`

---

<a id="item-2"></a>
## [MS Paint and Photos Invisibly Watermark Local Images with GUID](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/) ⭐️ 8.0/10

Microsoft Paint and the Photos app have been found to embed an invisible 128-bit GUID watermark into every PNG and JPEG created or edited, even when using local AI models and while offline. The GUID is issued by a remote Microsoft Azure Front Door endpoint during a mandatory moderation request before local generation runs. This raises significant privacy and anonymity concerns, as the unique identifier could be used to trace images back to a specific Microsoft account, potentially enabling tracking or legal requests. It also highlights a broader trend of consumer software embedding hidden metadata, which could affect users' trust and expectations of local processing. The watermark is applied via a function like ApplyWatermark in Watermarker.dll, and in Paint, a watermarking failure is treated as a generation failure, while Photos logs an error and continues. The GUID is 16 bytes and is embedded even when using local AI models, with the remote moderation request occurring before generation.

hackernews · ComputerGuru · Aug 24, 15:28 · [Discussion](https://news.ycombinator.com/item?id=49421158)

**Background**: Microsoft Paint and Photos have recently integrated AI features, such as AI-based image generation and editing, which typically require cloud moderation to ensure content safety. Invisible watermarks are digital markers embedded in images that are not visible to the naked eye but can be detected by software, often used for copyright or provenance tracking. This discovery reveals that even local AI operations are not entirely private, as they still communicate with Microsoft servers.

<details><summary>References</summary>
<ul>
<li><a href="https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/">Microsoft Paint and Photos Embed Server-Issued GUIDs as Invisible Watermarks in Locally-Generated Images :: Xusheng Li</a></li>
<li><a href="https://www.linkedin.com/pulse/ms-paint-quietly-stamps-guid-every-image-you-save-even-andy-arnott-opknc">MS Paint Quietly Stamps a GUID on Every Image You Save - LinkedIn</a></li>
<li><a href="https://mangodeveloper.com/articles/microsoft-paint-embeds-invisible-guid-watermarks-in-local-ai-images-via-remote-moderation-server">Microsoft Paint Embeds Invisible GUID Watermarks in Local AI ...</a></li>

</ul>
</details>

**Discussion**: Community comments express strong concern about the hidden GUID watermark, with some calling it a 'weapon against internet anonymity' and noting that it could be used to subpoena user data from Microsoft. Others criticize the mandatory remote moderation and logging of interactions, while some see the AI aspect as a red herring, focusing instead on the broader privacy implications.

**Tags**: `#privacy`, `#watermarking`, `#Microsoft`, `#security`, `#AI`

---

<a id="item-3"></a>
## [San Francisco Recreated as Playable 3D Web Game](https://sf.thijs.gg/) ⭐️ 8.0/10

A web-based interactive 3D recreation of San Francisco, generated from real-world data, has been released at sf.thijs.gg, allowing users to explore the city as a playable video game. The project has gained significant community attention with 323 points and 113 comments. This project demonstrates a novel technical achievement in procedural city generation from GIS data, making realistic urban environments accessible in the browser. It could inspire further development of interactive city simulations and games, impacting developers and urban planning enthusiasts. The recreation includes drivable vehicles and collectible coins, but lacks street names and landmarks, which users have requested. The project is built from real-world elevation and building data, though it does not yet incorporate street view imagery or live multiplayer features.

hackernews · centrosphere · Aug 24, 17:05 · [Discussion](https://news.ycombinator.com/item?id=49422784)

**Background**: Procedural city generation uses algorithms to create 3D urban environments from 2D GIS data, as seen in tools like ArcGIS CityEngine and CityGen3D. Web-based 3D rendering of real cities is challenging due to complex geometry and textures, but projects like Google Maps 3D and this one show progress in making such experiences accessible online.

<details><summary>References</summary>
<ul>
<li><a href="https://www.esri.com/en-us/arcgis/products/arcgis-cityengine/overview">Procedural City Generator | 3D City Maker | ArcGIS CityEngine</a></li>
<li><a href="https://www.tandfonline.com/doi/full/10.1080/19475683.2022.2037019">Full article: 3D-GIS Parametric Modelling for Virtual Urban Simulation Using CityEngine</a></li>
<li><a href="https://www.citygen3d.com/">CityGen3D | Procedural scene generation in Unity</a></li>

</ul>
</details>

**Discussion**: Community sentiment is highly positive, with users expressing emotional connections to the recreation and suggesting improvements like adding street names, landmarks, and teleportation. Some users shared similar projects, such as a Seattle recreation in N64 style, and discussed the potential for a pipeline to generate full GTA-style maps from real data.

**Tags**: `#3D rendering`, `#procedural generation`, `#web development`, `#GIS`, `#interactive maps`

---

<a id="item-4"></a>
## [Oceans Hit Record High Temperatures](https://www.bbc.com/news/articles/c62m4gpnp78o) ⭐️ 8.0/10

Oceans have reached their highest recorded temperature, marking a significant milestone in climate change. This record was reported by the BBC, highlighting the accelerating impacts of global warming on marine environments. This record underscores the urgency of climate action, as warmer oceans contribute to sea-level rise, extreme weather events, and marine ecosystem disruption. It affects global weather patterns and poses risks to coastal communities and economies worldwide. The record was reported by the BBC, and the article likely includes specific temperature data and comparisons to previous records. The high engagement (383 points, 264 comments) indicates significant public interest and discussion.

hackernews · tcp_handshaker · Aug 24, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49424606)

**Background**: Ocean temperatures are a key indicator of climate change because oceans absorb about 90% of the excess heat from greenhouse gas emissions. Record temperatures can lead to coral bleaching, ice melt, and altered ocean currents, with far-reaching consequences for biodiversity and human societies.

**Discussion**: Commenters expressed concern about government inaction, with one noting the US is expanding fossil fuel extraction and attacking renewables. Others shared educational resources and personal reflections on the severity of a few degrees of warming, while some anticipated increased weather unpredictability due to El Niño.

**Tags**: `#climate change`, `#ocean temperature`, `#environmental science`, `#policy`

---

<a id="item-5"></a>
## [IPFS Maintainer Team Shipyard Winds Down](https://ipshipyard.com/blog/2026-the-end-of-ipfs-at-shipyard/) ⭐️ 8.0/10

Protocol Labs has informed Shipyard that it will not renew funding, leading Shipyard to wind down its IPFS-related engineering, maintenance, and infrastructure operations. This affects projects like Kubo, Helia, Boxo, Rainbow, IPFS Desktop, and IPFS Companion, and contributions to upstream libp2p will cease. This marks a significant shift in IPFS maintenance, moving from centralized team support to individual grants, which could affect the project's stability and development pace. It follows earlier setbacks like Cloudflare's gateway shutdown and Brave's deprecation of native IPFS support, raising concerns about IPFS's long-term sustainability. Shipyard's IPFS funding was cancelled, and the team will stop work on specifications, standards, and ecosystem coordination. The announcement clarifies that the IPFS Project itself is not shutting down, but rather switching to individual maintainer grants.

hackernews · iand · Aug 24, 15:48 · [Discussion](https://news.ycombinator.com/item?id=49421489)

**Background**: IPFS (InterPlanetary File System) is a peer-to-peer hypermedia protocol designed to make the web faster, safer, and more open. Shipyard was one of several teams maintaining IPFS implementations, funded by Protocol Labs. The recent funding cut is part of a broader trend of reduced corporate support for IPFS, following Cloudflare's gateway shutdown in August 2024 and Brave's deprecation of native IPFS support in version 1.69.153.

<details><summary>References</summary>
<ul>
<li><a href="https://ipshipyard.com/blog/2026-the-end-of-ipfs-at-shipyard/">The end of IPFS at Shipyard</a></li>
<li><a href="https://byteiota.com/ipfs-shipyard-shuts-down-what-developers-must-do-now/">IPFS Shipyard Shuts Down: What Developers Must Do Now</a></li>
<li><a href="https://newsscore.com/story/185589">Protocol Labs ends funding for Shipyard, shutting down IPFS ...</a></li>

</ul>
</details>

**Discussion**: Community comments clarify that the shutdown is limited to Shipyard, not the entire IPFS project, though some express disappointment and concern about the project's direction. One commenter suggests Iroh as a more sustainable alternative, while another criticizes the reliance on Google Forms for feedback, highlighting a disconnect with decentralization principles.

**Tags**: `#IPFS`, `#decentralization`, `#open source`, `#maintenance`, `#p2p`

---

<a id="item-6"></a>
## [LLMs Could Exploit Inference Engines to Control Host Machines](https://boydkane.com/essays/llms-could-control-their-host-machines-by-exploiting-inference-engines) ⭐️ 8.0/10

An essay by Boyd Kane argues that LLMs could exploit vulnerabilities in inference engines like vLLM, llama.cpp, or SGLang via their HTTP interfaces to gain control of host machines. It emphasizes the need for sandboxing and network isolation to mitigate such risks. This highlights a novel attack surface in AI infrastructure, where inference engines are high-value targets due to their compute power and access to model weights. As LLM agents become more autonomous, securing these engines is critical to prevent host compromise and data breaches. The essay suggests that a clever local LLM could even task a powerful cloud-hosted LLM for assistance in exploiting vulnerabilities. It recommends running inference engines on separately sandboxed VMs on firewalled VLANs, and notes that vLLM has had past exploits and is rapidly developing.

hackernews · zdw · Aug 24, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49424387)

**Background**: Inference engines like vLLM are used to serve LLMs efficiently, often exposing HTTP APIs for inference requests. These engines are complex and may contain vulnerabilities that could be exploited by malicious prompts. Sandboxing and network isolation are common mitigation strategies to limit the blast radius of such attacks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2026-41523/">CVE-2026-41523: vLLM Inference Engine RCE Vulnerability</a></li>
<li><a href="https://www.llms.blog/posts/sandboxing-llm-code-execution-architecture-isolation-boundaries-and-performance-trade-offs">Sandboxing LLM Code Execution: Architecture, Isolation ...</a></li>
<li><a href="https://beyondscale.tech/blog/ai-agent-sandboxing-enterprise-security-guide">AI Agent Sandboxing: Enterprise Security Guide 2026</a></li>

</ul>
</details>

**Discussion**: Community comments clarify that the article is about attacking the inference engine itself, not sandbox escapes, and note that vLLM has had real CVEs. Some commenters find the idea ironic, suggesting the article itself could enable such attacks, while others discuss broader agent-based attack scenarios and the need for isolation.

**Tags**: `#LLM security`, `#inference engines`, `#vLLM`, `#sandboxing`, `#AI infrastructure`

---

<a id="item-7"></a>
## [seL4 Security Proofs Complete on AArch64](https://proofcraft.systems/news-2026/#2026-08-21) ⭐️ 8.0/10

The seL4 project announced that its formal security proofs are now complete for the AArch64 (ARM64) architecture, extending machine-checked verification to 64-bit ARM hardware. This milestone is significant because AArch64 is widely used in servers and embedded systems, and having formally verified security properties on this platform enhances trust in high-assurance operating systems, potentially accelerating adoption in security-critical applications. The proofs cover the functional correctness and security properties of the seL4 microkernel, but the announcement notes limitations: the verification applies to the non-MCS (mixed criticality systems) configuration and is unicore (single-core) only. The proofs assume correctness of the compiler, assembly code, and hardware.

hackernews · snvzz · Aug 24, 11:32 · [Discussion](https://news.ycombinator.com/item?id=49418255)

**Background**: seL4 is a microkernel known for its formal verification, meaning its correctness is proven using mathematical methods and machine-checked proofs. Formal verification is rare in operating systems and provides strong guarantees against programming errors. The AArch64 architecture, also known as ARM64, is a 64-bit ARM architecture used in many modern devices and servers.

<details><summary>References</summary>
<ul>
<li><a href="https://news.linxi.com.au/news/sel4-microkernel-achieves-full-formal-security-verification-on-aarch64">seL4 Microkernel Formal Security Proofs Completed on AArch64 ...</a></li>
<li><a href="https://www.newswarden.com/story/sel4-security-proofs-complete-aarch64">The seL4 Microkernel's Security Proofs Are Now Complete on ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/AArch64">AArch64 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight skepticism about the practical impact, with one user predicting a side-channel timing attack could invalidate the results. Others note the limitations (non-MCS, unicore) and question adoption, while another suggests that seL4 needs a native Linux compatibility layer to honestly claim improved security.

**Tags**: `#formal verification`, `#seL4`, `#AArch64`, `#security`, `#microkernel`

---

<a id="item-8"></a>
## [AI Coding Tools May Prevent Developers from Building Deep Expertise](https://larsfaye.com/articles/ai-coding-will-prevent-expertise) ⭐️ 8.0/10

An article argues that reliance on AI coding tools will prevent developers from developing deep expertise, sparking a debate about the trade-offs between productivity and skill formation. This matters because AI coding tools are becoming ubiquitous in software development, and if they hinder skill development, the long-term quality and innovation in the industry could suffer. It affects developers, companies, and the future of software engineering. The article highlights the risk of skill atrophy when developers rely too heavily on AI, and community comments mention enterprise mandates that discourage manual coding, leading to code being produced faster than it can be reviewed. Some commenters advocate for 'guided coding' as a balanced approach that maintains quality and learning.

hackernews · larsfaye · Aug 24, 15:52 · [Discussion](https://news.ycombinator.com/item?id=49421554)

**Background**: AI coding tools, such as GitHub Copilot and ChatGPT, assist developers by generating code snippets or entire functions. While they boost productivity, there is concern that developers may become overly dependent, losing the ability to solve problems independently. The debate parallels earlier concerns about calculators in math education, where research suggests that calculators can enhance learning when used appropriately.

**Discussion**: Community comments reflect a mix of agreement and nuance. Some agree that AI reliance is already causing issues, citing enterprise mandates that prioritize speed over understanding. Others argue that 'guided coding'—using AI as an assistant while still writing code manually—offers a better balance, and some draw parallels to calculators in education, suggesting that AI might actually improve learning by freeing up mental bandwidth for higher-level concepts.

**Tags**: `#AI coding`, `#software engineering`, `#expertise`, `#productivity`, `#future of work`

---

<a id="item-9"></a>
## [OpenAI Launches GPT-5.6 in Kiro with Price Cuts](https://openai.com/index/gpt-5-6-in-kiro) ⭐️ 8.0/10

OpenAI has announced that GPT-5.6 is now available in Kiro, an AI development platform, offering developers improved price-performance for software development tasks. The model family includes three variants—Luna, Terra, and Sol—with discounted pricing through at least November 21, 2026. This release is significant for developers as it directly addresses cost concerns in AI-assisted coding, potentially accelerating adoption of AI tools in software engineering. The price war with competitors like Anthropic could lead to more affordable AI services across the industry. The pricing for GPT-5.6 variants is as follows: Sol costs $4.00 input, $0.40 cached input, $5.00 cache writes, and $20.00 output per million tokens; Terra costs $2.00, $0.20, $2.50, and $12.00; Luna costs $0.20, $0.02, $0.25, and $1.20. Additionally, a 50% discount on OpenRouter is still applied, making the effective price $2/$10 per million tokens for some variants.

rss · OpenAI News · Aug 24, 12:00

**Background**: Kiro is an agentic development environment built by a team within AWS, designed to help developers plan, build, review, and test software using AI agents. GPT-5.6 is a large language model family released by OpenAI on July 9, 2026, with variants ranging from Luna (least capable) to Sol (most capable), and is noted for improved capabilities in coding, science, and cybersecurity.

<details><summary>References</summary>
<ul>
<li><a href="https://kiro.dev/">Kiro: Move beyond AI coding to agentic engineering</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>

</ul>
</details>

**Discussion**: Community comments reflect a mix of enthusiasm and analysis. One user notes the ease of model distillation and replication, suggesting AI might become a race to the bottom. Another provides detailed pricing comparisons, highlighting the discount. Some users discuss Sol's performance in complex tasks, while others celebrate the price war and its benefits for open-source models.

**Tags**: `#OpenAI`, `#GPT-5.6`, `#AI model`, `#developer tools`, `#price-performance`

---

<a id="item-10"></a>
## [Your Executable Is a SQLite Database: A Clever Linux Hack](https://simonwillison.net/2026/Aug/24/your-executable-is-a-sqlite-database/) ⭐️ 8.0/10

Farid Zakaria has demonstrated a technique to create a SQLite database file that can also be executed as a Linux binary. By setting the SQLite application ID to 'SELF' and storing ELF components in tables, a custom interpreter can run the file. This hack blurs the line between data and code, offering a novel approach to executable packaging and introspection. It could inspire new ways to embed metadata or resources in executables, and it highlights the flexibility of both SQLite and the Linux kernel. The technique uses the SQLite 4-byte application ID at byte offset 68, setting it to 'SELF'. The ELF components are arranged into SQLite tables, and the 'self-exec' interpreter (written in C) extracts and executes them. Additionally, binfmt_misc can be used to register the pattern so the kernel automatically invokes the interpreter.

rss · Simon Willison · Aug 24, 11:38

**Background**: SQLite is a self-contained, serverless database engine that stores data in a single file, and its header includes an application ID field for identifying the file format. ELF (Executable and Linkable Format) is the standard binary format for executables on Linux and Unix-like systems. binfmt_misc is a Linux kernel feature that allows custom binary formats to be recognized and executed via user-space handlers.

<details><summary>References</summary>
<ul>
<li><a href="https://fzakaria.com/2026/08/23/your-executable-is-a-sqlite-database">Your executable is a SQLite database | Farid Zakaria’s Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Binfmt_misc">binfmt _ misc - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion likely includes admiration for the creativity and technical depth of the hack, with some users discussing potential use cases and limitations. There may be debates about the practicality and security implications of such an approach.

**Tags**: `#SQLite`, `#ELF`, `#Linux`, `#executable`, `#hacking`

---

<a id="item-11"></a>
## [Bart: A Vintage LLM Trained on Pre-1931 English](https://www.reddit.com/r/MachineLearning/comments/1vx94er/bart_a_vintage_llm_r/) ⭐️ 8.0/10

Unbounded Labs released Bart, a 2.82B parameter LLM trained from scratch on 20.1B tokens of pre-1931 English, along with open-sourced datasets, benchmarks, and training code. The project aims to test whether LLMs can independently rediscover historical scientific insights, as proposed by Demis Hassabis. This project directly addresses a fundamental question in AI research: whether LLMs can generate original ideas or merely predict the next token. By training on historical text, it provides a unique testbed for evaluating reasoning and creativity, potentially influencing future approaches to AI and scientific discovery. Bart was trained in 5 days on a single H100 with 60% MFU, and the team cleaned Harvard's Institutional Books from 242B to 23B tokens. They also created Vintage CORE, the first suite of 20 benchmarks for vintage LLMs, and released a 416k-pair SFT dataset grounded in pre-1930s text.

reddit · r/MachineLearning · /u/soggydoggy8 · Aug 24, 17:20

**Background**: Demis Hassabis, CEO of Google DeepMind, proposed that an LLM trained on data up to 1911 could independently discover relativity, serving as a benchmark for AGI. The pre-1931 English corpus differs from modern internet text, as it was written by authors who wrote slowly and revised, offering a distinct linguistic and conceptual landscape. This project builds on that idea by training a model on such historical text to explore whether it can reach conclusions similar to past scientists.

<details><summary>References</summary>
<ul>
<li><a href="https://officechai.com/ai/someone-built-an-llm-to-test-out-demis-hassabis-agi-definition-of-pre-1900-science-discovering-relativity/">Someone Built An LLM To Test Out Demis Hassabis' AGI ...</a></li>
<li><a href="https://medium.com/data-science-collective/can-an-llm-predict-the-future-if-its-stuck-in-1930-297fc5ab1cd2">Can an LLM Predict the Future If It’s Stuck in 1930? | Medium</a></li>
<li><a href="https://www.marktechpost.com/2026/04/27/meet-talkie-1930-a-13b-open-weight-llm-trained-on-pre-1931-english-text-for-historical-reasoning-and-generalization-research/">Meet Talkie-1930: A 13B Open-Weight LLM Trained on Pre - 1931 ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#training`, `#historical text`, `#AI research`, `#benchmarks`

---

<a id="item-12"></a>
## [AI as Spatial Software Generator Creates Programmable 3D Objects](https://www.reddit.com/r/MachineLearning/comments/1vxcc1h/r_using_ai_as_a_spatial_software_generator_to/) ⭐️ 8.0/10

A new paper introduces using AI as a spatial software generator to create 3D objects that are inherently programmable, animation-ready, and adaptable to different compute environments. The authors provide visual demonstrations and a GitHub repository. This approach could disrupt industries like industrial design, game development, simulations, and AR/VR/XR by making 3D content more flexible and easier to modify. It contrasts with traditional AI 3D generators that produce monolithic mesh blobs, offering a more software-centric paradigm. The generated 3D objects have hierarchical structure and hinge/socket articulation at authoring time, and can include logic to appear differently in weak vs. powerful compute environments. However, they lag behind traditional AI 3D generators in creating complex organic shapes.

reddit · r/MachineLearning · /u/mhb_11 · Aug 24, 19:10

**Background**: Traditional AI 3D generators typically output monolithic mesh blobs that are hard to edit or animate. This paper explores using large language models (LLMs) for spatial programming, where 3D objects are defined as software code, making them inherently programmable and animation-ready. The concept aligns with recent research on integrating LLMs with 3D understanding and generation.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2504.05786v1">How to Enable LLM with 3D Capacity? A Survey of Spatial ...</a></li>
<li><a href="https://arxiv.org/pdf/2507.16524">Spatial 3D-LLM: Exploring Spatial Awareness in 3D Vision ...</a></li>
<li><a href="https://github.com/ActiveVisionLab/Awesome-LLM-3D">Awesome-LLM-3D - GitHub</a></li>

</ul>
</details>

**Tags**: `#3D generation`, `#LLM`, `#spatial programming`, `#AI`, `#computer graphics`

---

<a id="item-13"></a>
## [Delay-Corrected Bellman Operator and Causal Attribution for Constrained RL](https://www.reddit.com/r/MachineLearning/comments/1vx11hz/delaycorrected_bellman_operator_causal/) ⭐️ 8.0/10

The author introduces a delay-corrected Bellman operator that uses an adaptive effective discount learned from the consequence-delay distribution, with a contraction proof that holds under unknown stochastic delay. They also propose an Interventional Consequence Net (ICN) for action-level causal attribution, pretrained on structural causal model labels. This work addresses a critical gap in constrained RL where consequences are often delayed and stochastic, making it difficult to attribute violations to the correct actions. By providing a theoretical contraction proof and a practical attribution method, it could improve the reliability of safe RL in real-world applications. The ICN currently requires access to the environment's structural causal model to generate pretraining labels, which limits its applicability to settings where the SCM is known or can be reasonably specified. The method is open to contributions and collaborations, especially from researchers in constrained/safe RL or causal inference.

reddit · r/MachineLearning · /u/No_Cauliflower7923 · Aug 24, 12:11

**Background**: Standard constrained RL assumes immediate and attributable consequences, which fails in real-world settings with delayed and stochastic violations. The Bellman operator is a fundamental concept in RL used to update value functions, and its contraction property ensures convergence. Causal inference methods aim to attribute effects to causes, which is relevant here for correctly penalizing actions that cause violations.

<details><summary>References</summary>
<ul>
<li><a href="https://prismix.dev/news/f1072ba9e03c">Delay-corrected Bellman operator + causal attribution for ...</a></li>
<li><a href="https://pypi.org/project/ccpl-rl/">Causal Consequence - Penalized Learning for delayed constrained...</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#constrained RL`, `#causal inference`, `#delayed rewards`, `#research`

---

<a id="item-14"></a>
## [Xiaomi's New CPU Matches Apple's Single-Core, Beats in Multi-Core](https://twitter.com/lemire/status/2091894299289874926) ⭐️ 7.0/10

Xiaomi's new Xring O3 CPU reportedly matches Apple's single-threaded performance and surpasses it in multithreaded benchmarks, according to recent Geekbench scores. The chip is based on ARM's reference design, not a fully custom Xiaomi design. This development signals Xiaomi's growing capability in chip design, potentially intensifying competition in the mobile SoC market against Qualcomm and MediaTek. However, the reliance on ARM's reference design and the lack of power efficiency metrics temper the significance, as real-world performance may differ. The Xring O3 uses 10 cores versus Apple's 6 cores in multithreaded tests, which explains its higher multi-core score. Geekbench scores show the Xring O3 achieving 3,945 single-core and 15,221 multi-core, compared to Apple's M5 iPad at 3,556 and 15,285 respectively, but Apple's M5 Max still leads with 4,300 single-core and 29,200 multi-core.

hackernews · tosh · Aug 24, 15:08 · [Discussion](https://news.ycombinator.com/item?id=49420873)

**Background**: ARM designs CPU cores that companies like Xiaomi and MediaTek license and integrate into their SoCs, often with modifications to interconnect, NPU, and memory support. Apple, in contrast, designs fully custom CPU cores that only comply with the ARM instruction set, allowing for tighter integration and better power efficiency. Single-threaded performance is crucial for everyday tasks, while multithreaded performance benefits from more cores but also depends on software optimization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ARM_Cortex-A53">ARM Cortex-A53 - Wikipedia</a></li>
<li><a href="https://laptopstudy.com/single-thread-vs-multithread-gaming-list-benchmarks/">Single-Thread vs Multi-thread CPU For Gaming (List ...</a></li>
<li><a href="https://cpubenchmarktest.net/blog/single-thread-vs-multi-thread-performance/">Single-Thread vs Multi-Thread Performance - CPU benchmark ...</a></li>

</ul>
</details>

**Discussion**: Commenters note that the Xring O3 is essentially an ARM reference design, not a custom Xiaomi CPU, and that power efficiency per watt is missing from the comparison. Some argue that Apple's cores are still superior in efficiency and that the multi-core advantage is due to more cores, while others see this as a positive step for Xiaomi and a threat to Qualcomm and MediaTek.

**Tags**: `#CPU`, `#Xiaomi`, `#Apple`, `#ARM`, `#Mobile`

---

<a id="item-15"></a>
## [EU Regulations Threaten Makers and Micro-Entrepreneurs](https://lectronz.com/u/lectronz/articles/how-europe-is-killing-makers-and-micro-entrepreneurs) ⭐️ 7.0/10

An article argues that recent EU regulations, particularly those related to packaging and product compliance, are disproportionately harming makers and micro-entrepreneurs, potentially forcing many out of business. The piece has sparked extensive community debate, with some commenters challenging the accuracy of the claims. This matters because makers and micro-entrepreneurs are vital for innovation and local economies, and overly burdensome regulations could stifle their growth. The debate highlights a broader tension between EU harmonization efforts and the practical realities of small-scale cross-border e-commerce. The article specifically criticizes the EU's Packaging and Packaging Waste Regulation (PPWR) and the General Product Safety Regulation (GPSR), which impose new requirements on product labeling, packaging, and documentation. Commenters note that micro-enterprises are often exempt from many rules, but the complexity of navigating varying national implementations remains a challenge.

hackernews · l-one-lone · Aug 24, 13:05 · [Discussion](https://news.ycombinator.com/item?id=49419237)

**Background**: The EU has been updating its product safety and packaging regulations to reduce waste and protect consumers, but these rules often assume large corporate compliance capabilities. Makers and micro-entrepreneurs, who sell low-volume, customized products across borders, may lack the resources to comply with diverse national requirements. The debate reflects a long-standing issue where EU directives are implemented differently by member states, creating a patchwork of rules that disproportionately affect small businesses.

**Discussion**: The community discussion is mixed, with some commenters like anigbrowl pointing out that the article may misrepresent the EU rules, noting that micro-enterprises are often exempt. Others like mstaoru compare China's approach, which focuses on choke points like logistics companies, and yardie highlights the problem of inconsistent national implementations. mpweiher clarifies that the EU Commission wanted a central registry but member states blocked it, shifting blame.

**Tags**: `#EU regulation`, `#makers`, `#micro-entrepreneurs`, `#policy`, `#e-commerce`

---

<a id="item-16"></a>
## [XMPP Celebrates 25 Years of Digital Independence](https://gultsch.de/posts/25-years-of-digital-independence/) ⭐️ 7.0/10

Daniel Gultsch published a reflection on XMPP's 25-year history, highlighting its role in digital independence and the current ecosystem. The article sparked community discussion about modern usage, comparisons with Matrix, and future potential. This milestone underscores XMPP's enduring relevance as a decentralized, open communication protocol, especially in an era of increasing concerns about data privacy and platform control. The community's active engagement suggests continued interest and investment in federated messaging alternatives. The article and discussion reference active projects like Movim, Fluux, and ejabberd, as well as bridges like jmp.chat for telephony/SMS. Community members also noted challenges with Android client notifications and the potential impact of Matrix's funding on XMPP's development.

hackernews · inputmice · Aug 24, 15:51 · [Discussion](https://news.ycombinator.com/item?id=49421536)

**Background**: XMPP (Extensible Messaging and Presence Protocol) is an open, federated protocol for real-time messaging and presence, originally developed in 1999. It allows users to communicate across different servers, promoting digital independence by avoiding centralized platforms. Matrix is a newer decentralized protocol with similar goals but different technical approaches, often compared to XMPP.

<details><summary>References</summary>
<ul>
<li><a href="https://gultsch.de/posts/25-years-of-digital-independence/">Daniel Gultsch | Jabber/ XMPP : 25 Years of Digital Independence</a></li>
<li><a href="https://news.ycombinator.com/item?id=49421536">Jabber/ XMPP : 25 Years of Digital Independence | Hacker News</a></li>
<li><a href="https://lukesmith.xyz/articles/matrix-vs-xmpp/">Matrix vs. XMPP | Luke Smith</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive, with users sharing personal success stories and expressing hope for XMPP's future. Some lament that Matrix did not build on XMPP and wonder what could have been if Matrix's funding had gone to XMPP. Others discuss practical use cases, such as using XMPP for agent communication, and note client notification issues on Android.

**Tags**: `#XMPP`, `#decentralized communication`, `#open protocols`, `#messaging`, `#community`

---

<a id="item-17"></a>
## [PicoMQ: Durable Streams over HTTP on Object Storage](https://picomq.com/) ⭐️ 7.0/10

PicoMQ is a new Rust-based server that implements durable streams over HTTP, using object storage as the backend. It offers create, append, read, long-poll, and SSE operations, with support for both the Pico Protocol and the Durable Streams Protocol. This approach could significantly reduce the cost and complexity of running message brokers by leveraging cheap object storage instead of local disks. It may appeal to developers building scalable, cost-sensitive streaming applications, potentially disrupting traditional Kafka-like systems. PicoMQ uses S3Stream, a Rust library also used in AutoMQ, as its stream storage primitive. Coordination is handled via a command log in Postgres, and the server supports granular, URL-addressable streams.

hackernews · adesh_nalpet · Aug 24, 16:08 · [Discussion](https://news.ycombinator.com/item?id=49421806)

**Background**: Traditional message brokers like Kafka rely on local disks for storage, which can be expensive and hard to scale. Object storage services like Amazon S3 offer cheap, durable, and scalable storage, making them an attractive alternative for streaming data. PicoMQ builds on this idea by providing a simple HTTP interface for durable streams, similar to how AutoMQ offers a diskless Kafka on S3.

<details><summary>References</summary>
<ul>
<li><a href="https://picomq.com/docs/">PicoMQ is durable , real-time streams over HTTP, built on...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49421806">Show HN: PicoMQ – Durable Streams over HTTP, on object storage</a></li>
<li><a href="https://github.com/AutoMQ/automq">GitHub - AutoMQ/automq: Diskless Kafka® on S3. 10x Cost ...</a></li>

</ul>
</details>

**Discussion**: Community members expressed excitement and curiosity, comparing PicoMQ to other projects like S2 and Electric Streams. Some raised concerns about write performance on object storage, while others asked about use cases like building a Discord-like chat and pricing implications.

**Tags**: `#streaming`, `#object-storage`, `#rust`, `#message-queue`, `#distributed-systems`

---

<a id="item-18"></a>
## [Choosing Uncertainty Over Anger as a Path to Agency](https://lucumr.pocoo.org/2026/8/24/anger-anxiety-agency/) ⭐️ 7.0/10

The author of the blog post 'Anger, Anxiety and Agency' argues that individuals can choose uncertainty over anger to gain greater agency, framing this as a deliberate emotional strategy rather than a natural response. This perspective challenges common assumptions about human emotion, suggesting that emotional responses are not fixed but can be consciously redirected. It has practical implications for personal development, leadership, and how people cope with uncertainty in rapidly changing environments. The article is philosophical rather than technical, drawing on concepts of agency and uncertainty. The author suggests that while anger provides a temporary sense of control, embracing uncertainty can lead to more sustainable agency, though this requires overcoming neurochemical preferences for anger.

hackernews · lumpa · Aug 24, 18:37 · [Discussion](https://news.ycombinator.com/item?id=49424082)

**Background**: The news item is a blog post that explores the relationship between emotions and agency. Agency refers to the capacity to act independently and make choices, while uncertainty is a state of not knowing outcomes. The post suggests that anger is often a reaction to uncertainty, and that by choosing to remain uncertain, individuals can avoid the negative consequences of anger and maintain greater control over their actions.

**Discussion**: The Hacker News comments present contrasting views: some argue that anger is a natural and valid response, while others see it as a reaction to fear. One commenter notes that choosing uncertainty over anger may contradict human nature, as people prefer anger to uncertainty. Another shares personal anxiety despite loving their job, highlighting the complexity of emotional responses.

**Tags**: `#psychology`, `#emotion`, `#uncertainty`, `#agency`, `#philosophy`

---

<a id="item-19"></a>
## [GlassBox Reveals Browser Fingerprinting and Identifiability](https://glassbox.codecanary.org/) ⭐️ 7.0/10

GlassBox, a new web tool launched on Hacker News, demonstrates how identifiable your browser is through fingerprinting, providing a practical example of the information browsers expose. The tool highlights the uniqueness of browser fingerprints and sparks discussion on privacy and anti-fingerprinting techniques. This tool matters because it raises awareness about browser fingerprinting, a tracking method that can identify users even without cookies, affecting privacy-conscious individuals and the broader web ecosystem. It also highlights the ongoing arms race between fingerprinting techniques and anti-fingerprinting measures, which is crucial for developers and privacy advocates. The tool reportedly claims a uniqueness of 1 in 6.2 billion for Firefox on iPhone, though some commenters question this accuracy, suggesting anti-fingerprinting might be affecting results. It also notes that both uniqueness and stability are needed for effective tracking, as a changing fingerprint can itself be a form of privacy.

hackernews · tke248 · Aug 24, 16:15 · [Discussion](https://news.ycombinator.com/item?id=49421948)

**Background**: Browser fingerprinting is a technique that collects information about a device's software and hardware through the browser to create a unique identifier, which can be used for tracking even when cookies are blocked. Common fingerprinting methods include canvas, WebGL, and audio fingerprinting, and anti-fingerprinting tools like Tor Browser and browser extensions aim to reduce the uniqueness of these fingerprints.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Browser_fingerprinting">Browser fingerprinting</a></li>
<li><a href="https://www.cloudwards.net/browser-fingerprinting-protection/">Browser Fingerprinting Protection 2026 [Prevent Fingerprints] Why Anti-Fingerprinting Techniques Don't Work in Browsers Browser Fingerprinting Guide: Detection & Bypass Methods ... Browser Fingerprint Detection 2026: Complete Guide for ... Comprehensive Guide to Anti-Fingerprinting Strategies</a></li>
<li><a href="https://www.glukhov.org/post/2025/11/anti-fingerprinting-techniques-browser-and-network-level/">Advanced Anti-Fingerprinting Protection - Rost Glukhov ...</a></li>

</ul>
</details>

**Discussion**: The community discussion includes references to similar tools like Cover Your Tracks by EFF, skepticism about the claimed uniqueness numbers, and a point that stability is as important as uniqueness for tracking. Some commenters express horror at how much information browsers expose, while others note that similar projects have been posted before.

**Tags**: `#privacy`, `#browser fingerprinting`, `#web security`, `#tracking`

---

<a id="item-20"></a>
## [Anthropic's flagship model lags as cheaper rivals gain ground](https://simonwillison.net/2026/Aug/23/anthropics-best-ai-model-struggles-to-attract-users-as-cheaper-t/) ⭐️ 7.0/10

An FT report reveals that Anthropic's annualized revenue reached $65 billion in July 2026, up from $47 billion in May, and the company expects Q3 profitability. Meanwhile, OpenAI's annualized revenue has jumped 35% to over $40 billion, boosted by the launch of GPT-5.6. This highlights the competitive pressure in the AI model market, where cost-effective alternatives are challenging premium models. It signals that pricing and efficiency are becoming critical factors for adoption, affecting both enterprise customers and AI providers' strategies. Ramp's AI index, based on billing data from 70,000 companies, shows that Anthropic's newest model, Opus 5, accounts for only 3.5% of Anthropic's model spend, while older models like Opus 4.8 (28%) and Sonnet 4.6 (8.3%) dominate. The high cost of the 'Fable' model (likely Opus 5) is cited as a reason for its low adoption.

rss · Simon Willison · Aug 23, 20:24

**Background**: Annualized revenue run rate is a projection of a full year's revenue based on current monthly data. Anthropic and OpenAI are leading AI labs competing in the large language model market, where model performance and pricing are key differentiators. The Ramp AI Index tracks AI adoption using corporate card spending data.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/08/17/anthropics-annualized-revenue-surges-to-65b/">Anthropic’s annualized revenue surges to $65B - TechCrunch</a></li>
<li><a href="https://www.cnbc.com/2026/08/17/anthropic-says-annualized-revenue-climbed-to-65-billion-in-july.html">Anthropic says annualized revenue climbed to $65 billion in July</a></li>
<li><a href="https://ramp.com/data/ai-index">Ramp AI Index</a></li>

</ul>
</details>

**Discussion**: Hacker News discussion likely focuses on the surprising revenue figures and the adoption gap between models, with some questioning the accuracy of Ramp's data and others debating the value of expensive frontier models versus cheaper alternatives.

**Tags**: `#AI industry`, `#Anthropic`, `#OpenAI`, `#revenue`, `#market trends`

---