---
layout: default
title: "Horizon Summary: 2026-08-07 (ZH)"
date: 2026-08-07
lang: zh
---

> 从 35 条内容中筛选出 11 条重要资讯。

---

1. [DeepSeek V4 Flash 0731：快速、廉价、能力更强的模型更新](#item-1) ⭐️ 8.0/10
2. [汇编耻辱堂：一个收集极慢 x86 指令的项目](#item-2) ⭐️ 8.0/10
3. [为什么科技从业者如此悲伤：对行业失去信心](#item-3) ⭐️ 8.0/10
4. [Oracle 的 OpenJDK 禁止 AI 生成的代码贡献](#item-4) ⭐️ 8.0/10
5. [pgrust 用 Rust 重写 Postgres，宣称分析查询快 300 倍](#item-5) ⭐️ 8.0/10
6. [2027 年 HBM 产能售罄，DRAM 供应承压](#item-6) ⭐️ 8.0/10
7. [与爬虫作战：150 万页网站的防守战](#item-7) ⭐️ 8.0/10
8. [新墨西哥州法院裁定 Meta 支付 5.67 亿美元 赔偿儿童心理健康损害](#item-8) ⭐️ 8.0/10
9. [Gemini 遇挫，GCP 反而受益](#item-9) ⭐️ 8.0/10
10. [美国审查中国 AI 企业海外获取英伟达芯片渠道](#item-10) ⭐️ 8.0/10
11. [sub2api 曝 OAuth 高危漏洞，仅凭邮箱即可接管账户](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Flash 0731：快速、廉价、能力更强的模型更新](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 8.0/10

DeepSeek 发布了更新版 V4 Flash 0731 模型，这是一个效率优化的混合专家（MoE）大语言模型，总参数 284B、激活参数 13B。与之前的预览版相比，它在推理速度、成本和调试/数据分析能力上都有明显提升。 这次发布为开发者提供了一个极具吸引力的开放权重选择，兼具顶尖的编程性能和极低的推理成本，进一步缩小了与领先闭源模型的差距。对于预算有限但需要构建 agent 或重度推理应用的团队来说尤为重要。 该模型采用混合专家（MoE）架构，总参数 284B，每个 token 仅激活 13B 参数，并支持 100 万 token 的上下文窗口。07/31 版本相比早期预览版有大幅提升，另有一个 V4 Flash-Max 变体，在给予更多思考时间时推理能力接近 Pro 版本。

hackernews · tosh · 8月7日 17:56 · [社区讨论](https://news.ycombinator.com/item?id=49214008)

**背景**: DeepSeek 是一家发布开放权重大语言模型的 AI 实验室，与各类开源和专有系统竞争。混合专家（MoE）模型的总参数量很大，但每个 token 只激活其中一小部分，从而降低计算量和成本。V4 Flash 是 DeepSeek-V4 系列中主打效率的型号，面向快速、低成本的推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash">DeepSeek V 4 Flash - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://ollama.com/library/deepseek-v4-flash">deepseek - v 4 - flash</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体非常正面，用户称赞其成本低（每天约 5 美元或每月不到 100 美元）和速度快，包括在 RTX Pro 6000 Blackwell GPU 上优秀的本地表现。多位用户表示它现在几乎可以胜任所有任务，另有一条无关评论提到了 Claude 账号被封的问题。

**标签**: `#AI`, `#DeepSeek`, `#LLM`, `#Model Release`, `#Benchmark`

---

<a id="item-2"></a>
## [汇编耻辱堂：一个收集极慢 x86 指令的项目](https://github.com/xoreaxeaxeax/asm-hall-of-shame) ⭐️ 8.0/10

GitHub 仓库“Assembly Hall of Shame”汇集了臭名昭著的慢速 x86 指令，并给出了测量这些指令耗时的方法，揭示了令人意外的硬件性能陷阱。其中包含耗时 12 毫秒的 ACPI IO 端口写入，目前位列榜单第 8 名。 该项目表明，现代 x86 CPU 上的指令级性能并不直观，差距可能高达数个数量级，这对底层开发者、操作系统工程师和安全研究人员都很重要。它还为各种慢速路径的滥用带来了讨论，例如将它们用于触发或破坏系统管理模式（SMM）的场景。 该仓库规定，陷入（trap）、模拟或虚拟化的指令只能测量陷入本身的耗时，而不能测量处理程序的耗时，以保证测量结果有意义。但有评论者怀疑，耗时 12 毫秒的 ACPI IO 端口写入实际上可能由 SMM 处理，这会模糊上述界限。

hackernews · piotrgrabowski · 8月7日 18:01 · [社区讨论](https://news.ycombinator.com/item?id=49214098)

**背景**: x86 处理器包含许多执行时间变化极大的指令，具体取决于操作数、寻址方式和微架构状态。测量通常借助时间戳计数器（TSC）以及 RDTSC 指令完成，但乱序执行、频率缩放和 SMM 中断等陷阱会使测量结果失真。Agner Fog 的指令表以及专门的计时指南记录了 AMD 和 Intel 处理器的延迟与吞吐量。该项目延续了这一传统，收集了现实世界中那些运行慢得令人惊讶的指令案例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Time_Stamp_Counter">Time Stamp Counter - Wikipedia</a></li>
<li><a href="https://www.agner.org/optimize/instruction_tables.pdf">Introduction Page 1 4. Instruction tables By Agner Fog</a></li>
<li><a href="https://wassenberg.dreamhosters.com/articles/timing_pitfalls.pdf">Timing Pitfalls and Solutions</a></li>

</ul>
</details>

**社区讨论**: 评论展现出广泛的兴趣和幽默感：有用户开玩笑说 NOP 指令相对于它所做的事情来说是无限慢的，还有人将这个项目与 Core War 游戏联系起来。更严肃的讨论质疑 ACPI 端口写入是否会陷入 SMM，并附上了一个利用慢速指令破坏 SMI 的相关项目链接。还有评论感叹抽象层浪费了大量计算资源，这与该仓库的主题相呼应。

**标签**: `#assembly`, `#x86`, `#performance`, `#low-level`, `#hardware`

---

<a id="item-3"></a>
## [为什么科技从业者如此悲伤：对行业失去信心](https://www.noemamag.com/why-is-everyone-in-tech-so-sad/) ⭐️ 8.0/10

一篇发表在《Noema》杂志上的文章《为什么科技行业人人都如此悲伤？》探讨了科技从业者中普遍的忧郁与幻灭感，并将当下比作印刷业等技能行业的衰败。文章认为，这个行业曾许诺的前景已暗淡，从业人员正对自己的职业未来失去信心。 这篇文章之所以重要，是因为它道出了科技从业者中广泛存在的职业倦怠与幻灭，而这样一个群体的士气极少被如此深入地讨论。与印刷工人历史的类比表明，如今的科技从业者可能面临永久性的行业震荡，促使人们思考职业韧性与行业变革。 作者以印刷工人这一延续数百年后消失的技能职业作为警喻，提醒今天的科技从业者。文章暗示，当初创造了科技职业生涯的革新力量，如今可能正在反过来瓦解这些职业，让从业者难以找到乐观的前景。

hackernews · RickJWagner · 8月7日 12:42 · [社区讨论](https://news.ycombinator.com/item?id=49209539)

**背景**: 科技行业长期以来被视为充满无限机遇的领域，技术工人获得高薪和有意义的工作。然而近年来，关于职业倦怠、裁员和目标感下降的报道屡见不鲜，出现了一种所谓“科技忧郁症”的现象。文章借助印刷术发明后印刷行业变迁等历史案例，来类比当下行业的不确定性。

**社区讨论**: 社区评论显示出人们对这篇文章的强烈共鸣。有用户以印刷工人为例，指出该职业如何被技术淘汰；其他人则强调网络的毒性以及职场严肃性普遍下降。许多人表达了个人幻灭感，一位从业 20 年的老手说自己会幻想成为无家可归者，可见其深深的不满。

**标签**: `#tech culture`, `#burnout`, `#mental health`, `#software engineering`, `#industry analysis`

---

<a id="item-4"></a>
## [Oracle 的 OpenJDK 禁止 AI 生成的代码贡献](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 8.0/10

OpenJDK 项目在 openjdk.org/legal/ai 上发布了一项临时政策，禁止或限制 AI 生成的代码贡献。Oracle 的律师仍在起草该政策的最终版本。 这是对一个全球最重要的开源项目之一而言重大的政策转变，影响着 Java 贡献者的工作方式，也推动了关于开源中 AI 来源的讨论。它还凸显了一种讽刺：Oracle（在 Larry Ellison 领导下）大力推广 AI，却拒绝外部提交的 AI 生成代码。 该政策被明确描述为风险管控措施，关注法律来源而非仅为代码质量。最终版本仍由 Oracle 法律团队撰写，因此临时规则可能会改变。

hackernews · delduca · 8月7日 17:36 · [社区讨论](https://news.ycombinator.com/item?id=49213754)

**背景**: OpenJDK 是 Java 平台的开源参考实现，由 Oracle 和一个开发者社区维护。AI 生成的代码可能带有不确定的版权来源，因为模型可能在受许可或受版权保护的代码上训练，这会给接受此类贡献的项目带来法律风险。Oracle 在 Java 相关的版权执法上有悠久而激进的记录，包括针对 Java API 的诉讼。

**社区讨论**: 评论者普遍理解这一决定是法律/风险管控举动，不过许多人指出这与 Oracle 自身对 AI 的推动形成讽刺。一些人对最终政策表示怀疑，另一些人则指出人类审查者的负担是真实关切。

**标签**: `#OpenJDK`, `#Oracle`, `#AI-generated code`, `#open source policy`, `#software licensing`

---

<a id="item-5"></a>
## [pgrust 用 Rust 重写 Postgres，宣称分析查询快 300 倍](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 8.0/10

这篇题为“让 Postgres 分析查询快 300 倍”的博客文章介绍了 pgrust——一个用 Rust 重写的 PostgreSQL 实现，通过批处理、算子融合和 SIMD，在分析型查询上实现了最高 300 倍的加速。pgrust 还编译为 WebAssembly，可以直接在浏览器中运行。 这件事意义重大，因为它挑战了“Postgres 查询引擎性能已接近上限”的普遍看法，展示现代技术能带来数量级的性能提升。它可能影响 Postgres 未来的演进方向，并推动自适应规划和向量化执行等技术在传统数据库中得到更广泛应用。 加速来自三项技术：对行进行批处理以减少逐行的开销、融合算子以避免物化中间结果、以及利用 SIMD 指令一次处理多个值。作者将正确性列为第一优先级，通过形式化验证和差分模糊测试来证明 1000 多个函数与 Postgres 的逻辑完全一致。

hackernews · poly2it · 8月7日 11:00 · [社区讨论](https://news.ycombinator.com/item?id=49208535)

**背景**: PostgreSQL 是一款广泛使用的开源关系型数据库，但其逐行(row-at-a-time)执行器在处理分析型负载时，比 ClickHouse 等列式存储和向量化系统要慢。pgrust 是作者用 Rust 做的实验性重写，旨在展示“如果 Postgres 在今天从头构建会是什么样子”；它可以编译为 WebAssembly，让查询直接在浏览器中运行。批处理、算子融合和 SIMD 都是数据库引擎中已被验证的技术，DuckDB 等系统正是通过它们来降低逐行开销并更好地利用现代 CPU。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now faster than Postgres and Clickhouse · GitHub</a></li>
<li><a href="https://pgrust.com/">pgrust — postgres, rewritten in rust</a></li>

</ul>
</details>

**社区讨论**: 作者在评论中表示正确性是最优先事项，并已通过形式化验证和差分模糊测试证明 1000 多个函数与 Postgres 一致。一些评论者质疑，关键数据库能否在官方 Postgres 团队之外获得信任；另一些人则对自适应规划表示兴奋，这是 Postgres 核心团队长期拒绝采纳的功能。

**标签**: `#postgres`, `#query-engine`, `#rust`, `#performance`, `#simd`

---

<a id="item-6"></a>
## [2027 年 HBM 产能售罄，DRAM 供应承压](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

内存行业报告称，受人工智能需求激增推动，2027 年的 HBM（高带宽内存）产能已被全部订满。这导致留给普通 DRAM 的晶圆产能减少，整体内存供应趋紧。 这标志着内存供应将面临多年紧张态势，不仅影响 AI 加速器，还会波及 PC、游戏机和手机等消费电子产品。DRAM 及终端设备价格可能上涨，AI 硬件生产也可能遭遇瓶颈。 在相同工艺节点下，生产相同比特数的 HBM 所需晶圆大约是标准 DDR5 的三倍，因为 HBM 裸片更大。由于 HBM 被优先供应，非 HBM DRAM 的产出增长将受到限制。

hackernews · inigyou · 8月7日 07:58 · [社区讨论](https://news.ycombinator.com/item?id=49207236)

**背景**: HBM 是一种与 GPU 和加速器配合使用的 3D 堆叠 DRAM 接口，由三星、AMD 和 SK 海力士等公司开发。它通过垂直堆叠存储裸片并利用硅通孔连接到逻辑裸片，提供了远超普通 DRAM 的带宽。AI 模型的训练和推理需要极高的内存带宽，因此 HBM 至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://medium.com/the-low-end-disruptor/the-great-wall-of-high-bandwidth-memory-hbm-4d19b9f48549">The Great Wall of High Bandwidth Memory ( HBM ) | Medium</a></li>
<li><a href="https://acepcba.com/what-is-hbm-memory-why-does-ai-hardware-need-it/">What Is HBM Memory and Why Does AI Hardware Depend on It ?</a></li>

</ul>
</details>

**社区讨论**: 评论者对更广泛的市场影响表示担忧：有人指出 HBM 产能售罄意味着用于 DDR5 的晶圆减少，有人担心消费产品通货膨胀，还有用户表示想囤积单片机。也有用户从个人层面反思，称 AI 对内存和存储的压力让他们对使用 AI 感到犹豫。

**标签**: `#HBM`, `#memory`, `#semiconductors`, `#supply chain`, `#AI`

---

<a id="item-7"></a>
## [与爬虫作战：150 万页网站的防守战](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

一位拥有 150 万页网站的站长发了一篇详细回顾，讲述自己一年来与爬虫和机器人流量作战的经历，并透露某个月份的账单从约 90 美元飙涨了近 500%。文章介绍了包括 Cloudflare 验证挑战在内的各种应对策略，以及对抗爬虫所带来的实际成本和观念层面的代价。 这一事件的重要性在于，它量化了 AI 爬虫和机器人给独立网站运营者带来的实际运营与财务负担，并引发了关于 Cloudflare 等集中式防护服务与自托管替代方案之间取舍的讨论。它还与当前围绕 AI 训练数据抓取和开放网络未来的行业辩论直接相关。 该网站运行在 Cloudflare Workers 和 D1（Cloudflare 的无服务器 SQLite 数据库）上，一个“糟糕的峰值月份”让约 90 美元的月度账单上涨了大约 500%。作者还承认，自己的网站本身也会抓取公开文件，并坦言“一个爬虫在写抱怨爬虫的博客文章”，这是一件很讽刺的事情。

hackernews · petercooper · 8月7日 14:51 · [社区讨论](https://news.ycombinator.com/item?id=49211386)

**背景**: 网络爬虫（Web scraping）是指从网站上自动提取数据的行为，对网站所有者而言，当机器人消耗带宽和数据库查询时，可能导致服务器过载并推高账单。许多网站依赖 Cloudflare 的机器人防护服务，其中包括 Turnstile——一种用于区分人类与自动化客户端的验证码替代方案。OpenAI 的 GPTBot 等 AI 爬虫的兴起，使得抓取的数量和复杂程度不断升级，这已成为独立网站发布者日益担忧的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Cloudflare_Turnstile">Cloudflare Turnstile</a></li>
<li><a href="https://datadome.co/bots/gptbot/">What is the GPTBot?</a></li>

</ul>
</details>

**社区讨论**: 评论者大多对作者表示理解，但在解决方案上存在分歧：一些人警告不要依赖 Cloudflare 的集中控制，并推荐 Anubis 等自托管“工作量证明”工具；另一些人则建议放弃 D1，改用静态站点以降低成本。还有人分享了自身遭遇的数据——例如 Claude-searchbot 在 72 小时内抓取了约 20.5 万页，却只带来 1 次引导访问——并指出作者自己的网站也在抓取公开文件的事实颇具讽刺意味。

**标签**: `#web scraping`, `#bot protection`, `#Cloudflare`, `#website security`, `#AI crawlers`

---

<a id="item-8"></a>
## [新墨西哥州法院裁定 Meta 支付 5.67 亿美元 赔偿儿童心理健康损害](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta) ⭐️ 8.0/10

新墨西哥州一家法院裁定 Meta 支付 5.67 亿美元，原因是其社交媒体平台损害了儿童心理健康，并责令其为未成年用户做出整改。该判决源自一项诉讼，指控 Meta 违反公共妨害法，通过设计成瘾性功能对未成年人造成伤害。 这是针对大型社交媒体公司涉及青少年心理健康的金额最高的州级判决之一，可能为其他州和司法管辖区提起类似诉讼开创先例。这将迫使 Meta 乃至整个行业重新审视算法设计和儿童保护措施。 该裁决依据新墨西哥州公共妨害法（NMSA 1978 § 30-8-1），而非联邦 Section 230 保护条款。关于总金额的报道存在差异：路透社和《卫报》称其中 5.67 亿美元用于青少年心理健康基金，而《华尔街日报》报道判决总额为 9.42 亿美元。

hackernews · boplicity · 8月7日 00:06 · [社区讨论](https://news.ycombinator.com/item?id=49204352)

**背景**: 社交媒体公司因平台对年轻用户心理健康的影响而面临越来越多的审查，研究将过度使用与焦虑和抑郁联系起来。新墨西哥州总检察长提起的这起诉讼试图依据州公共妨害法追究 Meta 的责任，这种策略绕过了保护平台免受第三方内容发布者责任的联邦豁免条款。

**社区讨论**: 评论者指出，尽管 5.67 亿甚至 9.42 亿美元相对于 Meta 的全球收入而言只是很小一部分，但按新墨西哥州 210 万人口分摊来说，这是一笔巨额罚款。一位用户列出了具体的公共妨害法规及其适用条款，其他人则将 Instagram Reels 和 TikTok 比作成瘾物质，并敦促 Meta 改变其算法。

**标签**: `#social-media`, `#regulation`, `#mental-health`, `#meta`, `#legal`

---

<a id="item-9"></a>
## [Gemini 遇挫，GCP 反而受益](https://newsletter.semianalysis.com/p/gemini-is-cooked-but-gcp-is-cooking) ⭐️ 8.0/10

SemiAnalysis 的一篇文章认为，DeepMind 旗下 Gemini AI 模型遇到的困境，反而会在短期内推动 Google Cloud Platform 的增长。这篇分析把 DeepMind 的长期挑战重新解读为 GCP 云基础设施业务的短期利好。 这之所以重要，是因为它揭示了谷歌内部的一种战略分化：一边是 DeepMind 的长期 AI 雄心，另一边是 GCP 的商业增长势头。它意味着，即使谷歌的前沿模型落后，其云业务仍能从整体 AI 热潮中获得可观收入。 文章的核心论点是存在一种时间错配：DeepMind 的长期失败会变成 GCP 的短期收益，因为无论模型质量如何，AI 算力需求和云收入都在持续增长。该文侧重于商业战略和市场动态，而非技术基准或具体产品发布。

rss · Semianalysis · 8月7日 02:32

**背景**: Google DeepMind 是谷歌负责 Gemini 系列大语言模型的 AI 研究部门，该系列与 OpenAI 的 GPT 系列竞争。Google Cloud Platform（GCP）向外部客户出售云计算和 AI 基础设施服务。这篇文章的论点建立在这样一个观察之上：一家公司自研模型的质量与其云基础设施收入可能发生背离，尤其是在外部对 AI 算力需求强劲的时候。

**标签**: `#AI`, `#Google Cloud`, `#DeepMind`, `#Strategy`, `#Cloud Computing`

---

<a id="item-10"></a>
## [美国审查中国 AI 企业海外获取英伟达芯片渠道](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 8.0/10

美国商务部工业与安全局（BIS）已启动一项系统性审查，调查中国 AI 企业如何在海外获取和使用英伟达芯片，包括通过远程访问海外算力的方式。此次审查的部分导火索是月之暗面近期发布的 Kimi K3 模型，一名白宫官员指控该模型使用了非法获取的英伟达芯片，并通过泰国远程访问。 此次审查可能将美国出口管制从硬件销售扩展到云计算远程访问，直接影响英伟达等美国科技公司的全球客户服务能力。这也标志着中美科技竞争的新战线，可能重塑全球 AI 企业获取先进芯片的方式。 BIS 正在整理两份名单：一份是涉嫌将受限芯片走私入中国的黑市所在地名单，另一份是中国企业远程租用芯片的国家名单。报道还称，阿里巴巴通过开曼实体控制的壳公司，经由已被美方调查的 Megaspeed，使用了位于马来西亚的英伟达芯片。

telegram · zaihuapd · 8月7日 11:18

**背景**: 自 2022 年以来，美国对向中国出口先进 AI 芯片实施了限制，但中国企业试图通过租用其他国家数据中心的算力来规避这些管制。远程访问芯片本身并不违法，BIS 是否有权限制此类云计算协议尚不明确。美国众议院已通过一项两党法案，拟明确授予该权力，但预计会遭到英伟达等科技公司的反对。

**标签**: `#US-China tech policy`, `#export controls`, `#AI hardware`, `#Nvidia`, `#cloud computing`

---

<a id="item-11"></a>
## [sub2api 曝 OAuth 高危漏洞，仅凭邮箱即可接管账户](https://github.com/Wei-Shaw/sub2api/issues/5350) ⭐️ 8.0/10

sub2api v0.1.171 及之前版本存在一个 CVSS 8.8 的高危 OAuth 账户接管漏洞，攻击者仅凭受害者邮箱即可接管账户，无需密码、验证码或用户交互。该漏洞利用 pending session 流程中 existingUser 分支不校验密码和验证码的问题，将攻击者的 OAuth 身份绑定到受害者账户。 该漏洞可导致账户被完全接管，攻击者能够控制受害者的 API 密钥、账单余额和订阅配额。由于 OAuth 被广泛使用，此事件凸显了在 OAuth 绑定流程中验证身份步骤的重要性。 该利用针对 pending session 流程中的 existingUser 分支，该分支在绑定 OAuth 身份时不验证密码或验证码。绑定后，攻击者每次 OAuth 登录都会解析为受害者账户。

telegram · zaihuapd · 8月7日 14:59

**背景**: OAuth 2.0 是一种广泛使用的框架，允许用户通过社交媒体账户登录网站。常见的 OAuth 漏洞包括重定向 URI 操作、CSRF 保护缺失以及缺少 PKCE，但本案例源于 sub2api 中不安全的账户绑定逻辑。账户接管是指攻击者将自己的身份绑定到受害者的现有账户，从而获得完全访问权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://portswigger.net/web-security/oauth">OAuth 2.0 authentication vulnerabilities | Web Security Academy</a></li>
<li><a href="https://outpost24.com/blog/common-oauth-vulnerabilities-mitigations/">7 common OAuth vulnerabilities (plus mitigations)</a></li>

</ul>
</details>

**标签**: `#security`, `#oauth`, `#vulnerability`, `#account-takeover`, `#sub2api`

---