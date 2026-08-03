---
layout: default
title: "Horizon Summary: 2026-08-03 (EN)"
date: 2026-08-03
lang: en
---

> From 25 items, 9 important content pieces were selected

---

1. [Kakehashi: Experimental Userspace Runs macOS Binaries on Linux ARM](#item-1) ⭐️ 8.0/10
2. [Open Letters Debate AI Open Weights and Safety](#item-2) ⭐️ 8.0/10
3. [OpenAI's Astra Model Solves Ten Decade-Old Math Problems](#item-3) ⭐️ 8.0/10
4. [Karpathy's Pelican Benchmark Sparks Debate on LLM Physical World Understanding](#item-4) ⭐️ 7.0/10
5. [NixOS-DGX-Spark Brings Nix and NixOS to NVIDIA DGX Spark](#item-5) ⭐️ 7.0/10
6. [F*: A Proof-Oriented Language for Formal Verification](#item-6) ⭐️ 7.0/10
7. [California DROP Data Deletion Requests Become Enforceable Aug. 1](#item-7) ⭐️ 7.0/10
8. [eBay Harassment Campaign Leads to $56M Payout and Prison Sentences](#item-8) ⭐️ 7.0/10
9. [Mathematician Reflects on AI's Impact on Mathematics](#item-9) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Kakehashi: Experimental Userspace Runs macOS Binaries on Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi is an experimental userspace that successfully runs macOS CLI binaries like 7-Zip and curl on Linux ARM. It has working prototypes, with 7-Zip passing multi-threaded compression tests and curl passing over 200 commands and options. This project addresses a significant technical challenge of running macOS binaries on Linux ARM, potentially expanding software compatibility. It could inspire collaboration with existing projects like Darling and pave the way for running macOS applications on Linux ARM devices. Kakehashi currently runs 7-Zip at about 5.2x slower than native Linux execution, but the developer has a clear optimization plan. It also runs Xcode Tools Git with basic version control functionality, and the project is still early-stage.

hackernews · vlad_kalinkin · Aug 2, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49145937)

**Background**: Running macOS binaries on Linux requires translating macOS system calls and libraries to Linux equivalents, which is complex due to differences in kernels and ABIs. Darling is a similar project that provides a compatibility layer for macOS software on Linux, but it lacks full ARM64 support. Kakehashi aims to fill this gap by focusing on CLI binaries and ARM architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Darling_(software)">Darling (software) - Wikipedia</a></li>
<li><a href="https://www.darlinghq.org/">Darling | macOS translation layer for Linux</a></li>
<li><a href="https://en.wikipedia.org/wiki/Application_binary_interface">Application binary interface - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments show strong interest and engagement. Users compare Kakehashi to Darling and suggest potential collaboration, while others question the naming and note the project is still early. The developer responds with details about current progress and future plans.

**Tags**: `#macOS`, `#Linux`, `#ARM`, `#binary compatibility`, `#userspace`

---

<a id="item-2"></a>
## [Open Letters Debate AI Open Weights and Safety](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

Simon Willison summarized recent open letters about AI development, notably Microsoft's 'Open Weights and American AI Leadership' signed by 235 companies, and Anthropic's counter-position, plus 'Pacing the Frontier' signed by 1,324 AI employees. This debate shapes US AI policy on open-weight models, balancing innovation and safety. The outcome affects the entire AI ecosystem, from startups to national security. Microsoft's letter supports distillation, a practice Anthropic wants regulated. Notably, OpenAI signed Microsoft's letter, while Anthropic did not, highlighting industry divisions.

rss · Simon Willison · Aug 2, 04:16

**Background**: Open-weight models release trained neural network parameters, allowing public use and modification. Proponents argue they increase transparency and competition, while critics worry about misuse by malicious actors.

<details><summary>References</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.nytimes.com/2026/07/28/technology/open-weight-ai.html">What Is Open-Weights A.I.? - The New York Times</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open source`, `#policy`, `#open weights`, `#industry`

---

<a id="item-3"></a>
## [OpenAI's Astra Model Solves Ten Decade-Old Math Problems](https://simonwillison.net/2026/Aug/1/ten-advances-in-mathematics/#atom-everything) ⭐️ 8.0/10

OpenAI announced that an internal version of its next major model, Astra, has produced ten new results in mathematics and theoretical computer science, each problem having been open for at least a decade. The company claims each solution cost less than $2,000 at GPT-5.6 Sol token prices. This development signals a potential paradigm shift in mathematical research, where AI can tackle long-standing open problems at low cost. It could accelerate progress in mathematics and theoretical computer science, and may prompt a reevaluation of the role of human mathematicians. OpenAI has released a GitHub repository (openai/ten-proofs) containing Lean 4 formalizations of the results, along with a paper and an LLM-generated PDF that reconstructs the proof process. However, the post notes that there is no information on how many problems were attempted without success, and the prompts used were not disclosed.

rss · Simon Willison · Aug 1, 20:34

**Background**: This news follows a recent trend of AI models making significant contributions to mathematics, such as Anthropic's Claude discovering cryptographic weaknesses. Terence Tao has described a future of 'big mathematics' where humans and AI collaborate on complex tasks, with AI handling technical grunt work. The use of formal proof assistants like Lean 4 is becoming more common in verifying AI-generated proofs.

<details><summary>References</summary>
<ul>
<li><a href="https://the-decoder.com/openai-announces-its-next-major-model-astra-by-dropping-ten-previously-unsolved-math-solutions/">OpenAI announces its "next major model" Astra by dropping ten previously unsolved math solutions</a></li>
<li><a href="https://thenextweb.com/news/openai-astra-model-ten-math-proofs-non-sofic-groups">OpenAI says its next model, Astra, has solved ten open problems in mathematics</a></li>
<li><a href="https://openrouter.ai/openai/gpt-5.6-sol">GPT-5.6 Sol - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (referenced in the post) likely includes a mix of awe and skepticism, with some commenters praising the transparency of releasing formalizations and papers, while others question the lack of information on failed attempts and the undisclosed prompts. The post itself highlights the need for more transparency.

**Tags**: `#AI`, `#mathematics`, `#OpenAI`, `#research`, `#theoretical computer science`

---

<a id="item-4"></a>
## [Karpathy's Pelican Benchmark Sparks Debate on LLM Physical World Understanding](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

Andrej Karpathy tweeted about the 'Pelican' benchmark, which tests LLMs by asking them to generate an SVG of a pelican riding a bicycle. This sparked a high-engagement discussion on Hacker News about using vector graphics generation as a new benchmark for physical world understanding. This benchmark represents a shift from traditional image generation to a more interpretable and code-based evaluation of LLMs' understanding of physical concepts. It could influence how AI models are evaluated and drive progress in spatial reasoning and world modeling. The benchmark was popularized by Simon Willison, who asked models to render an SVG of a pelican on a bicycle. Community members noted that while the output quality is often poor, the benchmark provides a qualitative measure of physical world understanding, and some have experimented with similar prompts using other models and scenes.

hackernews · delichon · Aug 2, 04:05 · [Discussion](https://news.ycombinator.com/item?id=49140998)

**Background**: Vector graphics formats like SVG and TikZ describe images using geometric primitives and coordinates, requiring models to understand spatial relationships and object composition. Traditional benchmarks often focus on text or image generation, but this benchmark tests the model's ability to translate a natural language description into precise, executable code, which is seen as a proxy for physical world understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2024/Oct/25/pelicans-on-a-bicycle/">Pelicans on a bicycle | Simon Willison’s Weblog</a></li>
<li><a href="https://arxiv.org/pdf/2407.10972">VGBench : Evaluating Large Language Models on Vector Graphics</a></li>
<li><a href="https://explainx.ai/blog/are-ai-labs-pelicanmaxxing-study-july-2026">Are AI Labs Pelicanmaxxing? A Statistical Study | explainx.ai</a></li>

</ul>
</details>

**Discussion**: The community discussion was largely positive, with users highlighting the benchmark's value in exposing models' physical understanding. Some shared their own experiments, such as generating 3D animations or interpreting literary scenes, while others noted the lack of reproducibility for Karpathy's specific example. There was also debate about whether the benchmark could be 'gamed' by training on similar prompts, though a statistical study found no significant evidence of that.

**Tags**: `#AI`, `#LLM`, `#benchmark`, `#vector graphics`, `#Karpathy`

---

<a id="item-5"></a>
## [NixOS-DGX-Spark Brings Nix and NixOS to NVIDIA DGX Spark](https://github.com/graham33/nixos-dgx-spark) ⭐️ 7.0/10

A new GitHub project, NixOS-DGX-Spark, provides Nix and NixOS support for the NVIDIA DGX Spark and Asus Ascent GX10, including USB images and a NixOS module. It enables users to run Nix playbooks on DGX OS or install NixOS for a full Nix experience. This project is significant for the NixOS and AI hardware community, as it enables reproducible and declarative system configurations on powerful AI workstations like the DGX Spark. It lowers the barrier for AI developers and DevOps to manage these devices with Nix, aligning with the trend of reproducible infrastructure. The repository provides USB images and a NixOS module with settings specifically for DGX Spark systems. It works on both the NVIDIA DGX Spark and the Asus Ascent GX10, and the author presented a 5-minute lightning talk at Planet Nix.

hackernews · graham33 · Aug 2, 17:05 · [Discussion](https://news.ycombinator.com/item?id=49146267)

**Background**: NixOS is a Linux distribution built on the Nix package manager, which uses a declarative approach to system configuration, making setups reproducible and easy to manage. The NVIDIA DGX Spark is a personal AI supercomputer powered by the GB10 Superchip, designed for local AI workloads. NixOS modules are reusable components that combine to form a full system configuration, allowing users to define options and settings declaratively.

<details><summary>References</summary>
<ul>
<li><a href="https://nixos.wiki/wiki/NixOS_modules">NixOS modules - NixOS Wiki</a></li>
<li><a href="https://www.nvidia.com/en-us/products/workstations/dgx-spark/">Personal AI Supercomputer Powered by Blackwell | NVIDIA DGX Spark</a></li>
<li><a href="https://grokipedia.com/page/ASUS_Ascent_GX10">ASUS Ascent GX10</a></li>

</ul>
</details>

**Discussion**: Community comments are positive, with users reporting successful use on Asus GX10 machines with k3s and DeepSeek, and expressing gratitude for the project. Some also highlight related projects like microvm.nix for sandboxing and Flox for Nix/CUDA in capital markets, indicating broader interest in Nix for AI workflows.

**Tags**: `#NixOS`, `#NVIDIA DGX Spark`, `#AI hardware`, `#reproducible builds`, `#DevOps`

---

<a id="item-6"></a>
## [F*: A Proof-Oriented Language for Formal Verification](https://fstar-lang.org/) ⭐️ 7.0/10

The F* programming language, a general-purpose proof-oriented language developed by Microsoft Research and Inria, is highlighted as a mature tool for formal verification. It supports refinement types, dependent types, and effectful programming, and can translate code to OCaml, F#, C, WebAssembly, or assembly. F* enables developers to write programs with machine-checked proofs of correctness and security properties, which is critical for high-assurance software. Its ability to incrementally migrate existing C codebases makes it practical for real-world adoption in safety-critical industries. F* was introduced in 2011 and is under active development on GitHub. Its type system combines dependent types, monadic effects, and refinement types, and it uses SMT solving and manual proofs for verification. The Steel language, built on F*, enables proof-oriented programming in concurrent separation logic.

hackernews · ducktective · Aug 2, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49143925)

**Background**: Formal verification uses mathematical methods to prove that software meets its specifications, preventing bugs and security vulnerabilities. Refinement types extend standard types with predicates, allowing precise preconditions and postconditions. F* is part of a broader ecosystem of proof-oriented languages that aim to make verification more accessible and practical.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/F*_(programming_language)">F* (programming language)</a></li>
<li><a href="https://fstar-lang.org/">F*: A Proof - Oriented Programming Language</a></li>
<li><a href="https://en.wikipedia.org/wiki/Refinement_type">Refinement type</a></li>

</ul>
</details>

**Discussion**: Community comments show interest in F*'s practical use, such as incremental migration of C codebases, and questions about industry adoption. Some users criticize the homepage for lacking code examples, while others point to the tutorial for more details. Overall sentiment is positive but with suggestions for better presentation.

**Tags**: `#formal verification`, `#programming language`, `#proof-oriented`, `#functional programming`, `#F*`

---

<a id="item-7"></a>
## [California DROP Data Deletion Requests Become Enforceable Aug. 1](https://www.nbcsandiego.com/nbc-7-responds-2/californians-data-deletion-requests-drop-become-enforceable-aug-1/4054771/) ⭐️ 7.0/10

California's new Data Deletion Request (DROP) system becomes enforceable on August 1, allowing residents to request deletion of their personal data from data brokers, with fines for non-compliance. The California Privacy Protection Agency has already fined 12 data brokers tens of thousands of dollars each for failing to register in the DROP system. This marks a significant step in data privacy enforcement, giving Californians a practical tool to control their personal information and setting a precedent for other states. Tech companies and data brokers must now comply or face substantial daily fines, potentially reshaping data handling practices across the industry. Companies that fail to comply can face fines of $200 per day for each affected Californian. The DROP system is tied to individuals, and data brokers must delete data only if they achieve a 100% match in their databases; otherwise, they may continue to hold the data.

hackernews · MilnerRoute · Aug 2, 22:16 · [Discussion](https://news.ycombinator.com/item?id=49148987)

**Background**: The DROP system is part of California's broader privacy framework, including the California Consumer Privacy Act (CCPA) and the Data Broker Law, updated by SB 362 and SB 361. Data brokers are entities that collect and sell personal information, and the new law aims to give consumers more control over their data. Starting January 1, 2028, data brokers must also undergo independent third-party audits every three years to ensure compliance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nbcsandiego.com/nbc-7-responds-2/californians-data-deletion-requests-drop-become-enforceable-aug-1/4054771/">California DROP tool lets residents stop data sales – NBC 7 San Diego</a></li>
<li><a href="https://www.bruceb.com/2026/04/drop-promises-privacy-but-the-river-still-flows/">DROP Promises Privacy But The River Still Flows | Bruceb Consulting</a></li>
<li><a href="https://www.leadgen-economy.com/blog/california-drop-august-1-200-dollars-per-day-data-broker-lead-gen/">California DROP Aug 1: $200/Day per Request Lands</a></li>
<li><a href="https://www.coblentzlaw.com/news/navigating-californias-data-broker-requirements-in-2026/">Navigating California’s Data Broker Requirements in 2026 - Coblentz Law</a></li>
<li><a href="https://cppa.ca.gov/data_brokers/">Information for Data Brokers - California Privacy Protection Agency (CPPA)</a></li>

</ul>
</details>

**Discussion**: Commenters expressed hope that other states adopt similar measures, with one user lamenting spam calls from data brokers. Others raised questions about enforcement for out-of-state companies, potential unintended data deletion (e.g., credit reports), and the possibility of automated deletion request services. Some speculated about technical quirks, like companies using a table named 'drop' to track requests.

**Tags**: `#data privacy`, `#regulation`, `#California`, `#data deletion`, `#compliance`

---

<a id="item-8"></a>
## [eBay Harassment Campaign Leads to $56M Payout and Prison Sentences](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

eBay has agreed to pay $56 million to David and Ina Steiner, a couple targeted by a harassment campaign orchestrated by eBay's security team. Several former eBay security executives, including Jim Baugh, have been sentenced to prison terms for their roles in the campaign. This case highlights the severe consequences of corporate misconduct and the importance of accountability at the highest levels of security operations. It serves as a warning to companies about the legal and financial risks of using unethical tactics to silence critics. The harassment campaign included sending disturbing deliveries, surveillance, and threats to the Steiners, who were critical of eBay on their blog. Jim Baugh, former Senior Director of Safety and Security, received a 57-month prison sentence, while other executives received shorter sentences or fines.

hackernews · JumpCrisscross · Aug 2, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49147435)

**Background**: eBay's security team, which included former police captains, launched the campaign in 2019 to intimidate the Steiners after they published critical articles about the company. The case underscores the potential for corporate security teams to abuse their power when acting without proper oversight.

**Discussion**: Commenters expressed skepticism that the harassment was limited to one couple, suggesting other critics may have been targeted. Some also noted the broader implications for corporate accountability and the behavior of former law enforcement officials in private security roles.

**Tags**: `#corporate accountability`, `#legal`, `#security`, `#ethics`, `#eBay`

---

<a id="item-9"></a>
## [Mathematician Reflects on AI's Impact on Mathematics](https://www.reddit.com/r/singularity/comments/1vd9snp/mathematician_reflects_on_the_impact_of_recent_ai/) ⭐️ 7.0/10

A mathematician, Kirwin Hampshire, published a reflective piece titled 'The Dark Night of Mathematics' discussing the recent progress of AI and its implications for the field of mathematics, which was shared on Reddit's r/singularity community. This reflection is significant because it offers a domain expert's perspective on how AI advancements, particularly in verifiable domains like formalized mathematics, might reshape the discipline, potentially affecting mathematicians' roles and the nature of mathematical research. The article likely discusses the argument that AI progress in verifiable domains like formalized mathematics and coding may outpace progress in intuitive or unformalizable domains, as noted in the search results. It also touches on the broader implications for the singularity community.

reddit · r/singularity · /u/Successful-Earth678 · Aug 2, 05:51

**Background**: The concept of the AI singularity refers to a hypothetical future point where AI surpasses human intelligence, leading to unpredictable changes. In mathematics, recent AI models have shown surprising abilities in solving problems and formalizing proofs, prompting reflections from mathematicians like Terence Tao. The r/singularity subreddit is a community focused on discussing such transformative AI developments.

<details><summary>References</summary>
<ul>
<li><a href="https://borretti.me/article/mathematics-without-mathematicians">Mathematics Without Mathematicians | Fernando Borretti</a></li>
<li><a href="https://www.theatlantic.com/technology/2026/02/ai-math-terrance-tao/686107/">The Edge of Mathematics - The Atlantic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Singularity_Institute">Singularity Institute</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion likely includes a mix of awe and concern, with some users agreeing that AI will transform mathematics, while others debate the limits of AI in intuitive domains. Some may reference the 'RL doesn't generalize well' argument as a counterpoint to rapid progress.

**Tags**: `#AI`, `#mathematics`, `#singularity`, `#impact`, `#reflection`

---