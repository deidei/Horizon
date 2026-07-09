---
layout: default
title: "Horizon Summary: 2026-07-09 (ZH)"
date: 2026-07-09
lang: zh
---

> 从 36 条内容中筛选出 12 条重要资讯。

---

1. [TypeScript 7.0 用 Go 重写，构建速度提升 12 倍](#item-1) ⭐️ 9.0/10
2. [FTC 协议要求约翰迪尔允许用户自行维修设备](#item-2) ⭐️ 8.0/10
3. [OpenAI 分析揭示编程基准测试中的噪音问题](#item-3) ⭐️ 8.0/10
4. [Bun 借助 AI 将运行时代码从 Zig 重写为 Rust](#item-4) ⭐️ 8.0/10
5. [SpaceXAI 发布 Grok 4.5：更快、更便宜、达到 Opus 水平的 AI 模型](#item-5) ⭐️ 8.0/10
6. [解码优衣库 T 恤上的混淆 Bash 脚本](#item-6) ⭐️ 8.0/10
7. [Cloudflare Meerkat：首个生产级异步共识算法](#item-7) ⭐️ 8.0/10
8. [OpenAI 推出 GPT-Live，升级 ChatGPT 语音模式](#item-8) ⭐️ 8.0/10
9. [灵波视频：开源稀疏 MoE 视频扩散变换器](#item-9) ⭐️ 8.0/10
10. [美团 OWL 模型对话数据疑似泄露于 GitHub](#item-10) ⭐️ 8.0/10
11. [通过泄漏电磁信号识别手机应用，准确率达 99%](#item-11) ⭐️ 8.0/10
12. [LineageOS 推出浏览器刷机工具](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [TypeScript 7.0 用 Go 重写，构建速度提升 12 倍](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

微软正式发布 TypeScript 7.0，这是一个用 Go 语言重写的主版本，相比 TypeScript 6，构建速度最高提升 12 倍，例如 vscode 的构建时间从 125.7 秒降至 10.6 秒。 这一性能提升大幅减少了大型代码库的开发者等待时间，使 TypeScript 更适用于庞大项目，并可能加速 CI/CD 流水线，同时展示了用底层语言重写性能关键的编译器所带来的好处。 新版本引入了 --checkers 和 --builders 参数以自定义并行度，并提供了兼容包以便与 TypeScript 6 并存；但 Vue、Svelte 等嵌入式语言的工具链尚未就绪，目前仍需使用旧版本。

hackernews · DanRosenwasser · 7月8日 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48833715)

**背景**: TypeScript 是 JavaScript 的超集，它添加了静态类型，帮助开发者早期捕获错误。此前，TypeScript 编译器是用 TypeScript 自身编写的，这限制了其在大型代码库上的性能。用 Go 重写使其能够利用原生编译和多线程，从而实现了本次发布中显著的性能提升。

**社区讨论**: 评论称赞团队取得的成就，用户分享了基准测试数据并对速度提升表示兴奋。一些用户表示仍然喜欢 JSDoc 类型语法，另一些则开玩笑期待 Rust 重写版本。

**标签**: `#TypeScript`, `#performance`, `#Go`, `#compiler`, `#programming languages`

---

<a id="item-2"></a>
## [FTC 协议要求约翰迪尔允许用户自行维修设备](https://apnews.com/article/john-deere-right-to-repair-agriculture-equipment-cb7514ffedb95c130a976af661f2bc02) ⭐️ 8.0/10

美国联邦贸易委员会（FTC）已与约翰迪尔达成和解，要求该公司允许农民和独立维修店修理迪尔设备。该和解结束了多年来迪尔限制诊断软件和维修工具使用的做法。 这一和解是维修权运动的重要胜利，赋予农民自行修理拖拉机的权利，减少了对昂贵经销商维修的依赖。它可能为电子、汽车等其他存在类似限制的行业树立先例。 约翰迪尔需向五个州共同支付 100 万美元的反垄断执法费用，并接受为期十年的合规监督。该和解特别针对此前阻止车主未经经销商授权诊断和修复问题的软件锁。

hackernews · djoldman · 7月8日 23:37 · [社区讨论](https://news.ycombinator.com/item?id=48838876)

**背景**: 现代拖拉机包含精密的计算机系统，控制从发动机正时到 GPS 导航的方方面面。约翰迪尔等制造商利用数字版权管理（DRM）锁定这些系统，迫使农民只能依赖授权经销商进行维修。这种做法导致农民自行破解设备或从海外购买非法诊断工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pirg.org/resources/john-deere-and-right-to-repair-over-the-years/">John Deere and Right to Repair over the years - pirg.org</a></li>
<li><a href="https://copperhilltech.com/blog/farmers-are-hacking-their-tractors-because-of-a-right-to-repair-ban/">Farmers Are Hacking Their Tractors Because of a Right to Repair Ban</a></li>

</ul>
</details>

**社区讨论**: 评论赞扬了路易斯·罗斯曼等活动家在维修权运动中的贡献。有人批评 100 万美元罚款相对于迪尔的利润微不足道，也有人讨论了这对科技公司和消费者权利的广泛影响。

**标签**: `#right-to-repair`, `#consumer rights`, `#agriculture technology`, `#FTC`, `#regulatory policy`

---

<a id="item-3"></a>
## [OpenAI 分析揭示编程基准测试中的噪音问题](https://openai.com/index/separating-signal-from-noise-coding-evaluations/) ⭐️ 8.0/10

OpenAI 发布分析报告，指出流行的编程基准测试 SWE-Bench Pro 存在大量噪音，许多任务规格不完整或自相矛盾，并提出了改进评估可靠性的方法。 准确的编程评估对于安全部署 AI 模型至关重要，有缺陷的基准测试可能会误导对模型能力的判断，进而影响整个 AI 行业的开发和安全决策。 OpenAI 团队手动审查了 SWE-Bench Pro 中全部 798 个任务，发现 48%存在问题，包括缺失测试、需求模糊或真实解决方案中存在错误，导致模型性能被高估。

hackernews · sk4rekr0w · 7月8日 21:03 · [社区讨论](https://news.ycombinator.com/item?id=48837396)

**背景**: SWE-Bench Pro 是一个旨在评估 AI 模型在真实软件工程任务（如修复漏洞或实现功能）上表现的基准测试。信噪比概念源自工程学，用于描述评估结果中有意义数据（信号）与无关或误导数据（噪音）的比例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/separating-signal-from-noise-coding-evaluations/">Separating signal from noise in coding evaluations - OpenAI</a></li>
<li><a href="https://judyailab.com/en/posts/ai-news-20260709-separating-signal-from-noise-in-coding-evaluations/">How to Distinguish Real Capability from Noise in Code Evaluations</a></li>
<li><a href="https://en.wikipedia.org/wiki/Signal-to-noise_ratio">Signal-to-noise ratio - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了怀疑态度，指出基准测试的缺陷早已知晓但被低估，并呼吁采用结合效率与智能的新指标，例如衡量每单位 API 花费的成果。其他人还指出了作弊和硬件配置操纵等问题。

**标签**: `#AI evaluation`, `#coding benchmarks`, `#OpenAI`, `#machine learning`, `#benchmark reliability`

---

<a id="item-4"></a>
## [Bun 借助 AI 将运行时代码从 Zig 重写为 Rust](https://bun.com/blog/bun-in-rust) ⭐️ 8.0/10

流行的 JavaScript 运行时 Bun 借助 AI 工具 Fable 和 Claude Code，将其核心运行时代码从 Zig 重写为 Rust，实现了 20% 的二进制文件缩小、稳定性提升以及 5% 的性能改进。 此次重写展示了 AI 辅助代码翻译在大幅降低工程成本和时间方面的潜力，同时也引发了关于语言选择以及高性能运行时的系统编程未来的讨论。 该项目由一位工程师使用 Fable（自动翻译管道）和 Claude Code 进行代码审查和修复，在更短的时间内完成了一个工程团队可能需要一年才能完成的工作。

hackernews · afturner · 7月8日 21:49 · [社区讨论](https://news.ycombinator.com/item?id=48837877)

**背景**: Bun 是一个快速的一体化 JavaScript 运行时，用于捆绑、安装和运行 JavaScript 和 TypeScript。它最初使用 Zig 编写，Zig 是一种旨在改进 C 语言的系统编程语言。Rust 则是另一种注重内存安全和并发性且无需垃圾回收的系统语言。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/bun: Incredibly fast JavaScript runtime, bundler, test runner, and package manager – all in one</a></li>

</ul>
</details>

**社区讨论**: 评论者们讨论了这一事件对 Zig 的影响，一些人指出从 Zig 的简单重写就修复了内存泄漏并提高了稳定性，这对 Zig 的声誉不利。其他人则强调了使用 AI 而非雇佣工程师的成本效益，而有些人批评了过渡的处理方式，例如放弃对 Zig 版本的修复。

**标签**: `#Rust`, `#Zig`, `#AI-assisted development`, `#JavaScript runtime`, `#software engineering`

---

<a id="item-5"></a>
## [SpaceXAI 发布 Grok 4.5：更快、更便宜、达到 Opus 水平的 AI 模型](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

SpaceXAI 发布了 Grok 4.5，这是一款新型 AI 模型，其推理效率比 Opus 提升 4 倍，而成本仅为每百万输入令牌 2 美元、每百万输出令牌 6 美元。 Grok 4.5 卓越的令牌效率和更低的价格可能颠覆 AI 市场，但有关 xAI 可信度的伦理担忧可能阻碍其在敏感商业应用中的采用。 Grok 4.5 是一款“Opus 级别模型”，比竞争对手更快、令牌效率更高；它基于数万亿令牌的 Cursor 数据训练而成，这些数据捕获了真实的开发者交互。

hackernews · BoumTAC · 7月8日 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48835111)

**背景**: Grok 4.5 是 xAI 的最新型号，xAI 由埃隆·马斯克于 2023 年创立，后来被 SpaceX 收购成为 SpaceXAI。该模型利用了被 SpaceXAI 收购的 AI 编码初创公司 Cursor 的数据，以增强编码和代理任务的能力。令牌效率指模型每令牌生成更有用输出的能力，从而降低用户的总体成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/news/grok-4-5">Introducing Grok 4.5 | SpaceXAI</a></li>
<li><a href="https://techcrunch.com/2026/07/08/spacexai-releases-grok-4-5-which-elon-describes-as-an-opus-class-model/">SpaceXAI releases Grok 4.5, which Elon describes as an 'Opus-class model' | TechCrunch</a></li>
<li><a href="https://www.axios.com/2026/07/08/spacexai-grok-new-model">Scoop: SpaceXAI launches new model, Grok 4.5</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人称赞 Grok 4.5 的速度和成本效益，而另一些人则因 xAI 的政治倾向和伦理问题（如对儿童性虐待材料审核不足）表示不信任。技术用户将其在基准测试上与 GPT 和 Opus 进行有利比较。

**标签**: `#AI`, `#LLM`, `#Grok`, `#xAI`, `#machine learning`

---

<a id="item-6"></a>
## [解码优衣库 T 恤上的混淆 Bash 脚本](https://tris.sherliker.net/blog/obfuscated-self-evaluating-bash-script-by-cdn-akamai-being-supplied-to-consumers-via-retail-stores/) ⭐️ 8.0/10

Tristan Sherliker 的博客文章解码了印在优衣库 T 恤上的混淆 bash 脚本，发现它是一个自我求值的脚本，运行后会打印一个数学公式。 这个例子展示了 bash 中巧妙的混淆技术，引发了社区关于代码美学、字体排印以及编程与时尚交叉的讨论。 该脚本使用了 bash 混淆中常见的自我求值技术，衬衫上的字体是 Roboto Mono，并采用了光学字距调整，使得 OCR 识别困难。

hackernews · speerer · 7月8日 08:46 · [社区讨论](https://news.ycombinator.com/item?id=48829312)

**背景**: Bash 混淆是指故意使 shell 脚本难以阅读，通常通过编码、压缩或变量替换来实现。自我求值脚本会在运行时构建并执行代码。这款与 Akamai 合作的优衣库 T 恤将脚本作为时尚宣言印在衣服上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vuink.com/post/gevf-d-dfureyvxre-d-darg/blog/obfuscated-self-evaluating-bash-script-by-cdn-akamai-being-supplied-to-consumers-via-retail-stores">Obfuscated, self-evaluating bash script by CDN Akamai being ...</a></li>
<li><a href="https://github.com/Bashfuscator/Bashfuscator">GitHub - Bashfuscator/Bashfuscator: A fully configurable and ...</a></li>
<li><a href="https://www.baeldung.com/linux/bash-obfuscate-script">How to Obfuscate a Bash Script to Make It Unreadable - Baeldung</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了设计的巧妙。有人指出字体是 Roboto Mono 但字距调整是光学的，破坏了等宽一致性。其他人分享了类似作品，比如 Martin Kleppe 的 Quine Clock。还有关于 OCR 难度的讨论，以及好奇原始脚本是否由 LLM 编写。

**标签**: `#obfuscation`, `#bash`, `#hackernews`, `#t-shirt`, `#Uniqlo`

---

<a id="item-7"></a>
## [Cloudflare Meerkat：首个生产级异步共识算法](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 8.0/10

Cloudflare Research 推出了基于 QuePaxa 算法的全球分布式共识服务 Meerkat，这是首个生产级实现的异步无领导共识协议。该服务旨在为键值存储等应用提供强一致性和容错能力。 这标志着异步共识——无需依赖超时并能容忍极端网络延迟——从研究走向实际部署的重要一步。它可能提升那些在恶劣网络条件下难以使用 Raft 等基于领导者的协议的全球分布式系统的可靠性。 Meerkat 使用 QuePaxa，该算法通过 hedging（向多个提议者发送冗余提议）来在无超时情况下保持活性，即使在网络分区或延迟下也能推进。但每次读取操作都需要全局共识，这可能会增加读取延迟，相比优化本地读取的系统有所妥协。

hackernews · bobnamob · 7月8日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=48831565)

**背景**: 生产环境中大多数共识算法（如 Paxos 和 Raft）都是部分同步的：它们依赖超时检测故障，并假设网络延迟有界。像 QuePaxa 这样的异步共识算法完全避免超时，因此在无限延迟下依然稳健，但历史上因效率低而不实用。QuePaxa 在 SOSP 2023 上发表，引入了自适应 hedging 等技术，在正常情况下的性能具有竞争力，同时在最坏情况下保持韧性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/meerkat-introduction/">Introducing Meerkat: an experiment in global consensus</a></li>
<li><a href="https://bford.info/pub/os/quepaxa/quepaxa.pdf">QuePaxa: Escaping the Tyranny of Timeouts in Consensus QuePaxa: Escaping the Tyranny of Timeouts in Consensus GitHub - dedis/quepaxa: This is the code repository for ... QuePaxa: Escaping the Tyranny of Timeouts in Consensus Post by @cloudflare.social — Bluesky Artifact Review Summary: QuePaxa: Escaping the tyranny of ...</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，将无领导的 Meerkat 与基于领导者的 Raft 进行比较有些令人困惑，并强调了 QuePaxa 异步特性的新颖性。部分人质疑每次读取都要共识的权衡，而另一些人则认为这对网络混乱、以领导者协议易受影响的环境很有价值。

**标签**: `#distributed systems`, `#consensus algorithms`, `#Cloudflare`, `#QuePaxa`, `#asynchronous consensus`

---

<a id="item-8"></a>
## [OpenAI 推出 GPT-Live，升级 ChatGPT 语音模式](https://simonwillison.net/2026/Jul/8/introducing-gptlive/#atom-everything) ⭐️ 8.0/10

OpenAI 宣布推出 GPT-Live，这是一个为 ChatGPT 语音模式提供支持的新模型，它可以在后台将复杂任务委托给 GPT-5.5，同时保持对话流畅。 这次升级显著提高了 ChatGPT 语音模式的实用性，使其能够进行实时、自然的对话，同时处理网络搜索、推理等复杂任务而不中断。 GPT-Live 目前在 iPhone 应用中可用，使用 GPT-5.5 作为其前沿模型，并计划随着新模型的发布持续更新。有用户报告了一个不恰当笑声的 bug，据称已修复。

rss · Simon Willison · 7月8日 23:20

**背景**: ChatGPT 之前的语音模式基于较旧的 GPT-4o 时代模型，知识截止于 2024 年，限制了其用途。GPT-Live 代表了新一代语音模型，旨在实现更自然的人机交互，能够通过将复杂查询卸载给更强大的模型（如 GPT-5.5）来执行多任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT-Live | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT‑5.5 - OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-Live`, `#ChatGPT`, `#voice mode`, `#AI update`

---

<a id="item-9"></a>
## [灵波视频：开源稀疏 MoE 视频扩散变换器](https://www.reddit.com/r/MachineLearning/comments/1ur0bxq/lingbotvideo_sparsemoe_video_diffusion/) ⭐️ 8.0/10

灵波视频是一个 13B 参数（1.4B 激活）的稀疏混合专家视频扩散变换器，采用强化学习后训练，使用 VLM 评分的物理合理性奖励。它以开源形式发布，包含权重、代码和 Diffusers/SGLang 栈，并具有用于机器人滚动预测的动作到视频模式。 该模型代表了机器人开源视频生成的重要一步，结合了稀疏 MoE 效率和基于强化学习的物理合理性奖励。然而，它也提出了关键问题：VLM 评分的奖励能否可靠地判断物理合理性？仅靠视频生成是否能作为真正的机器人策略世界模型？ 灵波视频采用单流扩散变换器，具有 DeepSeek-V3 风格的稀疏 MoE（128 个专家，前 8 路由）。它使用六种奖励进行后训练，包括由 VLM 从采样帧评分的物理合理性奖励，并添加真实视频负样本以防止奖励破解。

reddit · r/MachineLearning · /u/Savings-Display5123 · 7月8日 17:58

**背景**: 混合专家（MoE）是一种技术，模型使用多个专门的子网络（专家）和路由机制，每个输入只激活一部分专家，从而实现更大的总容量和更低的计算成本。稀疏 MoE 如 DeepSeek-V3，每个令牌只激活一部分专家。动作条件世界模型根据机器人动作预测未来视频帧，充当机器人领域的规划器或评估器。灵波视频被定位为此类模型，但只展示了视频生成结果，没有闭环机器人评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://arxiv.org/abs/2606.04463">OSCAR: Omni-Embodiment Action-Conditioned World Model for ...</a></li>

</ul>
</details>

**社区讨论**: Reddit 帖子作者邀请批评，特别质疑 VLM 能否成为物理合理性的可靠评判者，还是会导致奖励破解，以及在没有闭环机器人数据的情况下，视频生成器和世界模型之间的界限在哪里。作者表达了希望社区对这些问题的看法。

**标签**: `#video diffusion`, `#sparse MoE`, `#reinforcement learning`, `#world model`, `#open source`

---

<a id="item-10"></a>
## [美团 OWL 模型对话数据疑似泄露于 GitHub](https://github.com/gumusserv/ProducerBenchV2/blob/83cad6007ef3fe8df33386e8f43738fe62337e16/parsed_source_data/data/) ⭐️ 8.0/10

美团免费测试模型 OWL（LongCat）的对话数据疑似在 GitHub 仓库上泄露，该仓库已被下架。泄露由 Discord 机器人令牌扫描器发现，并触发了令牌重置。 此事件凸显了大语言模型部署中反复出现的安全与隐私风险，尤其是当用户对话被记录并暴露时。它强调了企业保护 AI 工作流中敏感数据的迫切需求，以及用户应避免向 AI 模型分享凭证或专有信息。 根据用户截图，该仓库至少在 2026 年 7 月 7 日公开可见。泄露的数据据称包含美团 OWL 模型的对话记录，OWL 是 OpenRouter 上的测试模型，泄露事件被一个 Discord 机器人令牌扫描器发现。

telegram · zaihuapd · 7月8日 13:35

**背景**: 美团近期开源了 LongCat-2.0，这是一个 1.6 万亿参数的 MoE 模型，每个令牌激活约 480 亿参数，该模型驱动着 OpenRouter 上的 OWL 模型。OpenRouter 是一个统一 API 平台，提供对数百个来自不同提供商的大语言模型的访问。类似的数据泄露此前也曾发生在 Google、DeepSeek 等 AI 提供商身上，其用户对话被用于模型改进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geopolitechs.org/p/longcat-20-chinas-most-unexpected">LongCat-2.0: China's Most Unexpected AI Model</a></li>
<li><a href="https://venturebeat.com/technology/meituan-open-sources-longcat-2-0-the-1-6t-near-frontier-agentic-coding-model-thats-been-leading-openrouter-trained-entirely-on-chinese-chips">Meituan open sources LongCat-2.0, the 1.6T, near-frontier agentic coding model that's been leading OpenRouter — trained entirely on Chinese chips | VentureBeat</a></li>

</ul>
</details>

**标签**: `#data leak`, `#AI security`, `#privacy`, `#large language models`, `#Meituan`

---

<a id="item-11"></a>
## [通过泄漏电磁信号识别手机应用，准确率达 99%](https://www.scmp.com/news/china/science/article/3359688/chinese-researchers-find-peephole-any-smartphone-its-leaked-radio-signal) ⭐️ 8.0/10

中国研究人员开发出一种非接触式技术，通过分析手机泄漏的低频电磁信号来识别正在使用的应用，在 iPhone 15 Pro、小米 15 Pro 和 OPPO Reno 13 上的准确率最高达到 99.07%。 这项技术代表了一种新型侧信道攻击，即使设备处于离线、飞行模式、加密或锁定状态也能工作，给隐私带来重大风险，同时为数字取证提供了无需物理接触的新能力。 该研究测试了抖音（TikTok）、微信视频通话、百度地图、短信、浏览器、相机和云存储等应用。该方法无需访问操作系统或存储数据，仅依赖每个应用独特的电磁信号特征。

telegram · zaihuapd · 7月8日 16:05

**背景**: 侧信道攻击利用电磁辐射等物理泄漏来推断敏感信息。智能手机在运行时会产生低频电磁信号，不同应用会生成独特模式。这种非接触式数字取证技术可从远处捕获这些信号，从而在不接触设备的情况下识别应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ckhq.net/html/6c1af61946e47994a7d682373d5f7757.html">中国科研团队研发非接触式智能手机应用识别技术，准确率达99.07%</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/25590891831">什么是 Side Channel Attack（侧信道攻击）？ - 知乎</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#smartphone`, `#electromagnetic signals`, `#side-channel attack`

---

<a id="item-12"></a>
## [LineageOS 推出浏览器刷机工具](https://www.androidauthority.com/lineageos-summertime-update-2026-3685112/) ⭐️ 8.0/10

LineageOS 发布了 Lineage Flash Tools，这是一款基于网页的工具，用户无需本地安装 adb 和 fastboot 即可直接在浏览器中刷机。团队还宣布基于 Android 17 的 LineageOS 24 已开始开发。 这降低了安装自定义 ROM 的门槛，使不太懂技术的用户也能轻松上手。即将推出的基于 Android 17 的 LineageOS 24 表明团队持续致力于支持最新 Android 版本。 该工具支持 Fastboot、ADB 以及三星的 Odin 协议，需要使用支持 WebUSB 的浏览器（如 Chrome 或 Edge）。它必须配合设备专属的 Wiki 安装指南使用，并不能完全替代传统刷机流程。

telegram · zaihuapd · 7月9日 01:46

**背景**: WebUSB 是一种 JavaScript API，允许网页应用安全地与 USB 设备通信，从而实现基于浏览器的刷机。三星设备通常使用 Odin 协议而非 fastboot 进行固件刷写。A/B OTA 流式安装只下载更新包中需要的部分，以节省空间并加快更新速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebUSB">WebUSB - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Odin_(firmware_flashing_software)">Odin (firmware flashing software) - Wikipedia</a></li>
<li><a href="https://source.android.com/docs/core/ota/ab">A/B (seamless) system updates | Android Open Source Project</a></li>

</ul>
</details>

**标签**: `#LineageOS`, `#Android`, `#custom ROM`, `#WebUSB`, `#flashing`

---