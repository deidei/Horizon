---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> 从 33 条内容中筛选出 12 条重要资讯。

---

1. [OpenAI 发布数学与理论计算机科学十大进展](#item-1) ⭐️ 9.0/10
2. [LLM 奖励深厚专业知识，成为能力放大器](#item-2) ⭐️ 8.0/10
3. [开发工具必须开源，LLM 使其可行](#item-3) ⭐️ 8.0/10
4. [MiniMax H3 发布即接入 ComfyUI：开放权重、原生音频与 2K 视频](#item-4) ⭐️ 8.0/10
5. [Andy Pavlo 加入 ClickHouse，成立 ClickHouse Labs。](#item-5) ⭐️ 8.0/10
6. [Jane Street 的 Bonsai 将 OCaml 带到 Web 前端](#item-6) ⭐️ 8.0/10
7. [Rust 项目目标：不可移动类型与保证析构](#item-7) ⭐️ 8.0/10
8. [Kimi K3：压缩记忆、跨深度注意力与潜在专家路由](#item-8) ⭐️ 8.0/10
9. [ML 审稿人呼吁：没有可复现代码的论文应直接拒稿](#item-9) ⭐️ 8.0/10
10. [美国犯罪实验室 DNA 设备存漏洞，30 年证据面临篡改风险](#item-10) ⭐️ 8.0/10
11. [《华盛顿邮报》：至少 50 名美国警员滥用车牌摄像头窥探前任](#item-11) ⭐️ 8.0/10
12. [英国政府再逼苹果为 iCloud 加密备份开后门，仅限英国公民](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 发布数学与理论计算机科学十大进展](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 9.0/10

OpenAI 发布了一篇题为《数学与理论计算机科学十大进展》的文章，总结了人工智能在数学发现和证明领域的一系列突破。这篇文章引发了关于大型语言模型在数学研究中作用的广泛讨论。 这一事件意义重大，因为它集中展示了大型语言模型正从模式匹配走向真正的数学推理，可能变革数学研究的方式。它会影响数学家、理论计算机科学家以及人工智能研究者。 据报道，这十项进展包括与高维球堆积和多色拉姆齐数相关的结果。评论指出，虽然当前模型尚不能自如地提出猜想，但它们能快速帮助证伪猜想并辅助生成证明，使数学探索更加可行。

hackernews · milkshakes · 8月3日 16:27 · [社区讨论](https://news.ycombinator.com/item?id=49157930)

**背景**: 数学推理是检验人工智能的重要基准，因为它需要精确的逻辑和强大的泛化能力。OpenAI 此前发布了专门为复杂推理任务设计的 o1 等模型。这篇文章很可能是对这些模型在数学和理论计算机科学开放问题上应用的阶段性总结。

**社区讨论**: 评论者总体上持乐观但谨慎的态度：有人认为 AI 能力正呈指数级增长，也有人强调暴力计算与人类直觉之间的区别。有评论者分享了第 1 题和第 9 题的直观可视化解释。整体情绪是 AI 对数学的影响已不可否认。

**标签**: `#AI`, `#mathematics`, `#theoretical-computer-science`, `#OpenAI`, `#LLMs`

---

<a id="item-2"></a>
## [LLM 奖励深厚专业知识，成为能力放大器](https://www.seangoedecke.com/llms-reward-expertise/) ⭐️ 8.0/10

文章认为，当用户具备并能清晰表达深厚的领域专业知识时，LLM 能产生明显更好的输出，成为知识型人才的“力量倍增器”。它强调要传递专业信号和精确上下文，而非依赖通用的提示技巧。 这一观点挑战了“LLM 能拉平能力差距”的假设，反而表明 AI 可能会拉大专家与新手之间的差距。这对提示工程、AI 工具设计以及企业如何培训员工使用 AI 都有重要影响。 作者认为，驱动 LLM 性能的是领域专业知识，而不仅仅是提示语的措辞；用户应主动表明自己的背景和约束条件。文章还指出，专家可以用更少时间完成更多工作，这可能改变对专业工作的评价方式。

hackernews · MaxMussio · 8月3日 21:13 · [社区讨论](https://news.ycombinator.com/item?id=49161518)

**背景**: 大型语言模型（LLM）是在海量文本数据上训练的人工智能系统，能够生成连贯且符合上下文的回答。提示工程（Prompt Engineering）逐渐成为一门通过精心设计输入以获得理想输出的实践，但本文认为，真正的领域专业知识比任何提示公式更有价值。“力量倍增器”这个比喻指 LLM 能够放大那些已经知道该问什么、知道哪些细节重要的人的生产力和洞察力。

**社区讨论**: 评论者参与度高，但观点存在分歧。一些人赞同“传递专业信号能显著改善结果”，并分享个人案例，例如告诉模型自己有多年经验。另一些人则反驳，举出 Anthropic 数学家的例子——一个非常简单的提示（“解决这个猜想，认真思考”）也效果很好。还有人公开呼吁开展正式研究，避免仅凭轶事下结论。

**标签**: `#LLM`, `#Prompt Engineering`, `#AI`, `#Expertise`, `#Human Knowledge`

---

<a id="item-3"></a>
## [开发工具必须开源，LLM 使其可行](https://blog.exe.dev/devtools-must-be-open-source) ⭐️ 8.0/10

这篇博文主张开发工具必须开源，并声称大型语言模型可以让代码级修改变得切实可行。这挑战了开发工具中传统上依赖配置文件、选项和插件系统的做法。 这一观点可能会重塑开发者定制工具的方式，从配置驱动的调整转向由 LLM 辅助的直接源码修改。它会影响维护者、用户以及开源开发工具的可持续性。 博文提议通过夜间定时任务自动获取上游变更并重基本地修改，由 LLM 处理所需的代码编辑。评论者指出了潜在的效率低下、可靠性风险以及维护分支所涉及的实际劳动。

hackernews · bryanmikaelian · 8月3日 14:15 · [社区讨论](https://news.ycombinator.com/item?id=49156111)

**背景**: 开源软件一直承诺用户可以自由查看和修改代码，但实践中大多数人都是依靠他人来完成修改。LLM 可能降低直接修改代码的门槛，使开源初衷对普通用户更加可行。许多开发工具目前通过配置文件和插件来实现定制，而不是要求直接编辑源代码。

**社区讨论**: 评论者意见不一：simonw 认为 LLM 让旧日的开源梦想变得可行，而 kelnos 称每次修改都从源码重建工具既低效又浪费。theamk 警告夜间 AI 重基可能会破坏工作流程，维护者 lalitmaganti 则认为这种做法过于理想化，忽视了维护分支的实际工作。

**标签**: `#open-source`, `#devtools`, `#LLM`, `#software-engineering`, `#opinion`

---

<a id="item-4"></a>
## [MiniMax H3 发布即接入 ComfyUI：开放权重、原生音频与 2K 视频](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 8.0/10

MiniMax H3 作为通用全模态生成模型，在发布当天即获得 ComfyUI 的 Day-0 支持，并开放权重。该集成支持原生音频与 2K 视频生成，其最小模型变体据称可在 RTX 3060 等消费级 GPU 上本地运行。 这是开放权重生成式媒体领域一个重要的实践里程碑，让社区能够通过 ComfyUI 的节点式工作流立即使用前沿的视频/音频模型。这降低了艺术家和开发者在自有硬件上尝试带同步音频的高质量 2K 视频的门槛，有望加速 AI 视频制作的创新。 该模型的调制权重（约占参数总量的 40%）可以被裁剪并替换为功能等效的查找表，使总内存占用减少 66%——从全精度的 123.6 GB 降至最小变体的 42.5 GB。结合动态 VRAM 卸载，这一技术让下一代 2K 视频模型能够在 RTX 3060 等 GPU 上本地运行。

hackernews · vblanco · 8月3日 13:34 · [社区讨论](https://news.ycombinator.com/item?id=49155629)

**背景**: MiniMax H3 是一个全模态生成模型，能够联合理解并生成文本、图像、视频和音频。ComfyUI 是一款开源的节点式界面，用于构建和运行扩散模型工作流，被 AI 创作者广泛使用。开放权重允许用户下载并在本地运行模型，而不是依赖付费 API，从而在大量使用时显著降低成本。社区已开始分享早期使用体验，包括消费级 GPU 上的生成时间和输出质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://huggingface.co/MiniMaxAI/MiniMax-H3">MiniMaxAI/MiniMax-H3 · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/ComfyUI">ComfyUI</a></li>

</ul>
</details>

**社区讨论**: 早期社区反应热烈，用户称输出“非常惊艳”，并认为部分片段比当前最先进模型有大幅提升，不过其中一条饮料广告片段仍带有“AI 平滑”效果。多位评论者对该调制权重裁剪技术表示好奇，询问它能否应用于大语言模型，以及在 16 GB RTX 3060 上生成速度如何；一位用户分享称，在 4070 Ti Super 上生成一段 10 秒的 480p 视频约需 10 分钟。

**标签**: `#AI video`, `#ComfyUI`, `#MiniMax`, `#open weights`, `#generative media`

---

<a id="item-5"></a>
## [Andy Pavlo 加入 ClickHouse，成立 ClickHouse Labs。](https://clickhouse.com/blog/andy-pavlo-joins-clickhouse) ⭐️ 8.0/10

知名数据库研究者 Andy Pavlo 加入 ClickHouse，成立名为 ClickHouse Labs 的新研究团队，该消息在 ClickHouse 官方博客上公布。 这一举措表明 ClickHouse 正在加大对数据库研究的投入，并可能影响 OLAP 系统的未来方向，尤其是在存算分离和列式架构方面。这也凸显了数据库领域学术界与产业界合作日益紧密的趋势。 社区讨论中，用户提出了关于 ClickHouse 和 StarRocks 等快速 OLAP 产品如何与 Trino 等引擎融合的开放问题，尤其是在数据摄入、索引以及 Iceberg 等存储格式方面。评论者还指出 ClickHouse 是列式 OLAP 数据库，也有人希望 ClickHouse 能够资助学术数据库研究。

hackernews · nikolay_sivko · 8月3日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49156011)

**背景**: 在线分析处理（OLAP）是一种用于从多个角度分析业务数据的软件技术，通常与在线事务处理（OLTP）相对。ClickHouse 是一款快速的开源列式 OLAP 数据库，使用 SQL 并支持连接操作，但按列存储数据。现代数据平台的一大趋势是存算分离，例如将数据集中存放在 S3 等对象存储中，让多个计算集群可以共享相同的数据集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Online_analytical_processing">Online analytical processing - Wikipedia</a></li>
<li><a href="https://clickhouse.com/docs/en/faq/general/columnar-database">What is a columnar database ? | ClickHouse Docs</a></li>
<li><a href="https://www.linkedin.com/pulse/decoupled-storage-compute-paradigm-shift-building-modern-kamdar">Decoupled Storage and Compute – A paradigm shift to building Modern Data Platforms</a></li>

</ul>
</details>

**社区讨论**: 评论者总体上非常热情，有人说自己大学时看过 Pavlo 在 CMU 的讲座，并对这两个世界如今走到一起感到惊讶。也有人提出了实质性问题，包括 ClickHouse 是否会资助学术数据库研究、ClickHouse 和 StarRocks 等 OLAP 引擎如何与 Trino 融合，以及 Pavlo 的讲座系列能否以赞助形式继续。评论中还有一些轻松的玩笑，比如调侃 Pavlo 被巴尔的摩附近的邮局禁入。

**标签**: `#databases`, `#ClickHouse`, `#OLAP`, `#research`, `#Andy Pavlo`

---

<a id="item-6"></a>
## [Jane Street 的 Bonsai 将 OCaml 带到 Web 前端](https://github.com/janestreet/bonsai) ⭐️ 8.0/10

Jane Street 已将其内部 OCaml UI 库 Bonsai 公开发布在 GitHub 上。Bonsai 是一个基于 Js_of_ocaml 构建的高性能、反应式 Web 应用库，使全栈 OCaml 开发成为可能。 Bonsai 的重要性在于它允许开发者在后端和前端使用相同的语言和类型，减少上下文切换并实现代码复用。作为一个在 Jane Street 内部广泛使用的生产级库，它标志着 OCaml 是现实世界前端开发的可行选择。 Bonsai 部分借鉴了 Elm 架构，并被用于构建 Jane Street 内部几乎所有 Web 应用，从公司目录到监控工具。它通过 Js_of_ocaml 将 OCaml 编译为 JavaScript，不过当前仓库中缺少 docs 目录，导致部分链接无法访问。

hackernews · KolmogorovComp · 8月3日 08:29 · [社区讨论](https://news.ycombinator.com/item?id=49152842)

**背景**: OCaml 是一种通用、多范式的编程语言，以其强大的静态类型系统和编译期安全性而闻名。Js_of_ocaml 是一个将 OCaml 字节码编译为 JavaScript 的工具链，使 OCaml 代码能够在浏览器中运行。Bonsai 正是基于这一思路构建的 UI 库，借鉴 Elm 的反应式模型来构建动态 Web 应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/janestreet/bonsai">GitHub - janestreet/bonsai: A library for building dynamic webapps, using Js_of_ocaml · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/OCaml">OCaml</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者对于终于能在 OCaml 中共享后端和前端类型表示兴奋。然而，一些人提出了文档链接缺失和 DOM 更新机制的问题，还有人将 Bonsai 与 Melange 库进行比较，质疑它是否意味着要放弃 JavaScript 生态系统。也有评论者认为默认 UI 样式不够精致，尽管承认其性能优秀。

**标签**: `#OCaml`, `#UI`, `#Jane Street`, `#web development`, `#functional programming`

---

<a id="item-7"></a>
## [Rust 项目目标：不可移动类型与保证析构](https://github.com/rust-lang/rust-project-goals/blob/main/src/2026/move-trait.md) ⭐️ 8.0/10

Rust 项目目标（rust-project-goals）中新增了一项 2026 年目标，提出引入 `!Move` 不可移动类型和保证析构（guaranteed destructors），长期目标是用它取代现有的 `Pin` 机制。该提案还讨论了一种“必须移动”的线性类型，要求值必须被显式消费而不能直接丢弃。 这将填补 Rust 类型系统中长期存在的缺口，让自引用类型无需借助 `Pin` 这个“补丁”即可安全、符合人体工程学地使用。同时它还能支持线性类型，为必须恰好使用一次的资源（如文件描述符或句柄）提供更安全的 API。 该提案的关键细节包括：不可移动性将成为类型本身的属性（`!Move`），而不是位置或引用的属性（`Pin`）；同时 `!Forge` 保证可以防止 `mem::forget` 之类的漏洞绕过析构，从而支持安全的 scoped spawn。提案还概述了必须移动的（`!Destruct`）线性类型，这类值必须由某个函数消费，而不能被隐式丢弃。

hackernews · paavohtl · 8月3日 06:42 · [社区讨论](https://news.ycombinator.com/item?id=49152023)

**背景**: Rust 通常允许值在内存中被移动，这使得自引用类型难以安全编写，因为移动会使内部指针失效。当前的变通方案 `Pin<T>` 可以在值被固定后阻止移动，但被广泛认为是一个“补丁”，而且无法保证析构函数一定会运行。新提案希望让不可移动性成为类型系统的一等概念，并同时处理线性类型——即值必须被恰好消费一次的类型。它建立在关于 must-move 类型的既有讨论之上，也回应了 Rust 参考文档中关于 `mem::forget` 可以绕过析构保证的说明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rust-lang.github.io/rust-project-goals/2026/move-trait.html">Immobile types and guaranteed destructors - Rust Project Goals</a></li>
<li><a href="https://doc.rust-lang.org/reference/destructors.html">Destructors - The Rust Reference</a></li>
<li><a href="https://lobste.rs/s/sp2wji/rust_project_goals_immobile_types">Rust Project Goals: Immobile types and guaranteed destructors | Lobsters</a></li>

</ul>
</details>

**社区讨论**: 整体反响积极，用户认为这填补了 Rust 的一个明显缺陷。也有评论提醒，这只是一个项目目标而非已通过的语言变更，设计仍可能大幅调整。讨论中还出现了关于该方案是否会取代 Without Boats 提出的 “pinned places” 替代设计的分歧，以及 `!Destruct` 线性类型意义的热烈探讨。

**标签**: `#rust`, `#language-design`, `#type-system`, `#memory-safety`, `#linear-types`

---

<a id="item-8"></a>
## [Kimi K3：压缩记忆、跨深度注意力与潜在专家路由](https://newsletter.semianalysis.com/p/kimi-k3-the-manos-the-mythos-the) ⭐️ 8.0/10

SemiAnalysis 发表了一篇关于 Kimi K3 新架构的深度技术分析，重点介绍了四项创新：压缩记忆、跨模型深度注意力、潜在专家路由，以及优化的推理性能。 这项分析对 AI/ML 从业者意义重大，因为它罕见地深入剖析了 Moonshot AI 的 Kimi K3 如何在效率和推理能力上突破边界，并可能为模型架构和推理优化开辟新方向。 该架构据说结合了用于高效长上下文处理的压缩记忆、用于更好特征聚合的跨深度注意力，以及用于降低推理成本的潜在专家路由，从而在吞吐量和延迟方面带来了显著改进。

rss · Semianalysis · 8月3日 19:42

**背景**: 压缩记忆（compressed memory）指将历史上下文进行摘要或蒸馏，使其能放入有限的上下文窗口内。跨深度注意力（attention across depth）是一种让某一层关注前面层表征的机制，而非只关注 token 位置。潜在专家路由（latent expert routing）是一种在低维潜在空间中完成路由的专家混合（MoE）变体，可提升参数效率与可扩展性。这些都是一些新兴技术，旨在提升 LLM 的推理效率与长上下文处理能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sebastianraschka.com/llm-architecture-gallery/attention-residuals/">Attention Residuals (AttnRes) | Sebastian Raschka, PhD</a></li>
<li><a href="https://aman.ai/primers/ai/mixture-of-experts/">Aman's AI Journal • Primers • Mixture of Experts</a></li>
<li><a href="https://www.datacamp.com/blog/how-does-llm-memory-work">How Does LLM Memory Work? Building Context-Aware AI... | DataCamp</a></li>

</ul>
</details>

**标签**: `#AI/ML`, `#LLM`, `#architecture`, `#inference`, `#model design`

---

<a id="item-9"></a>
## [ML 审稿人呼吁：没有可复现代码的论文应直接拒稿](https://www.reddit.com/r/MachineLearning/comments/1vei12v/its_time_to_desk_reject_papers_that_dont_include/) ⭐️ 8.0/10

一位机器学习审稿人报告称，随着 NeurIPS 审稿季结束，他们在 2025 年为三大顶会审阅的 12 篇论文中，只有 1 篇提供了可完整运行训练流程的代码；在提供了部分代码的 5 篇论文中，有 3 篇含有足以颠覆结论的 bug。他们主张对未包含可复现代码的论文直接拒稿（desk reject）。 这凸显了机器学习研究中系统性的可复现性危机：作者可以通过隐藏代码来规避审查。如果该政策被采纳，将促使研究者公开完整的训练流程，从而提高各大 AI 顶会的论文质量门槛。 在 12 篇论文中，4 篇只提供无法端到端运行的片段代码，7 篇完全没有代码。审稿人认为，当前激励机制让公开代码反而更容易因被审稿人发现 bug 而受罚，因此只有对隐藏代码施加真正的惩罚才能解决问题。

reddit · r/MachineLearning · /u/Flaky-Ambition5900 · 8月3日 16:17

**背景**: Desk reject（直接拒稿）指编辑或程序委员会在送外部同行评审之前就拒绝稿件，通常是因为稿件明显不符合主题范围或质量要求。AUROC（ROC 曲线下面积）是评估二分类模型性能的常用指标，它概括了不同阈值下真阳性率与假阳性率之间的权衡，常被用作机器学习论文的最终报告结果。当前顶级机器学习会议通常不强制要求作者公开代码，这种机制助长了不可复现投稿的泛滥。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AUROC">AUROC</a></li>
<li><a href="https://en.wikipedia.org/wiki/Desk_reject">Desk reject</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#reproducibility`, `#peer review`, `#academic publishing`, `#code sharing`

---

<a id="item-10"></a>
## [美国犯罪实验室 DNA 设备存漏洞，30 年证据面临篡改风险](https://www.wsj.com/tech/cybersecurity/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking-1932775a) ⭐️ 8.0/10

研究人员在 Thermo Fisher Scientific DNA 分析设备中发现一个安全漏洞，这些设备被美国大多数犯罪实验室使用，可能导致 DNA 证据文件被无法察觉地篡改。借助 Anthropic 的 Claude 生成的 AI 代码，他们在大约 45 分钟内修改了一个 DNA 扫描文件，且未触发常用分析软件的警报。 该漏洞威胁到刑事案中多达 30 年的法医 DNA 证据的完整性，可能动摇已定罪案件和正在审理的案件。全美 200 多家犯罪实验室缺乏统一监管，难以评估或控制风险，凸显了 AI、网络安全与关键基础设施之间日益交叉的问题。 Thermo Fisher 于 7 月承认该漏洞，并在报道发布前的那个周五发布高风险安全公告，推出加入数字签名的软件更新以保护文件。目前尚无该漏洞被实际利用的案例，在审或已结案件中的证据是否受影响尚不明确。

telegram · zaihuapd · 8月3日 05:15

**背景**: 犯罪实验室的法医 DNA 分析依赖专用仪器（如 Thermo Fisher 的测序仪），这些仪器生成法院用作证据的电泳图谱文件。研究人员证明，这些专有文件格式缺乏数字签名等完整性保护，使具有服务器访问权限的攻击者能够悄无声息地修改扫描结果。Claude 等 AI 助手使攻击变得更容易，因为 AI 可以生成代码来解析和修改这些格式，所需工作量极小。这建立在早前研究的基础上，该研究已表明 DNA 测序软件常常缺乏健全的安全保护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.remio.ai/post/ai-assisted-code-exposed-a-hidden-weakness-in-forensic-dna-evidence">AI-Assisted Code Exposed a Hidden Weakness in Forensic DNA ...</a></li>
<li><a href="https://dissenter.com/tech/thermo-fisher-dna-software-flaw-allowed-undetectable-evidence-tamperin">Thermo Fisher DNA Software Flaw Allowed Undetectable Evidence ...</a></li>
<li><a href="https://www.techtimes.com/articles/322771/20260803/ai-assisted-code-can-alter-forensic-dna-scan-files-without-any-detectable-trace.htm">AI-Assisted Code Can Alter Forensic DNA Scan Files Without Any...</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#forensics`, `#AI`, `#vulnerability`, `#DNA analysis`

---

<a id="item-11"></a>
## [《华盛顿邮报》：至少 50 名美国警员滥用车牌摄像头窥探前任](https://www.washingtonpost.com/technology/2026/08/02/how-police-officers-used-vast-network-cameras-spy-their-exes/) ⭐️ 8.0/10

《华盛顿邮报》8 月 2 日发布的调查发现，至少 50 名美国执法人员被指控或起诉滥用 Flock 等自动车牌识别系统，其中 26 起案件涉及窥探现任或前任伴侣。报道揭示了系统性的隐私滥用和监管缺失。 这项调查暴露了监控技术治理的现实失败，表明强大的车牌识别网络可能被用于个人跟踪，且基本处于监管空白。这凸显了加强审计要求和刑事处罚以保护公民隐私的紧迫性。 目前只有 13 个州要求对 ALPR 使用进行审计，至少 8 个州将滥用行为定为犯罪。Flock 在 6000 多个社区运营超过 12 万台摄像头，每月记录 200 亿次车牌扫描，虽然推出了可选的“审计辅助”功能，但 CEO 承认滥用“难以完全避免”。

telegram · zaihuapd · 8月3日 09:03

**背景**: 自动车牌识别系统（ALPR）是用于采集车牌和车辆细节的摄像头，常安装在警车或固定杆上，执法部门用它来定位涉案车辆。Flock Safety 是此类摄像头网络的主要私营供应商，将社区、企业和警方连接成一个共享监控网络。然而，这类系统积累了大量位置数据，为警员出于个人目的滥用提供了机会。佐治亚州警察局长 Michael Steffman 案就是典型例证，他约 600 次搜索前女友的车牌，后在开庭前自杀身亡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://sls.eff.org/technologies/automated-license-plate-readers-alprs">Automated License Plate Readers</a></li>
<li><a href="https://ij.org/police-have-reportedly-used-license-plate-readers-to-stalk-romantic-interests-at-least-14-times-in-recent-years/">Police Have Reportedly Used License Plate Readers to Stalk...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#surveillance`, `#law enforcement`, `#ethics`, `#regulation`

---

<a id="item-12"></a>
## [英国政府再逼苹果为 iCloud 加密备份开后门，仅限英国公民](https://t.me/zaihuapd/42953) ⭐️ 8.0/10

9 月初，英国内政部再次向苹果发出技术能力通知，要求为其加密云备份开后门，这次仅针对英国公民数据。此前 1 月份的通知曾要求全球访问权限，引发英美外交冲突。 如果成功，这将迫使苹果削弱端到端加密，开创威胁全球用户隐私的先例，并可能使所有用户的数据更不安全。此事也考验英国《调查权力法》如何应对国际科技公司和外交压力。 在 1 月份的通知后，苹果已于 2 月份从英国撤回了其最安全的云存储服务 iCloud 高级数据保护功能。新通知据称仅适用于英国公民，不同于此前要求全球数据访问的指令，但隐私活动人士警告，任何被迫削弱安全架构的行为都会影响到所有人。

telegram · zaihuapd · 8月3日 15:40

**背景**: 英国的技术能力通知是 2016 年《调查权力法》下的一项法律工具，要求企业协助执法部门访问加密内容。iCloud 高级数据保护是苹果提供的可选端到端加密功能，用于云备份，只有用户持有解密密钥。英国要求苹果为此功能创建解锁机制，但苹果一直抵制；1 月份的全球数据访问要求曾促使特朗普政府施压英国撤回。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/zh-cn/guide/security/sec973254c5f/web">iCloud 高 级 数 据 保 护 - 官方 Apple 支持 (中国)</a></li>
<li><a href="https://14th.day/posts/浅谈icloud-高级数据保护/">浅谈 iCloud 高 级 数 据 保 护 - Fourteenth-Day Adventist</a></li>
<li><a href="https://www.v2ex.com/t/948629">云上贵州 iCloud 高 级 数 据 保 护 靠谱吗？ - V2EX</a></li>

</ul>
</details>

**标签**: `#privacy`, `#security`, `#Apple`, `#encryption`, `#government`

---