---
layout: default
title: "Horizon Summary: 2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> 从 32 条内容中筛选出 12 条重要资讯。

---

1. [vLLM v0.26.0 发布：支持 Inkling 模型和 DeepSeek-V4 优化](#item-1) ⭐️ 9.0/10
2. [要求对开放权重模型进行强制性安全测试](#item-2) ⭐️ 9.0/10
3. [月之暗面发布 3T 参数开放权重模型 Kimi-K3](#item-3) ⭐️ 9.0/10
4. [Fastjson 1.x 高危 RCE 漏洞，无需 autoType 或 gadgets](#item-4) ⭐️ 9.0/10
5. [中芯国际测试中国首台国产 DUV 光刻机](#item-5) ⭐️ 9.0/10
6. [月之暗面将开源 3T 参数模型 Kimi-K3](#item-6) ⭐️ 9.0/10
7. [法官驳回谷歌用 DMCA 阻止数据抓取的请求](#item-7) ⭐️ 8.0/10
8. [Libsm64：将《超级马里奥 64》转变为可复用库](#item-8) ⭐️ 8.0/10
9. [Bun 的 Rust 重写进展与 v1.4 延迟](#item-9) ⭐️ 8.0/10
10. [长鑫科技科创板首日暴涨 471.59%，成史上最大 IPO](#item-10) ⭐️ 8.0/10
11. [存储芯片涨价加剧，华为与长鑫关系趋紧](#item-11) ⭐️ 8.0/10
12. [谷歌透露 Gemini 4：迄今最雄心预训练，预计 2026 年底发布](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 发布：支持 Inkling 模型和 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 引入了全新的 Inkling 模型系列并提供完整支持栈，对 DeepSeek-V4 进行了显著的性能优化（包括专用路由内核实现 2.94% 端到端 TPOT 提升），增加了 fp32 lm_head 支持、灵活注意力后端，并大大提升了 KV 卸载与分层二级存储的成熟度。 此版本显著提升了 DeepSeek-V4 和全新 Inkling 系列等前沿模型的推理性能与灵活性，巩固了 vLLM 作为顶级开源 LLM 推理引擎的地位。来自 212 名贡献者的 411 次提交体现了活跃的社区生态。 关键技术细节包括 Inkling 模型的分段 CUDA 图支持、Hopper FA4 相对注意力、MTP=1 投机解码、LoRA 支持以及标准 ModelOpt NVFP4 量化。对于 DeepSeek-V4，优化包括 fused_topk_bias（内核速度提升 1.5-2 倍）和冗余重复/复制删除（端到端 TPOT 提升 1.8%）。

github · khluu · 7月27日 01:06

**背景**: vLLM 是一个高吞吐、内存高效的大语言模型推理引擎，广泛应用于生产和研究。Inkling 模型是由 Thinking Machines Lab 以 Apache 2.0 许可证发布的开源通用多模态模型。Flash Attention 4 (FA4) 是最新版本的注意力高效算法，针对 Hopper GPU 进行了优化，通过 CuTeDSL 支持超越了 FA3。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/cuda_graphs/">CUDA Graphs - vLLM</a></li>
<li><a href="https://pytorch.org/blog/flexattention-flashattention-4-fast-and-flexible/">FlexAttention + FlashAttention-4: Fast and Flexible – PyTorch</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#model optimization`, `#open source`, `#GPU`

---

<a id="item-2"></a>
## [要求对开放权重模型进行强制性安全测试](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 9.0/10

Anthropic 发布政策声明，认为不应禁止开放权重 AI 模型，但所有足够强大的模型（无论是开放还是封闭）都应接受强制性安全测试。 这家领先 AI 公司的立场直接回应了开源 AI 与安全监管之间的张力，可能影响未来的政策决策和行业实践。 Anthropic 特别支持禁止向中国出售芯片以及打击走私等措施，批评者认为这些措施可能因测试成本过高而实际上等同于禁止开放权重模型。

hackernews · surprisetalk · 7月27日 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重模型是指其训练参数公开发布的 AI 模型，任何人都可以下载、运行和修改。与封闭模型不同，它们促进了广泛访问，但也引发了关于滥用的安全担忧，例如生成有害内容或支持恶意应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**社区讨论**: 社区评论者普遍批评 Anthropic 的立场实际上是变相禁令，认为强制性安全测试可能成本过高或被行政操纵。一些人认为这是保护 Anthropic 专有模型免受竞争的商业举措，另一些人则质疑其反对禁令却支持对华硬件限制的一致性。

**标签**: `#AI safety`, `#open-weights`, `#regulation`, `#Anthropic`, `#open-source AI`

---

<a id="item-3"></a>
## [月之暗面发布 3T 参数开放权重模型 Kimi-K3](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 9.0/10

月之暗面（Moonshot AI）在 HuggingFace 上发布了 Kimi-K3，这是一个 3 万亿参数的开放权重模型，并附带了技术报告。这是目前公开可用的最大模型之一。 此次发布推动了开放权重模型的边界，使研究人员和初创公司能够接触到前所未有的规模模型。这可能普及前沿 AI 能力，并激发定制化和微调方面的创新。 该模型采用原生 mxfp4 精度，托管约需 1.5TB 显存，因此需要高端硬件如 8 块 B200 或更多。许可证包含对模型即服务业务的收入限制，超过 2000 万美元营收需遵守额外条款。

hackernews · nateb2022 · 7月27日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=49065752)

**背景**: 开放权重模型意味着训练后的参数被公开发布，允许任何人下载并在本地运行模型、研究其行为，以及针对特定任务进行微调。然而，开放权重模型并非完全开源，因为通常缺少训练数据和代码。月之暗面是一家位于北京的人工智能公司，以开发 Kimi 系列等大语言模型而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**社区讨论**: 社区评论主要围绕三个主题：定价、定制化和硬件需求。还有一个细节是模型最初自我介绍为“Claude”，引发了疑问。

**标签**: `#AI/ML`, `#large language model`, `#open-source`, `#model release`, `#HuggingFace`

---

<a id="item-4"></a>
## [Fastjson 1.x 高危 RCE 漏洞，无需 autoType 或 gadgets](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

安全研究员 Kirill Firsov 披露了 Fastjson 1.x 版本 1.2.68 至 1.2.83 中存在的高危远程代码执行漏洞。该漏洞无需开启 autoTypeSupport，也无需依赖 classpath 上的 gadget 链，且在 JDK 8、17 和 21 上均可利用。 该漏洞极为严重，因为 Fastjson 被广泛用于 Java 应用中，且此漏洞无需启用 autoType 也无须特定 gadget 链，降低了利用门槛。由于 Fastjson 1.x 已于 2024 年 10 月停止维护，官方不会发布补丁，用户必须紧急升级到 Fastjson 2。 该漏洞影响 Fastjson 1.2.68 至 1.2.83 版本，攻击者无需开启 autoType 或依赖 classpath 上的特定 gadget。Fastjson 1.x 已于 2024 年 10 月停止维护，阿里不会发布安全更新。

telegram · zaihuapd · 7月27日 10:31

**背景**: Fastjson 是阿里巴巴开发的流行 Java JSON 解析库。反序列化漏洞通常需要启用 autoType（允许反序列化任意类）并利用已有的“gadget 链”——一系列方法调用最终导致代码执行。这个新漏洞绕过了这两个要求，使其更加危险。Fastjson 2 是推荐的替代方案，它仍在积极维护且具有更安全的默认配置。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson2/blob/main/docs/autotype_en.md">fastjson 2/docs/autotype_en.md at main · alibaba/ fastjson 2 · GitHub</a></li>
<li><a href="https://github.com/frohoff/ysoserial">GitHub - frohoff/ysoserial: A proof-of-concept tool for ... Gadget chains in Java: how unsafe deserialization leads to ... Developing a custom gadget chain for Java deserialization ... Lab: Developing a custom gadget chain for Java deserialization Java Deserialization Attacks: From Gadget Chains to RCE</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#fastjson`, `#RCE`, `#java`

---

<a id="item-5"></a>
## [中芯国际测试中国首台国产 DUV 光刻机](https://t.me/zaihuapd/42800) ⭐️ 9.0/10

中芯国际正在试运行中国首台由上海初创公司宇量昇自主研发的先进深紫外（DUV）光刻机。该公司利用该机器生产 28 纳米芯片，并尝试通过多重图形化工艺延伸至 7 纳米甚至 5 纳米节点，尽管良率较低。 这一进展标志着中国在日益严峻的出口管制下实现半导体自给自足的关键里程碑。若成功，可能减少对荷兰 ASML 设备的依赖，并重塑全球芯片供应链。 该 DUV 光刻机的大部分零部件已实现国产化，但仍有部分依赖进口。业内人士估计，实现稳定良率量产需要一至两年，且该设备至少要到 2027 年才能与 ASML 的产品竞争。

telegram · zaihuapd · 7月27日 14:10

**背景**: 深紫外（DUV）光刻技术使用 193 纳米波长的光在硅片上蚀刻电路，结合多重图形化技术可生产低至 7 纳米的芯片。多重图形化通过将单层电路拆分为多次曝光来突破分辨率限制。相比之下，极紫外（EUV）光刻使用 13.5 纳米波长，是 7 纳米以下先进节点所必需的。中国目前最先进的芯片仍依赖荷兰 ASML 的 DUV 设备，而 EUV 对华销售受美国出口管制禁止。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Multiple_patterning">Multiple patterning - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Extreme_ultraviolet_lithography">EUV lithography - Wikipedia</a></li>
<li><a href="https://www.semi.org/en/changes-and-challenges-abound-multi-patterning-lithography">Changes and Challenges Abound in Multi-patterning Lithography | SEMI</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#lithography`, `#SMIC`, `#DUV`, `#China chips`

---

<a id="item-6"></a>
## [月之暗面将开源 3T 参数模型 Kimi-K3](https://t.me/zaihuapd/42802) ⭐️ 9.0/10

月之暗面宣布将开源 Kimi-K3，这是一个 2.8T 参数（被称为 3T 级）的模型，采用 Kimi Delta Attention 和 Attention Residuals 架构，原生支持工具调用和百万 token 上下文窗口。模型权重预计于 2026 年 7 月 27 日在 Hugging Face 发布。 这标志着首个前沿规模（3T 参数）模型的开源，可能使最先进的 AI 能力更加民主化。其新颖的架构可能影响未来 LLM 设计，推动高效线性注意力和智能体工作流的发展。 该模型采用混合 MoE 架构，每 3 个 KDA 层搭配 1 个完整注意力层，上下文窗口支持高达 100 万 token。尽管被称为 3T 级，实际参数量为 2.8T。

telegram · zaihuapd · 7月27日 15:15

**背景**: 大语言模型通常使用全注意力机制，其计算量随序列长度二次增长，导致长上下文处理成本高昂。Kimi Delta Attention (KDA) 是一种线性注意力变体，在保持表达力的同时提升效率。智能体能力指模型自主使用工具、规划和执行多步任务的能力。月之暗面是一家中国 AI 公司，以 Kimi 模型系列闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture GitHub - MoonshotAI/Kimi-Linear Kimi-Linear A arXiv:2510.26692v2 [cs.CL] 1 Nov 2025 Images hwilner/kimi-delta-attention - GitHub Linear Attention: Kimi Delta Attention | Jianyu Huang Kimi K3 Tech Blog: Open Frontier Intelligence KDA (Kimi Delta Attention) | fla-org/flash-linear-attention ...</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#large language model`, `#attention mechanism`, `#Moonshot AI`

---

<a id="item-7"></a>
## [法官驳回谷歌用 DMCA 阻止数据抓取的请求](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

一位美国法官裁定，谷歌不能利用《数字千年版权法案》(DMCA)来阻止第三方抓取其搜索结果，因为这些结果中的事实数据缺乏版权保护所需的原创性。 这一裁决为网络抓取和数据访问树立了重要的法律先例，可能限制大型科技公司利用版权法控制公开信息的能力。它可能会为依赖抓取进行创新和问责的小型竞争者和研究人员赋权。 谷歌曾辩称其搜索引擎结果页面(SERP)是可受版权保护的汇编，但法官认为它们缺乏创造性的选择或编排。该案是针对 SerpAPI（一家为客户抓取谷歌结果的服务商）提起的。

hackernews · cdrnsf · 7月27日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: 《数字千年版权法案》(DMCA)是美国一项法律，为版权所有者提供了在线保护其作品的框架，但不涵盖事实数据。网络抓取，即从网站自动提取数据的行为，通常处于法律灰色地带。像网络爬虫和代理服务这样的工具常被用于提取公共数据，这正是本案的核心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://webscraper.io/">Web Scraper Cloud | Enterprise Web Scraping Platform</a></li>
<li><a href="https://llanj.org/wiki/how-to-crawl-webpages-requiring-login">How To Crawl Webpages Requiring Login - Llanj</a></li>
<li><a href="https://thunderbit.com/">Thunderbit: AI Web Scraper - Scrape any website in 2 clicks</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，谷歌这家建立在抓取开放网络之上的公司，现在却试图阻止他人抓取其结果，这颇具讽刺意味。一些人指出，谷歌废弃其搜索 API 的行为迫使用户依赖第三方抓取工具，反而创造了谷歌正在起诉的需求。其他人则讨论了美国和欧盟在数据库版权法上的差异。

**标签**: `#legal`, `#web scraping`, `#Google`, `#DMCA`, `#API`

---

<a id="item-8"></a>
## [Libsm64：将《超级马里奥 64》转变为可复用库](https://github.com/libsm64/libsm64) ⭐️ 8.0/10

Libsm64 是一个软件库，它将《超级马里奥 64》的动作和渲染代码提取为可复用 API，使开发者能够将马里奥角色和机制集成到其他游戏引擎如 Unity 或 Source 中。 这使得新颖的跨游戏集成和对经典游戏代码的创造性复用成为可能，展示了反编译项目将游戏资产拓展到原始环境之外的潜力，而不依赖专有元宇宙概念。 该库基于 n64decomp/sm64 项目对《超级马里奥 64》的完整反编译，提供了动作和渲染的干净 C 语言接口。截至报道，已有示例集成如马里奥在《半条命 2》中，以及展示基本功能的演示视频。

hackernews · klaussilveira · 7月27日 10:04 · [社区讨论](https://news.ycombinator.com/item?id=49067352)

**背景**: 《超级马里奥 64》是 1996 年在 Nintendo 64 上的一款里程碑式平台游戏。2019 年，一个社区驱动的反编译项目从原始机器码生成了完全可读的 C 源代码，实现了修改和移植。Libsm64 进一步将其核心逻辑封装成库，供外部使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm 64 / libsm 64 : Mario 64 as a library for use in external...</a></li>
<li><a href="https://github.com/n64decomp/sm64">GitHub - n64decomp/sm64: A Super Mario 64 decompilation, brought to you by a bunch of clever folks. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者反应热烈，称其为‘最喜欢的库’，并指出它体现了可互操作游戏资产的承诺，没有加密炒作。一位用户询问演示视频，另一位列出了 awesome-libsm64 仓库以收录有趣的项目。

**标签**: `#reverse engineering`, `#game development`, `#open source`, `#emulation`

---

<a id="item-9"></a>
## [Bun 的 Rust 重写进展与 v1.4 延迟](https://lockwood.dev/ai/2026/07/27/how-is-the-bun-rewrite-in-rust-going.html) ⭐️ 8.0/10

Bun 的 Rust 重写已在一个多月前悄然部署到 Claude Code 中，v1.4 版本因需要达到特定数量的新通过 Node.js 测试而延迟发布。 此次重写对 JavaScript 生态系统意义重大，有望提升 Bun（一种流行的 Node.js 替代方案）的性能和兼容性。在翻译过程中使用 LLM 也凸显了大规模代码库重写的新方法。 Bun 的创建者 Jarred 表示，Rust 重写已部署到 Claude Code 而未引起广泛注意，但 v1.4 因需达到承诺的 Node.js 测试通过数而推迟。社区讨论还提到一个基于 Zig 的竞争分支实现了亚秒级构建时间。

hackernews · tomlockwood · 7月27日 11:12 · [社区讨论](https://news.ycombinator.com/item?id=49067854)

**背景**: Bun 是一个快速的一体化 JavaScript 运行时，最初用 Zig 编写，旨在作为 Node.js 的替代品。决定用 Rust 重写是为了利用 Rust 的安全性和性能，并且这一转变部分借助了 LLM 的帮助。Claude Code 是 Anthropic 开发的一款 AI 辅助编码工具，可帮助开发者理解和编辑代码库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/ bun : Incredibly fast JavaScript runtime , bundler...</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>

</ul>
</details>

**社区讨论**: 社区评论态度不一：Jarred 对重写和延迟进行了透明更新；一些用户称赞 LLM 辅助的翻译，而另一些用户则质疑其长期可维护性；与一个宣称构建速度更快的 Zig 分支的比较引发了关于重写必要性的讨论。

**标签**: `#Bun`, `#Rust`, `#JavaScript Runtime`, `#Rewrite`, `#Performance`

---

<a id="item-10"></a>
## [长鑫科技科创板首日暴涨 471.59%，成史上最大 IPO](https://www.stcn.com/article/detail/4042119.html) ⭐️ 8.0/10

7 月 27 日，长鑫科技（CXMT）在上交所科创板上市，开盘价 49.5 元，较发行价 8.66 元飙升 471.59%。本次 IPO 实际募资约 579 亿元，超过中芯国际 2020 年 532 亿元的纪录，成为科创板史上最大 IPO。 此次上市凸显了中国本土存储芯片产业的快速发展，以及投资者对科创板半导体公司的强烈追捧。长鑫科技的高估值和盈利预期表明，中国在减少对三星、SK 海力士等国外 DRAM 供应商依赖方面取得了进展。 长鑫科技的 IPO 包含超额配售选择权，若全额行使，总募资额可达 666 亿元。公司预计 2026 年上半年归母净利润为 500 亿至 570 亿元，同比实现大幅扭亏。

telegram · zaihuapd · 7月27日 01:29

**背景**: 科创板（上海证券交易所科技创新板）于 2019 年启动，旨在以更包容的上市规则支持科技创新企业，常被比作中国的纳斯达克。长鑫科技成立于 2016 年，是中国最大的 DRAM 制造商，产能位居全球第四，主要生产 DDR4、DDR5 和 LPDDR 内存芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Shanghai_Stock_Exchange_STAR_Market">Shanghai Stock Exchange STAR Market - Wikipedia</a></li>
<li><a href="https://www.cxmt.com/en/">About cxmt - cxmt</a></li>
<li><a href="https://chinaidb.com/companies/cxmt/">CXMT ( ChangXin Memory ) — China AI Index</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#IPO`, `#memory chip`, `#CXMT`, `#Chinese tech`

---

<a id="item-11"></a>
## [存储芯片涨价加剧，华为与长鑫关系趋紧](https://t.me/zaihuapd/42788) ⭐️ 8.0/10

AI 数据中心需求推高存储芯片价格，长鑫存储议价能力增强。华为要求长鑫缓解采购成本未获让步；今年 6 月，与华为关系密切的设备商新凯来工程师被要求离开长鑫核心研发区，此后未获准返回。 这表明随着 AI 需求重塑市场格局，中国半导体供应链内部摩擦加剧，可能影响华为获取关键存储芯片。长鑫作为全球第四大 DRAM 制造商，可能优先考虑其他客户，从而影响华为的 AI 基础设施计划。 长鑫已成为全球第四大 DRAM 制造商，产品因 AI 数据中心建设而供应趋紧。新凯来事件凸显了战略紧张：华为希望降低成本，但长鑫甚至对主要客户也持续涨价。

telegram · zaihuapd · 7月27日 03:17

**背景**: 长鑫存储（CXMT）是中国 DRAM 芯片制造商，尽管受到美国制裁仍取得技术突破。新凯来（SiCarrier Technologies）是深圳半导体设备公司，由深圳市政府支持并与华为关系密切，提供前端工艺设备。该事件发生在长鑫合肥研发中心，反映了华为对稳定芯片供应的需求与长鑫在 AI 驱动需求下的利润动机之间的微妙平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://chip.com.cn/cxmt.html">长 鑫 存 储 ( CXMT ) - Glochip.com</a></li>
<li><a href="https://gaohaojun.cn/Blog/2026/01/21/红色内存潮流长鑫存储的战略分析和围绕DRAM的地缘政治斗争/">内 存 的赤色潮流： 长 鑫 存 储 （ CXMT ... - Gao Haojun</a></li>
<li><a href="https://en.wikipedia.org/wiki/SiCarrier">SiCarrier - Wikipedia</a></li>

</ul>
</details>

**标签**: `#storage chips`, `#Huawei`, `#CXMT`, `#AI data centers`, `#supply chain`

---

<a id="item-12"></a>
## [谷歌透露 Gemini 4：迄今最雄心预训练，预计 2026 年底发布](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 8.0/10

谷歌 CEO Sundar Pichai 在 Alphabet 2026 年第二季度财报电话会议上宣布，下一代大语言模型 Gemini 4 已投入训练，这是该公司迄今为止最具雄心的预训练项目。他对内部进展感到兴奋，并预计在 2026 年底前发布。 这一公告标志着谷歌加大力度推进大语言模型和通用人工智能（AGI）研究。Gemini 4 的发布可能深刻影响 AI 竞争格局，有望提升谷歌生态系统及整个行业的产品能力。 Pichai 强调，算力资源将优先用于前沿 AGI 研发，以确保 Gemini 4 在发布时仍处于领先地位。此外，Gemini 3.x Flash 系列将保持几乎每月一次的迭代频率，重点提升智能编码能力。

telegram · zaihuapd · 7月27日 04:06

**背景**: 大语言模型（LLM）如 Gemini 通常在大量文本数据上进行预训练以预测下一个词，然后针对特定任务进行微调。Gemini 是 Google DeepMind 开发的多模态 LLM 系列，继承自 LaMDA 和 PaLM 2，包含 Gemini Pro、Flash 等变体。预训练是计算最密集的阶段，因此雄心的预训练项目是重大的战略投资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(AI_model)">Gemini (AI model)</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Gemini`, `#large language models`, `#announcement`

---