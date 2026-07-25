---
layout: default
title: "Horizon Summary: 2026-07-25 (ZH)"
date: 2026-07-25
lang: zh
---

> 从 26 条内容中筛选出 9 条重要资讯。

---

1. [vLLM v0.26.0 发布：支持 Inkling、DeepSeek-V4 优化与 fp32 lm_head](#item-1) ⭐️ 9.0/10
2. [SGLang v0.5.16：DSpark 推测解码与 Inkling 支持](#item-2) ⭐️ 9.0/10
3. [开源权重大模型迎来 Kubernetes 式时刻](#item-3) ⭐️ 8.0/10
4. [Ruff v0.16.0：默认规则从 59 条激增至 413 条](#item-4) ⭐️ 8.0/10
5. [Claude Opus 5 抵御提示注入能力最强](#item-5) ⭐️ 8.0/10
6. [AMD 能否打破英伟达的 CUDA 护城河？](#item-6) ⭐️ 8.0/10
7. [携程因数据出境违规被罚 1000 万元](#item-7) ⭐️ 8.0/10
8. [中国对携程罚款 51.79 亿元反垄断](#item-8) ⭐️ 8.0/10
9. [微软通过 TPM 芯片封堵盗版 Windows 激活](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 发布：支持 Inkling、DeepSeek-V4 优化与 fp32 lm_head](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 新增了对 Inkling 模型系列（1 万亿参数多模态 MoE）的完整支持，针对 DeepSeek-V4 的推理优化（专用路由内核、fused_topk_bias），通过 head_dtype 支持 fp32 lm_head，以及按 KV-cache 组灵活选择注意力后端。 这些增强显著提升了最先进大语言模型的推理性能和准确性，使 vLLM 成为面向 AI 社区更通用、更可投产的推理引擎。 Inkling 支持包括基础建模、CUDA graphs、Hopper FA4 注意力、MTP=1 投机解码、LoRA 和 NVFP4 量化。DeepSeek-V4 通过专用路由内核获得 2.94% 的端到端 TPOT 提升，此外还有针对稀疏解码/预填充的 ROCm 和 XPU 优化。

github · khluu · 7月25日 10:38

**背景**: vLLM 是一个开源的高吞吐量大语言模型推理引擎。Thinking Machines Lab 的 Inkling 模型是一个 975B 参数 MoE 变压器，支持 1M 上下文长度，需要高级优化才能高效推理。NVFP4 是 NVIDIA ModelOpt 的 4 位浮点量化格式，可减少内存使用且几乎不损失准确性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm.ai/blog/2026-07-15-inkling">TML Inkling on vLLM: Day-0 Support with Optimized Performance | vLLM Blog</a></li>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM Documentation</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#performance`, `#release`, `#deep learning`

---

<a id="item-2"></a>
## [SGLang v0.5.16：DSpark 推测解码与 Inkling 支持](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 9.0/10

SGLang v0.5.16 引入了置信度驱动的推测解码算法 DSpark，在 DeepSeek-V4-Pro 上达到 383.7 tok/s，并新增对 975B 参数 Inkling 多模态 MoE 模型的支持，在 Blackwell 硬件上输入可达 71.7k tok/s，每用户解码达 171.0 tok/s。 此次发布通过 DSpark 的自适应验证大幅提升了大语言模型的推理吞吐量，并为最大的开源多模态模型之一（Inkling）提供服务，有望降低复杂 AI 应用的成本和延迟。 DSpark 以块为单位进行半自回归草稿，并根据自身置信度确定验证窗口大小，通过 `--speculative-algorithm DSPARK` 启用。Inkling 是一个 975B 参数的多模态 MoE，拥有 1M token 上下文，混合了滑动窗口、全局和 Mamba2 注意力，并支持原生 MTP 和 NVFP4。

github · Qiaolin-Yu · 7月25日 00:13

**背景**: 推测解码通过使用草稿模型生成多个 token 并用目标模型验证来加速大模型推理。SGLang 是一个开源的大模型服务框架。DSpark 通过根据置信度动态调整验证窗口改进了固定长度草稿方式。Inkling 是 Thinking Machines Lab 推出的具有开放权重的大型多模态 MoE 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hyper.ai/en/papers/DSpark">DSpark : Confidence-Scheduled Speculative Decoding with... | HyperAI</a></li>
<li><a href="https://thinkingmachines.ai/inkling/">Inkling - Thinking Machines Lab</a></li>

</ul>
</details>

**标签**: `#speculative decoding`, `#LLM serving`, `#SGLang`, `#multimodal MoE`, `#performance`

---

<a id="item-3"></a>
## [开源权重大模型迎来 Kubernetes 式时刻](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

Tobi Knaup 发表文章指出，开源权重大模型正沿着与 Kubernetes 相似的轨迹发展，成为提供成本基准并促进去中心化创新的基础性基础设施。 这种范式转变可能使 AI 开发民主化，减少对专有模型的依赖，并通过实现去中心化创新和设定推理成本基准来影响地缘政治格局。 文章强调，开源权重模型为推理成本提供了基准，并讨论了模型来源验证等挑战，以及需要像 Linux 这样的开源软件进行协作开发。

hackernews · tknaup · 7月25日 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: Kubernetes 是一个用于管理容器化工作负载的开源平台，被广泛采用为标准基础设施。开源权重大模型发布训练后的参数但不一定包含训练数据，允许他人运行推理。文章将两者类比，认为开源权重模型可能成为 AI 领域的 Kubernetes，实现去中心化创新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/open-models/">Open models by OpenAI</a></li>
<li><a href="https://openai.com/global-affairs/open-weights-and-ai-for-all/">Open weights and AI for all | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tokenomics">Tokenomics</a></li>

</ul>
</details>

**社区讨论**: 社区评论对按来源禁止模型的可行性表示怀疑，批评 Tokenomics 定价不透明，并呼吁类似 Linux 的协作式开源权重开发。部分评论指出 OpenAI 已发布有用的开源权重模型，但希望更新更频繁。

**标签**: `#open-weight AI`, `#open-source models`, `#AI infrastructure`, `#geopolitics`, `#tokenomics`

---

<a id="item-4"></a>
## [Ruff v0.16.0：默认规则从 59 条激增至 413 条](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0 于 2026 年 7 月 23 日发布，将默认启用的检查规则从 59 条增加到 413 条，新增了许多可检测语法错误和运行时错误的检查。 默认规则的大幅扩展将使许多现有 Python 项目和 CI 流水线因新警告而失败，迫使开发者更新代码库或调整配置。这体现了 Ruff 日益成熟，以及 Python 生态中默认代码检查日趋严格的趋势。 此次更新影响了 Datasette、sqlite-utils 和 LLM 等工具，使用`ruff check --fix --unsafe-fixes`后发现并修复了数百个警告。新增的默认检查包括无时区 datetime 使用（DTZ005）、盲目捕获异常（BLE001）和无效属性访问（B018）。

rss · Simon Willison · 7月25日 22:44

**背景**: Ruff 是 Astral 开发的用 Rust 编写的极速 Python 代码检查器和格式化器，可作为 Flake8、isort、pyupgrade 等工具的替代品。默认规则集自 Ruff v0.1.0 以来未更新，而可用规则总数已从 708 条增长到 968 条。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/linter/">The Ruff Linter | Ruff - Astral</a></li>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ruff: An extremely fast Python linter and code ...</a></li>
<li><a href="https://astral.sh/">Astral: High-performance Python tooling</a></li>

</ul>
</details>

**标签**: `#ruff`, `#python`, `#linting`, `#astral`, `#tooling`

---

<a id="item-5"></a>
## [Claude Opus 5 抵御提示注入能力最强](https://simonwillison.net/2026/Jul/25/boris-cherny/#atom-everything) ⭐️ 8.0/10

鲍里斯·切尔尼指出，根据 Anthropic 系统卡的评估结果，Claude Opus 5 是最不易受提示注入影响的模型。这标志着大型语言模型安全性的重大改进。 提示注入是大型语言模型的一个关键漏洞，因此更强的防御能力直接提升了 AI 安全性和部署可信度。这可能促进大型语言模型在敏感应用中的更广泛采用。 系统卡显示，Opus 5 在提示注入评估和红队测试中表现良好，难以被成功攻击。该模型价格与 Opus 4.8 相同，并提供双倍成本的快速模式。

rss · Simon Willison · 7月25日 00:42

**背景**: 提示注入是一种网络安全攻击，通过精心设计的输入覆盖系统指令，导致大型语言模型出现意外行为。系统卡是 AI 开发者发布的文档，详细说明模型能力、安全评估和保护措施。这则新闻展示了解决大型语言模型部署中关键漏洞的持续努力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>
<li><a href="https://openai.com/index/gpt-5-5-system-card/">GPT‑5.5 System Card - OpenAI</a></li>

</ul>
</details>

**标签**: `#prompt-injection`, `#anthropic`, `#claude`, `#generative-ai`, `#ai`

---

<a id="item-6"></a>
## [AMD 能否打破英伟达的 CUDA 护城河？](https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing) ⭐️ 8.0/10

一份详细分析 AMD 在挑战英伟达 CUDA 生态系统时所面临挑战和策略的报告，涵盖了智能内核生成、软件质量改进以及 Helios MI455X 生产问题。 AMD 能否打破 CUDA 护城河对于削弱英伟达在 AI 硬件领域的主导地位至关重要，有望降低成本并促进 GPU 市场的创新。 文章提到了利用 LLM 代理进行自动优化的智能内核生成、AMD 不稳定的内部开发集群、Helios MI455X 机架的量产挑战，以及来自金融工程高达 105%的折扣。

rss · Semianalysis · 7月25日 00:33

**背景**: CUDA 是英伟达于 2007 年推出的专有并行计算平台，构建了一个将开发者锁定在英伟达硬件上的软件生态系统。这种“CUDA 护城河”使得即使 AMD 等竞争对手提供有竞争力的硬件，也难以获得市场份额。AMD 正试图通过 ROCm 等举措以及智能内核生成等新方法来克服这一障碍，该方法利用大语言模型自动生成和优化 GPU 内核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://priyanka-dalmia.medium.com/the-cuda-trap-why-nvidias-real-moat-is-software-not-chips-6f97b25b02bc">The “ CUDA Trap”: Why Nvidia’s Real Moat is Software, Not... | Medium</a></li>
<li><a href="https://www.theregister.com/on-prem/2024/12/17/nvidias-cuda-moat-may-not-be-as-impenetrable-as-you-think/1487298">Nvidia's CUDA moat may not be as impenetrable as you think</a></li>
<li><a href="https://introl.com/blog/amd-helios-mi455x-nvidia-competition-ces-2026">AMD Helios Challenges NVIDIA: The MI 455 X and the... | Introl Blog</a></li>

</ul>
</details>

**标签**: `#AMD`, `#CUDA`, `#AI Hardware`, `#Software Ecosystem`, `#GPU Competition`

---

<a id="item-7"></a>
## [携程因数据出境违规被罚 1000 万元](https://t.me/zaihuapd/42758) ⭐️ 8.0/10

2023 年 6 月 13 日，上海携程商务有限公司因未落实数据出境安全评估要求、违法出境个人信息，被上海市网信办处以 1000 万元罚款，并责令限期改正。 此次罚款标志着中国在数据隐私领域加强监管执法，尤其对涉及跨境数据传输的企业。这警示其他互联网公司必须遵守中国数据出境安全评估要求。 处罚包括 1000 万元罚款及限期改正。涉事企业已配合整改。上海市网信办指出，部分民生领域互联网企业仍存在违法出境个人信息行为。

telegram · zaihuapd · 7月25日 02:24

**背景**: 中国的《数据出境安全评估办法》自 2022 年 9 月 1 日起施行，要求数据处理者在向境外提供某些数据前进行安全评估。该法规旨在保护个人信息和国家安全。这些措施是《网络安全法》、《数据安全法》和《个人信息保护法》等更广泛框架的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gov.cn/zhengce/zhengceku/2022-07/08/content_5699851.htm">数据出境安全评估办法_国务院部门文件_中国政府网</a></li>

</ul>
</details>

**标签**: `#data privacy`, `#regulation`, `#cross-border data`, `#China`

---

<a id="item-8"></a>
## [中国对携程罚款 51.79 亿元反垄断](https://t.me/zaihuapd/42767) ⭐️ 8.0/10

2023 年 7 月 25 日，国家市场监督管理总局以滥用市场支配地位为由对携程罚款 51.79 亿元，并责令其退还强制扣除的 1.22 亿元订单储备金，进行全面整改。 这是中国科技行业最大的反垄断罚款之一，表明对在线旅游领域垄断行为的严格监管。它影响携程的主导地位，并为其他平台树立了先例。 罚款包括没收违法所得 16.58 亿元和罚款 35.21 亿元。携程还被要求退还强制从酒店经营者处扣除的 1.22 亿元'订单储备金'。

telegram · zaihuapd · 7月25日 11:56

**背景**: 滥用市场支配地位是指具有市场支配地位的经营者利用其权力限制竞争的行为，例如施加不公平的交易条件。'订单储备金'是携程从酒店经营者处扣留的保证金，监管机构认定这是滥用行为。中国《反垄断法》禁止此类行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.boss-young.com/newsDetail?id=52ddd620-e6d1-45fd-9b5e-08dc0b651319">邦信阳律师事务所</a></li>
<li><a href="https://k.sina.com.cn/article_7879996025_1d5af327906803iaki.html?from=tech">k.sina.com.cn/article_7879996025_1d5af327906803iaki.html?from=tech</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#China`, `#regulation`, `#online travel`, `#monopoly`

---

<a id="item-9"></a>
## [微软通过 TPM 芯片封堵盗版 Windows 激活](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 8.0/10

微软宣布将为 KMS（密钥管理服务）服务器强制要求 TPM 2.0 证明，即服务器必须通过加密方式向微软证明其硬件身份后，才能处理批量激活请求。该强制要求从下一版 Windows Server 开始实施，并将在 2026 年 8 月向 Windows Server 2025 推送准备提示。 此举直接打击了广泛使用的基于 KMS 的盗版方法——攻击者运行伪造的 KMS 服务器来激活未授权的 Windows 副本。通过将激活绑定到可信硬件，微软大大增加了非法激活的难度，可能影响数百万盗版安装，并迫使盗版社区开发新的绕过方法。 TPM 证明功能仅对批量激活强制要求，不影响消费版 Windows。下一个 Windows Server 版本将率先要求 TPM 证明，Windows Server 2025 将在 2026 年 8 月收到准备提示。博文还指出，微软已于 2025 年封堵了 KMS38 漏洞，但 Massgrave 组织推出的新工具 TSforge 声称可以绕过整个 Windows DRM 激活架构。

telegram · zaihuapd · 7月25日 15:55

**背景**: KMS（密钥管理服务）是微软的批量激活方法，供组织在本地激活多个 Windows 和 Office 副本。盗版者长期利用此方法，在互联网或本地设置伪造的 KMS 服务器来激活未授权副本。TPM 2.0（可信平台模块）是一种硬件安全芯片，提供加密证明，确保只有真实且未被篡改的 KMS 服务器才能处理激活请求。这是 Windows 中基于硬件的安全强制执行的更广泛趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/manage/component-updates/tpm-key-attestation">TPM Key Attestation | Microsoft Learn</a></li>
<li><a href="https://massgrave.dev/kms38">KMS38 Documentation | MAS</a></li>
<li><a href="https://github.com/massgravel/TSforge">GitHub - massgravel/TSforge: A collection of activation/evaluation extension methods for Windows Vista through 11. · GitHub</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#Windows`, `#TPM`, `#DRM`, `#Piracy`

---