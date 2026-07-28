---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> 从 36 条内容中筛选出 17 条重要资讯。

---

1. [Anthropic 明确其对开放权重 AI 模型的立场](#item-1) ⭐️ 9.0/10
2. [研究人员攻破沃尔沃/埃契尔车队平台，获得完全控制权](#item-2) ⭐️ 9.0/10
3. [Moonshot AI 发布 2.8 万亿参数 Kimi K3 权重](#item-3) ⭐️ 9.0/10
4. [vLLM v0.26.0 新增 Inkling 支持与 DeepSeek-V4 优化](#item-4) ⭐️ 8.0/10
5. [python-build-standalone 驱动现代 Python 工具链](#item-5) ⭐️ 8.0/10
6. [缺失下划线导致无辜者被错判入狱 18 个月](#item-6) ⭐️ 8.0/10
7. [法官驳回谷歌利用 DMCA 阻止爬取的企图](#item-7) ⭐️ 8.0/10
8. [LLM 代币中继市场助长欺诈与转售](#item-8) ⭐️ 8.0/10
9. [NVIDIA Cosmos-H-Dreams：手术机器人的实时生成式仿真](#item-9) ⭐️ 8.0/10
10. [OpenAI 拒绝加入英伟达的开放安全 AI 联盟](#item-10) ⭐️ 8.0/10
11. [用户通过 25GbE 在 80 块 RTX 5090 上运行 Kimi K3](#item-11) ⭐️ 8.0/10
12. [案例研究：用 HTMX 替换 React 的论坛平台](#item-12) ⭐️ 7.0/10
13. [Paged Out #9：免费技术杂志发布](#item-13) ⭐️ 7.0/10
14. [FeyNoBg：开源背景移除模型与训练库](#item-14) ⭐️ 7.0/10
15. [Libsm64：将《超级马里奥 64》作为可复用库嵌入游戏引擎](#item-15) ⭐️ 7.0/10
16. [Ethan Mollick 的 AI 指南从聊天转向代理系统](#item-16) ⭐️ 7.0/10
17. [Ninfer 在 RTX 5090 上实现 Qwen 3.6 35B 每秒 700 token 的推理速度](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 明确其对开放权重 AI 模型的立场](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 9.0/10

Anthropic 发布官方立场，声明其不主张禁止开放权重模型，而是呼吁对所有足够强大的 AI 模型（包括开放和封闭模型）进行强制性安全测试。 这一来自领先 AI 公司的政策声明可能影响监管辩论，因为强制性安全测试若成本高昂或审批受阻，可能实质上限制开放权重模型，进而影响开源 AI 开发和竞争格局。 Anthropic CEO Dario Amodei 还支持禁止向中国销售芯片并打击走私，批评者认为这与他声称反对禁令的立场相矛盾。该公司未明确说明由谁管理安全测试或采用何种标准。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重 AI 模型是指其训练参数（权重）公开发布，允许任何人下载、修改和运行的模型。与完全开源模型不同，开放权重模型可能不包含训练数据或代码。强制性安全测试（即“评估”）是在部署前评估风险的测试，各国政府正越来越多地考虑将其作为前沿 AI 模型的强制要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_safety">AI safety - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为 Anthropic 的立场实质上是在禁止开放权重模型，认为由政府或行业机构控制的强制性测试可能被用来阻止开放模型。还有人指责 Anthropic 虚伪，一方面支持硬件出口禁令，另一方面反对软件禁令，并优先考虑利润而非安全。

**标签**: `#AI safety`, `#open-weights models`, `#regulation`, `#Anthropic`, `#policy`

---

<a id="item-2"></a>
## [研究人员攻破沃尔沃/埃契尔车队平台，获得完全控制权](https://eaton-works.com/2026/07/27/my-eicher-hack/) ⭐️ 9.0/10

安全研究员 Eaton Works 发现并利用了沃尔沃/埃契尔 My Eicher 车队管理平台的一个严重漏洞，可实现完全账户接管并控制所有用户和车辆。该漏洞经过负责任披露，并在 17 天内得到修复。 该漏洞凸显了集中式云端车队管理系统存在的严重风险，一个缺陷即可危及整个车队。这强调了汽车远程信息处理领域加强安全性的紧迫性，并强化了维修权运动。 该漏洞涉及 API 身份验证绕过，可导致未授权访问内部 API。研究人员于 2025 年 11 月 3 日报告问题，经过跟进，修复于 2025 年 11 月 20 日部署；披露于 2026 年 7 月 27 日发布。

hackernews · EatonZ · 7月27日 15:08 · [社区讨论](https://news.ycombinator.com/item?id=49070756)

**背景**: 像 My Eicher 这样的车队管理平台利用远程信息处理技术远程监控和控制车辆，包括跟踪、诊断甚至发动机熄火。集中式云端控制造成了单点故障；类似漏洞在其他车队系统（如 iTrack、ProTrack）和联网汽车功能中也曾被发现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eaton-works.com/2026/07/27/my-eicher-hack/">Exploiting Volvo / Eicher ’s fleet management platform to gain control...</a></li>
<li><a href="https://thepixelspulse.com/posts/exploiting-volvoeichers-fleet-platform-to-gain-control-over-all-usersvehicles/">Exploiting VolvoEicher's fleet platform to gain control over all...</a></li>
<li><a href="https://vicone.com/blog/how-authentication-and-api-vulnerabilities-undermine-fleet-management-systems">How Authentication and API Vulnerabilities Undermine Fleet Management Systems - VicOne</a></li>

</ul>
</details>

**社区讨论**: 评论者赞扬了研究人员在 17 天修复时间内的耐心，并对现代汽车对云服务的依赖提出了更广泛的担忧，一位用户提到一辆宝马因无手机信号而无法启动。其他人则将这一问题与维修权和安全剧场联系起来。

**标签**: `#security`, `#automotive`, `#vulnerability`, `#fleet management`, `#responsible disclosure`

---

<a id="item-3"></a>
## [Moonshot AI 发布 2.8 万亿参数 Kimi K3 权重](https://simonwillison.net/2026/Jul/27/kimi-k3/#atom-everything) ⭐️ 9.0/10

Moonshot AI 在 Hugging Face 上发布了拥有 2.8 万亿参数的开源权重模型 Kimi K3，其许可证要求大型模型即服务（MaaS）企业另行签订协议。 此次发布是开源权重 AI 领域的一个重要里程碑，Kimi K3 是当前可用的最大模型之一，其新颖的许可方式可能影响其他公司在开放性与商业控制之间的平衡。 该模型采用混合专家架构，包含 896 个专家，每 token 激活 16 个，支持 100 万上下文长度，并通过 MXFP4 量化感知训练，权重约 1.4 TB。许可证要求年收入超过 2000 万美元的 MaaS 提供商另行签订协议。

rss · Simon Willison · 7月27日 23:39

**背景**: Kimi K3 是 Kimi K2 的后续版本，K2 使用了修改版 MIT 许可证，要求大型商业实体进行署名。新许可证不再自称“修改版 MIT”，并为大型 MaaS 提供商增加了更严格的条款。Moonshot AI 始终使用“开源权重”而非“开源”一词。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/ Kimi - K 3 · Hugging Face</a></li>
<li><a href="https://vllm.ai/blog/2026-07-22-kimi-k3-preview">A Preview of Production-Scale Kimi K 3 Support on vLLM | vLLM Blog</a></li>

</ul>
</details>

**社区讨论**: Reddit 评论聚焦于托管 K3 的实际挑战，一家提供商指出 8×A100 节点仅提供 640 GB 内存，不足以容纳 1.4 TB 权重，且 Ampere GPU 缺乏 FP4 张量核心，需要反量化或使用 INT4 内核。

**标签**: `#AI`, `#open-source`, `#large language model`, `#Kimi K3`, `#Moonshot AI`

---

<a id="item-4"></a>
## [vLLM v0.26.0 新增 Inkling 支持与 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 首次支持 Thinking Machines Lab 的 1T 参数 Inkling 多模态模型家族，并针对 DeepSeek-V4 进行了性能优化，包括专用路由内核和 fused_topk_bias。该版本还通过 head_dtype 添加了 fp32 lm_head、每个 KV-cache 组可灵活选择注意力后端，并完善了分层二级存储的 KV 卸载功能。 此版本大幅扩展了 vLLM 的模型覆盖范围和推理效率，支持 1T 参数多模态模型的部署，并将 DeepSeek-V4 的吞吐量提升高达 2.94%。灵活的注意力后端和 KV 卸载增强使 vLLM 能更好地适应不同硬件和内存受限环境。 该版本包含来自 212 位贡献者的 411 次提交，新增了对 Inkling、BertForMaskedLM 和 RobertaForTokenClassification 等模型的支持。关键技术特性包括 Inkling 的 Hopper FA4 相对注意力、ModelOpt NVFP4 量化，以及支持多模态视频和音频的 Rust 前端。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个高吞吐、内存高效的 LLM 推理引擎，广泛用于生产环境。Inkling 模型家族是一个 1T 参数的多模态模型，支持文本、图像和音频输入，上下文长度可达 100 万。FlashAttention-4 (FA4) 是最新的注意力算法，针对 Hopper GPU 进行了优化，相比之前版本有显著加速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm.ai/blog/2026-07-15-inkling">TML Inkling on vLLM: Day-0 Support with Optimized Performance</a></li>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/inkling/">inkling - vLLM</a></li>
<li><a href="https://alphasignal.ai/news/vllm-v0-26-0-ships-day-0-support-for-inkling-s-1t-parameter-multimodal-model">vLLM v0.26.0 Ships Day-0 Support for Inkling's 1T-Parameter ...</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#DeepSeek`, `#CUDA`, `#ROCm`

---

<a id="item-5"></a>
## [python-build-standalone 驱动现代 Python 工具链](https://gregoryszorc.com/docs/python-build-standalone/main/) ⭐️ 8.0/10

python-build-standalone 提供自包含、高度可移植的 Python 发行版，现已被 uv、pipx、Hatch、Poetry 和 Bazel 等主流工具用于安装 Python。Astral 已接管维护工作，确保持续开发和上游整合。 这些发行版消除了系统依赖，使工具能够无缝捆绑 Python，从而简化了 Python 部署。下载量已超过 7000 万次，它们对现代 Python 打包生态系统至关重要。 这些发行版基于上游 CPython 构建，仅做最小修改，确保兼容性。它们不仅用于工具链，还可将 Python 捆绑到 macOS 桌面应用等应用程序中。

hackernews · jcbhmr · 7月27日 18:43 · [社区讨论](https://news.ycombinator.com/item?id=49073942)

**背景**: 传统上，安装 Python 需要系统级安装或手动编译，且因平台而异。python-build-standalone 提供预构建、可重定位的二进制文件，支持 Linux、macOS 和 Windows，解决了可移植性问题。相关项目如 PyOxy 和 Cosmopolitan 提供了单文件可执行文件和跨平台二进制文件等替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/astral-sh/python-build-standalone">GitHub - astral-sh/ python - build - standalone : Produce redistributable...</a></li>
<li><a href="https://astral.sh/blog/python-build-standalone">A new home for python - build - standalone</a></li>
<li><a href="https://grokipedia.com/page/python-build-standalone">python-build-standalone</a></li>

</ul>
</details>

**社区讨论**: 社区成员对这些发行版表示赞赏，uv 创建者 charliermarsh 确认 uv 使用它们，并提到 Astral 正在向上游贡献。Simonw 强调了它们在将 Python 捆绑到桌面应用中的实用性。其他人提到了 PyOxy 和 Cosmopolitan 等作为特定用例的替代方案。

**标签**: `#Python`, `#tooling`, `#packaging`, `#portability`, `#open-source`

---

<a id="item-6"></a>
## [缺失下划线导致无辜者被错判入狱 18 个月](https://arstechnica.com/tech-policy/2026/07/police-missed-one-underscore-and-sent-the-wrong-man-to-prison/) ⭐️ 8.0/10

Kik 用户名中缺失的一个下划线导致警方逮捕并起诉了错误的人，此人被定罪并服刑 18 个月后才被发现错误。 此案凸显了微小的软件错误如何导致刑事司法系统的灾难性失败，削弱了对数字证据和问责制的信任。 受害人在美国，被告在加拿大；尽管没有证据将 Klayme 与犯罪联系起来，他仍被定罪并监禁。错误直到他服刑后才被纠正。

hackernews · quantified · 7月27日 22:10 · [社区讨论](https://news.ycombinator.com/item?id=49076116)

**背景**: Kik 是一款消息应用，用户名区分大小写且可包含下划线。一个下划线的缺失导致警方锁定了错误的账户，而检方未能正确核实数字证据。

**社区讨论**: 评论者质疑被告律师为何未能质疑证据，并指出被错判者缺乏赔偿。有人引用经典故事《计算机不争辩》作为类比。

**标签**: `#software error`, `#wrongful conviction`, `#criminal justice`, `#forensic evidence`, `#accountability`

---

<a id="item-7"></a>
## [法官驳回谷歌利用 DMCA 阻止爬取的企图](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

一名法官裁定谷歌不能利用《数字千年版权法》（DMCA）阻止第三方爬取其搜索结果，驳回了爬取行为规避技术保护措施的主张。 该裁决确立了法律先例，即 DMCA 反规避条款可能不适用于爬取公开数据，从而可能限制科技巨头利用版权法控制数据访问的能力。 该案涉及爬取谷歌搜索结果的 SerpAPI 服务；谷歌曾主张爬取行为规避了其技术措施，违反了 DMCA 第 1201 条。法官认为谷歌的措施并未有效控制对版权内容的访问。

hackernews · cdrnsf · 7月27日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: DMCA 第 1201 条禁止规避控制版权作品访问的技术措施。网络爬取是指自动提取网站数据，其合法性通常取决于数据是否受版权保护以及是否绕过了访问控制。谷歌此前已弃用其官方搜索 API，使得第三方爬虫成为程序化访问搜索结果的唯一途径。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nortonlaw.com/2026/05/14/dmca-section-1201-claims-the-new-battleground-for-ai-and-data-scraping-litigation/">DMCA Section 1201 Claims: The New Battleground for AI and Data Scraping Litigation - the NORTON law firm</a></li>
<li><a href="https://scrapfly.io/blog/posts/google-serp-api-and-alternatives">Best SERP APIs in 2026: Official Google Alternatives & Third-Party Providers</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，谷歌建立在爬取开放网络的基础上，如今却试图阻止爬取，颇具讽刺意味。许多人注意到，谷歌弃用搜索 API 反而催生了对爬虫的需求，还有人强调爬取对于揭露虚假 ETA/ESTA 网站等骗局的重要性。

**标签**: `#web scraping`, `#DMCA`, `#Google`, `#legal`, `#tech policy`

---

<a id="item-8"></a>
## [LLM 代币中继市场助长欺诈与转售](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

Matt Lenhard 的一项调查揭示了一个中国市场，转售商通过汇集 API 密钥、滥用免费试用和使用被盗凭证来提供折扣 LLM 代币，这些操作由 one-api 和 new-api 等开源代理软件驱动。 这一生态系统对 LLM 供应商和开发者构成重大安全和经济风险，因为它助长了欺诈、模型蒸馏和未经授权的访问，可能导致未保护端点产生巨额代币账单。 代理软件 one-api 及其分支 new-api 是合法的开源 API 管理工具，可在汇集凭证之间进行请求负载均衡。买家寻求廉价代币、绕过地理限制或收集数据用于模型蒸馏。

rss · Simon Willison · 7月26日 19:30

**背景**: LLM API 代币用于支付对 GPT-4 等大型语言模型的访问。转售商通过汇集来自免费试用、被盗信用卡或未保护支持机器人的密钥，利用定价差异和安全漏洞，然后通过代理服务器以折扣价转售访问权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/26/relay-market/">An Inside Look at the Relay Market Powering Token Resellers and Fraud</a></li>
<li><a href="https://github.com/songquanpeng/one-api">GitHub - songquanpeng/one-api: LLM API 管理 & 分发系统，支持 Open...</a></li>

</ul>
</details>

**社区讨论**: 在 Hacker News 上，讨论突出了对 API 安全的担忧以及需要更好的速率限制和支出上限。一些评论者指出检测此类滥用的难度，并呼吁供应商实施更严格的控制。

**标签**: `#LLM`, `#API security`, `#fraud`, `#AI economics`, `#open-source`

---

<a id="item-9"></a>
## [NVIDIA Cosmos-H-Dreams：手术机器人的实时生成式仿真](https://huggingface.co/blog/nvidia/cosmos-h-dreams) ⭐️ 8.0/10

NVIDIA 推出了 Cosmos-H-Dreams，这是 Cosmos-H-Surgical-Simulator 的微调变体，能够通过键盘或 Meta Quest 控制器输入实现手术机器人的实时生成式仿真。 该框架通过提供逼真的交互式虚拟环境，加速了手术机器人的开发和训练，减少了对物理数据的依赖，并实现了更快的迭代。 Cosmos-H-Dreams 包含自己的检查点和流式服务器服务层，支持实时手术仿真。它基于 NVIDIA 的 Cosmos 平台构建，该平台具有用于物理 AI 的生成式世界基础模型。

rss · Hugging Face Blog · 7月27日 09:32

**背景**: 手术机器人训练传统上需要昂贵的物理设置或预录数据。像 Cosmos 这样的生成式世界模型可以从初始帧和机器人动作合成逼真的手术视频序列，实现超实时评估和合成数据生成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/blog/nvidia/cosmos-h-dreams">NVIDIA Cosmos-H-Dreams: Bringing Real-Time Generative ...</a></li>
<li><a href="https://github.com/isaac-for-healthcare/Cosmos-H-Dreams">GitHub - isaac-for-healthcare/Cosmos-H-Dreams</a></li>
<li><a href="https://docs.nvidia.com/cosmos/index.html">NVIDIA Cosmos - NVIDIA Docs</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#generative AI`, `#surgical robotics`, `#simulation`, `#real-time`

---

<a id="item-10"></a>
## [OpenAI 拒绝加入英伟达的开放安全 AI 联盟](https://www.reddit.com/r/LocalLLaMA/comments/1v8e36c/openai_management_decided_earlier_today_not_to/) ⭐️ 8.0/10

OpenAI 管理层决定不加入由英伟达 CEO 黄仁勋发起、已有 30 多家公司参与的开放安全 AI 联盟，这一决定引发了内部员工的强烈反对。 这一决定使 OpenAI 在 AI 安全与保障方面与一项重要的行业合作努力脱节，可能削弱整个行业的信任与协调，而内部反弹则表明员工对公司在开放安全倡议上的立场存在严重担忧。 开放安全 AI 联盟于 2026 年 7 月 30 日宣布成立，包括英伟达及 Meta、微软、谷歌等 36 家合作伙伴，旨在共享用于 AI 安全的开放工具、模型和研究。OpenAI 的拒绝正值关于模型蒸馏的持续辩论之际，黄仁勋认为蒸馏是一种学习形式而非盗窃。

reddit · r/LocalLLaMA · /u/KickLassChewGum · 7月27日 21:37

**背景**: 开放安全 AI 联盟是一个行业组织，旨在通过开放工具和共享研究促进负责任的 AI 使用。模型蒸馏是一种让较小模型从较大模型中学习的技术，一些人视其为威胁，但黄仁勋认为这对进步至关重要。OpenAI 拒绝加入的决定与其早期的开源立场形成对比，可能反映了战略分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/open-secure-ai-alliance/">Industry Leaders Join Open Secure AI Alliance for AI Safety ...</a></li>
<li><a href="https://seekingalpha.com/news/4618582-nvidia-and-over-30-firms-form-open-secure-ai-alliance-for-ai-safety">Nvidia and over 30 firms form Open Secure AI Alliance for AI ...</a></li>
<li><a href="https://thehackernews.com/2026/07/nvidia-forms-37-member-open-secure-ai.html">NVIDIA Forms 37-Member Open Secure AI Alliance and Open ...</a></li>

</ul>
</details>

**社区讨论**: 内容中未提供 Reddit 评论，但该帖子本身有活跃讨论。社区普遍支持开放安全倡议并批评 OpenAI 的决定，一些人猜测是出于竞争动机或对知识产权的担忧。

**标签**: `#OpenAI`, `#AI Security`, `#Industry Alliance`, `#Nvidia`, `#Governance`

---

<a id="item-11"></a>
## [用户通过 25GbE 在 80 块 RTX 5090 上运行 Kimi K3](https://www.reddit.com/r/LocalLLaMA/comments/1v8hli2/a_user_has_managed_to_run_kimi_k3_on_80xrtx_5090/) ⭐️ 8.0/10

一位用户成功将 2.8 万亿参数的 Kimi K3 模型部署在 80 块通过 25GbE 以太网互联的 RTX 5090 GPU 上，展示了使用消费级硬件进行分布式推理的实用方案。 这一成就证明，大规模 LLM 推理可以使用广泛可用的消费级 GPU 和标准网络来实现，可能降低组织运行巨大模型的门槛，无需昂贵的专有互连。 该设置使用了 80 块 RTX 5090 GPU（每块 32 GB 显存），通过 25GbE 以太网连接，这比 NVLink 的 600 GB/s 慢得多，但对推理来说仍然足够。Kimi K3 模型有 2.8 万亿参数，支持高达 100 万 token 的上下文。

reddit · r/LocalLLaMA · /u/panchovix · 7月27日 23:56

**背景**: Kimi K3 是一个拥有 2.8 万亿参数的开源大语言模型，是最大的公开可用模型之一。分布式推理将模型拆分到多个 GPU 上，需要高带宽通信；NVLink 提供 600 GB/s，而 25GbE 提供约 3.125 GB/s。像 RTX 5090 这样的消费级 GPU 缺乏 NVLink，因此用户依赖以太网进行多 GPU 设置。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3/tree/main">moonshotai/ Kimi - K 3 at main</a></li>
<li><a href="https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/rtx-5090/">NVIDIA GeForce RTX 5090 Graphics Cards</a></li>

</ul>
</details>

**标签**: `#LLM`, `#distributed inference`, `#hardware`, `#networking`, `#Kimi K3`

---

<a id="item-12"></a>
## [案例研究：用 HTMX 替换 React 的论坛平台](https://misago-project.org/t/removing-reactjs-from-the-codebase-and-adapting-htmx-for-ui-interactivity/1267/) ⭐️ 7.0/10

Misago 论坛项目从代码库中移除了 React.js，转而采用 HTMX 实现 UI 交互，并在 2023 年分享了详细的迁移案例研究。 这一实际迁移案例展示了 HTMX 在服务端渲染交互中的可行性，与 React 等重型客户端框架相比，可能降低复杂性和代码体积。 HTMX 通过自定义属性扩展 HTML，无需编写 JavaScript 即可直接启用 AJAX、WebSocket 和服务器发送事件。该库体积小巧（压缩后约 14KB），与 React 相比可将代码库大小减少 67%。

hackernews · Ralfp · 7月27日 09:58 · [社区讨论](https://news.ycombinator.com/item?id=49067301)

**背景**: HTMX 是由 Carson Gross 创建的开源 JavaScript 库，允许开发者使用超文本（HTML）而非重型客户端框架构建动态 Web 界面。它遵循超媒体驱动的方法，将服务器响应（通常是 HTML 片段）插入页面而无需完全重新加载，从而以最少的 JavaScript 实现类似 SPA 的行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍称赞这一举措，许多人分享了使用 HTMX 构建服务端渲染应用的积极经验。一些人指出 HTMX 非常适合论坛等内容密集型网站，而另一些人建议将其与小型 Vue/React 组件结合用于高度交互的功能。少数用户报告了复杂筛选表单的性能问题，但总体态度是支持的。

**标签**: `#HTMX`, `#React`, `#web development`, `#server-side rendering`, `#case study`

---

<a id="item-13"></a>
## [Paged Out #9：免费技术杂志发布](https://pagedout.institute/download/PagedOut_009.pdf) ⭐️ 7.0/10

Paged Out #9 是一本免费 PDF 技术杂志，涵盖底层编程、复古计算和黑客文化，因其深度和设计获得社区好评。 该杂志填补了对深度技术、黑客好奇内容的 niche，让人想起 Phrack 和 2600 等经典杂志，促进了社区知识分享。 本期包含《C 语言入门》和《亚像素动物园》等文章，印刷版可通过 Lulu 购买。

hackernews · laurensr · 7月27日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49070138)

**背景**: Paged Out 是一本免费的社区驱动技术杂志，发表关于底层编程、安全、复古计算和其他黑客好奇主题的文章。它以 PDF 形式分发，并提供按需印刷版本。

**社区讨论**: 评论者称赞杂志的深度和设计，将其与 Phrack 和 2600 相提并论。具体文章如《C 语言入门》和《亚像素动物园》受到关注，读者表示有兴趣购买印刷版。

**标签**: `#hacker culture`, `#technical magazine`, `#low-level programming`, `#retro computing`, `#zine`

---

<a id="item-14"></a>
## [FeyNoBg：开源背景移除模型与训练库](https://usefeyn.com/blog/feynobg/) ⭐️ 7.0/10

Feyn 发布了 FeyNoBg，一个先进的背景移除模型，并开源了用于训练它的 NoBg Python 库，可在 Hugging Face 和 GitHub 上获取。 这为开发者提供了一个高质量、可定制的背景移除工具，在多个基准测试上优于现有模型，同时配套的库简化了训练和部署流程。 FeyNoBg 扩展了 BiRefNet，将其第三特征提取阶段从 18 个块增加到 24 个块，参数量从 2.22 亿增加到 2.63 亿，并在八个基准测试中的四个上取得了最佳成绩。

hackernews · snyy · 7月27日 16:59 · [社区讨论](https://news.ycombinator.com/item?id=49072462)

**背景**: 背景移除（即图像抠图）涉及通过估计每个像素的前景不透明度来将主体与背景分离。这是一项常见的 AI 任务，用于照片编辑、电子商务和视频会议，但由于头发或运动模糊等细节而仍然具有挑战性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://usefeyn.com/blog/feynobg/">FeyNoBg: A SOTA Model For Background Removal | Feyn</a></li>
<li><a href="https://github.com/feyninc/nobg">GitHub - feyninc/ nobg : a library for image and video matting · GitHub</a></li>
<li><a href="https://huggingface.co/spaces/feyninc/feynobg">Feynobg - a Hugging Face Space by feyninc</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，称赞该工具的实用性和成熟度。一些用户对基于 MIT 许可的 BiRefNet 衍生模型采用 CC-BY-NC-4.0 许可表示担忧，其他人则询问分辨率限制以及与 Adobe 解决方案的比较。

**标签**: `#background removal`, `#open-source`, `#computer vision`, `#machine learning`, `#Python library`

---

<a id="item-15"></a>
## [Libsm64：将《超级马里奥 64》作为可复用库嵌入游戏引擎](https://github.com/libsm64/libsm64) ⭐️ 7.0/10

Libsm64 是一个开源库，它提取了《超级马里奥 64》中的移动和渲染代码，使开发者能够将马里奥嵌入到外部游戏引擎中。社区项目已展示了马里奥出现在《半条命 2》等游戏中的实例。 该项目展示了经典游戏代码的创造性复用，无需专有中间件即可实现新颖的跨游戏交互。它凸显了逆向工程和开源工作延长复古游戏生命周期的潜力。 该库基于《超级马里奥 64》的反向工程项目构建，提供了干净的 C 语言 API，用于将马里奥角色集成到其他引擎中。它不是一个独立游戏，而是供开发者嵌入自己项目的组件。

hackernews · klaussilveira · 7月27日 10:04 · [社区讨论](https://news.ycombinator.com/item?id=49067352)

**背景**: 《超级马里奥 64》最初于 1996 年在 Nintendo 64 上发布。sm64 反向工程项目从原始二进制文件中逆向推导出了游戏源代码，从而实现了向其他平台的移植。Libsm64 进一步将角色逻辑打包为可复用库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm64/libsm64: Mario 64 as a library for use in ...</a></li>
<li><a href="https://github.com/n64decomp/sm64">GitHub - n64decomp/sm64: A Super Mario 64 decompilation ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员表达了兴奋和怀旧之情，有人称其实现了元宇宙概念，但没有区块链的炒作。其他人分享了演示视频和 awesome-libsm64 的链接，这是一个使用该库的项目精选列表。

**标签**: `#game development`, `#reverse engineering`, `#library`, `#retro gaming`, `#open source`

---

<a id="item-16"></a>
## [Ethan Mollick 的 AI 指南从聊天转向代理系统](https://simonwillison.net/2026/Jul/27/an-opinionated-guide-to-which-ai-to-use-to-do-stuff/#atom-everything) ⭐️ 7.0/10

Ethan Mollick 发布了其主观 AI 使用指南的更新版本，将重点从基于聊天的模型转向能够自主工作数小时的代理系统。值得注意的是，Google 的 Gemini 被排除在外，因为它在 Codex/ChatGPT Work/Cowork 类别中缺乏成熟的条目。 该指南反映了从对话式 AI 到自主代理的重大行业转变，帮助用户驾驭令人困惑的 AI 工具格局。它提供了关于使用 ChatGPT Work 和 Claude Cowork 等代理模式的实用建议，这些模式正成为提高生产力的关键。 该指南解释说，ChatGPT Work 和 Claude Cowork 允许 AI 访问用户的计算机以执行自主任务，而 ChatGPT Codex 和 Claude Code 则专用于软件开发。命名约定令人困惑，因为移动设备上的 Work 和 Cowork 模式与桌面应用程序上的不同。

rss · Simon Willison · 7月27日 21:55

**背景**: 代理型 AI 指的是能够通过自身行动追求目标的系统，而不仅仅是产生供人类采取行动的输出。与需要逐步指令的传统聊天机器人不同，代理型 AI 可以独立观察、推理、学习和做出决策。OpenAI 和 Anthropic 等主要 AI 公司现在提供能够使用工具、浏览网页和控制计算机的代理模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/20001275-chatgpt-work-and-codex">ChatGPT Work and Codex - OpenAI Help Center</a></li>
<li><a href="https://agentic.ai/what-is-agentic-ai">What Is Agentic AI? Definition, 6 Levels & Examples (2026)</a></li>

</ul>
</details>

**社区讨论**: Simon Willison 的评论强调了 ChatGPT Work 和 Codex 之间令人困惑的命名约定，指出移动版和桌面版的行为不同。讨论可能包括对代理系统实用价值的认同，以及对 Google 在这一类别中落后的不满。

**标签**: `#AI`, `#agentic systems`, `#LLMs`, `#practical guide`

---

<a id="item-17"></a>
## [Ninfer 在 RTX 5090 上实现 Qwen 3.6 35B 每秒 700 token 的推理速度](https://www.reddit.com/r/LocalLLaMA/comments/1v8a7wb/nifer_is_insane_700ts_with_qwen_36_35b_no/) ⭐️ 7.0/10

一款名为 Ninfer 的新型推理引擎在单张 RTX 5090 GPU 上，对 Qwen 3.6 35B 模型实现了每秒 550-720 token 的推理速度，并支持完整的 25 万上下文长度。这一性能可与 Cerebras 晶圆级推理速度相媲美。 这一突破大幅降低了高速本地 LLM 推理的硬件门槛，此前只有昂贵的云服务或专用硬件才能实现。它使得在消费级硬件上进行实时、单实例推理成为可能，有望加速本地 AI 应用的发展。 Ninfer 是一个从头编写的 C++/CUDA 引擎，专门为 RTX 5090 优化，仅支持 Qwen 3.6 27B 和 35B 模型。它通过命令行或兼容 OpenAI/Anthropic 的 API 运行文本、图像和视频提示。

reddit · r/LocalLLaMA · /u/BringTea_666 · 7月27日 19:17

**背景**: 本地 LLM 推理在消费级 GPU 上通常只能达到每秒几十到几百 token。Cerebras 提供每秒 3000+ token 的速度，但需要专用的晶圆级硬件。Ninfer 在单张 RTX 5090 上实现每秒 700 token，是本地推理的一次重大飞跃。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Neroued/ninfer">GitHub - Neroued/ninfer: High-performance single-GPU ...</a></li>
<li><a href="https://www.cerebras.ai/inference">Inference - Cerebras</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-35B-A3B">Qwen/Qwen3.6-35B-A3B · Hugging Face</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#RTX 5090`, `#performance`, `#local LLM`, `#Qwen`

---