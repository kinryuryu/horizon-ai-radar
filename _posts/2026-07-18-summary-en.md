---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 45 items, 19 important content pieces were selected

---

1. [Firefox Compiled to WebAssembly Runs Inside Another Browser](#item-1) ⭐️ 9.0/10
2. [Kimi K3 2.8T-A50B: Largest Open Model, Opus 4.8-Class at Sonnet Pricing](#item-2) ⭐️ 9.0/10
3. [Anthropic SDK Python v0.117.0 Adds Dreaming and MCP Tunnels](#item-3) ⭐️ 8.0/10
4. [JWST Confirms First Atmosphere on Rocky Exoplanet LHS 1140b](#item-4) ⭐️ 8.0/10
5. [Open Source AI Overtakes Closed Models](#item-5) ⭐️ 8.0/10
6. [FAA Restores Boeing's Self-Certification Authority for 737 MAX, 787](#item-6) ⭐️ 8.0/10
7. [DeepMind & Isomorphic Labs Unveil Bioresilience AI Approach](#item-7) ⭐️ 8.0/10
8. [Thinking Machines Lab Releases Inkling, a 975B Open-Weights Model](#item-8) ⭐️ 8.0/10
9. [Linus Torvalds Declares Linux Not Anti-AI](#item-9) ⭐️ 8.0/10
10. [Lila Sciences: Future Lab as Data Center](#item-10) ⭐️ 8.0/10
11. [Newer AI Models Keep Performance Edge](#item-11) ⭐️ 8.0/10
12. [White House Launches Gold Eagle to Control Frontier AI Access](#item-12) ⭐️ 8.0/10
13. [GPT-5.6 Sol beats Mythos 5 on AISI cyber challenge](#item-13) ⭐️ 8.0/10
14. [Kaiser Nurses: AI and Surveillance Harm Patient Care](#item-14) ⭐️ 7.0/10
15. [Practical SQLite Tips: Backups and .expert Mode](#item-15) ⭐️ 7.0/10
16. [Texas Court Orders Domain Suspension for Porn Site Over Age-Verification Law](#item-16) ⭐️ 7.0/10
17. [GPT-5.6 Codex Bug Can Delete $HOME Directory](#item-17) ⭐️ 7.0/10
18. [NVIDIA NeMo Automodel Integrates with Hugging Face Diffusers](#item-18) ⭐️ 7.0/10
19. [Google Gemini 3.5 Pro Delayed Over Coding Issues](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Firefox Compiled to WebAssembly Runs Inside Another Browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter has compiled the full Firefox browser (Gecko engine) to WebAssembly, enabling it to run entirely inside another browser tab. The project used an estimated $25,000 in Claude Opus and Fable tokens, leveraging a Claude Max subscription to reduce actual costs. This demonstrates a groundbreaking technical achievement in browser engineering, showing that a full browser can be sandboxed within another browser via WebAssembly, with potential applications in browser isolation, security testing, and web-based virtual environments. It also highlights the growing role of AI-assisted development in complex software projects. The demo uses the Wisp protocol to proxy all network traffic through Puter's server, as WebAssembly code in browsers cannot open arbitrary network connections. The project chose Firefox/Gecko for its strong single-process support, and the team had to scale up servers to handle traffic from Hacker News attention.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (Wasm) is a low-level binary instruction format that allows code written in multiple languages to run in web browsers at near-native speed. Compiling a full browser like Firefox to Wasm is extremely challenging due to the complexity of browser engines, which typically require multiple processes and direct access to system resources. Puter's approach leverages Firefox's single-process mode and uses AI-assisted development to overcome engineering hurdles.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.puter.com/labs/firefox-wasm/">Firefox in WebAssembly - developer.puter.com</a></li>
<li><a href="https://github.com/HeyPuter/firefox-wasm">HeyPuter/firefox-wasm: Firefox in WebAssembly - GitHub</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion expressed widespread amazement at the technical feat, with many praising the clever use of AI tools. Some commenters raised concerns about the cost of proxying all traffic through Puter's server and the potential for abuse, while others discussed the implications for browser isolation and web-based computing.

**Tags**: `#WebAssembly`, `#Firefox`, `#browser engineering`, `#AI-assisted development`, `#web platform`

---

<a id="item-2"></a>
## [Kimi K3 2.8T-A50B: Largest Open Model, Opus 4.8-Class at Sonnet Pricing](https://www.latent.space/p/ainews-kimi-k3-28t-a50b-the-largest) ⭐️ 9.0/10

Moonshot AI released Kimi K3, a 2.8 trillion parameter open-weight model, claiming it is the largest open model ever and achieves performance comparable to Claude Opus 4.8 at pricing similar to Claude Sonnet 5. Open weights are promised by July 27, 2026. This marks a major milestone in open-source AI, as Kimi K3 surpasses DeepSeek's 1.6T model in size and rivals top proprietary models in performance. Its competitive pricing could democratize access to frontier-level AI capabilities. Kimi K3 uses a Stable LatentMoE architecture and is available via API at $3/M input tokens and $15/M output tokens. It leads the Frontend Code arena on Arena.ai, surpassing even Claude Fable 5, and uses 21% fewer output tokens than its predecessor K2.6.

rss · Latent Space · Jul 17, 01:46

**Background**: Open-weight models allow developers to download and fine-tune the model weights, fostering transparency and customization. Moonshot AI is a Beijing-based AI lab known for its Kimi series of large language models. The model's size (2.8T parameters) is more than double that of the previous largest open model, DeepSeek V4 Pro (1.6T).

<details><summary>References</summary>
<ul>
<li><a href="https://www.latent.space/p/ainews-kimi-k3-28t-a50b-the-largest">[AINews] Kimi K3 2.8T-A50B: the largest open model ever ...</a></li>
<li><a href="https://www.aimadetools.com/blog/kimi-k3-complete-guide/">Kimi K3 Complete Guide: Moonshot's 2.8T Open-Weight Frontier ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments highlight skepticism about the 'pelican on a bicycle' test, noting that such images may be in the training set. Others propose more rigorous benchmarks like SWE-bench with interruptions, and one user points out that Kimi K3's tokenizer may include a hidden 85-token system prompt.

**Tags**: `#open-source`, `#large language model`, `#AI breakthrough`, `#Kimi K3`

---

<a id="item-3"></a>
## [Anthropic SDK Python v0.117.0 Adds Dreaming and MCP Tunnels](https://github.com/anthropics/anthropic-sdk-python/releases/tag/v0.117.0) ⭐️ 8.0/10

Anthropic released version 0.117.0 of its Python SDK on July 16, 2026, adding support for the 'dreaming' feature and MCP Tunnels, along with a security fix for credential exposure using SecretStr. The 'dreaming' feature addresses memory rot in long-running Claude agents, improving reliability for enterprise deployments, while MCP Tunnels enable secure connections to private infrastructure without exposing ports, simplifying agent integration. The 'dreaming' feature is designed to combat memory degradation in persistent AI agents, and MCP Tunnels are currently in research preview, allowing agents to reach outward to private servers without VPN or IP allowlisting.

github · stainless-app[bot] · Jul 16, 19:36

**Background**: Anthropic's Python SDK is the official library for interacting with Claude models. 'Dreaming' is a mechanism that helps long-running agents maintain context by periodically refreshing or consolidating memory. MCP (Model Context Protocol) Tunnels provide a secure transport layer for connecting agents to private data sources or services.

<details><summary>References</summary>
<ul>
<li><a href="https://www.devdigest.org/articles/stop-anthropomorphizing-ai-dreaming-features-mislead-developers">Stop Anthropomorphizing AI: ' Dreaming ' Features Mislead... | Devdigest</a></li>
<li><a href="https://stacklok.com/solutions/deploy-anthropic-mcp-tunnels/">Deploy Anthropic MCP Tunnels | Stacklok</a></li>
<li><a href="https://www.infoq.com/news/2026/05/claude-mcp-tunnels/">Anthropic Introduces MCP Tunnels for Private Agent Access... - InfoQ</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#SDK`, `#Python`, `#API`, `#MCP`

---

<a id="item-4"></a>
## [JWST Confirms First Atmosphere on Rocky Exoplanet LHS 1140b](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

The James Webb Space Telescope (JWST) has confirmed the first atmosphere on a rocky exoplanet, LHS 1140b, located 48 light-years away in the habitable zone of a red dwarf star. This rules out the possibility that it is a mini-Neptune. This is the first confirmed atmosphere on a rocky planet in a habitable zone, a major milestone in the search for potentially habitable worlds. It demonstrates JWST's capability to characterize Earth-like exoplanet atmospheres. LHS 1140b is a super-Earth about 5.6 times Earth's mass and 70% larger in radius, with a density suggesting it may be an ocean world. JWST's emission spectroscopy during a secondary eclipse ruled out a thick hydrogen-helium atmosphere typical of mini-Neptunes.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: Exoplanets in the habitable zone are at distances from their star where liquid water could exist on the surface. Red dwarfs are cooler and smaller than the Sun, making their habitable zones much closer, which often leads to tidal locking and intense stellar activity that can strip atmospheres. LHS 1140b was discovered in 2017 and initially thought to be a rocky planet, but its true nature was debated until JWST observations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - NASA Science</a></li>
<li><a href="https://www.bbc.com/news/articles/cy4kdd1e0ejo">First atmosphere found around Earth-like planet LHS 1140b</a></li>

</ul>
</details>

**Discussion**: Commenters debated whether LHS 1140b is truly Earth-like, with some noting red dwarfs' instability and potential for atmospheric stripping. Others discussed propulsion methods for future probes and the Fermi paradox, suggesting that the short window of technological civilization reduces the probability of contact.

**Tags**: `#exoplanets`, `#JWST`, `#astronomy`, `#habitable zone`, `#atmosphere`

---

<a id="item-5"></a>
## [Open Source AI Overtakes Closed Models](https://stateofopensource.ai/) ⭐️ 8.0/10

Mozilla's report 'The State of Open Source AI' reveals that open source AI models have overtaken closed models in market share, with OpenRouter data showing open models now hold 63% of token volume, up from 40% four months ago. This shift threatens the business models of closed AI providers like OpenAI and Anthropic, as hyperscalers and device makers can deploy open models without licensing fees, potentially rendering frontier models a costly liability. Open models processed 4.19 trillion tokens on March 19, up from 888 billion four months earlier—a nearly 5x increase. The report's presentation style has been criticized as LLM-generated and difficult to follow.

hackernews · rellem · Jul 17, 14:31 · [Discussion](https://news.ycombinator.com/item?id=48947825)

**Background**: Open source AI models are publicly available with permissive licenses, allowing anyone to use, modify, and deploy them. Closed models, like those from OpenAI and Anthropic, are proprietary and typically accessed via API with usage fees. The shift in market share indicates growing preference for open models due to cost and flexibility.

**Discussion**: Commenters debate whether open models will kill closed AI companies, with data showing rapid growth. Some criticize the report's quality as LLM-generated and hard to parse, while others express support for open models but want more serious analysis.

**Tags**: `#open source`, `#AI`, `#market analysis`, `#LLMs`

---

<a id="item-6"></a>
## [FAA Restores Boeing's Self-Certification Authority for 737 MAX, 787](https://www.cnbc.com/2026/07/17/faa-boeing-737-max-787.html) ⭐️ 8.0/10

The FAA announced on July 17, 2026, that Boeing can once again issue airworthiness certificates for its 737 MAX and 787 Dreamliner aircraft, an authority stripped after the 2018 and 2019 fatal crashes of the 737 MAX. This regulatory shift marks a significant vote of confidence in Boeing's safety improvements, but it also reignites debate over whether the company can be trusted to self-certify after past failures. The decision affects the certification process for two of Boeing's most important commercial aircraft models. The FAA had also revoked Boeing's self-certification authority for the 787 in 2022 due to production quality issues. The restoration follows several successful FAA-led certifications and what inspectors saw as real process improvements at Boeing.

hackernews · hmm37 · Jul 17, 21:22 · [Discussion](https://news.ycombinator.com/item?id=48952439)

**Background**: An airworthiness certificate is a formal document issued by a national aviation authority (like the FAA) that permits an aircraft to operate commercially. After the 737 MAX crashes, the FAA revoked Boeing's delegated authority to self-certify airworthiness, requiring FAA inspectors to directly approve each aircraft. Self-certification allows manufacturers to issue these certificates themselves under FAA oversight, a common practice in the industry.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news4jax.com/business/2026/07/17/faa-will-allow-boeing-to-resume-certifying-its-planes-are-airworthy-after-years-of-safety-efforts/">FAA says Boeing can resume self - certifying its jets as airworthy</a></li>
<li><a href="https://aviationa2z.com/index.php/2026/07/18/faa-restores-boeing-authority-to-self-certify-new-737-max-and-787-jets/">FAA Restores Boeing Authority to Self - Certify New... - Aviation A2Z</a></li>
<li><a href="https://www.faa.gov/aircraft/air_cert/aw_cert">Airworthiness Certification of Aircraft | Federal Aviation ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed confusion over the difference between airworthiness certificates and type certificates, with some noting that the 737 has undergone many recertifications and now differs greatly from the original 1960s design. Others voiced distrust, stating they would never trust a company kept alive by the US government with their lives.

**Tags**: `#aviation`, `#safety`, `#regulation`, `#Boeing`, `#FAA`

---

<a id="item-7"></a>
## [DeepMind & Isomorphic Labs Unveil Bioresilience AI Approach](https://deepmind.google/blog/our-approach-to-bioresilience/) ⭐️ 8.0/10

Google DeepMind and Isomorphic Labs have publicly shared their joint approach to bioresilience, leveraging AI models to enhance prevention, detection, and response to biological threats. This initiative signals a major step in applying frontier AI to biosecurity, potentially transforming pandemic preparedness and reducing risks from biological misuse. It positions DeepMind and Isomorphic Labs at the forefront of responsible AI development in biology. The approach focuses on using AI models to support three pillars: prevention, detection, and response. It builds on DeepMind's AlphaFold technology and Isomorphic Labs' drug discovery expertise.

rss · Google DeepMind Blog · Jul 16, 09:30

**Background**: Bioresilience refers to the ability of biological systems—from individuals to ecosystems—to adapt to change and withstand threats. Google DeepMind is a leading AI research lab, and Isomorphic Labs is its spin-off focused on AI-driven drug discovery. This announcement comes amid growing concerns about AI misuse in biology and the need for proactive biosecurity measures.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/our-approach-to-bioresilience/">Google DeepMind and Isomorphic Labs approach to bioresilience</a></li>
<li><a href="https://www.artificialintelligence-news.com/news/examining-google-deepmind-ai-bioresilience-push/">Examining Google DeepMind's AI bioresilience push</a></li>
<li><a href="https://www.axios.com/2026/07/16/google-deepmind-biosecurity-safety">Google DeepMind expands biosecurity effort amid AI safety push</a></li>

</ul>
</details>

**Tags**: `#AI`, `#bioresilience`, `#DeepMind`, `#Isomorphic Labs`, `#biology`

---

<a id="item-8"></a>
## [Thinking Machines Lab Releases Inkling, a 975B Open-Weights Model](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, an open-weights Mixture-of-Experts multimodal model with 975B total parameters (41B active), trained on 45 trillion tokens of text, images, audio, and video, under the Apache-2.0 license. This release strengthens the US open-weights ecosystem with a competitive alternative to Chinese open models, offering a strong base for fine-tuning via the Tinker platform. However, sparse documentation on training data may limit reproducibility and trust. Inkling is not a frontier model but a strong base model for customization, with a smaller 276B (12B active) variant called Inkling-Small still under testing. The model card and training data documentation are notably brief, lacking detailed dataset information.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) models use multiple specialized sub-networks (experts) within transformer layers, activating only a subset per input to improve efficiency. Open-weights models release trained parameters but not necessarily training data or code, unlike fully open-source models. Apache-2.0 is a permissive license allowing broad use, including commercial applications.

<details><summary>References</summary>
<ul>
<li><a href="https://machinelearningmastery.com/mixture-of-experts-architecture-in-transformer-models/">Mixture of Experts Architecture in Transformer Models</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://neysa.ai/blog/open-weights-open-source/">Open Weights vs Open Source : What’s the Real Difference?</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#model release`

---

<a id="item-9"></a>
## [Linus Torvalds Declares Linux Not Anti-AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds, the creator and top maintainer of Linux, stated on the Linux Media mailing list that Linux is not an anti-AI project and that AI is a clearly useful tool, inviting dissenters to fork or leave. This definitive statement from the highest authority in the Linux kernel project signals a strong endorsement of AI tools within the open-source community, potentially influencing project direction and community norms. Torvalds emphasized that AI's usefulness is no longer in question, though he acknowledged other open questions about AI's economic impact. The statement was made in response to community pushback against AI use in kernel development.

rss · Simon Willison · Jul 16, 13:26

**Background**: The Linux kernel is a massive open-source project with a large community of contributors. Recently, some developers have expressed concerns about the use of AI tools in kernel development, citing issues like code quality and licensing. Torvalds' statement clarifies his stance and sets a clear direction for the project.

**Tags**: `#Linux`, `#AI`, `#Linus Torvalds`, `#open source`, `#kernel`

---

<a id="item-10"></a>
## [Lila Sciences: Future Lab as Data Center](https://www.latent.space/p/the-lab-of-the-future-should-feel) ⭐️ 8.0/10

Lila Sciences envisions the future laboratory as a data center, using AI and robotics to turn scientific experimentation into a source of training data for AI models. This vision could transform scientific discovery by automating and scaling experimentation, potentially accelerating breakthroughs in medicine, materials, and sustainability. Lila aims to build the world's first scientific superintelligence platform and autonomous labs for life, chemical, and materials sciences, using AI to design, conduct, observe, and redesign experiments.

rss · Latent Space · Jul 16, 13:30

**Background**: Traditional labs rely on manual experimentation, which is slow and limited in scale. Lila Sciences proposes treating lab workflows like data center operations, where robots and AI handle repetitive tasks and data collection, freeing scientists to focus on high-level analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lila.ai/">LILA | Scientific Superintelligence</a></li>
<li><a href="https://www.lila.ai/about">About | LILA | The World's First Operating System for Science</a></li>

</ul>
</details>

**Tags**: `#AI in Science`, `#Robotics`, `#Data Centers`, `#Scientific Discovery`, `#Lab Automation`

---

<a id="item-11"></a>
## [Newer AI Models Keep Performance Edge](https://huggingface.co/blog/Dharma-AI/newer-models-same-advantages) ⭐️ 8.0/10

A blog post on Hugging Face analyzes how newer AI models consistently outperform their predecessors, identifying key factors such as improved architectures, larger datasets, and better training techniques. This analysis helps practitioners understand the drivers of AI progress, guiding model selection and investment in research directions that yield the greatest performance gains. The article examines multiple model families across tasks like language modeling and image classification, showing consistent advantage patterns despite varying domains.

rss · Hugging Face Blog · Jul 16, 11:49

**Background**: In AI/ML, newer models often claim better performance, but quantifying and explaining these gains is crucial for informed decision-making. Factors like scaling laws, architectural innovations, and data quality play key roles.

**Tags**: `#AI`, `#machine learning`, `#model comparison`, `#deep learning`

---

<a id="item-12"></a>
## [White House Launches Gold Eagle to Control Frontier AI Access](https://www.reddit.com/r/singularity/comments/1uzfor4/white_house_launches_gold_eagle_moving_to_control/) ⭐️ 8.0/10

The Trump administration has launched 'Gold Eagle,' a program that requires government approval for companies and organizations to access new frontier AI models, shifting control from AI developers like OpenAI and Anthropic to the state. This marks a significant shift in AI governance, potentially setting a precedent for government oversight of advanced AI capabilities, affecting national security, innovation, and global AI competition. According to CNBC, future partner rollouts under Gold Eagle will require explicit government approval, though the White House states AI companies still control whether to release their models and are not required to participate in government testing or meetings.

reddit · r/singularity · /u/Outside-Iron-8242 · Jul 17, 23:29

**Background**: Frontier AI models are the most advanced AI systems, trained on massive datasets to perform a wide variety of tasks at state-of-the-art levels. Gold Eagle, initially launched as an AI-driven cybersecurity initiative under Executive Order 14409, is now being expanded to regulate access to these powerful models, raising questions about balancing security with innovation.

<details><summary>References</summary>
<ul>
<li><a href="https://cryptobriefing.com/white-house-gold-eagle-ai-vulnerability-initiative/">White House launches AI -driven Gold Eagle cybersecurity initiative...</a></li>
<li><a href="https://www.androidheadlines.com/2026/07/white-house-launches-gold-eagle-ai-cybersecurity-clearinghouse.html">White House Launches Gold Eagle AI Cybersecurity Program</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work - NVIDIA</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion shows mixed reactions: some users support the move for national security reasons, while others fear it could stifle innovation and lead to government overreach. A few commenters question the effectiveness of such regulation given the global nature of AI development.

**Tags**: `#AI regulation`, `#frontier AI`, `#government policy`, `#national security`

---

<a id="item-13"></a>
## [GPT-5.6 Sol beats Mythos 5 on AISI cyber challenge](https://www.reddit.com/r/singularity/comments/1uz91nn/gpt56_sol_outperforms_mythos_5_on_aisis_cyber/) ⭐️ 8.0/10

GPT-5.6 Sol outperformed Mythos 5 on AISI's cyber challenge, and open-weight models are now only 4-7 months behind closed models, narrowing from 6-10 months in 2025. This marks a significant narrowing of the capability gap between open-weight and closed-source frontier models, which could accelerate AI safety research and democratize access to advanced cyber capabilities. AISI also added GLM 5.2 and DeepSeek V4 Pro to the benchmark, but has not yet tested K3, which could further change the gap. The evaluation involves a 32-step cyber range completed end-to-end.

reddit · r/singularity · /u/Outside-Iron-8242 · Jul 17, 19:07

**Background**: The AISI cyber challenge is a benchmark designed to evaluate AI models' ability to autonomously perform cybersecurity tasks, such as penetration testing and vulnerability exploitation. Frontier models are the most advanced AI systems, often costing hundreds of millions to train. Open-weight models release their trained parameters but not the full training pipeline, allowing broader use while keeping some control.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aisi.gov.uk/blog/our-evaluation-of-claude-mythos-previews-cyber-capabilities">Our evaluation of Claude Mythos Preview’s cyber ... | AISI Work</a></li>
<li><a href="https://winbuzzer.com/2026/05/14/openais-gpt-55-matches-claude-mythos-in-security-tests-xcxwbn/">Claude Mythos Leads GPT-5.5 in AISI Cyber Range Tests</a></li>
<li><a href="https://huggingface.co/blog/daya-shankar/open-source-llm-models-to-run-locally">The Best Open Source and Open-Weight LLM Models to Run ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion highlights excitement about the shrinking gap between open and closed models, with some users noting that open-weight models are catching up faster than expected. Others debate the implications for AI safety and whether closed models still hold a meaningful lead.

**Tags**: `#AI`, `#benchmarking`, `#cybersecurity`, `#open-source`, `#frontier models`

---

<a id="item-14"></a>
## [Kaiser Nurses: AI and Surveillance Harm Patient Care](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

Kaiser Permanente nurses report that AI tools and workplace surveillance are worsening patient care and job satisfaction, citing a 2024 pilot of an AI empathy-assessment tool and pressure from call-center metrics. This highlights the tension between AI adoption and worker well-being in healthcare, potentially influencing how hospitals deploy AI and surveillance systems. The AI empathy tool was a 2024 pilot that has since been discontinued, but nurses remain concerned about metric-driven pressure to ration care and constant location tracking.

hackernews · gnabgib · Jul 17, 22:26 · [Discussion](https://news.ycombinator.com/item?id=48952880)

**Background**: Kaiser Permanente uses AI tools to improve health outcomes, but nurses argue that surveillance and metrics undermine care quality. The debate reflects broader concerns about AI in healthcare, where tools like note-taking and translation are valued by some clinicians.

<details><summary>References</summary>
<ul>
<li><a href="https://calmatters.org/economy/technology/2026/07/kaiser-nurses-workplace-surveillance-ai/">Kaiser nurses say surveillance of them is undermining healthcare</a></li>
<li><a href="https://about.kaiserpermanente.org/expertise-and-impact/public-policy/our-key-issues/artificial-intelligence">Artificial intelligence - Kaiser Permanente</a></li>
<li><a href="https://www.kpihp.org/wp-content/uploads/2026/03/4359655541_IHP-Brief-on-AI_031026_ADA-1.pdf">How Kaiser Permanente uses artificial intelligence to improve ...</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some criticize the misuse of metrics rather than AI itself, while others share positive experiences with AI note-taking and translation. A rural hospital nurse describes being tracked by location, leading to rushed patient visits.

**Tags**: `#AI in healthcare`, `#workplace surveillance`, `#nursing`, `#Kaiser Permanente`, `#ethics`

---

<a id="item-15"></a>
## [Practical SQLite Tips: Backups and .expert Mode](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 7.0/10

Julia Evans' blog post shares practical tips for running SQLite, including using the .expert mode to automatically recommend indexes and various backup strategies such as piping .dump to zstd compression. These tips help developers and database administrators improve SQLite performance and data safety with minimal effort, addressing common pain points like query optimization and non-blocking backups. The .expert mode analyzes queries and suggests indexes, while backup methods include using .dump with zstd compression and the Online Backup API for live databases.

hackernews · surprisetalk · Jul 17, 17:45 · [Discussion](https://news.ycombinator.com/item?id=48950122)

**Background**: SQLite is a widely used embedded database engine. The .expert mode is a CLI feature that recommends indexes to speed up queries. Backing up SQLite databases can be tricky because writes may block reads; strategies like using WAL mode and the Online Backup API help mitigate this.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/backup.html">SQLite Backup API</a></li>
<li><a href="https://databaseschool.com/series/high-performance-sqlite/videos/41">Where to add indexes - High Performance SQLite - Database School</a></li>

</ul>
</details>

**Discussion**: Commenters shared real-world backup workflows, such as using .dump with zstd and rsyncable flags for efficient incremental syncs, and a tool called s3-credentials to simplify AWS credential management for backups.

**Tags**: `#SQLite`, `#database`, `#backup`, `#performance`, `#tools`

---

<a id="item-16"></a>
## [Texas Court Orders Domain Suspension for Porn Site Over Age-Verification Law](https://www.texasattorneygeneral.gov/news/releases/attorney-general-ken-paxton-secures-landmark-legal-victory-lock-pornographic-website-domain-and) ⭐️ 7.0/10

Texas Attorney General Ken Paxton secured a default judgment ordering the suspension of the domain name motherless.com for violating the state's age-verification law, marking the first such enforcement against a pornographic website. This case sets a precedent for state-level internet censorship, potentially allowing any state to enforce its laws on websites with no physical presence there, raising serious interstate commerce and First Amendment concerns. The judgment was a default ruling because the website operator did not appear in court, so it does not reflect a contested legal analysis. The domain motherless.com is a .com domain registered through Verisign, which is based in Reston, Virginia.

hackernews · letmevoteplease · Jul 17, 22:35 · [Discussion](https://news.ycombinator.com/item?id=48952939)

**Background**: Texas passed a law requiring pornographic websites to implement age verification to prevent minors from accessing explicit content. Critics argue such laws violate the Commerce Clause of the U.S. Constitution, which reserves interstate commerce regulation to the federal government, and may also infringe on free speech protections.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Internet_censorship_in_the_United_States">Internet censorship in the United States - Wikipedia</a></li>
<li><a href="https://www.aclu.org/documents/state-state-internet-censorship-bills">State by State Internet Censorship Bills | American Civil Liberties Union</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong concerns about the precedent, arguing that a state court should not be able to enforce laws against out-of-state entities, and that this could lead to a fragmented internet where each state imposes its own censorship. Some noted that the default judgment is legally weak and may not withstand a contested challenge.

**Tags**: `#internet governance`, `#censorship`, `#domain law`, `#age verification`, `#jurisdiction`

---

<a id="item-17"></a>
## [GPT-5.6 Codex Bug Can Delete $HOME Directory](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 7.0/10

OpenAI has confirmed a bug in GPT-5.6 Codex that can delete the user's $HOME directory when full access mode is enabled without sandboxing or auto-review protections. This bug highlights critical safety risks in AI coding agents, especially for users who grant unrestricted file system access. It underscores the need for proper sandboxing and review mechanisms to prevent irreversible data loss. The bug occurs when the model attempts to override the $HOME environment variable to define a temporary directory, but mistakenly deletes $HOME instead. It most commonly happens with full access mode enabled, no sandboxing, and auto-review disabled.

rss · Simon Willison · Jul 16, 17:45

**Background**: Codex is an AI coding agent from OpenAI that can execute commands on the user's machine. Full access mode gives the model unrestricted write access to the filesystem, while sandboxing and auto-review are safety features that limit or review actions. Without these protections, a mistake by the model can have severe consequences.

<details><summary>References</summary>
<ul>
<li><a href="https://vladimirsiedykh.com/blog/codex-cli-approval-modes-2025">Codex CLI approval modes explained: auto vs read only vs...</a></li>
<li><a href="https://www.vincentschmalbach.com/how-codex-cli-flags-actually-work-full-auto-sandbox-and-bypass/">How Codex CLI Flags Actually Work (Full-Auto, Sandbox, and ...</a></li>
<li><a href="https://learn.chatgpt.com/docs/sandboxing/auto-review">Auto-review | ChatGPT Learn</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-18"></a>
## [NVIDIA NeMo Automodel Integrates with Hugging Face Diffusers](https://huggingface.co/blog/nvidia/scale-diffusers-finetuning-nemo-automodel) ⭐️ 7.0/10

Hugging Face and NVIDIA have announced the integration of NVIDIA NeMo Automodel with the Diffusers library, enabling scalable fine-tuning of video and image diffusion models. This integration allows practitioners to fine-tune large-scale video and image models more efficiently, leveraging NeMo Automodel's distributed training capabilities directly from the Diffusers API. NeMo Automodel is a PyTorch DTensor-native SPMD training library that supports day-0 Hugging Face model compatibility, while Diffusers provides a modular framework for diffusion models.

rss · Hugging Face Blog · Jul 17, 15:57

**Background**: Fine-tuning large diffusion models for custom video and image generation tasks often requires significant computational resources and distributed training expertise. NeMo Automodel simplifies this by providing a scalable, open-source training library with built-in parallelism. Diffusers is a popular library for working with diffusion models, offering pre-built pipelines and components.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/nvidia-nemo/automodel">GitHub - NVIDIA-NeMo/Automodel: 🚀 Pytorch Distributed native training library for LLMs/VLMs with OOTB Hugging Face support</a></li>
<li><a href="https://docs.nvidia.com/nemo/automodel/latest/index.html">NeMo AutoModel Documentation | NVIDIA NeMo AutoModel</a></li>
<li><a href="https://huggingface.co/blog/nvidia/accelerating-fine-tuning-nvidia-nemo-automodel">Accelerating Transformers Fine-Tuning with NVIDIA NeMo AutoModel</a></li>

</ul>
</details>

**Tags**: `#fine-tuning`, `#NVIDIA NeMo`, `#Diffusers`, `#video models`, `#image models`

---

<a id="item-19"></a>
## [Google Gemini 3.5 Pro Delayed Over Coding Issues](https://www.reddit.com/r/singularity/comments/1uzeihc/bloomberg_feat_9to5_gemini_35_pro_delays_due_to/) ⭐️ 7.0/10

Google has delayed the launch of Gemini 3.5 Pro, originally expected in June 2026, due to disappointing coding performance after a training data reset in late June. An upgraded Flash model is reportedly in testing. This delay highlights Google's struggle to compete with OpenAI and Anthropic in AI coding capabilities, a critical area for developer adoption. Internal cultural divides and capacity constraints further complicate Google's AI strategy. The training reset occurred between Google I/O in mid-May and the missed June deadline, indicating a significant setback. Engineers also face capacity constraints when using internal AI coding tools due to competition for computing power.

reddit · r/singularity · /u/kiki-le-koala · Jul 17, 22:40

**Background**: Gemini 3.5 Pro is Google's flagship general-purpose AI model with advanced reasoning, coding, and multimodal capabilities. Google has been working to unify its fragmented internal AI coding tools under a project called Antigravity, but faces internal resistance from engineers who believe important code should be human-written.

<details><summary>References</summary>
<ul>
<li><a href="https://www.neowin.net/news/google-gemini-35-pro-faces-delays-over-coding-performance-misses/">Google Gemini 3.5 Pro faces "delays" over coding performance ...</a></li>
<li><a href="https://9to5google.com/2026/07/16/gemini-3-5-pro-delays/">Gemini 3.5 Pro delays due to coding performance - 9to5Google</a></li>
<li><a href="https://developers.slashdot.org/story/26/04/21/1655253/googles-internal-politics-leave-it-playing-catch-up-on-ai-coding">Google 's Internal Politics Leave It Playing Catch-Up On AI Coding</a></li>

</ul>
</details>

**Tags**: `#Google`, `#Gemini`, `#AI`, `#coding`, `#industry news`

---