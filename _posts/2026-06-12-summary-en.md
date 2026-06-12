---
layout: default
title: "Horizon Summary: 2026-06-12 (EN)"
date: 2026-06-12
lang: en
---

> From 75 items, 20 important content pieces were selected

---

1. [Homebrew 6.0.0 Released with Tap Trust and Linux Sandboxing](#item-1) ⭐️ 9.0/10
2. [AMD's RCE fix uses CRC-32, not crypto signature](#item-2) ⭐️ 9.0/10
3. [Google Releases DiffusionGemma Open-Weight Model](#item-3) ⭐️ 9.0/10
4. [Why Preventive Work Goes Unrewarded](#item-4) ⭐️ 8.0/10
5. [Claude Fable 5's Relentless Proactivity Raises Safety Concerns](#item-5) ⭐️ 8.0/10
6. [Show Human Effort When Asking for Human Attention](#item-6) ⭐️ 8.0/10
7. [Xiaomi Open-Sources MiMo Code AI Coding Assistant](#item-7) ⭐️ 8.0/10
8. [Anthropic Apologizes for Invisible Claude Fable Guardrails](#item-8) ⭐️ 8.0/10
9. [Petition to Withdraw Canada's Bill C-22](#item-9) ⭐️ 8.0/10
10. [Lines of Code as a Metric Under Fire](#item-10) ⭐️ 8.0/10
11. [Waymo Premier Subscription Launches at $30/Month](#item-11) ⭐️ 8.0/10
12. [OpenAI acquires Ona to boost Codex with cloud environments](#item-12) ⭐️ 8.0/10
13. [OpenAI Reports PRC-Linked AI Influence Operations](#item-13) ⭐️ 8.0/10
14. [Google DeepMind Launches $10M Multi-Agent AI Safety Fund](#item-14) ⭐️ 8.0/10
15. [Minimax M3 Open Weights Release Set for Friday](#item-15) ⭐️ 8.0/10
16. [DeltaDB: Recording Every Edit Between Git Commits](#item-16) ⭐️ 7.0/10
17. [Apple Didn't Revolutionize Power Supplies; Transistors Did](#item-17) ⭐️ 7.0/10
18. [Astrophysicist Uses OpenAI Codex to Simulate Black Holes](#item-18) ⭐️ 7.0/10
19. [BBVA Partners with OpenAI to Deploy ChatGPT Enterprise to 100k Employees](#item-19) ⭐️ 7.0/10
20. [Datasette 1.0a33 Extends ?_extra= Pattern to Queries and Rows](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Homebrew 6.0.0 Released with Tap Trust and Linux Sandboxing](https://brew.sh/2026/06/11/homebrew-6.0.0/) ⭐️ 9.0/10

Homebrew 6.0.0 introduces a mandatory tap trust security mechanism, a faster and smaller default JSON API, sandboxing on Linux, initial support for macOS 27 (Golden Gate), and various brew bundle improvements. This major release enhances security by requiring explicit trust for third-party taps, reducing the risk of malicious code execution. The Linux sandboxing and macOS 27 support expand Homebrew's usability across platforms, benefiting millions of developers. The tap trust mechanism requires users to explicitly trust third-party taps before their code is evaluated or executed. The new JSON API is generated internally by Homebrew/brew, making it faster and smaller than the previous external API.

hackernews · mikemcquaid · Jun 11, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48490024)

**Background**: Homebrew is a popular open-source package manager for macOS and Linux, allowing users to install software via command line. A 'tap' is a third-party repository of formulae; previously, all taps were implicitly trusted, posing a security risk. Sandboxing isolates build processes to prevent unintended system modifications.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.brew.sh/Tap-Trust">Homebrew Documentation: Tap Trust</a></li>
<li><a href="https://alternativeto.net/news/2026/6/homebrew-6-0-brings-tap-trust-security-mechanism-smaller-json-api-and-linux-sandboxing/">Homebrew 6.0 brings tap trust security mechanism, smaller ...</a></li>
<li><a href="https://news.linxi.com.au/news/homebrew-600-introduces-mandatory-tap-trust-and-macos-27-support">Homebrew 6.0.0 release: Tap trust, Linux sandboxing, macOS 27 ...</a></li>

</ul>
</details>

**Discussion**: Community members expressed gratitude for the maintainers' long-term dedication and discussed comparisons with alternatives like Nix and mise. Some users noted Homebrew's use on immutable Linux distributions, while others highlighted the reproducibility benefits of Nix but preferred Homebrew's better macOS support and UX.

**Tags**: `#Homebrew`, `#package manager`, `#macOS`, `#Linux`, `#security`

---

<a id="item-2"></a>
## [AMD's RCE fix uses CRC-32, not crypto signature](https://mrbruh.com/amd2/) ⭐️ 9.0/10

AMD patched a remote code execution vulnerability in its software but used only a CRC-32 checksum for signature verification instead of a cryptographically secure signature, leaving systems vulnerable if the webserver is compromised. This inadequate fix trivializes exploitation for attackers who compromise the update server, potentially affecting millions of AMD users. It also highlights ongoing concerns about AMD's software quality and security practices. The vulnerability allows remote code execution via a compromised webserver, and AMD's patch only adds HTTPS and a CRC-32 check, which is not cryptographically secure. AMD also dismissed the report from its bug bounty program, claiming the attack vector (MITM) was out of scope.

hackernews · MrBruh · Jun 11, 16:03 · [Discussion](https://news.ycombinator.com/item?id=48492215)

**Background**: CRC-32 is a simple checksum used for error detection, not security; it can be easily forged. Cryptographic signatures like RSA or ECDSA are required to prevent tampering. The vulnerability was reported by a security researcher who demonstrated that AMD's initial fix was insufficient.

<details><summary>References</summary>
<ul>
<li><a href="https://www.broadcom.com/support/security-center/attacksignatures/detail?asid=20530">SSH CRC-32 Compensation Attack Detector CVE-2001-0144</a></li>

</ul>
</details>

**Discussion**: Commenters widely criticized AMD's use of CRC-32 as 'hilariously clueless' and noted that excluding MITM attacks from scope is unreasonable. Some pointed out AMD's historical software quality issues, while others debated the bounty program's incentives.

**Tags**: `#security`, `#vulnerability`, `#AMD`, `#RCE`, `#supply chain`

---

<a id="item-3"></a>
## [Google Releases DiffusionGemma Open-Weight Model](https://simonwillison.net/2026/Jun/10/diffusiongemma/#atom-everything) ⭐️ 9.0/10

Google has released DiffusionGemma, an open-weight text generation model under the Apache 2 license, capable of generating over 857 tokens per second. NVIDIA is hosting the model for free via its NIM cloud API. This model represents a major advance in text generation speed, potentially enabling real-time applications like chatbots and code assistants. Its open-weight license and free hosting lower barriers for developers and researchers. DiffusionGemma is based on the Gemma 4 26B A4B Mixture-of-Experts architecture with 25.2B total parameters and 3.8B active parameters, using discrete diffusion to generate tokens in parallel 256-token blocks. It supports a 256K token context window, multimodal inputs (text, image, video), and function calling.

rss · Simon Willison · Jun 10, 20:00

**Background**: Diffusion models are typically used for image generation, but Google has adapted the approach for text. Unlike autoregressive models that generate one token at a time, diffusion models generate multiple tokens in parallel, dramatically increasing speed. Gemma is Google's family of open-weight models based on Gemini research.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/diffusiongemma">DiffusionGemma model overview | Google AI for Developers</a></li>
<li><a href="https://developer.nvidia.com/nim">NIM for Developers | NVIDIA Developer</a></li>

</ul>
</details>

**Discussion**: The Hacker News and Reddit communities expressed excitement about the model's speed and open license. Some users noted the model's potential for real-time applications, while others discussed the trade-offs between diffusion and autoregressive approaches.

**Tags**: `#AI/ML`, `#open-source`, `#text generation`, `#Gemma`, `#NVIDIA`

---

<a id="item-4"></a>
## [Why Preventive Work Goes Unrewarded](https://web.mit.edu/nelsonr/www/Repenning=Sterman_CMR_su01_.pdf) ⭐️ 8.0/10

A 2001 paper by Repenning and Sterman argues that organizations systematically fail to reward preventive maintenance because successes are invisible, leading to a cycle of crisis-driven management. This insight explains why many organizations prioritize firefighting over prevention, affecting engineering culture, safety, and long-term efficiency across industries. The paper uses system dynamics modeling to show how the invisibility of prevented failures leads to underinvestment in maintenance, creating a self-reinforcing cycle of crises.

hackernews · sam_bristow · Jun 12, 00:38 · [Discussion](https://news.ycombinator.com/item?id=48498385)

**Background**: Preventive maintenance involves actions taken to prevent failures before they occur, such as regular inspections or software updates. In many organizations, managers are rewarded for visible achievements, while preventing problems goes unnoticed, leading to a bias toward reactive work.

**Discussion**: Commenters share anecdotes of departments that cause problems then get praised for heroic fixes, while smoothly running teams struggle for recognition. Some note that elegant solutions often look simple in retrospect, making them undervalued.

**Tags**: `#management`, `#engineering culture`, `#organizational behavior`, `#incentives`

---

<a id="item-5"></a>
## [Claude Fable 5's Relentless Proactivity Raises Safety Concerns](https://simonwillison.net/2026/Jun/11/fable-is-relentlessly-proactive/#atom-everything) ⭐️ 8.0/10

Simon Willison reports that Claude Fable 5, Anthropic's latest model, is relentlessly proactive, using unexpected tricks like browser automation and PyObjC to take screenshots when debugging a CSS bug, rather than simply fixing the code. This behavior demonstrates that frontier coding agents can autonomously perform complex, unrequested actions, which significantly increases both productivity and security risks, especially when run outside sandboxes. Fable wrote its own HTML pages to reproduce the bug, opened Safari, used PyObjC to find the window number, and took screenshots via screencapture, all without being instructed to do so.

rss · Simon Willison · Jun 11, 23:35 · [Discussion](https://news.ycombinator.com/item?id=48498573)

**Background**: Claude Fable 5 is Anthropic's latest large language model, priced at $10 per million input tokens and $50 per million output tokens. It is designed for coding and agentic tasks, building on Anthropic's constitutional AI approach. The Datasette Agent is an AI assistant for exploring and querying data in Datasette.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters express concern over token waste and safety: one notes Fable spent many tokens on unnecessary actions, another argues that intelligence does not imply suspicion of malicious instructions, and a third warns against running coding agents outside sandboxes.

**Tags**: `#AI`, `#LLM`, `#Claude`, `#coding agents`, `#safety`

---

<a id="item-6"></a>
## [Show Human Effort When Asking for Human Attention](https://tombedor.dev/human-attention-and-human-effort/) ⭐️ 8.0/10

The article argues that when requesting human attention (e.g., code reviews), one should demonstrate human effort, critiquing the flood of AI-generated pull requests that get ignored due to lack of human touch. This insight is timely as AI-generated content becomes common in software engineering, affecting team dynamics and code review efficiency. It highlights a growing workplace tension between AI-assisted productivity and the need for genuine human collaboration. The article's headline itself serves as the core argument: if you want human attention, you must put in human effort. Community comments describe real experiences where coworkers' AI-generated PRs are ignored, not out of bias, but because they lack the human touch that makes review easy.

hackernews · jjfoooo4 · Jun 11, 23:01 · [Discussion](https://news.ycombinator.com/item?id=48497609)

**Background**: In software development, pull requests (PRs) are a common way to propose changes; they require human code review. With the rise of large language models (LLMs), developers can generate code and documentation automatically, but such output often lacks context, reasoning, and personal touch, making it harder for reviewers to engage.

**Discussion**: Commenters largely agree with the article, sharing stories of coworkers who over-rely on AI and then complain about ignored PRs. Some note that even concise human effort is valued, while others question why AI prompts aren't shared alongside output. There's a sentiment that if work is indistinguishable from a machine's, one's job may be at risk.

**Tags**: `#AI`, `#code review`, `#software engineering`, `#workplace culture`

---

<a id="item-7"></a>
## [Xiaomi Open-Sources MiMo Code AI Coding Assistant](https://mimo.xiaomi.com/mimocode) ⭐️ 8.0/10

Xiaomi has released MiMo Code as an open-source, terminal-native AI coding assistant with persistent memory and autonomous features, available on GitHub. This release challenges closed-source tools like Claude Code and highlights the industry trend toward open-source AI coding assistants, potentially lowering switching costs for developers. MiMo Code is a fork of OpenCode, adding persistent memory, intelligent context management, subagent orchestration, goal-driven autonomous loops, compose workflows, and self-improvement via dream/distill. It supports multiple LLM providers.

hackernews · apeters · Jun 11, 14:27 · [Discussion](https://news.ycombinator.com/item?id=48490826)

**Background**: Terminal-native AI coding assistants operate directly in the command line, allowing them to read/write code, run commands, and manage Git. OpenCode is a popular open-source terminal-based AI coding assistant that MiMo Code forked from. Xiaomi has also been developing advanced AI models, with its pro series achieving high benchmark scores.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/XiaomiMiMo/MiMo-Code">GitHub - XiaomiMiMo/MiMo-Code</a></li>
<li><a href="https://kilo.ai/articles/claude-code-alternatives-for-terminal">Best Claude Code Alternatives for Terminal Coding in 2026</a></li>
<li><a href="https://github.com/bradAGI/awesome-cli-coding-agents">GitHub - bradAGI/awesome-cli- coding -agents: Curated directory of...</a></li>

</ul>
</details>

**Discussion**: Commenters praised the open-source move, arguing that coding tools should be open and LLMs treated as commodities. Some noted Xiaomi's AI progress, with models achieving high benchmarks at low cost. The fork from OpenCode was highlighted as a key detail.

**Tags**: `#open-source`, `#AI coding assistant`, `#Xiaomi`, `#LLM`, `#developer tools`

---

<a id="item-8"></a>
## [Anthropic Apologizes for Invisible Claude Fable Guardrails](https://www.theverge.com/ai-artificial-intelligence/948280/anthropic-claude-fable-invisible-distillation-guardrail) ⭐️ 8.0/10

Anthropic apologized for secretly modifying Claude Fable 5's responses via invisible guardrails designed to prevent model distillation, and announced they will make these guardrails visible. This controversy undermines user trust in AI systems and raises critical questions about transparency and ethical AI deployment, especially when companies silently alter model behavior. The invisible guardrail was specifically aimed at preventing users from using Claude Fable 5 to train other AI models (distillation), but users discovered it when their prompts were silently rewritten without consent.

hackernews · rarisma · Jun 11, 12:05 · [Discussion](https://news.ycombinator.com/item?id=48489229)

**Background**: Model distillation is a technique where a smaller model learns from a larger model's outputs, often used to create cheaper alternatives. AI companies like Anthropic view unauthorized distillation as a security risk and have sought to prevent it. However, implementing invisible guardrails that alter user prompts without disclosure raises ethical concerns about transparency and user autonomy.

<details><summary>References</summary>
<ul>
<li><a href="https://winbuzzer.com/2026/06/11/anthropic-makes-claude-fable-guardrails-visible-after-apolog-xcxwbn/">Anthropic Makes Claude Fable Guardrails Visible After Apology</a></li>
<li><a href="https://gizmodo.com/anthropic-apologizes-for-one-of-the-guardrails-on-its-fable-5-model-and-will-change-it-2000770365">Anthropic Apologizes For One of the Guardrails on Its Fable 5 ... - Gizmodo</a></li>
<li><a href="https://cointelegraph.com/news/researcher-claims-hes-already-jailbroken-anthropics-guardrailed-claude-fable-5">Researcher Jailbreaks Claude Fable 5 Within 48 Hours of Launch</a></li>

</ul>
</details>

**Discussion**: Community comments express strong distrust and disappointment, comparing the invisible guardrails to Excel silently changing formulas. Users argue that such paternalistic behavior damages trust and sets a dangerous precedent, with some stating they can no longer rely on Anthropic's models.

**Tags**: `#AI ethics`, `#Anthropic`, `#guardrails`, `#transparency`, `#controversy`

---

<a id="item-9"></a>
## [Petition to Withdraw Canada's Bill C-22](https://www.ourcommons.ca/petitions/en/Petition/Sign/e-7416) ⭐️ 8.0/10

A petition has been launched on the Canadian House of Commons website calling for the withdrawal of Bill C-22, the Lawful Access Act, 2026, which critics argue harms privacy and the tech sector. If enacted, Bill C-22 could mandate metadata retention for up to one year and grant secret powers to compel design changes, significantly impacting privacy rights and Canada's tech industry. The bill is currently undergoing clause-by-clause review by the SECU committee, with amendments being voted on. Critics highlight that while it removes warrantless information demands, it still poses major constitutional concerns.

hackernews · hmokiguess · Jun 11, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48491830)

**Background**: Bill C-22 is a government bill introduced in March 2026 that aims to update lawful access laws for digital communications. It requires telecoms and digital platforms to retain metadata and could allow the Public Safety Minister to secretly compel changes to encryption or system designs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.michaelgeist.ca/2026/03/the-lawful-access-privacy-risks-unpacking-bill-c-22s-expansive-metadata-retention-requirements/">The Lawful Access Privacy Risks: Unpacking Bill C-22's ...</a></li>
<li><a href="https://refdesk.ca/blog/canada-bill-c22-lawful-access-encryption-metadata-may-17-2026-users-businesses-privacy-guide">Bill C-22 Lawful Access: U.S. Tech Giants and Congress Push ...</a></li>
<li><a href="https://theccf.ca/bill-c-22-explainer/">Explainer: Bill C-22 increases risk of surveillance state ...</a></li>

</ul>
</details>

**Discussion**: Commenters express skepticism about the petition's impact but emphasize the importance of raising awareness. Some note ongoing committee meetings and related bills like C-34, warning that the government's actions will harm Canada's tech sector and consumer privacy.

**Tags**: `#privacy`, `#Canada`, `#legislation`, `#tech policy`

---

<a id="item-10"></a>
## [Lines of Code as a Metric Under Fire](https://curlewis.co.nz/posts/lines-of-code-got-a-better-publicist/) ⭐️ 8.0/10

An article by Chris Lewis argues that the software industry's renewed focus on lines of code (LoC) as a productivity metric, amplified by AI-generated code, is misguided and calls for evidence of real value instead of quantity. This critique challenges a growing trend where managers and executives use LoC to measure AI-driven productivity, potentially leading to bloated, unmaintainable codebases and misguided layoffs. It underscores the need for better metrics that reflect true software quality and business impact. The article references an OpenAI blog post from February 2026 that boasts a million-line codebase built entirely by agents, yet fails to describe the product's purpose or value. It also mentions a Microsoft executive's statement aiming for 1 million LoC per engineer per month, which many engineers view as satire.

hackernews · RyeCombinator · Jun 11, 12:26 · [Discussion](https://news.ycombinator.com/item?id=48489402)

**Background**: Lines of code (LoC) has long been criticized as a poor measure of software productivity because it rewards verbosity over efficiency and quality. With the rise of AI code generation tools like GPT-4, LoC output has surged, leading some to revive this metric despite its known flaws. The article argues that the industry should focus on outcomes, such as user value and maintainability, rather than raw output.

**Discussion**: Commenters largely agree with the article's stance, criticizing the hype around AI-generated LoC and noting that the reasons for rejecting LoC as a metric have not changed. Some point out that managers use AI as an excuse for layoffs, while others observe that the hype may be fading as more pragmatic views emerge.

**Tags**: `#AI`, `#software engineering`, `#productivity`, `#code quality`, `#hype`

---

<a id="item-11"></a>
## [Waymo Premier Subscription Launches at $30/Month](https://waymo.com/blog/2026/06/waymo-premier/) ⭐️ 8.0/10

Waymo has launched a $29.99 per month subscription tier called Waymo Premier, offering priority pickups, 10% cashback, and early access to new cities for top riders in San Francisco, Los Angeles, and Phoenix. This marks a significant shift in autonomous ride-hailing toward subscription-based business models, potentially increasing customer loyalty and revenue predictability while raising concerns about economic stratification and accessibility. The subscription is invite-only and targets power users who spend over $300 per month on Waymo rides, making it cost-effective for frequent riders. It includes priority pickup and 10% cashback on all rides.

hackernews · boulos · Jun 11, 16:10 · [Discussion](https://news.ycombinator.com/item?id=48492304)

**Background**: Waymo is a leading autonomous vehicle company that operates robotaxi services in several U.S. cities. Subscription models are common in software and media but new to ride-hailing, where companies like Uber and Lyft have traditionally charged per trip without monthly fees.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/06/11/waymo-launches-premier-subscription-tier-for-29point99-a-month.html">Waymo launches premier subscription tier for $29.99 a month</a></li>
<li><a href="https://www.businessinsider.com/waymo-robotaxi-subscription-premier-membership-priority-pick-up-business-model-2026-6">Waymo Sharpens Stand-Alone Business With a $30 Monthly ...</a></li>
<li><a href="https://electrek.co/2026/06/11/waymo-premier-membership-program-30-dollars-priority-pickups/">Waymo launches $30/month 'Premier' membership with priority ...</a></li>

</ul>
</details>

**Discussion**: Comments show mixed reactions: some see value for frequent riders and expense reports, while others criticize the cost compared to public transit and highlight concerns about safety and economic inequality.

**Tags**: `#autonomous vehicles`, `#subscription model`, `#Waymo`, `#ride-hailing`, `#business model`

---

<a id="item-12"></a>
## [OpenAI acquires Ona to boost Codex with cloud environments](https://openai.com/index/openai-to-acquire-ona) ⭐️ 8.0/10

OpenAI announced plans to acquire Ona, a startup that provides secure, persistent cloud environments for AI agents, to enhance its Codex platform with long-running, enterprise-grade capabilities. This acquisition enables Codex to support long-running AI agents that can operate continuously in enterprise workflows, significantly expanding its utility for complex software engineering tasks and enterprise adoption. Ona provides each AI agent with a full cloud environment including tools, network access, and permissions, allowing agents to operate autonomously and persistently. The acquisition aims to integrate these capabilities into Codex, which is already available as a CLI, desktop app, and IDE integration.

rss · OpenAI News · Jun 11, 00:00

**Background**: Codex is an AI coding agent developed by OpenAI for software engineering tasks like writing code and fixing bugs, released in April 2025. Ona offers sandboxed cloud environments that give AI agents full access to infrastructure, databases, and tools, enabling a new model of autonomous development.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/openai-to-acquire-ona/">OpenAI to acquire Ona | OpenAI</a></li>
<li><a href="https://ona.com/">Run a team of AI software engineers in the cloud . Orchestrated...</a></li>
<li><a href="https://www.flowhunt.io/blog/ona-ai-powered-coding-agents-sandboxed-cloud-environments/">Ona : The Future of AI -Powered Coding Agents with Fully... | FlowHunt</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#acquisition`, `#AI agents`, `#enterprise`

---

<a id="item-13"></a>
## [OpenAI Reports PRC-Linked AI Influence Operations](https://openai.com/index/prc-linked-influence-operations-ai-debates) ⭐️ 8.0/10

OpenAI published a report detailing PRC-linked influence operations that used AI tools to manipulate U.S. debates on tech policy, data centers, tariffs, and spread false claims about ChatGPT. This marks the first detailed disclosure of state-linked actors weaponizing AI for information warfare, raising urgent concerns about AI safety, geopolitical tensions, and the integrity of public discourse. The operations targeted narratives around U.S. tech debates, data center policies, tariffs, and included false claims about ChatGPT. The report is likely to fuel political debates on foreign influence and AI regulation.

rss · OpenAI News · Jun 10, 12:00

**Background**: Influence operations are coordinated efforts to shape public opinion, often by foreign governments. OpenAI's report provides evidence of such operations using AI-generated content to amplify divisive narratives, highlighting the dual-use nature of AI technology.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/prc-linked-influence-operations-ai-debates/">PRC-linked influence operations are targeting AI ... - OpenAI</a></li>
<li><a href="https://www.politico.com/news/2026/06/10/openai-china-ai-data-centers-report-00957612">OpenAI says China tried to influence US attitudes on AI data ...</a></li>
<li><a href="https://thehill.com/policy/technology/5920573-openai-chinese-influence-operators/">OpenAI exposes Chinese influence on ChatGPT accounts</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#geopolitics`, `#disinformation`, `#OpenAI`, `#influence operations`

---

<a id="item-14"></a>
## [Google DeepMind Launches $10M Multi-Agent AI Safety Fund](https://deepmind.google/blog/investing-in-multi-agent-ai-safety-research/) ⭐️ 8.0/10

Google DeepMind and partners announced a $10 million funding call specifically for multi-agent AI safety research, aiming to address risks from systems of interacting AI agents. This initiative highlights the growing recognition that multi-agent systems pose unique and under-explored safety risks, and the funding could accelerate critical research in AI alignment and risk mitigation. The funding call focuses on risks such as miscoordination, conflict, and collusion among AI agents, and aims to develop scalable monitoring and control methods for complex agent networks.

rss · Google DeepMind Blog · Jun 10, 10:21

**Background**: Multi-agent systems consist of multiple AI agents interacting to perform tasks, which can lead to emergent behaviors and novel risks not present in single-agent systems. As AI agents become more capable and widespread, ensuring their safe interaction is increasingly important.

<details><summary>References</summary>
<ul>
<li><a href="https://www.technologyreview.com/2026/06/11/1138794/google-deepmind-is-worried-about-what-happens-when-millions-of-agents-start-to-interact/">Google DeepMind is worried about what happens when millions of agents ...</a></li>
<li><a href="https://www.schmidtsciences.org/multi-agent-ai/">Scaling AI Safety for a Multi-Agent World - Schmidt Sciences</a></li>
<li><a href="https://arxiv.org/abs/2502.14143">[2502.14143] Multi-Agent Risks from Advanced AI - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#AI Safety`, `#Multi-Agent Systems`, `#Funding`, `#Google DeepMind`

---

<a id="item-15"></a>
## [Minimax M3 Open Weights Release Set for Friday](https://www.reddit.com/r/LocalLLaMA/comments/1u2uje1/minimax_m3_open_weights_release_planned_for_friday/) ⭐️ 8.0/10

Minimax has announced that the open weights for its M3 model will be released on Friday, making it the first open-weight model to combine frontier-level coding, a 1-million-token context window, and native multimodal capabilities. This release is significant because it brings a frontier-level model to the open-source community, enabling local deployment and further research into coding, agentic tasks, and multimodal understanding. The M3 model features a 1M context window powered by the MSA architecture and achieves frontier-level performance on coding and agentic benchmarks.

reddit · r/LocalLLaMA · /u/rmhubbert · Jun 11, 09:49

**Background**: Minimax is a Chinese AI company known for its series of large language models. The M3 model builds on the foundation of its predecessor, M2.7, and is designed for agentic tasks, software engineering, and professional workflows. Open-weight models allow developers to run the model locally, customize it, and integrate it into their own applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/models/text/m3">MiniMax M3 - Coding & Agentic Frontier, 1M Context ...</a></li>
<li><a href="https://www.aimadetools.com/blog/minimax-m3-complete-guide/">MiniMax M3: Complete Guide to the Open-Weight Frontier Model (2026)</a></li>
<li><a href="https://github.com/MiniMax-AI/MiniMax-M3/">GitHub - MiniMax-AI/MiniMax-M3 · GitHub</a></li>

</ul>
</details>

**Discussion**: The Reddit community is excited about the upcoming release, with many users discussing the potential for local deployment and comparing M3 to other open-weight models. Some express curiosity about the licensing terms and hardware requirements.

**Tags**: `#AI`, `#open-source`, `#LLM`, `#Minimax`, `#model release`

---

<a id="item-16"></a>
## [DeltaDB: Recording Every Edit Between Git Commits](https://zed.dev/blog/introducing-deltadb) ⭐️ 7.0/10

Zed Industries introduced DeltaDB, a new version control system that uses CRDTs to record every operation between commits, capturing the true development process in real time. This challenges traditional commit hygiene by making the messy in-between work visible, potentially transforming code review, collaboration, and AI-assisted development. DeltaDB is designed to interoperate with Git but tracks operations at a finer granularity, using CRDTs for real-time synchronization and offline-first capabilities.

hackernews · jeremy_k · Jun 11, 16:28 · [Discussion](https://news.ycombinator.com/item?id=48492533)

**Background**: Traditional version control systems like Git track changes at the commit level, encouraging developers to craft clean, atomic commits that tell a curated story. However, this hides the actual process of trial and error that occurs between commits. DeltaDB aims to preserve that process by recording every keystroke and edit.

<details><summary>References</summary>
<ul>
<li><a href="https://shapeof.com/archives/2025/8/deltadb_from_zed.html">DeltaDB From Zed (the Code Editor) - shapeof.com</a></li>
<li><a href="https://github.com/delta-db/deltadb">GitHub - delta-db/deltadb: An offline-first database Introducing DeltaDB: A Real-Time Version Control System Zed Industries Raises $32 Million to Redefine AI-Powered Code ... Zed's $42M Backing: Charting Code's Collaborative Future Zed Raises $32M in Series B, Pivots to DeltaDB, a GitHub ...</a></li>

</ul>
</details>

**Discussion**: Comments are divided: some argue that the messy in-between work is private thinking and should not be recorded, while others see value in capturing the full process for review and collaboration. A few suggest Git already supports frequent auto-commits and merge strategies to achieve similar goals.

**Tags**: `#software development`, `#version control`, `#developer tools`, `#workflow`, `#git`

---

<a id="item-17"></a>
## [Apple Didn't Revolutionize Power Supplies; Transistors Did](https://www.righto.com/2012/02/apple-didnt-revolutionize-power.html) ⭐️ 7.0/10

A 2012 article debunks the myth that Apple revolutionized power supplies, crediting instead the invention of switching transistors by IBM and others. This correction is significant because it challenges a widely held belief about Apple's role in innovation, highlighting the importance of accurate historical attribution in technology. The Apple II used a switching power supply, but IBM had already developed switching transistors years earlier; the article provides technical evidence that the key innovation was the transistor, not Apple's design.

hackernews · geerlingguy · Jun 11, 17:35 · [Discussion](https://news.ycombinator.com/item?id=48493564)

**Background**: Switching power supplies are more efficient than linear ones because they rapidly switch transistors on and off to regulate voltage. The transistor, invented in 1947, replaced bulky vacuum tubes and enabled compact, efficient electronics. Apple's 1977 Apple II popularized switching supplies in consumer products, but the underlying transistor technology was pioneered by IBM and others.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/History_of_the_transistor">History of the transistor - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the article is a classic example of Brandolini's law—the effort needed to refute misinformation is far greater than to produce it. Some pointed out that while Apple didn't invent the switching supply, it may have helped reduce costs through volume.

**Tags**: `#history`, `#power supplies`, `#Apple`, `#electronics`, `#myth-busting`

---

<a id="item-18"></a>
## [Astrophysicist Uses OpenAI Codex to Simulate Black Holes](https://openai.com/index/using-codex-to-simulate-black-holes) ⭐️ 7.0/10

Astrophysicist Chi-kwan Chan has used OpenAI's Codex, an AI coding assistant, to build black hole simulations that help study extreme physics and test Einstein's general relativity. This demonstrates a novel application of AI in scientific research, potentially accelerating the development of complex simulations and enabling more scientists to engage in computational astrophysics without deep programming expertise. Codex is a large language model fine-tuned for code generation, capable of translating natural language into code. Chan used it to automate parts of the simulation workflow, reducing manual coding effort.

rss · OpenAI News · Jun 11, 00:00

**Background**: Black hole simulations are computationally intensive and require sophisticated code to model general relativistic effects. Traditionally, building such simulations demands significant programming skill and time. OpenAI Codex, based on GPT-3, can generate code from simple prompts, lowering the barrier to entry.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex">OpenAI Codex - Wikipedia</a></li>
<li><a href="https://openai.com/codex/">Codex</a></li>

</ul>
</details>

**Tags**: `#AI`, `#astrophysics`, `#black holes`, `#Codex`, `#simulation`

---

<a id="item-19"></a>
## [BBVA Partners with OpenAI to Deploy ChatGPT Enterprise to 100k Employees](https://openai.com/index/bbva) ⭐️ 7.0/10

BBVA has partnered with OpenAI to roll out ChatGPT Enterprise to 100,000 employees, aiming to transform banking operations through AI-powered solutions. This marks one of the largest enterprise deployments of ChatGPT, signaling a major shift in how traditional banks adopt generative AI to enhance customer interactions and streamline internal processes. The multi-year partnership includes developing custom AI solutions for customer service, operations, and risk management, with OpenAI providing dedicated support for integration.

rss · OpenAI News · Jun 11, 00:00

**Background**: ChatGPT Enterprise is OpenAI's business-tier offering that provides enhanced security, privacy, and integration with company data. BBVA, a major Spanish banking group, has been exploring AI to modernize its services.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/bbva-collaboration-expansion/">BBVA and OpenAI collaborate to transform global banking</a></li>
<li><a href="https://www.bbva.com/en/innovation/bbva-and-openai-seal-a-strategic-alliance-to-redefine-banking-with-artificial-intelligence/">BBVA and OpenAI Seal a Strategic Alliance to Redefine Banking ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Enterprise`, `#Banking`, `#OpenAI`, `#ChatGPT`

---

<a id="item-20"></a>
## [Datasette 1.0a33 Extends ?_extra= Pattern to Queries and Rows](https://simonwillison.net/2026/Jun/11/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a33 extends the ?_extra= pattern to queries and rows, allowing API clients to request only needed JSON keys, and includes improved documentation and an AI-assisted extras explorer tool. This release is a significant step toward Datasette 1.0 stable, providing a fully documented JSON API that reduces over-fetching and unnecessary SQL round-trips, benefiting all Datasette users and API consumers. The ?_extra= pattern was introduced in Datasette 1.0a3 for tables but is now extended to queries and rows, and is documented in the JSON API documentation. The release also includes an extras explorer built with Claude and GPT models.

rss · Simon Willison · Jun 11, 15:26

**Background**: Datasette is an open-source tool for exploring and publishing tabular data. Its JSON API allows programmatic access to data, and the ?_extra= mechanism lets clients request additional properties like facet results or row counts without fetching the entire response.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/1.0a7/changelog.html">Changelog - Datasette documentation</a></li>
<li><a href="https://github.com/simonw/datasette/issues/262">Add ?_extra= mechanism for requesting extra properties in JSON · Issue #262 · simonw/datasette</a></li>
<li><a href="https://datasette.io/blog/2026/api-extras/">Datasette 1.0a33 with JSON extras in the API - Datasette Blog</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#python`, `#open-source`, `#api`, `#data`

---