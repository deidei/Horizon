---
layout: default
title: "Horizon Summary: 2026-07-09 (ZH)"
date: 2026-07-09
lang: zh
---

> 从 40 条内容中筛选出 15 条重要资讯。

---

1. [OpenAI 发布 GPT-5.6 三个版本，Sol 在 ARC-AGI-3 上达到 SOTA](#item-1) ⭐️ 10.0/10
2. [使用 AI 将 Bun 从 Zig 重写为 Rust](#item-2) ⭐️ 9.0/10
3. [TypeScript 7.0 发布：Go 重写带来高达 12 倍速度提升](#item-3) ⭐️ 9.0/10
4. [蚂蚁开源 LingBot-Video，全球首个 MoE 具身视频基模](#item-4) ⭐️ 9.0/10
5. [欧盟议会通过 Chat Control 1.0，程序性操作引发争议](#item-5) ⭐️ 8.0/10
6. [用 Rust 重写的 PostgreSQL 通过全部回归测试](#item-6) ⭐️ 8.0/10
7. [美国陆军后勤脆弱性分析](#item-7) ⭐️ 8.0/10
8. [Meta 推出 Muse Spark 1.1 及商业 API](#item-8) ⭐️ 8.0/10
9. [AI 内容充斥社交媒体，尤其是 LinkedIn](#item-9) ⭐️ 8.0/10
10. [OpenAI 推出 GPT‑Live 语音模式，可委托 GPT‑5.5 处理复杂任务](#item-10) ⭐️ 8.0/10
11. [Meta 超级智能更新：RL 初创公司及算力扩展](#item-11) ⭐️ 8.0/10
12. [IMGNet：用符号模式替代余弦相似度的人脸验证模型](#item-12) ⭐️ 8.0/10
13. [大疆 EV50 无人机飞越珠峰 8861 米](#item-13) ⭐️ 8.0/10
14. [国家超算互联网核心节点在郑州上线](#item-14) ⭐️ 8.0/10
15. [OpenAI 与美国战争部拟禁 AI 监控公民](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-5.6 三个版本，Sol 在 ARC-AGI-3 上达到 SOTA](https://openai.com/index/gpt-5-6/) ⭐️ 10.0/10

OpenAI 宣布 GPT-5.6 系列全面可用，包括 Luna、Terra 和 Sol 三个模型。其中最大的 Sol 版本在 ARC-AGI-3 基准测试中以 7.8%的得分创下新纪录，成为首个通过验证的、成功解决 ARC-AGI-3 游戏的前沿模型。 此次发布标志着 AI 推理能力的重大飞跃，尤其是 Sol 在 ARC-AGI-3 上的突破——该基准专为衡量类人交互智能而设计。分层定价模式（Luna、Terra、Sol）让高级 AI 更易获取，同时为高要求任务提供高端选择，其强劲表现很可能提高竞争对手的门槛。 三个版本的定价为每百万输入/输出 token：Luna $1/$6，Terra $2.50/$15，Sol $5/$30。Sol 消耗大量计算资源——在 Plus 计划中，一次复杂查询可能用掉 5 小时配额的 95%。该模型系列还改进了意图理解，并保留原始图像尺寸。

hackernews · logickkk1 · 7月9日 17:04 · [社区讨论](https://news.ycombinator.com/item?id=48849066)

**背景**: GPT-5.6 是 OpenAI 最新的旗舰模型系列，接替 GPT-5。它分为三个版本：Luna（最快/最便宜）、Terra（中端）和 Sol（最强）。ARC-AGI-3 是一个交互式推理基准，挑战 AI 代理探索新环境、推断目标并有效规划。分层定价模式也沿用了 Anthropic 和 Google 的类似策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT‑5.6 Sol: a next-generation model - OpenAI</a></li>
<li><a href="https://andrew.ooo/answers/gpt-5-6-sol-vs-terra-vs-luna-tiered-model-explained-july-2026/">GPT-5.6 Sol vs Terra vs Luna: OpenAI's New Tier Explained</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极但意见不一。用户注意到 Sol 的高配额消耗（ekzy 报告一次查询消耗 95%），并分享了开发者指南中的实用技巧。一些人讨论与其他模型（如 Claude Code）的比较，一位评论者指出 OpenAI 在某些基准中省略了与 Fable 5 的比较，因其拒绝回答问题。总体而言，此次发布引发了大量讨论（939 分，703 条评论），证实了其重要性。

**标签**: `#GPT-5.6`, `#OpenAI`, `#AI`, `#large language models`, `#ARC-AGI`

---

<a id="item-2"></a>
## [使用 AI 将 Bun 从 Zig 重写为 Rust](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Jarred Sumner 宣布，JavaScript 运行时 Bun 已借助 AI 编程智能体从 Zig 重写为 Rust。基于 Rust 的新版本自 2026 年 6 月 17 日起已在 Claude Code v2.1.181 中投入使用，Linux 上启动速度提升了 10%。 此次重写挑战了长久以来“大型软件不应重写”的观念，证明了 AI 智能体可以使此类项目变得可行且经济高效。它还提升了 Bun 的可靠性，解决了大量与内存相关的错误，惠及其庞大的用户群体。 重写耗时 11 天，花费约 16.5 万美元的 AI API 令牌，使用了 59 亿未缓存输入令牌和 6.9 亿输出令牌。Bun 的 TypeScript 测试套件作为一致性测试套件来验证移植，此次移植新增了超过 100 万行代码。

rss · Simon Willison · 7月8日 23:57

**背景**: Bun 是一个一体化 JavaScript 运行时和工具集，旨在作为 Node.js 的快速替代品。它最初用 Zig 编写，Zig 是一种专注于健壮性和性能的低级系统编程语言。Rust 是另一种系统语言，通过其所有权模型提供内存安全保证，有助于防止困扰 Zig 版本的使用后释放和双重释放错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language) - Wikipedia</a></li>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/bun: Incredibly fast JavaScript runtime, bundler, test runner, and package manager – all in one</a></li>

</ul>
</details>

**标签**: `#Bun`, `#Rust`, `#Zig`, `#JavaScript runtime`, `#programming languages`

---

<a id="item-3"></a>
## [TypeScript 7.0 发布：Go 重写带来高达 12 倍速度提升](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

微软正式发布了 TypeScript 7.0，用 Go 语言完全重写了原来的 JavaScript 编译器，支持真正的多线程编译，构建速度提升 8 到 12 倍。开发者可通过 npm 安装，主流编辑器通过 LSP 支持新的语言服务器。 这一性能突破大幅减少了大型 TypeScript 代码库的编译时间，提升了开发者的生产力和 CI/CD 管道的效率。同时，它为用底层语言重写核心开发者工具以提高性能树立了先例。 新版本引入了 --checkers 和 --builders 参数以自定义并行度，并提供了兼容包以便与 TypeScript 6 共存。但由于 API 尚未就绪，Vue、Svelte 等嵌入式语言工具链目前仍需要使用旧版本。

telegram · zaihuapd · 7月9日 04:01

**背景**: TypeScript 是 JavaScript 的超集，增加了静态类型，其编译器原本用 JavaScript 编写。用 Go 重写编译器可以利用原生多线程和更好的内存管理，从而大幅提升速度。语言服务器协议（LSP）标准化了编辑器与语言服务器之间的通信，使主流 IDE 都能获得一致的支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol - Wikipedia</a></li>
<li><a href="https://visualstudiomagazine.com/articles/2026/06/22/typescript-7-0-rc-moves-microsofts-go-rewrite-into-the-mainline-compiler.aspx">TypeScript 7.0 RC Moves Microsoft's Go Rewrite Into the Mainline Compiler -- Visual Studio Magazine</a></li>

</ul>
</details>

**标签**: `#TypeScript`, `#compiler`, `#performance`, `#Microsoft`, `#Go`

---

<a id="item-4"></a>
## [蚂蚁开源 LingBot-Video，全球首个 MoE 具身视频基模](https://www.qbitai.com/2026/07/446458.html) ⭐️ 9.0/10

蚂蚁集团旗下灵波（LingBot）开源了 LingBot-Video，这是全球首个基于混合专家架构的具身视频基础模型，总参数量 300 亿，推理时仅激活 30 亿参数。 这是具身 AI 和机器人领域的重要里程碑，该开源模型能生成面向机器人操作的视频，加速仿真、世界模型和策略学习等方向的研究。 LingBot-Video 采用 DiT+MoE 架构，构建了包含 7 万小时具身数据的画像引擎，并引入多维强化学习奖励系统，重点关注物理合理性和任务完成度。

telegram · zaihuapd · 7月9日 04:30

**背景**: 混合专家（MoE）是一种神经网络设计，每个输入只激活部分参数，使大模型能够高效推理。扩散 Transformer（DiT）将 Transformer 架构应用于扩散生成模型。具身 AI 旨在创建能理解并与物理世界交互的模型，常用于机器人领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://openaccess.thecvf.com/content/ICCV2023/papers/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.pdf">Scalable Diffusion Models with Transformers William Peebles* UC Berkeley</a></li>

</ul>
</details>

**标签**: `#AI`, `#Embodied AI`, `#MoE`, `#Video Generation`, `#Open Source`

---

<a id="item-5"></a>
## [欧盟议会通过 Chat Control 1.0，程序性操作引发争议](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

欧洲议会未获明确多数支持便通过了 Chat Control 1.0，允许对 Gmail、Snapchat 等服务的私密消息进行大规模扫描，有效期至 2028 年。 这为欧盟数字权利开创了危险先例，立法可通过程序性操作强行通过，削弱了民主制衡。同时威胁到主要平台的用户隐私。 该法律仅适用于非端到端加密服务，并利用'紧急程序'通过，需要全体议员的绝对多数（361 票）才能否决，尽管有 314 票反对、276 票赞成。

hackernews · rapnie · 7月9日 11:03 · [社区讨论](https://news.ycombinator.com/item?id=48843923)

**背景**: Chat Control 指欧盟扫描私密消息以查找儿童性虐待材料的提案。批评者认为该技术不可靠且侵犯隐私。该法律 3 月两次被否决，但通过理事会支持的程序重新复活。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/">EU Parliament greenlights Chat Control 1.0 – Breyer: "Our children lose out"</a></li>
<li><a href="https://www.techtimes.com/articles/320010/20260709/eu-parliament-passes-chat-control-default-314-meps-couldnt-block-scanning-law.htm">EU Parliament Passes Chat Control by Default: 314 MEPs Couldn't Block Scanning Law</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对程序性操作表示愤慨，称其不民主，是迈向极权主义的一步。有用户指出，投票安排在暑假前夕，许多议员缺席，导致否决失败。

**标签**: `#privacy`, `#surveillance`, `#EU`, `#legislation`, `#digital rights`

---

<a id="item-6"></a>
## [用 Rust 重写的 PostgreSQL 通过全部回归测试](https://github.com/malisper/pgrust) ⭐️ 8.0/10

一个名为 pgrust 的项目使用大型语言模型（LLM）将 PostgreSQL 用 Rust 重写，目前已通过 100%的 PostgreSQL 回归测试。 这展示了 LLM 在大规模代码翻译方面的潜力，但也引发了关于代码质量、架构变更（如线程模型）以及原始 PostgreSQL 许可证与新 AGPL 许可证兼容性的关键问题。 该项目在不到一个月内生成了超过 7100 次提交，使得通过提交历史进行传统代码审查变得不切实际。许可证从宽松的 PostgreSQL 许可证改为 AGPL，这可能引发与原始代码库的兼容性问题。

hackernews · SweetSoftPillow · 7月9日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=48841676)

**背景**: PostgreSQL 是一款广泛使用的开源关系型数据库，已有 30 年历史。Rust 是一种以内存安全和性能著称的系统编程语言。回归测试是一组确保新变更不会破坏现有功能的测试套件。该项目利用 LLM 自动将 C 代码翻译为 Rust，这是一种新颖但有争议的方法。

**社区讨论**: 作者解释他们正在尝试用 LLM 构建更好的 Postgres。评论者指出，100%的回归测试并未涵盖线程架构变更，因此该成就并不全面。还有人担心，一个月内超过 7100 次提交的 LLM 生成代码难以审查，并且许可证从 PostgreSQL 改为 AGPL，质疑其与原始源代码的兼容性。

**标签**: `#database`, `#rust`, `#postgres`, `#llm`, `#open-source`

---

<a id="item-7"></a>
## [美国陆军后勤脆弱性分析](https://mwi.westpoint.edu/the-glass-backbone-why-the-armys-logistics-will-break-in-the-next-war/) ⭐️ 8.0/10

现代战争研究所最近的一项分析指出，由于对齿尾比的误解，美国陆军后勤体系极其脆弱，可能会在未来的冲突中崩溃。 这很重要，因为后勤对军事成功至关重要，如果陆军不改革其后勤体系，尽管拥有技术优势，仍可能在未来的战争中失败。 文章指出，齿尾比（作战人员与后勤人员的比例）被误解，导致对后勤投入不足。并警告现代战争的速度和复杂性将压垮当前的后勤支柱。

hackernews · baud147258 · 7月9日 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48845442)

**背景**: 齿尾比是衡量作战部队与支援部队比例的一项军事指标。历史上，后勤在预算优先级中一直被低估。该分析借鉴了历史案例以及乌克兰等当前冲突，指出了系统性风险。

**社区讨论**: 评论普遍赞同该分析，用户引用了历史类比（例如费边对抗汉尼拔的战术），并以乌克兰战争为例证。有评论指出 SpaceX 的 StarFall 等技术可能改变后勤，但其他人仍持怀疑态度。

**标签**: `#logistics`, `#military`, `#systems analysis`, `#strategic studies`, `#resilience`

---

<a id="item-8"></a>
## [Meta 推出 Muse Spark 1.1 及商业 API](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta 发布了其专有 AI 模型的新版本 Muse Spark 1.1，并推出了商业 API，开发者可通过付费订阅进行访问。 此举标志着 Meta 进军商业 AI 模型市场，可能以激进的价格和开放权重策略颠覆 OpenAI 和 Anthropic 等竞争对手，使编码模型商品化。 该模型在 Terminal-Bench-2.1 上进行了评估，但社区成员指出资源限制（6 个 CPU 核心、8GB RAM）被覆盖，质疑结果的可靠性。定价为每百万输入 token 1.25 美元、每百万输出 token 4.5 美元，缓存输入则为 0.15 美元。

hackernews · ot · 7月9日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48846184)

**背景**: Muse Spark 是 Meta Superintelligence Labs (MSL) 开发的专有大型语言模型，于 2026 年 4 月 8 日首次发布。商业 API 允许开发者付费将模型集成到其应用中。Meta 的开放权重策略公开模型权重，促进社区采用，但可能减少竞争对手的收入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Muse_Spark_AI_model">Muse Spark (AI model)</a></li>

</ul>
</details>

**社区讨论**: 社区反馈不一：一些用户称赞其定价和性能具有竞争力，而另一些则批评评估方法因资源限制被覆盖而存在缺陷。关于 Meta 作为‘搅局者’将 AI 模型商品化，还是与前沿实验室正面竞争的战略角色，存在争论。

**标签**: `#Meta AI`, `#Muse Spark`, `#open-source AI`, `#AI model evaluation`, `#commercial AI`

---

<a id="item-9"></a>
## [AI 内容充斥社交媒体，尤其是 LinkedIn](https://www.pangram.com/blog/ai-in-your-feed) ⭐️ 8.0/10

Pangram 上的一篇博文指出，AI 生成的内容在社交媒体（尤其是 LinkedIn）上越来越普遍，引发了关于真实性和线上讨论本质的辩论。 这一趋势威胁到专业网络上真正的人际联系和讨论，因为 AI 撰写的帖子可能侵蚀信任并贬低真实声音，影响人们建立人脉和分享知识的方式。 该帖因社区高度参与（162 分、141 条评论）而获得 8.0/10 评分，评论反映了从对 AI 写作的怀疑到对机器人和模仿 AI 语言模式的观察等多样观点。

hackernews · mukmuk · 7月9日 15:50 · [社区讨论](https://news.ycombinator.com/item?id=48847940)

**背景**: 像 GPT-4 这样的 AI 工具可以生成类似人类的文本，从而轻松大规模制作社交媒体帖子。作为专业网络，LinkedIn 依赖真实的个人见解来进行有意义的互动。AI 内容的兴起引发了关于平台价值及其用户声音真实性的问题。

**社区讨论**: 社区评论显示出强烈分歧：一些人认为 AI 写作破坏了个人的声音和真实性，而另一些人则指出 LinkedIn 一直存在套路化内容，AI 只是加速了这一过程。还有用户指出，即使不直接使用 AI，人们也越来越多地模仿 AI 的语言模式。

**标签**: `#AI`, `#social media`, `#content generation`, `#LinkedIn`, `#authenticity`

---

<a id="item-10"></a>
## [OpenAI 推出 GPT‑Live 语音模式，可委托 GPT‑5.5 处理复杂任务](https://simonwillison.net/2026/Jul/8/introducing-gptlive/#atom-everything) ⭐️ 8.0/10

OpenAI 推出了 GPT‑Live，这是 ChatGPT 升级后的语音模式模型，能够将网页搜索、深度推理等复杂任务委托给 GPT‑5.5，同时保持对话流畅。 此次更新显著提升了 ChatGPT 语音模式的实用性，使其成为更强大的头脑风暴伙伴，既能进行对话又能处理复杂推理任务。 GPT‑Live 取代了之前基于 GPT‑4o 的模型，允许用户进行长达一小时的对话，同时在后台无缝将困难任务委托给 GPT‑5.5。

rss · Simon Willison · 7月8日 23:20

**背景**: GPT‑5.5 是 OpenAI 于 2026 年 4 月 23 日发布的大型语言模型，代号 'Spud'。它在 Terminal-Bench 2.0 和 FrontierMath 等基准测试中取得了显著成绩。此前，OpenAI 在语音模式中使用的是 GPT‑4o 时代的模型，知识截止于 2024 年，能力有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-Live`, `#ChatGPT`, `#Voice Mode`, `#AI`

---

<a id="item-11"></a>
## [Meta 超级智能更新：RL 初创公司及算力扩展](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

Meta 超级智能计划的进展更新揭示了一个顶级强化学习环境初创公司的出现，以及据称有史以来最激进的算力扩展，跨度超过 2000 公里。 这表明 Meta 在超级智能研发上取得了快速进展，对 AI 行业和竞争格局（尤其是 Google DeepMind）具有重要影响。 更新中提到了一家新的强化学习环境初创公司、前所未有的跨越 2000 多公里的算力扩展，以及对 Google DeepMind 的战略建议，表明重大基础设施发展。

rss · Semianalysis · 7月9日 19:16

**背景**: 超级智能指的是在几乎所有领域超越人类认知能力的人工智能。Meta 一直在大力投资 AI，特别是强化学习和大规模算力基础设施。该 RL 环境初创公司可能提供用于训练高级 AI 代理的模拟平台。

**标签**: `#Meta`, `#Superintelligence`, `#Reinforcement Learning`, `#Compute Scaling`, `#AI Progress`

---

<a id="item-12"></a>
## [IMGNet：用符号模式替代余弦相似度的人脸验证模型](https://www.reddit.com/r/MachineLearning/comments/1urxvxh/i_built_imgnet_a_face_verification_model_that/) ⭐️ 8.0/10

这项工作挑战了人脸验证中默认使用余弦相似度的做法，表明符号模式一致性可以产生有竞争力的结果，可能为基于嵌入的识别系统的度量设计开辟新方向。 该模型包含一个新颖的 SW Block 层，计算多尺度关系差异，以及一个完全基于符号模式一致性、无幅度依赖的 IMG Sign MSE Loss。当直接应用于 ArcFace 嵌入（无需重新训练）时，IMG Sign Score 在 LFW 上达到 99.58%。

reddit · r/MachineLearning · /u/img-_- · 7月9日 18:00

**背景**: 人脸验证通常使用神经网络将人脸映射为嵌入向量，然后通过余弦相似度进行比较。余弦相似度衡量向量之间的角度，对全局方向敏感但忽略局部符号模式。IMGNet 则通过滑动窗口检查符号模式，保留关系结构。

**标签**: `#face verification`, `#machine learning`, `#embeddings`, `#novel approach`

---

<a id="item-13"></a>
## [大疆 EV50 无人机飞越珠峰 8861 米](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 8.0/10

大疆尚未发布的 EV50 垂直起降运载无人机参与‘巅峰使命’珠峰科考，在北坡飞越 8861 米，创下同类公开测试中的最高飞行升限。 这一成就展示了无人机在高海拔作业和低空物流方面的能力，可能对极端环境下的无人机配送和科研产生重要影响。 EV50 是一款复合翼无人机，可原地垂直起降，起飞后切换固定翼巡航。在为期 12 天的任务中，累计完成 32 架次起降，连续爬升 3730 米，返程时仍剩 30%电量。

telegram · zaihuapd · 7月9日 06:00

**背景**: 垂直起降（VTOL）无人机结合了多旋翼和固定翼飞机的优点，能在狭小空间起降并保持高效长航时飞行。高海拔飞行面临空气稀薄、低温和强风等挑战。大疆是领先的无人机制造商，EV50 设计用于货物运输和低空物流。

**标签**: `#无人机`, `#大疆`, `#珠峰`, `#航空科技`, `#物流`

---

<a id="item-14"></a>
## [国家超算互联网核心节点在郑州上线](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

2026 年 7 月 9 日，国家超算互联网核心节点在郑州正式上线，可提供超过 10 万张国产 AI 算力卡。 这标志着中国国家计算基础设施的重大里程碑，创建了超算互联网平台下最大的国产 AI 算力资源池，将加速全国的 AI 研发。 该节点承担运营管理、资源调度等核心功能，同时整合供需对接、产业孵化等综合服务，旨在构建覆盖全国的计算资源统筹调度体系。

telegram · zaihuapd · 7月9日 07:00

**背景**: 国家超算互联网是一个将全国超算中心和 AI 计算资源连接成统一网络的项目。郑州核心节点是接入该平台的最大单体资源池，提供庞大的国产 AI 算力。

**标签**: `#supercomputing`, `#AI infrastructure`, `#domestic computing`, `#China tech`, `#national project`

---

<a id="item-15"></a>
## [OpenAI 与美国战争部拟禁 AI 监控公民](https://t.me/zaihuapd/42459) ⭐️ 8.0/10

OpenAI 与美国战争部已达成一致，拟修订双方的 AI 合作协议，明确禁止使用 AI 系统监控美国公民，此举由 OpenAI 首席执行官 Sam Altman 主动提出，以回应伦理担忧。 这为军事合同中的 AI 伦理使用树立了重要先例，可能影响其他科技公司和政府政策，以保护公民自由免受 AI 驱动的监控侵害。 修订后的条款明确禁止有意监控美国公民，并禁止利用商业获取的个人身份信息进行追踪或监测。该协议修正案尚未正式签署。

telegram · zaihuapd · 7月9日 13:22

**背景**: OpenAI 一直在扩大与美国国防机构（包括原国防部、现战争部）的合作，引发了关于 AI 用于战争的伦理担忧。另一家 AI 公司 Anthropic 此前曾因争议中止了与战争部的类似合同。

**标签**: `#AI ethics`, `#OpenAI`, `#military AI`, `#surveillance`, `#AI regulation`

---