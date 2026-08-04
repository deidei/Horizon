---
layout: default
title: "Horizon Summary: 2026-08-04 (ZH)"
date: 2026-08-04
lang: zh
---

> 从 41 条内容中筛选出 7 条重要资讯。

---

1. [Keyv 及相关 npm 包遭 Shai-Hulud 供应链攻击](#item-1) ⭐️ 9.0/10
2. [Waymo 无人驾驶出租车服务全面开放达拉斯](#item-2) ⭐️ 8.0/10
3. [DeepSeek V4 Flash 在单块 AMD MI300X 上运行](#item-3) ⭐️ 8.0/10
4. [翁丽莲：缰绳工程，智能体自我改进的新前沿](#item-4) ⭐️ 8.0/10
5. [华为发布“韬定律”：以时间缩微取代几何缩微](#item-5) ⭐️ 8.0/10
6. [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](#item-6) ⭐️ 8.0/10
7. [首部 L3/L4 自动驾驶强制国标报批，2027 年实施](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Keyv 及相关 npm 包遭 Shai-Hulud 供应链攻击](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 9.0/10

新一轮 Shai-Hulud 蠕虫已攻陷广泛使用的 npm 包 Keyv 及数百个其他包，利用预安装脚本窃取凭证，并在可写的 npm 包和 GitHub 仓库中自我传播。 由于 Keyv 是拥有超过 1700 个下游项目的广泛采用的键值存储库，此次攻击可能波及整个 JavaScript 生态，导致开发者凭证、云密钥和下游仓库被窃取或进一步沦陷。这凸显了一个被攻破的依赖即可严重动摇开源软件信任的严峻问题。 恶意版本通过预安装脚本收集仓库、注册表、云服务和私钥凭证，然后借助可用的 npm 发布权限污染更多包。Keyv 仓库中还留有独立的 Claude Code 和 VS Code 工作区钩子，一旦开发者信任该工作区就会执行恶意载荷。

hackernews · cimi_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**背景**: Shai-Hulud 是一种自复制的 npm 蠕虫，于 2025 年 9 月首次被披露，迄今已感染数百个软件包。它通常通过窃取维护者凭证并发布合法包的恶意版本来传播。npm 包常使用 pre-install / post-install 脚本来在安装时执行代码，攻击者会利用这一点在审计之前于开发者或 CI 机器上运行恶意程序。由于依赖关系中包含大量传递依赖，一个包被攻破就可能迅速污染成千上万的项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.jfrog.com/post/shai-hulud-is-back-august/">Major Shai Hulud campaign strikes npm again, affecting keyv and 400+ packages - JFrog Security Research</a></li>
<li><a href="https://thehackernews.com/2026/08/keyv-linked-npm-worm-poisons-hundreds.html">Keyv-Linked npm Worm Poisons Hundreds of Packages, Plants Claude Code and VS Code Hooks</a></li>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem | CISA</a></li>

</ul>
</details>

**社区讨论**: 评论者反应强烈且沮丧，呼吁暂停使用 pre/post-install 钩子，并将任何新增安装钩子视为高度可疑。有人分享了实用的缓解措施，例如在 .npmrc 中设置 min-release-age=5，也有人请求提供扫描 node_modules 和 pnpm store 的命令。还有人感叹依赖系统异常脆弱，且一旦被污染很难彻底清理。

**标签**: `#security`, `#npm`, `#supply chain attack`, `#open source`, `#malware`

---

<a id="item-2"></a>
## [Waymo 无人驾驶出租车服务全面开放达拉斯](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo 宣布其无人驾驶叫车服务现已在德克萨斯州达拉斯向所有人开放。这让达拉斯成为最新一个任何人都能叫到完全自动驾驶车辆的主要都市区。 此次扩张将商用自动驾驶汽车带到一个高度依赖汽车、低密度的大型都会区，为有限的公共交通提供了替代方案。它还可能影响城市政策，一些人认为无人驾驶汽车可以减少停车需求并支持经济适用房。 该服务可通过 Waymo 应用使用，Google 支持页面显示了达拉斯服务区域。Waymo 是 Alphabet 的子公司，前身为 Google 自动驾驶汽车项目。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**背景**: Waymo 是一家自动驾驶汽车公司，也是美国领先的 Robotaxi 商业化运营商。它始于 Google 自动驾驶汽车项目，并已在凤凰城、旧金山和洛杉矶等城市运营。达拉斯-沃斯堡是美国前五大都会区之一，但人口密度极低、以汽车为中心，公共交通选择很少，因此成为一个重要的新测试场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://waymo.com/">Waymo - Self-Driving Cars - Autonomous Vehicles - Ride-Hail</a></li>
<li><a href="https://builtin.com/articles/waymo-robotaxis">Waymo Explained: Alphabet’s Autonomous Vehicle Company | Built In</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了积极的实际体验，指出 Waymo 已变得平常，且比人类驾驶员引发的事故更少，也有人提到偶尔会出现卡住的情况。一位商业房地产专业人士认为无人驾驶汽车是一种有效的经济适用房政策，另一位则表达了对 Waymo 这一先进消费级交互机器人的关注度意外地低。

**标签**: `#autonomous vehicles`, `#Waymo`, `#transportation`, `#urban policy`, `#AI`

---

<a id="item-3"></a>
## [DeepSeek V4 Flash 在单块 AMD MI300X 上运行](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

一份技术指南和基准测试展示了 DeepSeek V4 Flash 在单块 AMD MI300X GPU 上运行的可行性，性能良好（每秒超过 150 tokens），但上下文窗口从原来的 1M tokens 降低到了 256K tokens。 这意义重大，因为它表明大型混合专家（MoE）模型可以在单个 AMD 加速器上部署，降低了硬件门槛，并为推理提供了实用的权衡分析。这也凸显了 AMD 在 AI 推理领域日益重要的地位，以及平衡模型量化与上下文长度的重要性。 该基准测试保留了模型的完整推理权重，没有进行激进量化，速度仍超过每秒 150 tokens，主要代价是上下文窗口缩小到 256K tokens。MI300X 是 OAM 模组，配备 192GB HBM3 内存；而内存较小的 PCIe 版 MI350P（144GB）也应该能运行该模型，因为其 256 个混合专家（MoE）专家使用了原生 MXFP4 量化。

hackernews · zhoutong · 8月4日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49166386)

**背景**: DeepSeek V4 Flash 是一款混合专家（MoE）架构的大型语言模型，总参数量为 2840 亿，属于 DeepSeek V4 系列（该系列还包括 1.6 万亿参数的 V4-Pro）。该模型专为 1M token 的上下文窗口训练，是更大 Pro 型号的高性价比替代品；一个更新的检查点显著增强了其智能体（agent）能力。AMD Instinct MI300X 是 AMD 的旗舰数据中心加速器，配备 192GB HBM3 内存和 5.3 TB/s 带宽，可通过 RunPod 等云服务商租用。MXFP4 等量化技术可减少内存占用，使大型模型能够在单块 GPU 上运行，但有时会在长上下文任务上牺牲性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek V 4 Explained: V 4 -Pro 1.6T vs V 4 - Flash 284B (2026)</a></li>
<li><a href="https://canitrun.dev/gpus/mi300x/">AMD Instinct MI 300 X — 192 GB VRAM: Which LLMs... — CanItRun</a></li>
<li><a href="https://www.remio.ai/post/deepseek-v4-flash-reportedly-outperforms-its-larger-sibling-on-agent-tasks">DeepSeek V 4 Flash Reportedly Outperforms Its Larger Sibling on...</a></li>

</ul>
</details>

**社区讨论**: 评论者总体上持肯定态度，称赞这种诚实的权衡分析：该配置保留了全精度权重，速度超过每秒 150 tokens，只是上下文窗口从 1M 缩小到 256K。也有人提出了硬件方面的顾虑，指出 MI300X 通常以 8 卡整机形式销售、价格约 25 万欧元，而基于 PCIe 的 MI350P（144GB）由于模型原生 MXFP4 量化，也应该能够运行该模型。还有评论者提到 DwarfStar 等先前工作占用内存更少，并推荐通过 HotAisle 租用 MI300X 进行实验。

**标签**: `#deepseek`, `#amd`, `#mi300x`, `#llm-inference`, `#quantization`

---

<a id="item-4"></a>
## [翁丽莲：缰绳工程，智能体自我改进的新前沿](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 8.0/10

翁丽莲的博文提出“缰绳工程”（harness engineering）——即优化 AI 智能体周围的工具、技能、提示词和脚手架——作为实现智能体自我改进的新方向。该文将自我改进重新定义为一个优化缰绳而非仅调整模型权重的问题。 当模型能力趋于平台期时，优化缰绳可以为智能体带来性能、成本效益和可靠性上的显著提升。这一转变可能重塑组织规模化部署 AI 编程智能体的方式，也改变业界在权重训练之外看待自我改进的思路。 缰绳工程的概念源自软件测试中的测试脚手架（test harness），在智能体语境下涵盖其整个运行环境。实践者强调的关键杠杆包括：为代码库构建适应度函数、利用生产轨迹发现真实问题、让智能体自己编写工具（例如将上下文加载从 15 次调用消耗 20k tokens 降至单次调用 800 tokens），以及使用 eval/test 划分来防止奖励作弊。

hackernews · tosh · 8月4日 06:17 · [社区讨论](https://news.ycombinator.com/item?id=49164896)

**背景**: 缰绳工程是一门新兴学科，专注于设计、构建和维护大规模编排 AI 智能体的基础设施，包括提示词、工具、技能和评估循环。它与提示词工程（优化单次交互）和上下文工程（管理上下文窗口）不同，它构建的是智能体运行所处的外部世界。“Harness”一词借自软件工程中的测试脚手架，用于控制和观察被测系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/harness-engineering-discipline-decides-how-smart-your-parag-patil-uqhzf">Harness Engineering : The Discipline That Decides How Smart Your...</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-harness-engineering-beyond-prompt-context-engineering">How Stripe Ships 1,300 AI PRs a Week: Harness Engineering</a></li>
<li><a href="https://outcomeschool.com/blog/harness-engineering-in-ai">In this blog, we will learn about Harness Engineering in AI .</a></li>

</ul>
</details>

**社区讨论**: 实践者讨论展现出浓厚的动手兴趣：有人分享用生产轨迹自动化研究缰绳效果惊人，有人呼吁为代码库建立通用且准确的适应度函数以支持智能体自我优化。还有人认为正在从训练权重转向训练提示词和代码的范式，另有人提问缰绳何时能自行生成 RLHF/DPO 训练数据用于 LoRA 微调。也有轻松评论调侃对“Torment Nexus”的不懈追求。

**标签**: `#AI engineering`, `#LLM agents`, `#self-improvement`, `#harness optimization`

---

<a id="item-5"></a>
## [华为发布“韬定律”：以时间缩微取代几何缩微](https://t.me/zaihuapd/42966) ⭐️ 8.0/10

在上海举行的 2026 国际电路与系统研讨会（ISCAS 2026）上，华为半导体业务部总裁何庭波正式提出“韬定律”（τ定律），主张以“时间缩微”替代“几何缩微”作为半导体演进的新指导原则。华为称过去六年已据此设计量产 381 款芯片，今年秋季将推出采用逻辑折叠技术的新麒麟芯片。 在摩尔定律逼近物理与经济极限之际，“韬定律”为半导体产业提供了一条不单纯依赖制程缩小的替代演进路径，具有潜在的范式转换意义。若得到验证，它可能重塑芯片设计策略与产业竞争格局，尤其是在出口限制下对华为及中国半导体生态意义重大。 “韬定律”以系统性降低时间常数（韬τ）为目标，通过逻辑折叠等创新技术持续压缩信号传播时延，从而提升晶体管密度。华为预计到 2031 年，基于该定律的高端芯片晶体管密度可达 1.4 纳米制程同等水平；何庭波还撰写了题为《多层电子系统的时间缩微理论》的论文，发布在中国科学院科技论文预发布平台上。

telegram · zaihuapd · 8月4日 08:04

**背景**: 半个多世纪以来，半导体产业的进步主要依赖摩尔定律，即通过不断缩小晶体管几何尺寸来提升性能与集成度，但如今这一路径正逼近物理极限，进一步微缩的成本和难度急剧上升。“时间缩微”则转而压缩信号传播的时间常数（τ），在器件、电路、芯片、系统等多个层面进行协同优化，从而在不极度依赖制程缩小的前提下维持性能与密度提升。逻辑折叠正是实现这一目标的创新技术之一，通过优化信号路径、复用逻辑模块、降低时延来提升晶体管密度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260525/herald/1573642c437a5e4e76a15fc1c40f0a35.html">华为提出的“韬定律”是什么？跟摩尔定律有什么不同？ - 21经济网</a></li>
<li><a href="https://www.guancha.cn/economy/2026_05_25_818313.shtml">何庭波万字论文，详述华为“韬定律”-观察者网</a></li>
<li><a href="https://caifuhao.eastmoney.com/news/20260525164059876078810">从非系统观下的“几何压缩”到系统观下的“时间压缩”：什么是半导体的“逻辑折叠技术”？_财富号_东方财富网</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#Huawei`, `#chip design`, `#scaling`, `#logic folding`

---

<a id="item-6"></a>
## [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

据《金融时报》调查，谷歌悄然搭建了史上最大规模的基础设施融资架构之一，通过约 2000 亿美元的合同向 Anthropic 交付超过 1500 亿美元的 AI 芯片。参与方包括博通、阿波罗、黑石、摩根士丹利及多家加密矿企。 这种金融工程可能重塑 AI 算力的融资方式，将巨额硬件投资移出资产负债表，并把风险分散给华尔街机构。它凸显了扩展前沿 AI 所需的巨大资本，也可能影响其他大型云厂商为 AI 基础设施融资的模式。 今年 6 月，特殊目的载体 Compute SPV 完成首批交易，购入约 350 亿美元硬件，约合 1 吉瓦算力、100 万颗 TPU。该模式借鉴波音和 GE 推销飞机和发动机的厂商融资玩法：谷歌担保数据中心，博通购买并协助融资芯片，阿波罗和黑石购买硬件后回租给 Anthropic。

telegram · zaihuapd · 8月4日 10:52

**背景**: 特殊目的载体(SPV)是用于隔离金融风险的独立法律实体，常见于大型基础设施项目。张量处理单元(TPU)是谷歌为加速机器学习工作负载而设计的定制专用集成电路(ASIC)。由于 Anthropic 没有信用评级，这笔交易将风险分散给多个投资者，而不是把数千亿美元压在任何一个资产负债表上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.investopedia.com/terms/s/spv.asp">investopedia.com/terms/s/ spv .asp</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tensor_Processing_Unit">Tensor Processing Unit - Wikipedia</a></li>
<li><a href="https://345tool.com/news/apollo-and-blackstone-raise-36b-to-lease-google-tpus-for-anthropic-in-largest-ch-2">Apollo and Blackstone Raise $36B to Lease Google... | 345tool News</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#Anthropic`, `#Google`, `#financing`, `#cloud computing`

---

<a id="item-7"></a>
## [首部 L3/L4 自动驾驶强制国标报批，2027 年实施](https://t.me/zaihuapd/42972) ⭐️ 8.0/10

工信部已完成《智能网联汽车自动驾驶系统安全要求》强制性国家标准报批稿，并于 6 月 17 日起公示，建议 2027 年 7 月 1 日实施。这是我国首部针对 L3/L4 级自动驾驶的强制性安全标准。 这是一座监管里程碑，标志着中国自动驾驶监管从"概念松绑"转向"安全硬约束"。新标准将迫使车企通过 Safety Case 机制系统性论证安全性，对 L3/L4 车型开发、AI 安全验证和行业实践产生深远影响。 该标准适用于搭载 L3、L4 级系统的 M 类和 N 类车辆，不适用于自动泊车系统。标准引入 Safety Case（安全档案）机制，要求企业以"声明—论据—证据"的结构化论证证明安全性，并对 L3 人机交接和 L4 系统自主风险处置分别提出要求。

telegram · zaihuapd · 8月4日 13:06

**背景**: L3 级为有条件自动驾驶，L4 级为高度自动驾驶，均由系统在特定条件下执行驾驶任务。此前中国缺乏针对这两个级别的强制性国家安全标准，主要依靠推荐性指南和团体标准。全球范围内 Waymo、Uber 等自动驾驶车辆事故表明，功能实现不等于安全保障，因此监管机构开始引入如 Safety Case 这类结构化安全论证体系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.autohome.com.cn/news/202608/1316205.html">autohome.com.cn/news/202608/1316205.html</a></li>
<li><a href="https://www.163.com/dy/article/L01347E80547KOTE.html">163.com/dy/article/L01347E80547KOTE.html</a></li>
<li><a href="https://m.163.com/dy/article/K1BTJR1H0514R9KQ.html">m.163.com/dy/article/K1BTJR1H0514R9KQ.html</a></li>

</ul>
</details>

**标签**: `#autonomous-driving`, `#regulation`, `#safety-standards`, `#AI`, `#automotive`

---