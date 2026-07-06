---
layout: default
title: "Horizon Summary: 2026-07-06 (EN)"
date: 2026-07-06
lang: en
---

> From 46 items, 16 important content pieces were selected

---

1. [Digital Game Ownership Crisis: It's About Rights, Not Format](#item-1) ⭐️ 8.0/10
2. [World Map in 445 Bytes Using Deflate Compression](#item-2) ⭐️ 8.0/10
3. [Newer Claude Models Show Worse Tool-Call Adherence](#item-3) ⭐️ 8.0/10
4. [AI Rewrites Outsourcing Economics](#item-4) ⭐️ 8.0/10
5. [Damo Academy AI Agent Discovers Superconductors](#item-5) ⭐️ 8.0/10
6. [GitHub repo collects leaked AI system prompts](#item-6) ⭐️ 8.0/10
7. [Canada's AI strategy should avoid secret Palantir deals](#item-7) ⭐️ 7.0/10
8. [AI Tutor Boosts Learning by 0.71-1.30 SD, but Critics Question Study](#item-8) ⭐️ 7.0/10
9. [Website Cataloging Computers in Movies and TV](#item-9) ⭐️ 7.0/10
10. [Free Online Book on Compilers and Language Design](#item-10) ⭐️ 7.0/10
11. [New es40 Fork Runs Windows 2000 on DEC Alpha Emulator](#item-11) ⭐️ 7.0/10
12. [sqlite-utils 4.0rc2: AI catches critical bugs before release](#item-12) ⭐️ 7.0/10
13. [Google Unveils Gemini Omni Flash Multimodal AI](#item-13) ⭐️ 7.0/10
14. [US and China Dominate Global AI Model Training](#item-14) ⭐️ 7.0/10
15. [OpenAI Releases Codex Plugin for Claude Code](#item-15) ⭐️ 7.0/10
16. [RedKnot: Head-Aware KV Cache for Efficient Long-Context LLM Serving](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Digital Game Ownership Crisis: It's About Rights, Not Format](https://popcar.bearblog.dev/its-about-ownership/) ⭐️ 8.0/10

A widely discussed blog post argues that the core problem with digital games is the lack of true ownership, not the digital format itself, and calls for regulation to guarantee buyers property rights such as transferability and permanent access. This debate highlights a growing consumer concern as digital game sales surpass physical ones, and companies increasingly use DRM and licensing to restrict usage, potentially setting a precedent for all digital goods. The post notes that Steam does not apply hard DRM and allows offline play, but many other platforms lock games behind online checks. Recent moves like Sony's 30-day online verification for PlayStation digital games further erode ownership.

hackernews · popcar2 · Jul 5, 14:56 · [Discussion](https://news.ycombinator.com/item?id=48794750)

**Background**: Digital rights management (DRM) technologies restrict how consumers can use digital content they purchase. Most digital games are sold under a license, not as owned property, meaning companies can revoke access or impose conditions. California's AB 2426 law (2024) is an early attempt to regulate digital ownership transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_rights_management">Digital rights management - Wikipedia</a></li>
<li><a href="https://techwiser.com/sony-playstation-drm-policy/">Sony Just Killed Game Ownership: New PlayStation DRM Locks ... - TechWiser</a></li>
<li><a href="https://www.morganlewis.com/pubs/2024/10/the-evolving-landscape-of-digital-goods-ownership-californias-digital-marketplace-law-ab-2426">The Evolving Landscape of Digital Goods Ownership: California’s Digital Marketplace Law AB 2426</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that ownership is the core issue, with some supporting regulation to enforce transferability and permanent access. Others note that piracy and cracks provide de facto ownership, while some blame consumers for accepting digital convenience without demanding rights.

**Tags**: `#digital ownership`, `#gaming`, `#regulation`, `#DRM`, `#consumer rights`

---

<a id="item-2"></a>
## [World Map in 445 Bytes Using Deflate Compression](https://simonwillison.net/2026/Jul/4/building-a-world-map-with-only-500-bytes/#atom-everything) ⭐️ 8.0/10

Iwo Kadziela, assisted by Codex, created a credible ASCII world map using only 445 bytes of data by leveraging deflate compression and the JavaScript DecompressionStream API. This demonstrates an extremely efficient way to transmit complex data over the web, potentially inspiring new approaches to data compression and inline resource delivery in web applications. The technique uses fetch() with a data: URI containing base64-encoded deflate-raw compressed data, then pipes it through DecompressionStream to decompress and render the map inside a <pre> element.

rss · Simon Willison · Jul 4, 23:09

**Background**: Deflate is a widely used lossless compression algorithm (RFC 1951). The DecompressionStream API, part of the Compression Streams standard, allows streaming decompression in the browser. Data URIs enable embedding data directly in HTML or JavaScript without external files.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/DecompressionStream">DecompressionStream - Web APIs | MDN</a></li>
<li><a href="https://en.wikipedia.org/wiki/DEFLATE">Deflate - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data_URI_scheme">data URI scheme - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion praised the clever use of compression and modern APIs, with some commenters noting the potential for similar techniques in other domains like game development or data visualization.

**Tags**: `#compression`, `#JavaScript`, `#ASCII art`, `#web APIs`, `#data URI`

---

<a id="item-3"></a>
## [Newer Claude Models Show Worse Tool-Call Adherence](https://simonwillison.net/2026/Jul/4/better-models-worse-tools/#atom-everything) ⭐️ 8.0/10

Armin Ronacher reports that newer Claude models (Opus 4.8, Sonnet 5) invent extra fields in tool call arguments, causing Pi to reject the calls, while older models do not exhibit this issue. This regression in tool-calling fidelity for state-of-the-art models undermines reliability for third-party coding harnesses and raises concerns about overfitting to built-in tools. The extra fields appear in the nested 'edits[]' array of Pi's edit tool; the edit content itself is usually correct, but the invented keys cause schema validation failures.

rss · Simon Willison · Jul 4, 22:53

**Background**: Tool-calling is a key capability for LLMs used in coding agents, where the model must output structured JSON matching a predefined schema. Anthropic's Claude models include built-in edit tools optimized via reinforcement learning, which may inadvertently bias the model against third-party tool schemas.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/overview">Models overview - Claude Platform Docs</a></li>
<li><a href="https://arxiv.org/html/2604.13519v2">ToolSpec: Accelerating Tool Calling via Schema-Aware and Retrieval-Augmented Speculative Decoding</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#tool use`, `#Anthropic`, `#Claude`, `#reliability`

---

<a id="item-4"></a>
## [AI Rewrites Outsourcing Economics](https://www.reddit.com/r/singularity/comments/1uoall4/harvard_business_review_ai_is_rewriting_the/) ⭐️ 8.0/10

A Harvard Business Review analysis argues that generative AI is shifting the basis of outsourcing from labor arbitrage to task-level automation, forcing companies to reassess which work to keep in-house versus outsource. This shift could fundamentally alter global supply chains for services, reducing the cost advantage of offshore labor and pushing outsourcing partners toward higher-skill, outcome-based models. The analysis emphasizes that leaders must analyze work at the task and workflow level rather than deciding on entire functions, and that successful companies will redesign around AI-enabled speed, judgment, and control.

reddit · r/singularity · /u/ChokePaul3 · Jul 5, 19:08

**Background**: Outsourcing has historically been driven by labor arbitrage—moving jobs to countries with lower wages. Generative AI now automates many routine, rules-based tasks that were previously sent offshore, reducing the need for human labor in those areas. This forces companies to rethink which tasks can be automated internally and which still require external expertise.

<details><summary>References</summary>
<ul>
<li><a href="https://www.atlassian.com/agile/project-management/task-automation">What is task automation? How to cut repetitive work | Atlassian</a></li>
<li><a href="https://en.wikipedia.org/wiki/Labor_arbitrage">Labor arbitrage</a></li>
<li><a href="https://kenyarmosh.com/blog/outcome-based-services/">The Complete Guide to Creating Outcome-Based Services</a></li>

</ul>
</details>

**Tags**: `#AI`, `#outsourcing`, `#economics`, `#generative AI`, `#business strategy`

---

<a id="item-5"></a>
## [Damo Academy AI Agent Discovers Superconductors](https://www.reddit.com/r/singularity/comments/1unnrka/damo_academy_unveils_an_ai_agent_able_to_discover/) ⭐️ 8.0/10

Alibaba's DAMO Academy, in collaboration with Renmin University and the University of Chinese Academy of Sciences, released ElementsClaw, the first AI agent dedicated to discovering superconducting materials. It screened 2.4 million crystal structures in 28 GPU hours, identifying 68,000 potential superconductors, with four new materials synthesized and verified in the lab. This breakthrough dramatically accelerates the discovery of superconductors, which could revolutionize energy transmission, quantum computing, and medical imaging. It demonstrates AI's potential to transform materials science by reducing discovery time from years to hours. ElementsClaw was trained on 125 million molecular structures and used a high-throughput virtual screening workflow. The four discovered superconductors are entirely new materials, not previously known, marking an industry first for AI-driven superconductor discovery.

reddit · r/singularity · /u/yogthos · Jul 4, 23:59

**Background**: Superconductors are materials that conduct electricity with zero resistance when cooled below a critical temperature, enabling lossless power transmission and powerful magnets. Traditional discovery methods are slow and costly, relying on trial-and-error experimentation. AI agents like ElementsClaw can rapidly screen vast databases of crystal structures, predict properties, and prioritize candidates for lab synthesis.

<details><summary>References</summary>
<ul>
<li><a href="https://pandaily.com/alibaba-damo-elementsclaw-ai-superconductors-28-gpu-hours-jul2026">Alibaba DAMO Academy's ElementsClaw AI Agent Discovers 4 New ...</a></li>
<li><a href="https://finance.biggo.com/news/2414f7e6-4d3f-4950-9d4a-6e87cb1a3802">Alibaba's DAMO Academy AI Agent Makes Breakthrough ...</a></li>
<li><a href="https://www.nationpress.com/sciencetech/alibaba-ai-finds-4-new-superconductors">Alibaba's Elements Claw AI agent discovers 4 new ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#materials science`, `#superconductors`, `#research`, `#innovation`

---

<a id="item-6"></a>
## [GitHub repo collects leaked AI system prompts](https://github.com/asgeirtj/system_prompts_leaks) ⭐️ 8.0/10

A GitHub repository named 'asgeirtj/system_prompts_leaks' has been trending, collecting leaked system prompts from major AI labs including Anthropic (Claude Fable 5, Opus 4.8), OpenAI (ChatGPT 5.5 Thinking, GPT 5.5 Instant, Codex), Google (Gemini 3.5 Flash, 3.1 Pro), and xAI (Grok), among others. Leaked system prompts provide rare visibility into the proprietary instructions that shape the behavior of leading AI models, enabling researchers and developers to understand model guardrails, personality, and capabilities, which could accelerate AI research and prompt engineering. The repository is actively maintained and updated regularly, and it includes system prompts from tools like Cursor, Copilot, VS Code, Perplexity, and more, in addition to the major model names.

ossinsight · asgeirtj · Jul 6, 02:23

**Background**: System prompts are instructions given to an AI model at the start of a conversation to define its behavior, tone, and constraints. They are typically kept secret by companies to prevent misuse and maintain competitive advantage. Leaks like this one offer a rare glimpse into how top AI models are tuned.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools">GitHub - x1xhlol/system-prompts-and-models-of-ai-tools: FULL Augment Code, Claude Code, Cluely, CodeBuddy, Comet, Cursor, Devin AI, Junie, Kiro, Leap.new, Lovable, Manus, NotionAI, Orchids.app, Perplexity, Poke, Qoder, Replit, Same.dev, Trae, Traycer AI, VSCode Agent, Warp.dev, Windsurf, Xcode, Z.ai Code, Dia & v0. (And other Open Sourced) System Prompts, Internal Tools & AI Models · GitHub</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://artificialanalysis.ai/models/gpt-5-5-instant-06-26">GPT - 5 . 5 Instant (June 2026) - Intelligence, Performance & Price...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#system prompts`, `#leaks`, `#GitHub`, `#LLM`

---

<a id="item-7"></a>
## [Canada's AI strategy should avoid secret Palantir deals](https://www.readtheline.ca/p/al-vigier-canadas-ai-strategy-shouldnt) ⭐️ 7.0/10

An article argues that Canada's new national AI strategy, 'AI for All,' should not include secretive contracts with Palantir Technologies, a US data analytics firm known for government surveillance work. This debate highlights tensions between national security, privacy, and sovereignty in AI procurement, potentially influencing how Canada and other nations choose AI vendors. Palantir's software, including Gotham and Foundry, is used by US intelligence and defense agencies, raising concerns about data sovereignty and surveillance when deployed in Canada.

hackernews · ClearwayLaw · Jul 6, 00:04 · [Discussion](https://news.ycombinator.com/item?id=48799256)

**Background**: Canada launched its 'AI for All' strategy in June 2026, emphasizing responsible and sovereign AI development. Palantir Technologies, co-founded by Peter Thiel, specializes in data integration and analytics for government and corporate clients, but has faced criticism for its role in expanding surveillance and immigration enforcement.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Palantir_Technologies">Palantir Technologies</a></li>
<li><a href="https://ised-isde.canada.ca/site/ised/en/canadas-national-artificial-intelligence-strategy-ai-all">Canada’s National Artificial Intelligence Strategy: AI for All</a></li>
<li><a href="https://www.pm.gc.ca/en/news/news-releases/2026/06/04/prime-minister-carney-launches-ai-all-canadas-new-national-artificial">Prime Minister Carney launches AI for All: Canada’s new ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely oppose Palantir's involvement, with some calling it a national security threat and advocating for domestic or allied alternatives. One commenter cautioned that such calls might be self-serving from Canadian companies seeking sole-source contracts.

**Tags**: `#AI policy`, `#national security`, `#Palantir`, `#Canada`, `#government contracts`

---

<a id="item-8"></a>
## [AI Tutor Boosts Learning by 0.71-1.30 SD, but Critics Question Study](https://intextbooks.science.uu.nl/workshop2026/files/itb26_s1s2.pdf) ⭐️ 7.0/10

A study from Dartmouth College reports that an AI tutor, using Claude Sonnet 4.6 to grade constructed-response questions and a RAG chat assistant, improved student outcomes by 0.71 to 1.30 standard deviations in a multivariate calculus course. If validated, such large effect sizes could revolutionize personalized education by scaling one-on-one tutoring, but the lack of randomization and small sample size raise concerns about the reliability of the results. Only about 16 students (11% of the group) achieved 'full engagement' with the AI tutor, and the study used statistical modeling to adjust for past grades instead of a randomized controlled trial.

hackernews · jonahbard · Jul 5, 18:47 · [Discussion](https://news.ycombinator.com/item?id=48796817)

**Background**: Effect size measures the magnitude of an intervention's impact, typically in standard deviation units. In education research, an effect size above 0.4 is considered large, and values above 1.0 are rare. Randomized controlled trials (RCTs) are the gold standard for causal inference, as they eliminate selection bias.

<details><summary>References</summary>
<ul>
<li><a href="https://visible-learning.org/hattie-ranking-influences-effect-sizes-learning-achievement/">Hattie effect size list - 256 Influences Related To Achievement Context matters: Interpreting effect sizes in education ... Using Effect Size—or Why the P Value Is Not Enough - PMC Effect Size Basics: Understanding the Strength of a Program's ... Interpreting Effect Sizes of Education Interventions How Big Are Effect Sizes in International Education Studies?</a></li>
<li><a href="https://demo.collow.ai/course/view.php?id=95">Course: Course Outline: Conducting a Randomized Controlled Trial ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism, noting that the headline result applies only to fully engaged students (11% of the sample), and that the lack of randomization and potential Hawthorne effect undermine the findings. Some also argued the system is more a practice quiz platform with AI grading than a true tutor.

**Tags**: `#AI in Education`, `#EdTech`, `#LLM`, `#Research`, `#Hacker News Discussion`

---

<a id="item-9"></a>
## [Website Cataloging Computers in Movies and TV](https://www.starringthecomputer.com/computers.html) ⭐️ 7.0/10

Starring the Computer is a website that catalogs computers featured in movies and TV shows, with community discussion on iconic hardware and its cinematic appearances. This site appeals to tech enthusiasts and film buffs by documenting the intersection of computing history and pop culture, preserving the legacy of classic hardware. The website lists computers from various eras, with community comments providing additional context such as the reuse of IBM AN-FSQ-7 panels from the 1950s SAGE system in many movies.

hackernews · gitowiec · Jul 5, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48796093)

**Background**: Many movies and TV shows feature computers that are either period-appropriate or visually striking. Starring the Computer documents these appearances, often with photos and details about the hardware. The site is a niche resource for retro computing enthusiasts and film historians.

**Discussion**: Commenters discuss the authenticity of computer depictions, such as the 6502 assembly code in Westworld being anachronistic. They also note that some props, like IBM panels, are rented from prop houses and appear in many productions.

**Tags**: `#computer history`, `#movies`, `#hardware`, `#pop culture`, `#retro computing`

---

<a id="item-10"></a>
## [Free Online Book on Compilers and Language Design](https://dthain.github.io/books/compiler/) ⭐️ 7.0/10

A free online book titled 'Introduction to Compilers and Language Design' by Douglas Thain has been released, offering a practical project-based approach to learning compilers. 这本书为学生和开发者提供了易于上手、动手实践的编译器学习资源，填补了理论教材与实际实现之间的空白。 The book includes a step-by-step project to build a working C-style compiler, and has received strong community endorsement on Hacker News with 277 points and 45 comments.

hackernews · AlexeyBrin · Jul 5, 11:54 · [Discussion](https://news.ycombinator.com/item?id=48793454)

**Background**: Compilers translate high-level programming languages into machine code. Learning compiler design traditionally involves dense textbooks like the 'Dragon Book', which can be daunting for beginners. This new book aims to make the topic more approachable through hands-on projects.

**Discussion**: Commenters praised the book's practical approach, with one former student calling it the best class they took. Others suggested complementary resources like C4 and C4x86 for further study, while one commenter noted the book's focus on C and its idiosyncrasies.

**Tags**: `#compilers`, `#language design`, `#education`, `#programming`

---

<a id="item-11"></a>
## [New es40 Fork Runs Windows 2000 on DEC Alpha Emulator](https://raymii.org/s/blog/Run_Windows_2000_for_Dec_Alpha_on_a_new_es40_fork.html) ⭐️ 7.0/10

A new fork of the es40 emulator enables running Windows 2000 for DEC Alpha on modern x86_64 systems, reviving a long-lost platform. This project preserves a piece of computing history, allowing enthusiasts to experience Windows 2000 on the Alpha architecture, which was discontinued after RC2. The fork specifically targets Windows 2000 RC2 for Alpha, as later builds dropped Alpha support. It emulates the AlphaServer ES 40 hardware on x86_64 hosts.

hackernews · jandeboevrie · Jul 5, 13:47 · [Discussion](https://news.ycombinator.com/item?id=48794302)

**Background**: DEC Alpha was a 64-bit RISC architecture introduced in 1992, known for high performance. Windows NT and early Windows 2000 betas supported Alpha, but Microsoft ended support after NT 4.0 and Windows 2000 RC2. The es40 emulator is a portable emulator for the AlphaServer ES 40, originally capable of running OpenVMS and Linux.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DEC_Alpha">DEC Alpha - Wikipedia</a></li>
<li><a href="https://github.com/ES40-Emu/es40">GitHub - ES 40 - Emu / es 40 : AlphaServer ES 40 emulator · GitHub</a></li>
<li><a href="https://sourceforge.net/projects/es40/files/">AlphaServer ES 40 Emulator - Browse Files at SourceForge.net</a></li>

</ul>
</details>

**Discussion**: Commenters expressed nostalgia, with some recalling using Windows 2000 Beta on DEC Alphastations. One noted that emulating Alpha on x86_64 was not foreseen by Alpha designers, highlighting the project's novelty.

**Tags**: `#emulation`, `#retro computing`, `#DEC Alpha`, `#Windows 2000`, `#open source`

---

<a id="item-12"></a>
## [sqlite-utils 4.0rc2: AI catches critical bugs before release](https://simonwillison.net/2026/Jul/5/sqlite-utils-fable/#atom-everything) ⭐️ 7.0/10

Simon Willison used Claude Fable to review sqlite-utils 4.0rc1, uncovering five release-blocking bugs including a data-loss bug in delete_where(). After 37 prompts and 34 commits, sqlite-utils 4.0rc2 was released with fixes. This demonstrates how AI coding agents can significantly improve software quality by catching subtle bugs before major releases, potentially saving months of maintenance. It also highlights the practical value of AI in real-world software engineering workflows. The most critical bug was in Table.delete_where(), which left the connection in an uncommitted transaction, causing all subsequent operations to silently lose data. The review cost approximately $149.25 in Claude Fable usage and involved 1,321 lines added and 190 removed across 30 files.

rss · Simon Willison · Jul 5, 01:00

**Background**: sqlite-utils is a Python library and CLI tool for manipulating SQLite databases, widely used in the Datasette ecosystem. Claude Fable is Anthropic's latest state-of-the-art model, known for its ability to find software vulnerabilities. Semantic versioning (SemVer) uses a three-part version number (Major.Minor.Patch) to communicate compatibility changes.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable">Claude Fable</a></li>
<li><a href="https://en.wikipedia.org/wiki/Software_versioning">Software versioning - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#sqlite-utils`, `#software engineering`, `#release management`, `#Claude`

---

<a id="item-13"></a>
## [Google Unveils Gemini Omni Flash Multimodal AI](https://www.reddit.com/r/singularity/comments/1uoe6we/gemini_omni_flash/) ⭐️ 7.0/10

Google DeepMind has announced Gemini Omni Flash, a new multimodal AI model that combines Gemini's intelligence with generative media models, enabling video creation and editing from any input. This model represents a significant leap in multimodal AI, making high-quality video creation accessible to both professionals and beginners, and could transform industries like marketing and content production. Gemini Omni Flash is optimized for video generation, offering video output alongside text responses in a single model, and is currently available in preview on Google's enterprise agent platform.

reddit · r/singularity · /u/Gaiden206 · Jul 5, 21:33

**Background**: Gemini Omni Flash builds on Google's Gemini family of multimodal models, which process text, images, audio, and video. ComfyUI, mentioned in the Reddit post, is an open-source node-based interface for running diffusion models like Stable Diffusion, often used for AI image and video generation workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-omni-flash/">Gemini Omni Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://deepmind.google/models/gemini-omni/">Gemini Omni — Google DeepMind</a></li>
<li><a href="https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/gemini/omni-flash-preview">Gemini Omni Flash Preview | Gemini Enterprise Agent Platform ...</a></li>

</ul>
</details>

**Discussion**: The Reddit community expressed excitement about Gemini Omni Flash, with many users discussing its potential for video editing and integration with ComfyUI. Some users raised concerns about accessibility and pricing, while others praised the model's capabilities.

**Tags**: `#AI`, `#Gemini`, `#multimodal`, `#Google`, `#machine learning`

---

<a id="item-14"></a>
## [US and China Dominate Global AI Model Training](https://www.reddit.com/r/singularity/comments/1ungtw2/us_and_chinese_companies_train_almost_all_of_the/) ⭐️ 7.0/10

A Reddit post highlights that US and Chinese companies are responsible for training nearly all widely-used AI models, underscoring the concentration of AI development in two countries. This concentration of AI development in the US and China has significant geopolitical and economic implications, potentially shaping global tech competition and policy. The post does not provide specific model names or statistics, but it reflects a widely observed trend in the AI industry.

reddit · r/singularity · /u/Status_Commission264 · Jul 4, 18:48

**Background**: AI model training requires massive computational resources, data, and talent, which are concentrated in a few countries. The US and China have leading tech companies like OpenAI, Google, Baidu, and Alibaba that invest heavily in AI research and development.

**Discussion**: The Reddit discussion likely includes comments on the implications of this duopoly, concerns about national security, and calls for more distributed AI development.

**Tags**: `#AI`, `#geopolitics`, `#industry trends`, `#machine learning`

---

<a id="item-15"></a>
## [OpenAI Releases Codex Plugin for Claude Code](https://github.com/openai/codex-plugin-cc) ⭐️ 7.0/10

OpenAI has released an official plugin that allows users to invoke Codex from within Claude Code for code review and task delegation. This plugin bridges two major AI coding assistants, enabling developers to leverage Codex's specialized capabilities without leaving their Claude Code workflow, potentially improving productivity and code quality. The plugin supports three modes: standard code review, adversarial review, and task handoff to Codex. It is written in JavaScript and has gained 55 stars on GitHub in the first 24 hours.

ossinsight · openai · Jul 6, 02:23

**Background**: Codex is OpenAI's AI-powered code review and generation tool, while Claude Code is Anthropic's coding assistant. The Model Context Protocol (MCP) is an open standard for connecting LLMs to external tools, but this plugin uses a direct integration rather than MCP.

<details><summary>References</summary>
<ul>
<li><a href="https://community.openai.com/t/introducing-codex-plugin-for-claude-code/1378186">Introducing Codex Plugin for Claude Code - Codex - OpenAI Developer Community</a></li>
<li><a href="https://github.com/openai/codex-plugin-cc">GitHub - openai/codex-plugin-cc: Use Codex from Claude Code to review code or delegate tasks. · GitHub</a></li>

</ul>
</details>

**Tags**: `#AI`, `#code review`, `#OpenAI`, `#Claude Code`, `#plugin`

---

<a id="item-16"></a>
## [RedKnot: Head-Aware KV Cache for Efficient Long-Context LLM Serving](https://github.com/rednote-machine-learning/RedKnot) ⭐️ 7.0/10

RedKnot introduces Head-Aware KV Reuse and SegPagedAttention to improve efficiency in serving long-context large language models by decomposing the KV cache along attention heads. This addresses the dominant KV cache bottleneck in long-context LLM serving, potentially reducing memory usage and latency, which is critical for scaling LLMs to longer sequences. RedKnot breaks the conventional monolithic KV cache by decomposing it along KV heads, whose importance and effective attention ranges vary significantly. SegPagedAttention allows each head to own a compact KV page list, avoiding additive mask construction.

ossinsight · rednote-machine-learning · Jul 6, 02:23

**Background**: Large language models (LLMs) use a KV cache to store key-value pairs from previous tokens, which grows linearly with sequence length and becomes a bottleneck for long-context serving. Traditional methods treat the cache as a monolithic block, ignoring that different attention heads have varying importance and effective ranges. RedKnot exploits this head-level variation to improve efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.06256">RedKnot: Efficient Long-Context LLM Serving with Head-Aware ...</a></li>
<li><a href="https://github.com/rednote-machine-learning/RedKnot">GitHub - rednote-machine-learning/RedKnot: Efficient Long-Context...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#KV-cache`, `#efficient-inference`, `#long-context`, `#Python`

---