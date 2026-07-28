---
layout: default
title: "Horizon Summary: 2026-07-28 (EN)"
date: 2026-07-28
lang: en
---

> From 36 items, 17 important content pieces were selected

---

1. [Anthropic Clarifies Stance on Open-Weights AI Models](#item-1) ⭐️ 9.0/10
2. [Researcher Hacks Volvo/Eicher Fleet Platform, Gains Full Control](#item-2) ⭐️ 9.0/10
3. [Moonshot AI Releases 2.8T Parameter Kimi K3 Weights](#item-3) ⭐️ 9.0/10
4. [vLLM v0.26.0 Adds Inkling Support, DeepSeek-V4 Optimizations](#item-4) ⭐️ 8.0/10
5. [python-build-standalone Powers Modern Python Tooling](#item-5) ⭐️ 8.0/10
6. [Missing underscore leads to 18-month wrongful imprisonment](#item-6) ⭐️ 8.0/10
7. [Judge Rejects Google's DMCA Anti-Scraping Bid](#item-7) ⭐️ 8.0/10
8. [LLM Token Relay Market Fuels Fraud and Reselling](#item-8) ⭐️ 8.0/10
9. [NVIDIA Cosmos-H-Dreams: Real-Time Generative Simulation for Surgical Robotics](#item-9) ⭐️ 8.0/10
10. [OpenAI Declines to Join Nvidia's Open Secure AI Alliance](#item-10) ⭐️ 8.0/10
11. [User Runs Kimi K3 on 80 RTX 5090s via 25GbE](#item-11) ⭐️ 8.0/10
12. [Case Study: Replacing React with HTMX in a Forum Platform](#item-12) ⭐️ 7.0/10
13. [Paged Out #9: Free Technical Magazine Released](#item-13) ⭐️ 7.0/10
14. [FeyNoBg: Open-Source Background Removal Model and Library](#item-14) ⭐️ 7.0/10
15. [Libsm64: Super Mario 64 as a Reusable Library for Game Engines](#item-15) ⭐️ 7.0/10
16. [Ethan Mollick's AI Guide Shifts from Chat to Agentic Systems](#item-16) ⭐️ 7.0/10
17. [Ninfer Achieves 700 t/s on Qwen 3.6 35B with RTX 5090](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic Clarifies Stance on Open-Weights AI Models](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 9.0/10

Anthropic published an official position stating it does not advocate for a ban on open-weights models, but instead calls for mandatory safety testing for all sufficiently capable AI models, both open and closed. This policy statement from a leading AI company could shape regulatory debates, as mandatory safety testing may effectively restrict open-weights models if testing costs are high or approval is withheld, potentially impacting open-source AI development and competition. Anthropic's CEO Dario Amodei also supports banning chip sales to China and cracking down on smuggling, which critics argue contradicts his stated opposition to bans. The company has not specified who would administer the safety tests or what criteria would be used.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open-weights AI models are models whose trained parameters (weights) are publicly released, allowing anyone to download, modify, and run them. Unlike fully open-source models, open-weights models may not include training data or code. Mandatory safety testing, or 'evals,' are tests designed to assess risks before deployment, and governments are increasingly considering making them mandatory for frontier AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_safety">AI safety - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters largely view Anthropic's position as a de facto ban on open-weights models, arguing that mandatory testing controlled by a government or industry body could be used to block open models. Some also accuse Anthropic of hypocrisy for supporting hardware export bans while opposing software bans, and for prioritizing profit over safety.

**Tags**: `#AI safety`, `#open-weights models`, `#regulation`, `#Anthropic`, `#policy`

---

<a id="item-2"></a>
## [Researcher Hacks Volvo/Eicher Fleet Platform, Gains Full Control](https://eaton-works.com/2026/07/27/my-eicher-hack/) ⭐️ 9.0/10

Security researcher Eaton Works discovered and exploited a critical vulnerability in Volvo/Eicher's My Eicher fleet management platform, allowing full account takeover and control over all users and vehicles. The vulnerability was responsibly disclosed and fixed within 17 days. This vulnerability highlights the severe risks of centralized cloud-based fleet management systems, where a single flaw can compromise an entire fleet. It underscores the urgent need for robust security in automotive telematics and reinforces the right-to-repair movement. The vulnerability involved API authentication bypass, allowing unauthorized access to internal APIs. The researcher reported the issue on November 3, 2025, and after follow-ups, the fix was deployed by November 20, 2025; the disclosure was published on July 27, 2026.

hackernews · EatonZ · Jul 27, 15:08 · [Discussion](https://news.ycombinator.com/item?id=49070756)

**Background**: Fleet management platforms like My Eicher use telematics to monitor and control vehicles remotely, including tracking, diagnostics, and even engine shutdown. Centralized cloud control creates a single point of failure; similar vulnerabilities have been found in other fleet systems (e.g., iTrack, ProTrack) and connected car features.

<details><summary>References</summary>
<ul>
<li><a href="https://eaton-works.com/2026/07/27/my-eicher-hack/">Exploiting Volvo / Eicher ’s fleet management platform to gain control...</a></li>
<li><a href="https://thepixelspulse.com/posts/exploiting-volvoeichers-fleet-platform-to-gain-control-over-all-usersvehicles/">Exploiting VolvoEicher's fleet platform to gain control over all...</a></li>
<li><a href="https://vicone.com/blog/how-authentication-and-api-vulnerabilities-undermine-fleet-management-systems">How Authentication and API Vulnerabilities Undermine Fleet Management Systems - VicOne</a></li>

</ul>
</details>

**Discussion**: Commenters praised the researcher's patience with the 17-day fix timeline and raised broader concerns about modern cars' dependence on cloud services, with one user noting a BMW that wouldn't start due to lack of phone reception. Others linked the issue to right-to-repair and security theater.

**Tags**: `#security`, `#automotive`, `#vulnerability`, `#fleet management`, `#responsible disclosure`

---

<a id="item-3"></a>
## [Moonshot AI Releases 2.8T Parameter Kimi K3 Weights](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 9.0/10

Moonshot AI has released the open-weight model Kimi K3 with 2.8 trillion parameters on Hugging Face, under a modified license that requires separate agreements for large Model-as-a-Service businesses. This release marks a significant milestone in open-weight AI, as Kimi K3 is one of the largest models available, and its novel licensing approach could influence how other companies balance openness with commercial control. The model uses a Mixture-of-Experts architecture with 896 experts, 16 active per token, supports 1M context length, and is trained with MXFP4 quantization-aware training, resulting in ~1.4 TB weights. The license requires a separate agreement for MaaS providers with over $20M annual revenue.

rss · Simon Willison · Jul 27, 23:39

**Background**: Kimi K3 is the successor to Kimi K2, which used a modified MIT license requiring attribution for large commercial entities. The new license drops the 'modified MIT' label and adds stricter terms for large MaaS providers. Moonshot AI consistently uses the term 'open weight' rather than 'open source'.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/ Kimi - K 3 · Hugging Face</a></li>
<li><a href="https://vllm.ai/blog/2026-07-22-kimi-k3-preview">A Preview of Production-Scale Kimi K 3 Support on vLLM | vLLM Blog</a></li>

</ul>
</details>

**Discussion**: Reddit comments focus on the practical challenges of hosting K3, with one provider noting that 8x A100 nodes provide only 640 GB memory, insufficient for the 1.4 TB weights, and that Ampere GPUs lack FP4 tensor cores, requiring dequantization or INT4 kernels.

**Tags**: `#AI`, `#open-source`, `#large language model`, `#Kimi K3`, `#Moonshot AI`

---

<a id="item-4"></a>
## [vLLM v0.26.0 Adds Inkling Support, DeepSeek-V4 Optimizations](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 introduces day-0 support for the 1T-parameter Inkling multimodal model family from Thinking Machines Lab, along with DeepSeek-V4 performance optimizations including a specialized routing kernel and fused_topk_bias. The release also adds fp32 lm_head via head_dtype, flexible attention backends per KV-cache group, and matures KV offloading with tiered secondary storage. This release significantly expands vLLM's model coverage and inference efficiency, enabling production deployment of cutting-edge 1T-parameter multimodal models and improving DeepSeek-V4 throughput by up to 2.94%. The flexible attention backends and KV offloading enhancements make vLLM more adaptable to diverse hardware and memory-constrained environments. The release includes 411 commits from 212 contributors, with new model support for Inkling, BertForMaskedLM, and RobertaForTokenClassification. Key technical features include Hopper FA4 relative attention for Inkling, ModelOpt NVFP4 quantization, and a Rust frontend with multimodal video and audio support.

github · khluu · Jul 27, 01:06

**Background**: vLLM is a high-throughput, memory-efficient LLM inference engine widely used in production. The Inkling model family is a 1T-parameter multimodal model that accepts text, image, and audio inputs with up to 1M context length. FlashAttention-4 (FA4) is the latest attention algorithm optimized for Hopper GPUs, offering significant speedups over previous versions.

<details><summary>References</summary>
<ul>
<li><a href="https://vllm.ai/blog/2026-07-15-inkling">TML Inkling on vLLM: Day-0 Support with Optimized Performance</a></li>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/inkling/">inkling - vLLM</a></li>
<li><a href="https://alphasignal.ai/news/vllm-v0-26-0-ships-day-0-support-for-inkling-s-1t-parameter-multimodal-model">vLLM v0.26.0 Ships Day-0 Support for Inkling's 1T-Parameter ...</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#DeepSeek`, `#CUDA`, `#ROCm`

---

<a id="item-5"></a>
## [python-build-standalone Powers Modern Python Tooling](https://gregoryszorc.com/docs/python-build-standalone/main/) ⭐️ 8.0/10

python-build-standalone provides self-contained, highly-portable Python distributions that are now used by major tools like uv, pipx, Hatch, Poetry, and Bazel to install Python. Astral has taken over maintenance, ensuring continued development and upstream integration. These distributions simplify Python deployment by eliminating system dependencies, enabling tools to bundle Python seamlessly. With over 70 million downloads, they are critical to the modern Python packaging ecosystem. The distributions are built from upstream CPython with minimal modifications, ensuring compatibility. They are used not only for tooling but also for bundling Python into applications like macOS desktop apps.

hackernews · jcbhmr · Jul 27, 18:43 · [Discussion](https://news.ycombinator.com/item?id=49073942)

**Background**: Traditionally, installing Python required a system-wide installation or manual compilation, which varied across platforms. python-build-standalone provides pre-built, relocatable binaries that work on Linux, macOS, and Windows, solving portability issues. Related projects like PyOxy and Cosmopolitan offer alternative approaches for single-file executables and cross-platform binaries.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/astral-sh/python-build-standalone">GitHub - astral-sh/ python - build - standalone : Produce redistributable...</a></li>
<li><a href="https://astral.sh/blog/python-build-standalone">A new home for python - build - standalone</a></li>
<li><a href="https://grokipedia.com/page/python-build-standalone">python-build-standalone</a></li>

</ul>
</details>

**Discussion**: Community members praised the distributions, with charliermarsh (uv creator) confirming uv uses them and noting Astral's upstreaming efforts. Simonw highlighted their utility for bundling Python into desktop apps. Others mentioned related projects like PyOxy and Cosmopolitan as alternatives for specific use cases.

**Tags**: `#Python`, `#tooling`, `#packaging`, `#portability`, `#open-source`

---

<a id="item-6"></a>
## [Missing underscore leads to 18-month wrongful imprisonment](https://arstechnica.com/tech-policy/2026/07/police-missed-one-underscore-and-sent-the-wrong-man-to-prison/) ⭐️ 8.0/10

A missing underscore in a Kik username caused police to arrest and prosecute the wrong man, who was convicted and served 18 months in prison before the error was discovered. This case highlights how minor software errors can lead to catastrophic failures in the criminal justice system, undermining trust in digital evidence and accountability. The victim was in the US and the defendant in Canada; despite no evidence linking Klayme to the crime, he was convicted and imprisoned. The error was only corrected after he served his sentence.

hackernews · quantified · Jul 27, 22:10 · [Discussion](https://news.ycombinator.com/item?id=49076116)

**Background**: Kik is a messaging app where usernames are case-sensitive and can include underscores. A single missing underscore caused police to target the wrong account, and the prosecution failed to verify the digital evidence properly.

**Discussion**: Commenters question how the defendant's lawyers failed to challenge the evidence, and note the lack of compensation for the wrongfully convicted man. Some reference the classic story 'Computers Don't Argue' as a parallel.

**Tags**: `#software error`, `#wrongful conviction`, `#criminal justice`, `#forensic evidence`, `#accountability`

---

<a id="item-7"></a>
## [Judge Rejects Google's DMCA Anti-Scraping Bid](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

A judge ruled against Google's attempt to use the Digital Millennium Copyright Act (DMCA) to block third-party scraping of its search results, rejecting the argument that scraping circumvented a technical protection measure. This decision sets a legal precedent that DMCA anti-circumvention provisions may not apply to web scraping of publicly available data, potentially limiting tech giants' ability to use copyright law to control data access. The case involved SerpAPI, a service that scrapes Google search results; Google had argued that scraping violated DMCA Section 1201 by circumventing its technical measures. The judge found that Google's measures did not effectively control access to copyrighted content.

hackernews · cdrnsf · Jul 27, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49073513)

**Background**: The DMCA's Section 1201 prohibits circumvention of technological measures that control access to copyrighted works. Web scraping involves automated extraction of data from websites, and its legality often hinges on whether the data is copyrighted and whether access controls are bypassed. Google has previously deprecated its official Search API, leaving third-party scrapers as the only way to access search results programmatically.

<details><summary>References</summary>
<ul>
<li><a href="https://nortonlaw.com/2026/05/14/dmca-section-1201-claims-the-new-battleground-for-ai-and-data-scraping-litigation/">DMCA Section 1201 Claims: The New Battleground for AI and Data Scraping Litigation - the NORTON law firm</a></li>
<li><a href="https://scrapfly.io/blog/posts/google-serp-api-and-alternatives">Best SERP APIs in 2026: Official Google Alternatives & Third-Party Providers</a></li>

</ul>
</details>

**Discussion**: Commenters expressed irony that Google, built on crawling the open web, now tries to block scraping. Many noted that Google's deprecation of its search API created demand for scrapers, and some highlighted the importance of scraping for exposing scams like fake ETA/ESTA sites.

**Tags**: `#web scraping`, `#DMCA`, `#Google`, `#legal`, `#tech policy`

---

<a id="item-8"></a>
## [LLM Token Relay Market Fuels Fraud and Reselling](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

An investigation by Matt Lenhard reveals a Chinese market where resellers offer discounted LLM tokens by pooling API keys, abusing free trials, and using stolen credentials, powered by open-source proxy software like one-api and new-api. This ecosystem poses significant security and economic risks to LLM vendors and developers, as it enables fraud, model distillation, and unauthorized access, potentially leading to large token bills for unprotected endpoints. The proxy software one-api and its fork new-api are legitimate open-source API management tools that can load-balance requests across pooled credentials. Buyers seek cheap tokens, bypass geo-restrictions, or collect data for model distillation.

rss · Simon Willison · Jul 26, 19:30

**Background**: LLM API tokens are used to pay for access to large language models like GPT-4. Resellers exploit pricing differences and security gaps by pooling keys from free trials, stolen credit cards, or unprotected support bots, then resell access at a discount through proxy servers.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/26/relay-market/">An Inside Look at the Relay Market Powering Token Resellers and Fraud</a></li>
<li><a href="https://github.com/songquanpeng/one-api">GitHub - songquanpeng/one-api: LLM API 管理 & 分发系统，支持 Open...</a></li>

</ul>
</details>

**Discussion**: On Hacker News, the discussion highlighted concerns about API security and the need for better rate limiting and spending caps. Some commenters noted the difficulty of detecting such abuse and called for vendors to implement stricter controls.

**Tags**: `#LLM`, `#API security`, `#fraud`, `#AI economics`, `#open-source`

---

<a id="item-9"></a>
## [NVIDIA Cosmos-H-Dreams: Real-Time Generative Simulation for Surgical Robotics](https://huggingface.co/blog/nvidia/cosmos-h-dreams) ⭐️ 8.0/10

NVIDIA introduced Cosmos-H-Dreams, a fine-tuned variant of Cosmos-H-Surgical-Simulator that enables real-time generative simulation for surgical robotics, driven by keyboard or Meta Quest controller input. This framework accelerates the development and training of surgical robots by providing realistic, interactive virtual environments, reducing reliance on physical data and enabling faster iteration. Cosmos-H-Dreams includes its own checkpoint and a streaming server serving layer, allowing live surgical simulation. It builds on NVIDIA's Cosmos platform, which features generative world foundation models for physical AI.

rss · Hugging Face Blog · Jul 27, 09:32

**Background**: Surgical robotics training traditionally requires expensive physical setups or pre-recorded data. Generative world models like Cosmos can synthesize realistic surgical video sequences from initial frames and robot actions, enabling faster-than-real-time evaluation and synthetic data generation.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/nvidia/cosmos-h-dreams">NVIDIA Cosmos-H-Dreams: Bringing Real-Time Generative ...</a></li>
<li><a href="https://github.com/isaac-for-healthcare/Cosmos-H-Dreams">GitHub - isaac-for-healthcare/Cosmos-H-Dreams</a></li>
<li><a href="https://docs.nvidia.com/cosmos/index.html">NVIDIA Cosmos - NVIDIA Docs</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#generative AI`, `#surgical robotics`, `#simulation`, `#real-time`

---

<a id="item-10"></a>
## [OpenAI Declines to Join Nvidia's Open Secure AI Alliance](https://www.reddit.com/r/LocalLLaMA/comments/1v8e36c/openai_management_decided_earlier_today_not_to/) ⭐️ 8.0/10

OpenAI management decided not to join the Open Secure AI Alliance, a new industry group founded by Nvidia CEO Jensen Huang with over 30 other companies, sparking internal employee backlash. This decision isolates OpenAI from a major collaborative effort on AI security and safety, potentially weakening industry-wide trust and coordination, while the internal backlash signals significant employee concern about the company's stance on open security initiatives. The Open Secure AI Alliance, announced on July 30, 2026, includes Nvidia and 36 partners such as Meta, Microsoft, and Google, aiming to share open tools, models, and research for AI security. OpenAI's refusal comes amid ongoing debates about model distillation, which Huang defends as a form of learning rather than theft.

reddit · r/LocalLLaMA · /u/KickLassChewGum · Jul 27, 21:37

**Background**: The Open Secure AI Alliance is an industry group focused on promoting responsible AI use through open tools and shared research. Model distillation is a technique where a smaller model learns from a larger one, which some see as a threat but Huang argues is essential for progress. OpenAI's decision not to join contrasts with its earlier open-source stance and may reflect strategic differences.

<details><summary>References</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/open-secure-ai-alliance/">Industry Leaders Join Open Secure AI Alliance for AI Safety ...</a></li>
<li><a href="https://seekingalpha.com/news/4618582-nvidia-and-over-30-firms-form-open-secure-ai-alliance-for-ai-safety">Nvidia and over 30 firms form Open Secure AI Alliance for AI ...</a></li>
<li><a href="https://thehackernews.com/2026/07/nvidia-forms-37-member-open-secure-ai.html">NVIDIA Forms 37-Member Open Secure AI Alliance and Open ...</a></li>

</ul>
</details>

**Discussion**: Reddit comments on the news are not provided in the content, but the post itself has active discussion. The community generally supports open security initiatives and criticizes OpenAI's decision, with some speculating about competitive motives or concerns over intellectual property.

**Tags**: `#OpenAI`, `#AI Security`, `#Industry Alliance`, `#Nvidia`, `#Governance`

---

<a id="item-11"></a>
## [User Runs Kimi K3 on 80 RTX 5090s via 25GbE](https://www.reddit.com/r/LocalLLaMA/comments/1v8hli2/a_user_has_managed_to_run_kimi_k3_on_80xrtx_5090/) ⭐️ 8.0/10

A user successfully deployed the 2.8 trillion parameter Kimi K3 model across 80 RTX 5090 GPUs interconnected with 25 Gigabit Ethernet, demonstrating a practical distributed inference setup using consumer hardware. This achievement proves that large-scale LLM inference can be accomplished with widely available consumer GPUs and standard networking, potentially lowering the barrier for organizations to run massive models without expensive proprietary interconnects. The setup uses 80 RTX 5090 GPUs (each with 32 GB VRAM) connected via 25GbE Ethernet, which is significantly slower than NVLink's 600 GB/s but still sufficient for inference. The Kimi K3 model has 2.8 trillion parameters and supports up to 1M token context.

reddit · r/LocalLLaMA · /u/panchovix · Jul 27, 23:56

**Background**: Kimi K3 is an open-source large language model with 2.8 trillion parameters, making it one of the largest publicly available models. Distributed inference splits the model across multiple GPUs, requiring high-bandwidth communication; NVLink offers 600 GB/s, while 25GbE provides about 3.125 GB/s. Consumer GPUs like the RTX 5090 lack NVLink, so users rely on Ethernet for multi-GPU setups.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3/tree/main">moonshotai/ Kimi - K 3 at main</a></li>
<li><a href="https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5090/">NVIDIA GeForce RTX 5090 Graphics Cards</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#distributed inference`, `#hardware`, `#networking`, `#Kimi K3`

---

<a id="item-12"></a>
## [Case Study: Replacing React with HTMX in a Forum Platform](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 7.0/10

The Misago forum project removed React.js from its codebase and adopted HTMX for UI interactivity, sharing a detailed case study of the migration in 2023. This real-world migration demonstrates HTMX's viability for server-rendered interactivity, potentially reducing complexity and code size compared to heavy client-side frameworks like React. HTMX extends HTML with custom attributes to enable AJAX, WebSockets, and Server-Sent Events directly, without writing JavaScript. The library is small (~14k min.gz'd) and has been shown to reduce code base sizes by 67% compared to React.

hackernews · Ralfp · Jul 27, 09:58 · [Discussion](https://news.ycombinator.com/item?id=49067301)

**Background**: HTMX is an open-source JavaScript library created by Carson Gross that allows developers to build dynamic web interfaces using hypertext (HTML) rather than heavy client-side frameworks. It follows a hypermedia-driven approach, where server responses (usually HTML fragments) are inserted into the page without full reloads, enabling SPA-like behavior with minimal JavaScript.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>

</ul>
</details>

**Discussion**: Community members generally praised the move, with many sharing positive experiences using HTMX for server-rendered apps. Some noted that HTMX works well for content-heavy sites like forums, while others suggested combining it with small Vue/React components for highly interactive features. A few users reported performance issues with complex filter forms, but overall sentiment was supportive.

**Tags**: `#HTMX`, `#React`, `#web development`, `#server-side rendering`, `#case study`

---

<a id="item-13"></a>
## [Paged Out #9: Free Technical Magazine Released](https://pagedout.institute/download/PagedOut_009.pdf) ⭐️ 7.0/10

Paged Out #9, a free PDF technical magazine covering low-level programming, retro computing, and hacker culture, has been released with community praise for its depth and design. This magazine fills a niche for deeply technical, hacker-curious content reminiscent of classic zines like Phrack and 2600, fostering community knowledge sharing. The issue includes articles such as 'Baby Steps in C' and 'The Subpixel Zoo', and a print edition is available for purchase via Lulu.

hackernews · laurensr · Jul 27, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49070138)

**Background**: Paged Out is a free, community-driven technical magazine that publishes articles on low-level programming, security, retro computing, and other hacker-curious topics. It is distributed as a PDF and also offers print-on-demand editions.

**Discussion**: Commenters praised the magazine's depth and design, comparing it to Phrack and 2600. Specific articles like 'Baby Steps in C' and 'The Subpixel Zoo' were highlighted, and readers expressed interest in purchasing print editions.

**Tags**: `#hacker culture`, `#technical magazine`, `#low-level programming`, `#retro computing`, `#zine`

---

<a id="item-14"></a>
## [FeyNoBg: Open-Source Background Removal Model and Library](https://usefeyn.com/blog/feynobg/) ⭐️ 7.0/10

Feyn released FeyNoBg, a state-of-the-art background removal model, and open-sourced the NoBg Python library used to train it, available on Hugging Face and GitHub. This provides developers with a high-quality, customizable background removal tool that outperforms existing models on multiple benchmarks, while the accompanying library simplifies training and deployment. FeyNoBg extends BiRefNet by expanding its third feature extractor stage from 18 to 24 blocks, increasing parameters from 222M to 263M, and achieves best published scores on four of eight benchmarks.

hackernews · snyy · Jul 27, 16:59 · [Discussion](https://news.ycombinator.com/item?id=49072462)

**Background**: Background removal, or image matting, involves separating a subject from its background by estimating foreground opacity per pixel. It is a common AI task used in photo editing, e-commerce, and video conferencing, but remains challenging due to fine details like hair or motion blur.

<details><summary>References</summary>
<ul>
<li><a href="https://usefeyn.com/blog/feynobg/">FeyNoBg: A SOTA Model For Background Removal | Feyn</a></li>
<li><a href="https://github.com/feyninc/nobg">GitHub - feyninc/ nobg : a library for image and video matting · GitHub</a></li>
<li><a href="https://huggingface.co/spaces/feyninc/feynobg">Feynobg - a Hugging Face Space by feyninc</a></li>

</ul>
</details>

**Discussion**: Community comments were positive overall, praising the tool's utility and maturity. Some users raised concerns about the CC-BY-NC-4.0 license for a model derived from MIT-licensed BiRefNet, and others inquired about resolution limits and comparisons with Adobe's solution.

**Tags**: `#background removal`, `#open-source`, `#computer vision`, `#machine learning`, `#Python library`

---

<a id="item-15"></a>
## [Libsm64: Super Mario 64 as a Reusable Library for Game Engines](https://github.com/libsm64/libsm64) ⭐️ 7.0/10

Libsm64 is an open-source library that extracts the movement and rendering code from Super Mario 64, allowing developers to embed Mario into external game engines. Community projects have demonstrated Mario in Half-Life 2 and other games. This project showcases creative reuse of classic game code, enabling novel cross-game interactions without proprietary middleware. It highlights the potential of decompilation and open-source efforts to extend the lifespan of retro games. The library is built on the Super Mario 64 decompilation project, providing a clean C API for integrating Mario's character into other engines. It is not a standalone game but a component for developers to incorporate into their own projects.

hackernews · klaussilveira · Jul 27, 10:04 · [Discussion](https://news.ycombinator.com/item?id=49067352)

**Background**: Super Mario 64 was originally released in 1996 for the Nintendo 64. The sm64 decompilation project reverse-engineered the game's source code from the original binary, enabling ports to other platforms. Libsm64 takes this further by packaging the character logic as a reusable library.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm64/libsm64: Mario 64 as a library for use in ...</a></li>
<li><a href="https://github.com/n64decomp/sm64">GitHub - n64decomp/sm64: A Super Mario 64 decompilation ...</a></li>

</ul>
</details>

**Discussion**: Community members expressed excitement and nostalgia, with some calling it a realization of the metaverse concept without blockchain hype. Others shared demo videos and links to awesome-libsm64, a curated list of projects using the library.

**Tags**: `#game development`, `#reverse engineering`, `#library`, `#retro gaming`, `#open source`

---

<a id="item-16"></a>
## [Ethan Mollick's AI Guide Shifts from Chat to Agentic Systems](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 7.0/10

Ethan Mollick released an updated version of his opinionated guide to which AI to use, shifting focus from chat-based models to agentic systems that can perform hours of autonomous work. Notably, Google's Gemini is omitted because it lacks a mature entry in the Codex/ChatGPT Work/Cowork category. This guide reflects a major industry shift from conversational AI to autonomous agents, helping users navigate the confusing landscape of AI tools. It provides practical advice on using agentic modes like ChatGPT Work and Claude Cowork, which are becoming essential for productivity. The guide explains that ChatGPT Work and Claude Cowork allow AI to access a user's computer for autonomous tasks, while ChatGPT Codex and Claude Code are dedicated to software development. The naming conventions are confusing, as Work and Cowork modes on mobile differ from those on desktop apps.

rss · Simon Willison · Jul 27, 21:55

**Background**: Agentic AI refers to systems that can pursue goals through their own actions, rather than just producing output for humans to act on. Unlike traditional chatbots that require step-by-step instructions, agentic AI can observe, reason, learn, and make decisions independently. Major AI companies like OpenAI and Anthropic now offer agentic modes that can use tools, browse the web, and control computers.

<details><summary>References</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex">ChatGPT Work and Codex - OpenAI Help Center</a></li>
<li><a href="https://agentic.ai/what-is-agentic-ai">What Is Agentic AI? Definition, 6 Levels & Examples (2026)</a></li>

</ul>
</details>

**Discussion**: Simon Willison's commentary highlights the confusing naming conventions between ChatGPT Work and Codex, noting that the mobile and desktop versions behave differently. The discussion likely includes agreements on the practical value of agentic systems and frustrations with Google's lag in this category.

**Tags**: `#AI`, `#agentic systems`, `#LLMs`, `#practical guide`

---

<a id="item-17"></a>
## [Ninfer Achieves 700 t/s on Qwen 3.6 35B with RTX 5090](https://www.reddit.com/r/LocalLLaMA/comments/1v8a7wb/nifer_is_insane_700ts_with_qwen_36_35b_no/) ⭐️ 7.0/10

A new inference engine called Ninfer achieves 550-720 tokens per second on the Qwen 3.6 35B model using a single RTX 5090 GPU, with full 250k context support. This performance rivals Cerebras wafer-scale inference speeds. This breakthrough dramatically lowers the hardware barrier for high-speed local LLM inference, previously only achievable with expensive cloud or specialized hardware. It enables real-time, single-instance inference on consumer hardware, potentially accelerating local AI applications. Ninfer is a from-scratch C++/CUDA engine optimized exclusively for RTX 5090 and only supports Qwen 3.6 27B and 35B models. It runs text, image, and video prompts via CLI or OpenAI/Anthropic-compatible APIs.

reddit · r/LocalLLaMA · /u/BringTea_666 · Jul 27, 19:17

**Background**: Local LLM inference typically achieves tens to low hundreds of tokens per second on consumer GPUs. Cerebras offers 3,000+ t/s but requires specialized wafer-scale hardware. Ninfer's 700 t/s on a single RTX 5090 represents a significant leap for local inference.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Neroued/ninfer">GitHub - Neroued/ninfer: High-performance single-GPU ...</a></li>
<li><a href="https://www.cerebras.ai/inference">Inference - Cerebras</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-35B-A3B">Qwen/Qwen3.6-35B-A3B · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#RTX 5090`, `#performance`, `#local LLM`, `#Qwen`

---