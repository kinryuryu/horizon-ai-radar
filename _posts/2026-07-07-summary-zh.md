---
layout: default
title: "Horizon Summary: 2026-07-07 (ZH)"
date: 2026-07-07
lang: zh
---

> 从 31 条内容中筛选出 16 条重要资讯。

---

1. [Anthropic 发现 LLM 中存在全局工作空间证据](#item-1) ⭐️ 9.0/10
2. [Fable 的 AI 在 KernelBench 上登顶，暗示 RSI 循环](#item-2) ⭐️ 9.0/10
3. [Claude 展现出类似意识的核心](#item-3) ⭐️ 9.0/10
4. [OpenWrt One 开源硬件路由器发布](#item-4) ⭐️ 8.0/10
5. [GLM 5.2 与即将到来的 AI 利润崩溃](#item-5) ⭐️ 8.0/10
6. [腾讯发布 Hy3：295B 参数 MoE 模型，21B 活跃参数](#item-6) ⭐️ 8.0/10
7. [LeRobot v0.6.0：想象、评估、改进](#item-7) ⭐️ 8.0/10
8. [Hugging Face 重构内核基础设施](#item-8) ⭐️ 8.0/10
9. [伊利诺伊州长签署全美最严 AI 法律之一](#item-9) ⭐️ 8.0/10
10. [Linux 成功移植到仅有 2MB 内存的 Atari Jaguar](#item-10) ⭐️ 7.0/10
11. [AI 时代学习编程仍有价值](#item-11) ⭐️ 7.0/10
12. [sqlite-utils 4.0rc3：复合外键与大小写不敏感列名](#item-12) ⭐️ 7.0/10
13. [Photoroom PRX 数据策略：质量与多样性](#item-13) ⭐️ 7.0/10
14. [日本计划到 2040 年开发自主 AI 并部署 1000 万台机器人](#item-14) ⭐️ 7.0/10
15. [用户测试 Gemini Omni 处理手机视频](#item-15) ⭐️ 7.0/10
16. [OmniRoute：免费 AI 网关，支持 160 多家提供商](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 发现 LLM 中存在全局工作空间证据](https://www.reddit.com/r/singularity/comments/1up68u3/a_global_workspace_in_language_models_new/) ⭐️ 9.0/10

Anthropic 研究人员在语言模型中发现了一个“全局工作空间”，即一个跨层和跨上下文整合信息的共享表征空间（J-space），相关细节已在新论文中阐述。 这一发现通过提供 LLM 如何整合信息的机制性理解，推动了 AI 可解释性研究，有望带来更安全、更可控的模型。 J-space 定义为给定层微小扰动后最终 logits 的预期变化，实验表明交换 J-space 内容可以重定向 Claude 的推理过程。

reddit · r/singularity · /u/Tinac4 · 7月6日 18:42

**背景**: 全局工作空间理论（GWT）是一个认知框架，将意识比作一个舞台，不同脑区竞争进入全局工作空间。Anthropic 的研究将这一概念应用于 LLM，表明模型可能具有类似的整合中枢。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/global-workspace">A global workspace in language models \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/research/team/interpretability">Interpretability Research \ Anthropic</a></li>
<li><a href="https://customgpt.ai/ai-interpretability-research-from-anthropic/">Anthropic 's Groundbreaking AI Interpretability Research</a></li>

</ul>
</details>

**社区讨论**: 评论者对这项研究表示兴奋，一些人注意到与早期实验（如复制数学求解层）的相似之处。但一位用户警告不要过度解读与人类意识的比较，指出 J-space 本质上是一种信息几何度量。

**标签**: `#AI interpretability`, `#language models`, `#Anthropic`, `#machine learning research`

---

<a id="item-2"></a>
## [Fable 的 AI 在 KernelBench 上登顶，暗示 RSI 循环](https://www.reddit.com/r/singularity/comments/1uowkp0/fable_5_sits_at_the_top_of_kernelbench_jack_clark/) ⭐️ 9.0/10

Fable 的 AI 通过编写单个 CUDA megakernel，在 KernelBench-Mega 上实现了 18.71 倍的加速，超越了包括 Claude Opus 4.8 和 GPT-5.5 在内的所有其他模型。Jack Clark 称这是“RSI 循环的开始”。 这一里程碑展示了 AI 自主优化 GPU 内核的能力日益增强，这是 AI 研发中的基础任务。它使递归自我改进（RSI）更接近现实，即 AI 系统可以在没有人类干预的情况下自我改进。 该解决方案每个解码 token 仅启动一个协作内核，而其他顶级方案需要 4 到 14 次单独的内核启动。基准测试使用 RTX PRO 6000 Blackwell GPU，加速比相对于优化的 PyTorch 基线测量。

reddit · r/singularity · /u/manubfr · 7月6日 12:56

**背景**: KernelBench 是一个评估 LLM 编写快速且正确的 GPU 内核能力的基准测试。Megakernel 是执行多个功能的单个 GPU 内核，可减少启动开销。递归自我改进（RSI）指的是 AI 系统能够自主改进自身能力，可能导致快速进步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kernelbench.com/">kernelbench .com: Agentic GPU Kernel Benchmark Results</a></li>
<li><a href="https://github.com/ScalingIntelligence/KernelBench">ScalingIntelligence/ KernelBench : KernelBench : Can LLMs Write GPU ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区表达了兴奋和怀疑。许多人称赞这一技术成就，而一些人质疑单个基准测试是否真正标志着 RSI。其他人则强调了可重复性的重要性以及开源验证的必要性。

**标签**: `#AI`, `#GPU kernel`, `#RSI`, `#KernelBench`, `#CUDA`

---

<a id="item-3"></a>
## [Claude 展现出类似意识的核心](https://www.reddit.com/r/singularity/comments/1up59ul/whats_at_the_center_of_claudes_mind/) ⭐️ 9.0/10

Anthropic 的新论文揭示，Claude 已形成一小部分内部神经模式，其功能类似于人类有意识可访问的处理过程，表明大语言模型中存在可访问处理与自动处理的区分。 这项研究可能彻底改变对 AI 认知的理解，并对 AI 对齐和可解释性产生深远影响，因为它表明大语言模型可能拥有一个类似意识的核心，可能影响安全性和可控性。 该论文发表在 transformer-circuits.pub 上，包含 neuronpedia.org 上的演示，并由 Anthropic 在 X 上宣布。这些发现与神经科学中的可访问意识概念相似，即某些神经活动可被报告并用于推理。

reddit · r/singularity · /u/10b0t0mized · 7月6日 18:09

**背景**: 像 Claude 这样的大语言模型是基于海量文本数据训练的神经网络，用于生成和理解语言。神经科学家区分有意识（可访问）和无意识（自动）的大脑处理过程。Anthropic 的可解释性研究旨在通过分析 AI 系统的内部运作来理解并确保其安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/team/interpretability">Interpretability Research \ Anthropic</a></li>
<li><a href="https://plato.stanford.edu/entries/consciousness-neuroscience/">The Neuroscience of Consciousness (Stanford Encyclopedia of Philosophy)</a></li>

</ul>
</details>

**标签**: `#AI alignment`, `#interpretability`, `#LLM`, `#consciousness`, `#Anthropic`

---

<a id="item-4"></a>
## [OpenWrt One 开源硬件路由器发布](https://openwrt.org/toh/openwrt/one) ⭐️ 8.0/10

OpenWrt 项目正式发布了 OpenWrt One，这是一款专为运行 OpenWrt 固件设计的开源硬件路由器，不含外壳和天线的价格为 89 美元。 这标志着 OpenWrt 项目推出了首款专用开源硬件路由器，提供了一个完全开放且对黑客友好的平台，确保长期固件支持和社区驱动开发。 该路由器支持双频 Wi-Fi 6，配备两个以太网端口、三个 USB 端口，基于联发科 SoC。Wi-Fi 7 版本（OpenWrt Two）已在开发中。

hackernews · peter_d_sherman · 7月6日 18:23 · [社区讨论](https://news.ycombinator.com/item?id=48808482)

**背景**: OpenWrt 是一种流行的路由器及嵌入式设备开源固件，提供高级功能并延长设备寿命。OpenWrt One 是该项目的首个官方硬件参考设计，确保完全兼容性和社区支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/networking/open-source-openwrt-one-router-released-at-usd89-hacker-friendly-device-sports-two-ethernet-ports-three-usb-ports-with-dual-band-wi-fi-6">Open-source OpenWrt One router released at $89 — 'hacker-friendly device' sports two Ethernet ports, three USB ports, with dual-band Wi-Fi 6 | Tom's Hardware</a></li>

</ul>
</details>

**社区讨论**: 社区成员对 OpenWrt One 表示热情，有人提到即将推出的 Wi-Fi 7 版本。用户赞赏其价格和开放性，但也有人指出与 OPNSense 等替代方案相比，安装复杂且文档有待改进。

**标签**: `#OpenWrt`, `#open hardware`, `#router`, `#networking`, `#open source`

---

<a id="item-5"></a>
## [GLM 5.2 与即将到来的 AI 利润崩溃](https://martinalderson.com/posts/the-upcoming-ai-margin-collapse-part-1-glm-5-2/) ⭐️ 8.0/10

一篇分析文章认为，以 Z.ai 的 GLM 5.2 模型为代表的 AI 推理成本快速下降，将导致整个 AI 行业利润崩溃，并引发关于成本降低本身是否会导致商品化的讨论。 这很重要，因为如果推理成本持续暴跌，AI 模型提供商可能难以维持盈利，从而可能重塑竞争格局并加速 AI 模型的商品化。 GLM 5.2 是一个大规模推理模型，拥有 100 万 token 的上下文窗口，专为长期代理工作流和复杂多步骤自动化设计。据报道，AI 推理成本在两年内下降了超过 99%。

hackernews · martinald · 7月6日 20:14 · [社区讨论](https://news.ycombinator.com/item?id=48809877)

**背景**: AI 推理成本是指运行训练好的模型以生成输出的计算费用。由于模型效率提升和竞争，这些成本迅速下降，导致有人预测 AI 模型将变得商品化，利润将转移到应用和集成层面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_(AI)">GLM (AI) - Wikipedia</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM - 5 . 2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://openrouter.ai/z-ai/glm-5.2">GLM 5 . 2 - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**社区讨论**: 评论者就成本下降本身是否会导致商品化展开辩论，他们引用了云计算和开源办公套件等例子，这些领域成本下降了但利润率仍然保持。一些人认为中国的竞争压力阻止了价格合谋，而另一些人则指出持续的再训练成本可能维持利润率。

**标签**: `#AI`, `#economics`, `#LLMs`, `#market dynamics`, `#commoditization`

---

<a id="item-6"></a>
## [腾讯发布 Hy3：295B 参数 MoE 模型，21B 活跃参数](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

腾讯发布了 Hy3，这是一个 295B 参数的混合专家（MoE）模型，拥有 21B 活跃参数和 3.8B MTP 层参数，采用 Apache 2.0 许可证。它优于同类模型，并可媲美参数规模大 2-5 倍的模型。 此次发布意义重大，因为它提供了一款来自中国主要科技公司的极具竞争力的开源 MoE 模型，并在 OpenRouter 上免费使用至 7 月 21 日。它展示了中国 AI 的快速进步，并为社区提供了一个强大而高效的模型，适用于各种应用。 完整模型在 Hugging Face 上为 598GB，FP8 量化版本为 300GB，支持 256K token 的上下文长度。该模型由腾讯 Hy 团队开发，并在后训练阶段整合了来自 50 多个产品的反馈。

rss · Simon Willison · 7月6日 23:57

**背景**: 混合专家（MoE）是一种神经网络架构，它使用条件计算，对每个输入仅激活一部分参数，从而实现大规模模型的高效推理。活跃参数（21B）是每次前向传播时使用的参数，而总参数（295B）代表完整的模型大小。FP8 量化通过使用 8 位浮点数表示权重和激活值，减小模型大小并加速推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://www.ibm.com/think/topics/mixture-of-experts">What is mixture of experts? | IBM</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#LLM`, `#MoE`, `#Tencent`

---

<a id="item-7"></a>
## [LeRobot v0.6.0：想象、评估、改进](https://huggingface.co/blog/lerobot-release-v060) ⭐️ 8.0/10

LeRobot v0.6.0 新增了想象、评估和改进机器人策略的能力，推动了开源机器人研究的发展。 此次发布使研究人员和开发者能够更有效地设计和优化机器人学习算法，加速具身智能和现实世界机器人应用的进展。 此次更新包括策略想象工具、评估基准和改进循环，并与 Hugging Face Hub 集成，用于共享数据集和模型。

rss · Hugging Face Blog · 7月7日 00:00

**背景**: LeRobot 是一个开源的 Python 库，用于端到端的机器人学习，从硬件接口到可扩展训练和实时推理。它提供了多模态机器人数据的统一数据结构，并使用 Parquet 格式进行高效存储。机器人策略是将传感器输入映射到动作的 AI 模型，使机器人能够自主执行任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/huggingface/lerobot">GitHub - huggingface/lerobot: LeRobot: Making AI for Robotics ...</a></li>
<li><a href="https://www.emergentmind.com/topics/lerobot">LeRobot : Open-Source Robot Learning Platform</a></li>
<li><a href="https://learnopencv.com/vision-language-action-models-lerobot-policy/">Vision Language Action Models (VLA) & Policies for Robots</a></li>

</ul>
</details>

**标签**: `#robotics`, `#open-source`, `#AI`, `#reinforcement learning`, `#Hugging Face`

---

<a id="item-8"></a>
## [Hugging Face 重构内核基础设施](https://huggingface.co/blog/revamped-kernels) ⭐️ 8.0/10

Hugging Face 宣布对其内核基础设施进行重大更新，包括一个新的内核构建器，可自动将 C++ 内核编译成支持 CUDA、ROCm、Metal 和 Universal 等多个后端的 PyTorch 扩展。 这些更新显著提升了机器学习社区的性能和开发者体验，使得在多种硬件平台上实现更快的模型训练和推理成为可能。 内核构建器自动化了 PyTorch 扩展的构建过程，而内核中心允许跨批量大小共享和基准测试优化的 CUDA 内核，以实现实际性能调优。

rss · Hugging Face Blog · 7月6日 00:00

**背景**: 在机器学习中，内核指的是加速矩阵乘法等操作的底层 GPU 程序。Hugging Face 的内核基础设施简化了这些自定义内核的开发和分发，这些内核对于实现深度学习模型的高性能至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/huggingface/kernel-builder">huggingface/ kernel -builder | DeepWiki</a></li>
<li><a href="https://blog.aifoundry.org/p/from-ai-agents-to-faster-kernels">From AI Agents to Faster Kernels - AI Foundry</a></li>
<li><a href="https://botengine.co/cuda-kernels-how-do-you-build-one-for-production/">CUDA Kernels : How Do You Build One for Production? - Bot-Engine</a></li>

</ul>
</details>

**标签**: `#Hugging Face`, `#machine learning`, `#kernels`, `#AI infrastructure`

---

<a id="item-9"></a>
## [伊利诺伊州长签署全美最严 AI 法律之一](https://www.reddit.com/r/singularity/comments/1up8rdi/gov_pritzker_puts_signature_on_senate_bill_315/) ⭐️ 8.0/10

伊利诺伊州长 JB Pritzker 签署了参议院第 315 号法案，使伊利诺伊成为继加州和纽约之后第三个对前沿 AI 系统施加严格问责要求的州。 该法律为美国 AI 监管设立了新标准，要求大型 AI 公司进行年度独立审计、安全披露和举报人保护，可能影响联邦层面的监管。 该法律仅适用于年收入超过 5 亿美元的公司，要求对前沿 AI 模型的安全实践进行第三方审计并报告事件。

reddit · r/singularity · /u/SnoozeDoggyDog · 7月6日 20:12

**背景**: 前沿 AI 模型是最强大、最通用的 AI 系统，可能带来偏见、滥用或灾难性危害等风险。在缺乏全面联邦立法的情况下，伊利诺伊州的 SB 315 是美国各州制定 AI 法规这一日益增长趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/illinois-just-became-third-state-regulate-frontier-c1lte">Illinois Just Became the Third State to Regulate Frontier AI ....</a></li>
<li><a href="https://www.govtech.com/artificial-intelligence/illinois-landmark-ai-law-sets-a-new-standard-for-oversight">Illinois ’ Landmark AI Law Sets a New Standard for Oversight</a></li>
<li><a href="https://wgntv.com/news/illinois/gov-pritzker-puts-signature-on-senate-bill-315-one-of-toughest-ai-laws-in-country/">What is Senate Bill 315, signed into law by Illinois Gov. JB Pritzker as one of the toughest AI laws in the country to date?</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#policy`, `#Illinois`, `#ethics`, `#legislation`

---

<a id="item-10"></a>
## [Linux 成功移植到仅有 2MB 内存的 Atari Jaguar](https://cakehonolulu.github.io/linux-for-jaguar/) ⭐️ 7.0/10

一位开发者成功在 Atari Jaguar 游戏机上仅使用其原始的 2MB 内存启动了 Linux，并进入了 Busybox shell，无需任何专用硬件或烧录卡。 这一成就展示了在资源极度受限的复古硬件上运行现代操作系统的可行性，为爱好者项目和教学用途开辟了可能性。 该移植使用了较新的 Linux 内核，配置为无 MMU 和扁平内存模型，以适应 Jaguar 的 2MB 内存和定制的 Tom & Jerry 芯片。系统启动后进入 Busybox shell，提供了一个最小但可用的 Linux 环境。

hackernews · cakehonolulu · 7月6日 18:35 · [社区讨论](https://news.ycombinator.com/item?id=48808663)

**背景**: Atari Jaguar 于 1993 年发布，是一款 64 位游戏机，配备 68000 CPU、2MB 内存和定制协处理器。Linux 通常需要 MMU 和更多内存，因此将其移植到如此受限的硬件上是一项重大的技术挑战。Busybox 是一个多调用二进制文件，将许多 Unix 工具合并到一个可执行文件中，常用于嵌入式系统以节省空间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cakehonolulu.github.io/linux-for-jaguar/">Linux on the Atari Jaguar. No, really. - cakehonolulu's blog</a></li>
<li><a href="https://www.busybox.net/BusyBox.html">BusyBox - The Swiss Army Knife of Embedded Linux</a></li>

</ul>
</details>

**社区讨论**: 评论者对这一努力表示惊叹，有人指出 Jaguar 独特的架构，并建议通过使用 GPU/DSP 或通过卡带增加内存来增强功能。一位评论者回忆起几十年前见过类似的尝试，但对使用较新内核表示赞赏。

**标签**: `#Linux`, `#Retro Computing`, `#Atari Jaguar`, `#Embedded Systems`

---

<a id="item-11"></a>
## [AI 时代学习编程仍有价值](https://stevekrouse.com/learn-to-code) ⭐️ 7.0/10

Steve Krouse 发表观点文章，认为尽管 AI 取得进展，学习编程仍然有价值，引发了关于编程工作性质变化的深入讨论。 这场辩论影响着有志于成为开发者的人和教育者的职业决策，因为像大语言模型这样的 AI 工具正在重塑软件工程角色和成功所需的技能。 文章和评论强调，虽然 AI 可以自动化一些编码任务，但架构和最佳实践的基础知识仍然至关重要，工作越来越变成监督 AI 模型。

hackernews · stevekrouse · 7月6日 20:59 · [社区讨论](https://news.ycombinator.com/item?id=48810439)

**背景**: 长期以来，学习编程一直被视为技术职业的一项宝贵技能。最近 AI 的进步，特别是能够生成代码的大语言模型，引发了关于传统编程技能是否仍将相关的疑问。

**社区讨论**: 评论者表达了不同观点：有人将编程比作诗歌，认为它是一种职业前景有限的艺术形式；而另一些人则认为扎实的基础知识仍然至关重要，AI 主要自动化了开发的表层工作。

**标签**: `#programming`, `#AI`, `#career`, `#education`, `#software engineering`

---

<a id="item-12"></a>
## [sqlite-utils 4.0rc3：复合外键与大小写不敏感列名](https://simonwillison.net/2026/Jul/6/sqlite-utils/#atom-everything) ⭐️ 7.0/10

sqlite-utils 4.0rc3 引入了对复合外键的检查和创建支持，并遵循 SQLite 的大小写不敏感列名匹配约定。此候选版本还包含对 table.foreign_keys 属性的破坏性更改。 复合外键是用户长期要求的功能，支持更复杂的数据库关系，使 sqlite-utils 在数据建模方面更加强大。大小写不敏感列名匹配与 SQLite 行为一致，减少了从原始 SQL 迁移用户的意外。 对 table.foreign_keys 的破坏性更改意味着访问该属性的现有代码可能需要更新。此候选版本还包含许多其他修复和改进，自 rc2 以来变更日志显著增长。

rss · Simon Willison · 7月6日 05:40

**背景**: sqlite-utils 是一个用于操作 SQLite 数据库的 Python 库和命令行工具。外键强制表之间的引用完整性；复合外键涉及多个列，这在规范化数据库中很常见。SQLite 默认将列名视为大小写不敏感，但 sqlite-utils 之前并非如此，导致不一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sqlite.org/foreignkeys.html">SQLite Foreign Key Support</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#python`, `#database`, `#release`

---

<a id="item-13"></a>
## [Photoroom PRX 数据策略：质量与多样性](https://huggingface.co/blog/Photoroom/prx-part4-data) ⭐️ 7.0/10

Photoroom 在 Hugging Face 上发布了一篇详细博客，阐述了 PRX 文本到图像模型的数据策略，强调数据质量、多样性和数据整理技术以提升模型性能。 这为从业者提供了关于如何为生成式 AI 模型训练整理高质量数据集的可操作见解，这是模型开发中关键但常被忽视的方面。 该策略涵盖去重、过滤低质量样本以及确保风格和主题的多样性等技巧，并提供了 PRX 模型训练流程中的具体示例。

rss · Hugging Face Blog · 7月6日 15:30

**背景**: 数据整理是选择、清理和组织原始数据以提升机器学习模型性能和可靠性的过程。对于 PRX 这类文本到图像模型，训练数据的质量和多样性直接影响模型生成准确且多样化图像的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Photoroom">Photoroom ( Photoroom )</a></li>
<li><a href="https://huggingface.co/collections/Photoroom/prx">PRX - a Photoroom Collection | PRX text-to-image models</a></li>

</ul>
</details>

**标签**: `#data strategy`, `#machine learning`, `#data curation`, `#Hugging Face`, `#PRX`

---

<a id="item-14"></a>
## [日本计划到 2040 年开发自主 AI 并部署 1000 万台机器人](https://www.reddit.com/r/singularity/comments/1up0sin/japan_is_aiming_to_develop_its_own_ai_model_and/) ⭐️ 7.0/10

日本宣布了一项国家战略，通过包括软银、索尼、本田和 NEC 在内的 Noetra 联盟开发自己的 AI 模型，并计划到 2040 年在 18 个领域部署 1000 万台 AI 驱动的机器人。 这一举措减少了日本对外国 AI 技术的依赖，并应对严重的劳动力短缺，可能重塑全球 AI 和机器人领域的竞争格局。 该计划得到了日本经济产业省（METI）和创新机构 NEDO 的 61 亿美元投资支持，AI 模型将由政府正式委托的 Noetra 联盟开发。

reddit · r/singularity · /u/Distinct-Question-16 · 7月6日 15:34

**背景**: 日本面临劳动力减少的问题，且长期以来一直是工业机器人领域的领导者。由软银高管田叶博文领导的 Noetra 联盟旨在创建一个主权 AI 模型，为医疗、制造和养老等领域的下一代机器人提供动力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://asiatimes.com/2026/07/japan-rallies-tech-giant-alliance-to-build-sovereign-ai/">Japan rallies tech-giant alliance to build sovereign AI - Asia Times</a></li>
<li><a href="https://www.zerohedge.com/ai/japan-unveils-61-billion-sovereign-ai-plan-targeting-10-million-robots-across-18-sectors-2040">Japan Takes Next Step In $2.3 Trillion Plan With... | ZeroHedge</a></li>
<li><a href="https://www.rte.ie/news/newslens/2026/0701/1581186-japan-ai-robots/">Japan plans to have 10 m AI-equipped robots by 2040</a></li>

</ul>
</details>

**标签**: `#AI`, `#Robotics`, `#Japan`, `#National Strategy`, `#Industry Consortium`

---

<a id="item-15"></a>
## [用户测试 Gemini Omni 处理手机视频](https://www.reddit.com/r/singularity/comments/1uowx4u/i_tested_gemini_omni_on_my_phone_footage/) ⭐️ 7.0/10

一位 Reddit 用户用自己的手机视频测试了 Google 的 Gemini Omni 模型，并分享了结果，引发了社区对该模型能力的讨论。 这次真实世界测试提供了 Gemini Omni 在个人非精选视频上表现的重要见解，对于理解其在视频生成和编辑中的实际用途至关重要。 Gemini Omni Flash 是一种多模态 AI 模型，能够生成和编辑具有动态摄像机运动和原生音频的视频，正如 Google DeepMind 所描述的那样。

reddit · r/singularity · /u/voice_of_the_future · 7月6日 13:10

**背景**: 多模态 AI 整合文本、音频和视频等多种数据类型，实现全面理解。Gemini Omni 是 Google 最新的视频生成模型，接替 Veo 3.1，允许用户通过对话式交互创建和编辑视频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/gemini-omni/">Gemini Omni — Google DeepMind</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multimodal_AI">Multimodal AI</a></li>
<li><a href="https://gemini.google/us/overview/video-generation/?hl=en">Gemini Omni – Create & edit videos as easy as having a conversation</a></li>

</ul>
</details>

**标签**: `#Gemini Omni`, `#multimodal AI`, `#AI testing`, `#Google AI`

---

<a id="item-16"></a>
## [OmniRoute：免费 AI 网关，支持 160 多家提供商](https://github.com/diegosouzapw/OmniRoute) ⭐️ 7.0/10

OmniRoute 是一个免费的开源 AI 网关，过去 24 小时内在 GitHub 上获得了 11 颗星，它提供一个兼容 OpenAI 的单一端点，可连接超过 160 家 AI 提供商，其中 50 多家提供免费服务。 该工具通过消除管理多个 API 的需求，简化了开发者的 AI 集成，其令牌压缩功能可将成本降低 15-95%，使 AI 更易获取且更经济实惠。 OmniRoute 支持 RTK+Caveman 堆叠压缩以节省令牌、智能自动回退、MCP/A2A 协议、多模态 API，并可作为桌面应用或 PWA 使用。

ossinsight · diegosouzapw · 7月7日 02:11

**背景**: AI 网关充当多个 AI 模型提供商的统一接口，简化 API 管理并降低成本。RTK（Rust Token Killer）和 Caveman 等令牌压缩技术通过优化输入/输出来节省令牌。MCP（模型上下文协议）和 A2A（代理间协议）是用于代理互操作性的互补协议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/pitbaden/omniroute">GitHub - pitbaden/ omniroute : OmniRoute is an AI gateway for...</a></li>
<li><a href="https://www.everydev.ai/tools/omniroute">OmniRoute - Open Source AI Gateway Router | EveryDev. ai</a></li>
<li><a href="https://www.aitoolnet.com/omniroute">OmniRoute - Free AI Gateway for Multi-Provider LLMs - Aitoolnet</a></li>

</ul>
</details>

**标签**: `#AI Gateway`, `#TypeScript`, `#Open Source`, `#API`, `#Token Compression`

---