---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 57 items, 20 important content pieces were selected

---

1. [OpenAI Unveils First Custom AI Chip 'Jalapeno' with Broadcom](#item-1) ⭐️ 9.0/10
2. [Krea 2: SOTA Open-weights 12B Image Model Released](#item-2) ⭐️ 9.0/10
3. [Gemini 3.5 Flash Gains Computer Use Feature](#item-3) ⭐️ 9.0/10
4. [Qualcomm to Acquire AI Startup Modular for $4B](#item-4) ⭐️ 8.0/10
5. [NVIDIA's 45°C Cooling Cuts Data Center Water Use Near Zero](#item-5) ⭐️ 8.0/10
6. [GLM-5.2: Open-Weight Model Challenges Proprietary AI](#item-6) ⭐️ 8.0/10
7. [Nub: Bun-like toolkit for Node.js via preload hooks](#item-7) ⭐️ 8.0/10
8. [GPT-5 solves 3-year-old immunology mystery](#item-8) ⭐️ 8.0/10
9. [Databricks Leaders Advocate for Open Agent Cloud Ecosystem](#item-9) ⭐️ 8.0/10
10. [Claude Slackbot Upgrade: Multiplayer, Proactive, Persistent Agents](#item-10) ⭐️ 8.0/10
11. [Tech Giants Launch $500M Initiative to Eliminate Respiratory Viruses](#item-11) ⭐️ 8.0/10
12. [SpaceX Unveils AI1, Its First Orbital AI Data Center Satellite](#item-12) ⭐️ 8.0/10
13. [EU Funds Open-Source 400B+ Frontier AI Model](#item-13) ⭐️ 8.0/10
14. [John Carmack comments on datacenter infrastructure](#item-14) ⭐️ 8.0/10
15. [RubyLLM: A Unified Ruby Framework for Major AI Providers](#item-15) ⭐️ 7.0/10
16. [PR spam today mirrors early 2000s email spam](#item-16) ⭐️ 7.0/10
17. [Carmack Regrets Pushing id Software Too Hard](#item-17) ⭐️ 7.0/10
18. [OpenAI Joins Appia Foundation for AI Standards](#item-18) ⭐️ 7.0/10
19. [LLM-Generated Job Apps Obscure Candidate Identity](#item-19) ⭐️ 7.0/10
20. [Datasette 1.0a35 Adds Create/Alter Table with JSON APIs](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI Unveils First Custom AI Chip 'Jalapeno' with Broadcom](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI and Broadcom have unveiled Jalapeno, OpenAI's first custom AI inference chip, designed and manufactured in just nine months with help from OpenAI's own models. The chip is built by TSMC and is claimed to match Nvidia's Blackwell and Google's TPU in performance. This marks a major strategic move by OpenAI to reduce reliance on Nvidia GPUs and lower inference costs, potentially reshaping the AI hardware landscape. It also demonstrates the growing trend of AI companies designing custom silicon for specific workloads. Jalapeno is a reticle-sized ASIC designed specifically for large language model inference, with a highly repetitive tiled floorplan. Broadcom CEO Hock Tan stated the chip matches Nvidia's Blackwell and Google's TPU in performance, and it is manufactured by TSMC.

hackernews · jamdesk · Jun 24, 17:47 · [Discussion](https://news.ycombinator.com/item?id=48663324)

**Background**: AI inference chips are specialized processors that run trained AI models to generate responses, as opposed to training chips that build models. OpenAI has relied heavily on Nvidia GPUs for both training and inference, but custom chips like Jalapeno can offer better efficiency and cost savings for inference at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip | OpenAI</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/broadcom-and-openai-unveil-custom-built-jalapeno-inference-processor-openais-first-chip-is-a-massive-reticle-sized-asic-built-in-an-ultra-fast-nine-month-development-cycle">Broadcom and OpenAI unveil custom-built Jalapeño inference processor — OpenAI's first chip is a massive reticle-sized ASIC built in an ultra-fast nine-month development cycle | Tom's Hardware</a></li>
<li><a href="https://money.usnews.com/investing/news/articles/2026-06-24/openai-unveils-custom-chip-it-designed-with-broadcom-to-boost-its-ai-infrastructure">OpenAI Unveils Custom Chip It Designed With Broadcom to Boost Its AI Infrastructure</a></li>

</ul>
</details>

**Discussion**: Commenters expressed curiosity about how OpenAI's models accelerated chip design, with some skepticism that it might be marketing hype. Others discussed the potential of weight-in-ROM designs and referenced Taalas, a company that burns LLM weights directly into silicon for efficiency gains.

**Tags**: `#AI hardware`, `#OpenAI`, `#custom chip`, `#inference`, `#Broadcom`

---

<a id="item-2"></a>
## [Krea 2: SOTA Open-weights 12B Image Model Released](https://www.krea.ai/blog/krea-2-technical-report) ⭐️ 9.0/10

Krea has released Krea 2, a 12-billion-parameter open-weights text-to-image diffusion model, along with a detailed technical report covering training, data curation, and infrastructure. The release includes both a base model and a Turbo variant optimized for speed. Krea 2 achieves state-of-the-art results among locally hostable models, outperforming many competitors while being fast enough for practical use. This strengthens the open-weights ecosystem, enabling developers and researchers to run high-quality image generation on their own hardware without relying on proprietary APIs. The Turbo model uses guidance and timestep distillation for faster inference, achieving competitive quality in as few as 8 steps. The technical report provides deep insights into data curation, captioning, model architecture, post-training, RL pipelines, prompt expansion, and infrastructure.

hackernews · mattnewton · Jun 23, 15:31 · [Discussion](https://news.ycombinator.com/item?id=48646659)

**Background**: Open-weights models allow users to download and run the model on their own infrastructure, ensuring sovereignty and privacy. Krea 2 is built on a Diffusion Transformer architecture, a modern approach for image generation that scales well with model size.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stablediffusiontutorials.com/2026/06/krea2-base-turbo.html">Krea 2 Raw/Base & Turbo (BF16/FP8/NVFP4/INT8) High Quality...</a></li>
<li><a href="https://www.nextdiffusion.ai/tutorials/krea-2-uncensored-text-to-image-generations-in-comfyui">Krea 2: Unsencored Text-to- Image Generations in... | Next Diffusion</a></li>

</ul>
</details>

**Discussion**: The community response has been highly positive, with praise for the detailed technical report and the model's performance. Commenters noted that Krea 2 Turbo outperforms most locally hostable models in speed and quality, though it still falls short of some larger proprietary models like Ideogram 4. Some discussion centered on the model's ability to handle diverse styles and the availability of a GGUF quantized version.

**Tags**: `#AI/ML`, `#image generation`, `#open-source`, `#deep learning`, `#infrastructure`

---

<a id="item-3"></a>
## [Gemini 3.5 Flash Gains Computer Use Feature](https://deepmind.google/blog/introducing-computer-use-in-gemini-3-5-flash/) ⭐️ 9.0/10

Google DeepMind has integrated computer use as a built-in tool in Gemini 3.5 Flash, enabling the AI to interact with software interfaces via screenshots and mouse/keyboard control. This advancement significantly enhances AI agent capabilities, allowing Gemini to automate complex desktop tasks and potentially reshape software engineering and workflow automation. Previously available only as a standalone model, computer use is now natively integrated into Gemini 3.5 Flash, delivering the best performance yet for agentic computer use tasks.

rss · Google DeepMind Blog · Jun 24, 16:30

**Background**: Computer use agents are AI systems that can see a user's screen via screenshots and control mouse and keyboard to operate any desktop application like a human. This represents a shift from providing information to taking direct action on behalf of the user.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/">Introducing computer use in Gemini 3.5 Flash</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3.5 Flash — Google DeepMind</a></li>
<li><a href="https://9to5google.com/2026/06/24/gemini-chrome-select-screen/">Gemini in Chrome adds ‘Select from screen’ tool as Gemini 3.5 Flash gains computer use</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed reactions: some users report Gemini giving up on tasks or making destructive mistakes like running 'git reset --hard', while others note missing features like MCP support and lack of a Codex/Claude Code equivalent for coding tasks.

**Tags**: `#AI`, `#Gemini`, `#agents`, `#Google DeepMind`, `#computer use`

---

<a id="item-4"></a>
## [Qualcomm to Acquire AI Startup Modular for $4B](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 8.0/10

Qualcomm announced its acquisition of Modular, the AI infrastructure startup behind the Mojo programming language, for $4 billion. The deal is expected to close in late 2026. This acquisition strengthens Qualcomm's AI and RISC-V portfolio, positioning it to compete with NVIDIA in AI inference and training. It also brings the innovative Mojo language and Modular's AI stack under Qualcomm's hardware expertise. The $4 billion deal includes Modular's team, Mojo language, and MAX platform for heterogeneous AI compute. Qualcomm plans to integrate Modular's technology into its Snapdragon and RISC-V-based chips.

hackernews · timmyd · Jun 24, 13:49 · [Discussion](https://news.ycombinator.com/item?id=48659798)

**Background**: Modular, co-founded by Chris Lattner (creator of LLVM and Swift), developed Mojo, a Python-like language for high-performance AI on diverse hardware. Qualcomm has been expanding beyond mobile chips into AI and RISC-V, acquiring companies like Tenstorrent and Ventana. RISC-V is an open-source instruction set architecture that offers an alternative to ARM and x86.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language ) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/RISC-V">RISC-V - Wikipedia</a></li>
<li><a href="https://www.modular.com/">Modular: Inference from Kernel to Cloud</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some question the strategic fit given Qualcomm's limited presence in high-end AI, while others see it as a bold move to build a comprehensive AI portfolio. There is also debate about Mojo's design choices and whether Lattner's efforts could have been better spent.

**Tags**: `#acquisition`, `#AI`, `#Qualcomm`, `#Modular`, `#Mojo`

---

<a id="item-5"></a>
## [NVIDIA's 45°C Cooling Cuts Data Center Water Use Near Zero](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA has introduced a 45°C direct-to-chip liquid cooling architecture for AI data centers that dramatically reduces water consumption, enabling near-zero water usage and opening up possibilities for waste heat reuse in district heating. This innovation addresses the growing water and energy demands of AI infrastructure, making data centers more sustainable and potentially turning them into heat sources for communities, which could reshape data center location and design strategies. The system uses coolant at up to 45°C (113°F), much warmer than traditional liquid cooling, which reduces or eliminates the need for energy-intensive chillers and water evaporation for cooling. This design is specifically optimized for next-generation AI hardware.

hackernews · nitin_flanker · Jun 24, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48660178)

**Background**: Traditional data centers rely on air conditioning or liquid cooling with cold water (typically below 20°C) to remove heat from servers, consuming large amounts of electricity and water. Liquid cooling is becoming more common as AI rack densities increase, with 59% of data centers planning to implement it within five years. Higher coolant temperatures can significantly improve energy efficiency and enable waste heat recovery for district heating networks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45 ° C Liquid Cooling Design for AI Data Centers</a></li>
<li><a href="https://www.techbuzz.ai/articles/nvidia-s-45-c-liquid-cooling-redefines-ai-data-center-energy">NVIDIA's 45 ° C Liquid Cooling Redefines AI Data Center Energy</a></li>
<li><a href="https://www.networkworld.com/article/4149069/why-ai-rack-densities-make-liquid-cooling-nonnegotiable.html">Why AI rack densities make liquid cooling ... | Network World</a></li>

</ul>
</details>

**Discussion**: Commenters discussed the potential for district heating synergies, noting that 45°C is suitable for heating loops and could provide value to local communities. Some questioned the climate dependency and requested more details on efficiency across different climates, while others shared practical experiences with similar high-temperature cooling setups.

**Tags**: `#data center cooling`, `#liquid cooling`, `#energy efficiency`, `#NVIDIA`, `#sustainability`

---

<a id="item-6"></a>
## [GLM-5.2: Open-Weight Model Challenges Proprietary AI](https://www.interconnects.ai/p/glm-52-is-the-step-change-for-open) ⭐️ 8.0/10

Z.ai released GLM-5.2, an open-weight, MIT-licensed coding model with 753B parameters and a 1M-token context window, achieving competitive performance against proprietary models like Claude Opus and GPT-5.5 at a fraction of the cost. GLM-5.2 significantly lowers the barrier to high-quality AI coding assistance, making advanced capabilities accessible to individuals and organizations that cannot afford expensive proprietary subscriptions, potentially democratizing AI-powered development. The model uses an 'index share' trick to achieve cheap 1M-context processing, but users report aggressive token consumption—some burning through weekly quotas in under two days, consuming 20x more tokens than comparable proprietary models for similar tasks.

hackernews · vantareed · Jun 23, 03:23 · [Discussion](https://news.ycombinator.com/item?id=48639840)

**Background**: Open-weight models allow developers to inspect, modify, and self-host the model weights, offering transparency and control. GLM-5.2 is the latest in a series of competitive open models from Chinese labs, following DeepSeek and others, that are narrowing the performance gap with proprietary systems while offering much lower pricing.

<details><summary>References</summary>
<ul>
<li><a href="https://gptproto.com/news/what-is-glm-5-2">What Is GLM 5 . 2 ? Open - Weight Model vs Claude Opus...</a></li>
<li><a href="https://www.buildfastwithai.com/blogs/glm-5-2-review-2026">GLM - 5 . 2 Review 2026: Z.ai's 1M-Context AI Model</a></li>
<li><a href="https://www.youtube.com/watch?v=S2Jz4wBbQdw">First Look at GLM - 5 . 2 : Open Weights Model On Par with... - YouTube</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: many praise the model's intelligence and cost-effectiveness, but several users strongly criticize the aggressive token consumption, calling the pricing plan a 'scam.' One user noted that GLM-5.2 solved problems as well as Opus but used far more tokens, while another found it indistinguishable from Codex for straightforward coding tasks.

**Tags**: `#AI`, `#open-source`, `#LLM`, `#cost`, `#coding`

---

<a id="item-7"></a>
## [Nub: Bun-like toolkit for Node.js via preload hooks](https://github.com/nubjs/nub) ⭐️ 8.0/10

Colin McDonnell released Nub, an all-in-one toolkit that adds transpilation, module resolution, and polyfills to stock Node.js using --require preload hooks and module hooks, enabling TypeScript and modern JS execution without changing the runtime. Nub brings Bun-like developer experience to Node.js without replacing the runtime, offering a non-invasive way to run TypeScript and modern JS that could improve productivity for many Node.js developers. Nub uses the oxc transpiler as a Node-API add-on for fast transpilation, registers a module resolution hook, and injects polyfills for APIs like Worker and Temporal. It is purely additive and runs on stock Node.js.

hackernews · colinmcd · Jun 24, 14:14 · [Discussion](https://news.ycombinator.com/item?id=48660267)

**Background**: Bun is an all-in-one JavaScript runtime that includes a bundler, test runner, and package manager, offering a seamless developer experience. Node.js natively supports TypeScript stripping since recent versions, but lacks built-in transpilation for advanced features. Nub fills this gap by adding Bun-like capabilities via hooks.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all - in - one JavaScript runtime</a></li>

</ul>
</details>

**Discussion**: The community is positive, with users praising the clever approach and reporting smooth migration experiences. Some questioned why a transpiler is needed given Node's native TypeScript support, and others asked about ESM support nuances regarding the use of --require vs --import.

**Tags**: `#node.js`, `#typescript`, `#tooling`, `#developer-experience`, `#open-source`

---

<a id="item-8"></a>
## [GPT-5 solves 3-year-old immunology mystery](https://openai.com/index/gpt-5-immunology-mystery) ⭐️ 8.0/10

OpenAI's GPT-5 Pro model helped immunologist Derya Unutmaz solve a long-standing mystery about T cell behavior that had puzzled researchers for three years. This breakthrough demonstrates AI's potential to accelerate biomedical research, with implications for developing new cancer immunotherapies and autoimmune disease treatments. GPT-5 Pro is a version of GPT-5 with extended reasoning capabilities, launched on August 7, 2025, and available to Pro subscribers. The specific T cell behavior insights could inform future therapeutic strategies.

rss · OpenAI News · Jun 23, 17:00

**Background**: T cells are a type of immune cell that play a critical role in fighting infections and cancer. Understanding their behavior is key to developing effective immunotherapies. GPT-5 is OpenAI's latest multimodal large language model, succeeding GPT-4.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-5/">Introducing GPT - 5 | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5_Pro">GPT-5 Pro</a></li>

</ul>
</details>

**Tags**: `#AI`, `#immunology`, `#GPT-5`, `#scientific breakthrough`, `#medical research`

---

<a id="item-9"></a>
## [Databricks Leaders Advocate for Open Agent Cloud Ecosystem](https://www.latent.space/p/databricks) ⭐️ 8.0/10

In a rare double-interview, Databricks technical leaders Matei Zaharia and Reynold Xin argue that the frontier ecosystem must be open to enable every company to build Agent Clouds. This vision could shape the future of AI agent deployment, promoting interoperability and reducing vendor lock-in, which is critical as enterprises increasingly adopt AI agents. The interview focuses on the concept of Agent Clouds—platforms for deploying and managing AI agents—and why an open ecosystem is essential for widespread adoption.

rss · Latent Space · Jun 24, 18:53

**Background**: Databricks is a leading data and AI platform that provides a unified environment for data engineering, analytics, and machine learning. Agent Clouds refer to cloud-based platforms that enable the deployment and orchestration of autonomous AI agents. An open ecosystem means that the underlying technologies and standards are publicly available, allowing different systems to interoperate.

<details><summary>References</summary>
<ul>
<li><a href="https://www.databricks.com/">Databricks : Leading Data and AI Platform for Enterprises</a></li>
<li><a href="https://medium.com/@philippeandrepage/ai-agent-clouds-c8cf588f7392">Autonomous Agent Clouds . A Conceptual Framework for... | Medium</a></li>
<li><a href="https://www.agentcloud.dev/">Homepage | Agent Cloud - Open source platform to talk to your data</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open source`, `#Databricks`, `#agent clouds`, `#ecosystem`

---

<a id="item-10"></a>
## [Claude Slackbot Upgrade: Multiplayer, Proactive, Persistent Agents](https://www.latent.space/p/ainews-claude-tag-multiplayer-proactive) ⭐️ 8.0/10

Anthropic has upgraded Claude's Slack integration to support multiplayer, proactive, and persistent AI agents, allowing teams to collaborate with AI in real-time within Slack channels. This update transforms Claude from a reactive chatbot into a proactive team member that can persist across conversations, significantly enhancing team productivity and enabling new collaborative workflows. The upgrade enables 'multiplayer AI' where the entire channel can see the agent's work, build on it, and redirect it in real time, eliminating siloed windows. It also introduces proactive and persistent behaviors, allowing agents to take initiative and maintain context over time.

rss · Latent Space · Jun 24, 07:14

**Background**: Traditional AI assistants are reactive and stateless, waiting for user prompts and forgetting context after each interaction. Proactive agents can identify opportunities and act without explicit requests, while persistent agents maintain state across sessions. This upgrade aligns with the broader industry trend toward more autonomous and collaborative AI agents.

<details><summary>References</summary>
<ul>
<li><a href="https://www.salesforceben.com/anthropic-and-salesforce-announce-new-claude-to-slack-integration/">Anthropic and Salesforce Announce New Claude to... | Salesforce Ben</a></li>
<li><a href="https://github.com/ArkMaster123/agents-slackbot">GitHub - ArkMaster123/ agents - slackbot : Multi - agent Slack bot with...</a></li>

</ul>
</details>

**Tags**: `#Claude`, `#Slack`, `#AI agents`, `#collaboration`, `#productivity`

---

<a id="item-11"></a>
## [Tech Giants Launch $500M Initiative to Eliminate Respiratory Viruses](https://www.reddit.com/r/singularity/comments/1uefo1j/openai_anthropic_stripe_and_bill_gates_are/) ⭐️ 8.0/10

OpenAI, Anthropic, Stripe, and Bill Gates have jointly funded a new $500 million philanthropic organization called Intercept, which aims to radically reduce the burden of respiratory infections and eventually eliminate all respiratory viruses. This initiative brings together major tech and philanthropic figures to tackle a persistent global health problem that kills 1 million people annually and costs $600 billion per year, potentially transforming public health through innovative prevention approaches. Intercept will use grants and investments to back prevention approaches including vaccines and large-scale air-cleaning systems for schools, offices, and other public spaces, initially targeting the common cold and influenza.

reddit · r/singularity · /u/TorturedPoet30 · Jun 24, 14:50

**Background**: Respiratory viruses such as the common cold, flu, and COVID-19 cause widespread illness, death, and economic disruption. Despite advances in vaccines and treatments, no coordinated effort has aimed to eliminate entire classes of respiratory viruses. Intercept is a philanthropic initiative modeled after similar ambitious projects like the Gates Foundation's efforts against malaria.

<details><summary>References</summary>
<ul>
<li><a href="https://www.interceptfund.com/">Intercept</a></li>
<li><a href="https://www.technologyreview.com/2026/06/24/1139621/stripe-anthropic-and-openai-are-backing-an-effort-to-stop-respiratory-infections/">Stripe, Anthropic and OpenAI are backing an effort to stop respiratory ...</a></li>
<li><a href="https://cryptobriefing.com/stripe-500m-intercept-nonprofit-respiratory-viruses/">Stripe commits $500M to nonprofit Intercept in bid to eliminate ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#biotech`, `#funding`, `#public health`, `#philanthropy`

---

<a id="item-12"></a>
## [SpaceX Unveils AI1, Its First Orbital AI Data Center Satellite](https://www.reddit.com/r/singularity/comments/1uefbv5/spacex_unveils_ai1_its_first_orbital_ai_data/) ⭐️ 8.0/10

On June 8, 2026, SpaceX unveiled AI1, its first-generation orbital AI data center satellite, designed to provide space-based computing power for AI inference and data processing. This marks a major step toward space-based cloud computing, potentially reducing latency for global AI applications and enabling continuous solar-powered AI operations without Earth-bound energy constraints. Musk described AI1 as essentially solar cells, a radiator, and laser links — simpler than a Starlink satellite — and it operates at 120 kilowatts, with plans to scale up for orbital data centers.

reddit · r/singularity · /u/No-Blackberry-7564 · Jun 24, 14:37

**Background**: Space-based computing has evolved from onboard computers for space missions to potential orbital cloud infrastructure. AI1 leverages SpaceX's Starlink laser communication technology to connect satellites, enabling low-latency data processing in orbit.

<details><summary>References</summary>
<ul>
<li><a href="https://www.agenticbrew.ai/news/2c23f96e-1c9d-4fa8-9d4d-4a991865b4f8/spacex-unveils-ai1-its-first-orbital-ai-data-center-satellite">SpaceX unveils AI 1, its first orbital AI data center satellite — AI News</a></li>
<li><a href="https://digg.com/ai/5iti9pyn">Elon Musk announces SpaceX's AI 1 satellite , a 120-kilowatt orbital AI ...</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pIeHV1a0VSRTRCSkFqWUNsWDRpZ0FQAQ?hl=en-IN&gl=IN&ceid=IN:en">Elon Musk unveils SpaceX orbital AI data center satellite design...</a></li>

</ul>
</details>

**Discussion**: The r/singularity community expressed excitement about the potential for edge computing in space, though some questioned the technical feasibility and economic viability, noting analyst estimates of only 7% odds for orbital data centers.

**Tags**: `#SpaceX`, `#AI`, `#Satellite`, `#Data Center`, `#Space Computing`

---

<a id="item-13"></a>
## [EU Funds Open-Source 400B+ Frontier AI Model](https://www.reddit.com/r/singularity/comments/1ue8yy5/the_eu_is_funding_its_own_opensource_400b/) ⭐️ 8.0/10

The European Commission selected the EUROPA consortium, led by Italian company Domyn, as the winner of the Frontier AI Grand Challenge to build an open-source AI model with over 400 billion parameters, covering all 24 official EU languages, trained on European supercomputers. This initiative marks a significant step in AI geopolitics, offering an open-source alternative to US-dominated frontier models and ensuring multilingual inclusivity from the start, which could reshape the global AI landscape. The prize is compute time, not cash: up to 2.5% of total EuroHPC capacity for one year on AI-optimized supercomputers. However, there is no delivery timeline, no training cost estimate, and no measurable definition of 'frontier-level' yet.

reddit · r/singularity · /u/ocean_protocol · Jun 24, 09:45

**Background**: The European High-Performance Computing Joint Undertaking (EuroHPC JU) is a joint initiative to develop a world-class supercomputing ecosystem in Europe. The Frontier AI Grand Challenge aims to boost European AI sovereignty by leveraging this infrastructure. Open-source models allow public access to the underlying code and weights, fostering transparency and collaboration.

<details><summary>References</summary>
<ul>
<li><a href="https://dig.watch/updates/eu-selects-europa-consortium-frontier-ai-project">EU selects EUROPA consortium to build multilingual frontier AI model</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/news/commission-selects-europa-consortium-winner-frontier-ai-grand-challenge-project-build-european-open">Commission selects EUROPA consortium as the winner of the...</a></li>
<li><a href="https://ieu-monitoring.com/editorial/eu-commission-picks-europa-consortium-led-by-domyn-to-build-open-frontier-ai-model/1243623">EU Commission picks EUROPA consortium led by Domyn to build...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion expresses cautious optimism, noting the modest one-year compute window compared to multi-year runs by US labs, and the lack of a concrete timeline. Commenters appreciate the multilingual focus but question whether the project will deliver a truly frontier-level model.

**Tags**: `#AI`, `#open-source`, `#EU`, `#frontier model`, `#supercomputing`

---

<a id="item-14"></a>
## [John Carmack comments on datacenter infrastructure](https://www.reddit.com/r/singularity/comments/1ue1sya/john_carmack_weighs_in_on_datacenters/) ⭐️ 8.0/10

John Carmack, a highly respected figure in technology, shared his perspective on datacenter infrastructure and its implications in a Reddit post on r/singularity. Carmack's commentary is influential in the tech community and could shape discussions on datacenter design, especially for AI workloads, given his expertise in high-performance computing. The post is a link to a Reddit discussion, but the specific content of Carmack's comments is not provided in the news item; the high score (8.0/10) indicates strong community interest.

reddit · r/singularity · /u/Singularity-42 · Jun 24, 03:06

**Background**: Datacenters are centralized facilities that house computing and networking equipment for data processing and storage. John Carmack is known for his work in game engine development (e.g., Doom, Quake) and virtual reality, and he frequently comments on technology trends.

**Tags**: `#datacenters`, `#John Carmack`, `#infrastructure`, `#AI`, `#tech commentary`

---

<a id="item-15"></a>
## [RubyLLM: A Unified Ruby Framework for Major AI Providers](https://rubyllm.com/) ⭐️ 7.0/10

RubyLLM is a new Ruby framework that provides a unified interface for multiple major AI providers, including OpenAI, Anthropic, and local models via Ollama. It aims to simplify AI integration for Ruby developers, similar to Vercel's AI framework for JavaScript. RubyLLM fills a gap in the Ruby ecosystem by offering a consistent, easy-to-use abstraction over diverse AI APIs, potentially accelerating AI adoption in Ruby and Rails applications. Its community traction (348 points, 54 comments) indicates strong interest, though practical issues like cache inconsistencies and maintainer engagement may affect long-term adoption. The framework supports multiple providers with a single interface, but users report cache inconsistencies with providers like xAI that only support completions API. Additionally, some community members have experienced challenges with maintainer responsiveness to pull requests and observed merged PRs that appear to be 'vibe coded'.

hackernews · doener · Jun 24, 14:41 · [Discussion](https://news.ycombinator.com/item?id=48660711)

**Background**: RubyLLM is an open-source Ruby gem that provides a unified API for interacting with various large language model (LLM) providers. It aims to reduce boilerplate and provider-specific code, similar to how Rails simplifies web development. The framework is opinionated and productive, treating AI integration as a first-class citizen in Ruby applications.

<details><summary>References</summary>
<ul>
<li><a href="https://rubyllm.com/">RubyLLM | One beautiful Ruby framework for all major AI providers.</a></li>
<li><a href="https://github.com/crmne/ruby_llm">GitHub - crmne/ ruby _ llm : One delightful Ruby framework for every...</a></li>
<li><a href="https://medium.com/airtribe/rubyllm-and-the-return-of-rails-superpower-notes-from-euruko-2025-b72eeeb6b185">RubyLLM and the Return of Rails’ Superpower — Notes... | Medium</a></li>

</ul>
</details>

**Discussion**: Community sentiment is generally positive, with users praising RubyLLM's usability and ease of use, comparing it favorably to Vercel's AI framework. However, concerns include cache issues with certain providers, difficulty in achieving true trace observability, and frustration with maintainer responsiveness to contributions. Some users also noted that the responses API was initially missing but has since been added natively.

**Tags**: `#Ruby`, `#AI`, `#framework`, `#LLM`, `#open source`

---

<a id="item-16"></a>
## [PR spam today mirrors early 2000s email spam](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 7.0/10

A blog post on Greptile compares the surge of spammy pull requests in open-source projects to the email spam epidemic of the early 2000s, calling for better moderation tools. This comparison highlights a growing problem that burdens open-source maintainers, potentially discouraging contributions and harming project health. Addressing it is crucial for sustaining the open-source ecosystem. GitHub recently introduced configurable PR limits for maintainers to help mitigate spam, but the problem persists. The article notes that spam PRs often target events like Hacktoberfest for swag.

hackernews · dakshgupta · Jun 24, 14:32 · [Discussion](https://news.ycombinator.com/item?id=48660579)

**Background**: Pull request spam involves low-quality or automated PRs submitted to open-source projects, often for personal gain or promotion. In the early 2000s, email spam overwhelmed inboxes until tools like Bayesian filters and sender reputation systems emerged. Open-source maintainers now face a similar deluge without mature moderation solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/shitoberfest/spam-pullrequests">GitHub - shitoberfest/ spam - pullrequests : Show the world how many...</a></li>
<li><a href="https://garvitasood.medium.com/github-clean-up-spam-babc5e5b5ab0">GitHub Clean-up Spam . by Garvita Sood, Anuj Bansal, Garima | Medium</a></li>
<li><a href="https://github.com/topics/moderation-tools">moderation - tools · GitHub Topics · GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters noted differences between email and PR spam, such as the lack of sender reputation for individual users on GitHub. Some suggested requiring non-textual introductions before merging first PRs, while others proposed donating token credits to projects for maintainers to allocate.

**Tags**: `#open-source`, `#spam`, `#maintainers`, `#GitHub`, `#community`

---

<a id="item-17"></a>
## [Carmack Regrets Pushing id Software Too Hard](https://twitter.com/ID_AA_Carmack/status/2069799283369345247) ⭐️ 7.0/10

John Carmack, co-founder of id Software, publicly shared regrets about pushing his team too hard during the company's early days, stating that startup intensity can wear out a maturing company. This reflection offers valuable leadership lessons for the game development industry and startup culture, highlighting the long-term costs of unsustainable work intensity. Carmack specifically mentioned that he didn't appreciate how maturing companies need more slack, and that running people at startup intensity constantly will wear them out.

hackernews · shadowtree · Jun 24, 15:56 · [Discussion](https://news.ycombinator.com/item?id=48661825)

**Background**: id Software is known for pioneering first-person shooters like Doom and Quake. Carmack's tweet reflects on the intense development culture that produced Quake, which some argue gutted the company.

**Discussion**: Commenters largely agreed with Carmack's regrets, with some noting that Quake's success may have come at the cost of the company's long-term health. Others debated whether the ends justified the means.

**Tags**: `#leadership`, `#game development`, `#startup culture`, `#id Software`, `#John Carmack`

---

<a id="item-18"></a>
## [OpenAI Joins Appia Foundation for AI Standards](https://openai.com/index/helping-build-shared-standards-for-advanced-ai) ⭐️ 7.0/10

OpenAI announced its contribution to the Appia Foundation, an initiative under the Linux Foundation, to help develop shared standards, evaluation frameworks, and safety practices for advanced AI. This move signals a commitment to global cooperation and safety in AI development, potentially leading to widely adopted benchmarks that ensure AI systems meet consumer expectations across the supply chain. The Appia Foundation aims to establish modular open source specifications and conformity specifications for the AI value chain, building on the Joint Development Foundation's framework.

rss · OpenAI News · Jun 23, 13:00

**Background**: The Appia Foundation was launched by the Linux Foundation to create standardized conformity specifications across the AI value chain. It operates under the Joint Development Foundation, which provides a legal and governance framework for open standards projects. This effort addresses the need for practical means to assess AI systems' compliance with obligations and expectations.

<details><summary>References</summary>
<ul>
<li><a href="https://appiafoundation.org/">Appia Foundation</a></li>
<li><a href="https://www.linuxfoundation.org/press/linux-foundation-launches-appia-foundation-to-establish-standardized-conformity-specifications-across-the-ai-value-chain">Linux Foundation Launches Appia Foundation to Establish...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#AI governance`, `#OpenAI`, `#standards`, `#global cooperation`

---

<a id="item-19"></a>
## [LLM-Generated Job Apps Obscure Candidate Identity](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 7.0/10

Tom MacWright observes that job applications and portfolios increasingly appear to be entirely generated by LLMs, making candidates indistinguishable and generic. This trend undermines the purpose of job applications by erasing personal authenticity, making it harder for employers to assess true skills and fit. MacWright notes that LLM-generated applications often link to LLM-generated portfolio sites and GitHub projects with LLM-generated commit messages, revealing nothing about the candidate's actual abilities.

rss · Simon Willison · Jun 24, 18:13

**Background**: Large language models (LLMs) like GPT-4 can generate human-like text, including resumes, cover letters, and code. Job seekers increasingly use these tools to automate application materials, but over-reliance can produce content that lacks personal voice and genuine experience.

**Tags**: `#AI`, `#careers`, `#ethics`, `#hiring`, `#LLM`

---

<a id="item-20"></a>
## [Datasette 1.0a35 Adds Create/Alter Table with JSON APIs](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35 alpha release introduces a Create Table interface and an Alter Table interface, both backed by new JSON API endpoints for database schema management. These features significantly enhance Datasette's capability as a full-featured database management tool, allowing users to modify schemas directly through the UI or API without external tools. The Create Table API supports defining columns, primary keys, custom types, NOT NULL constraints, defaults, and single-column foreign keys. The Alter Table API allows adding, renaming, reordering, dropping columns, changing types and constraints, and renaming the table, including a Drop Table button.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing data, especially SQLite databases. It provides a web interface and JSON API for querying and browsing data. Prior to this release, Datasette lacked built-in schema modification capabilities, requiring users to use external tools like sqlite3 or DB Browser for SQLite.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2026/jun/23/datasette/">Release: datasette 1.0a35 | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#database`, `#JSON API`, `#open source`

---