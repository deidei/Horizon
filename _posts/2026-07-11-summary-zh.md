---
layout: default
title: "Horizon Summary: 2026-07-11 (ZH)"
date: 2026-07-11
lang: zh
---

> 从 29 条内容中筛选出 10 条重要资讯。

---

1. [vLLM v0.25.0：重大更新，默认使用 Model Runner V2](#item-1) ⭐️ 9.0/10
2. [人形机器人完成全球首例活猪手术](#item-2) ⭐️ 9.0/10
3. [OpenAI 发布 GPT-5.6 系列，旗舰模型 Sol 引领升级](#item-3) ⭐️ 9.0/10
4. [SGLang v0.5.15 发布：GLM-5.2 与 Spec V2 带来大幅性能提升](#item-4) ⭐️ 8.0/10
5. [ClickHouse 团队将 PgBouncer 吞吐量提升 4 倍](#item-5) ⭐️ 8.0/10
6. [VultronRetriever 模型登顶 MTEB 排行榜](#item-6) ⭐️ 8.0/10
7. [苹果起诉 OpenAI 系统性窃取商业机密](#item-7) ⭐️ 8.0/10
8. [U-Boot 引导程序存在六个漏洞，可在启动前执行代码](#item-8) ⭐️ 8.0/10
9. [智谱创始人启动‘摸高计划’聚焦 AGI](#item-9) ⭐️ 8.0/10
10. [上海计划 2027 年前实现高质量脑控，脑机接口取得突破](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0：重大更新，默认使用 Model Runner V2](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 版本发布，包含来自 232 位贡献者的 558 次提交，将 Model Runner V2 设为所有稠密模型的默认执行路径，移除了旧版 PagedAttention，并使 Transformers 后端达到与原生 vLLM 持平的速度。 此版本标志着 vLLM 架构的重大转变，通过移除旧组件简化代码库并提升建模后端的性能，直接惠及部署大型语言模型进行推理的用户。 Model Runner V2 现在支持 EVS（高效视频采样）、实时嵌入以及带有完整 CUDA 图的动态推测解码，而新的流式解析器引擎统一了工具调用/推理解析。

github · khluu · 7月11日 20:06

**背景**: vLLM 是一个由加州大学伯克利分校等开发的开源高吞吐量 LLM 推理引擎，最初使用 PagedAttention 来高效管理内存。Model Runner V2 是一个更新、更灵活的执行框架，取代了旧组件，提升了性能和可维护性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm -project/ vllm</a></li>
<li><a href="https://docs.vllm.ai/en/stable/features/speculative_decoding/dynamic_speculative_decoding/">Dynamic Speculative Decoding - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2025-10-31-run-multimodal-reasoning-agents-nvidia-nemotron">Run Multimodal Reasoning Agents with NVIDIA Nemotron on vLLM | vLLM Blog</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#release`, `#model serving`, `#performance`

---

<a id="item-2"></a>
## [人形机器人完成全球首例活猪手术](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

外科医生远程操控宇树 G1 人形机器人，成功在活猪身上完成了两例微创胆囊切除手术，这是全球首次将通用人形机器人用于活体手术，研究成果发表在《自然》期刊。 这一突破表明，低成本通用人形机器人有潜力替代昂贵的专用手术机器人（如达芬奇系统），使先进手术在资源有限的环境（农村、战场、太空）成为可能。其成本仅为传统系统的十分之一左右。 宇树 G1 基础款售价约 13,500 美元（约 9.9 万元人民币），配备灵巧手后约 67,000 美元；身高 1.5 米，重 27 公斤。该研究由加州大学圣地亚哥分校团队主导。

telegram · zaihuapd · 7月11日 02:29

**背景**: 传统手术机器人如达芬奇系统售价 50 万至数百万美元，且体积庞大。通用人形机器人原本设计用于一般任务，通过远程操控和灵巧手可以完成精细手术操作。灵巧手技术近年来发展迅速，结合 AI 大模型提高了操作的精确性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.dzplus.dzng.com/share/general/0/NEWS2139618WUMBNTSKAWAFL">半岛聚焦丨65...</a></li>
<li><a href="https://www.jinantimes.com.cn/news-243-5048472.html">jinantimes.com.cn/news-243-5048472.html</a></li>
<li><a href="http://www.news.cn/tech/20240827/d8f188d8e0b9486aadc1ce2ae72efd15/c.html">灵巧手引领人形机器人“心灵手巧”-新华网</a></li>

</ul>
</details>

**标签**: `#人形机器人`, `#手术`, `#医疗机器人`, `#远程手术`, `#低成本`

---

<a id="item-3"></a>
## [OpenAI 发布 GPT-5.6 系列，旗舰模型 Sol 引领升级](https://t.me/zaihuapd/42497) ⭐️ 9.0/10

OpenAI 正式发布 GPT-5.6 系列，推出三个模型：Sol（旗舰）、Terra（平衡）和 Luna（低成本高并发）。该系列大幅提升了代码、知识工作、设计、科研和网络安全能力，并引入了 max/ultra 推理模式、多智能体协作和程序化工具调用。 此次发布标志着 OpenAI 分层模型策略的重要一步，为不同应用场景提供了定制化的性能-成本权衡。新的推理模式和工具调用能力支持更高效、更复杂的任务自动化，有望降低成本并扩展大型语言模型在企业与研究中的应用范围。 GPT-5.6 Sol 在网络安全和长周期推理任务上能力最强，Terra 平衡性能与成本，Luna 面向高吞吐低成本的场景。max 推理模式赋予 Sol 更长的思考时间，ultra 模式支持生成子智能体进行并行任务分解。程序化工具调用使模型能通过代码编排工具，而非逐个 API 往返。

telegram · zaihuapd · 7月11日 13:34

**背景**: GPT-5.6 系列紧随 GPT-5.5 仅两个月后发布，体现了 OpenAI 的快速迭代节奏。分层模型系列（如 Sol、Terra、Luna）允许用户根据预算和性能需求选择最合适的模型。max/ultra 推理模式扩展了思维链概念，支持更深层次的思考或并行子智能体执行。程序化工具调用最初由 Anthropic 的 Claude 引入，通过减少延迟和提高可靠性实现更高效的工具使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>
<li><a href="https://www.freepixel.com/blog/openai-gpt-5-6-sol/">OpenAI GPT - 5 . 6 Sol : Ultimate Features, Availability Guide</a></li>
<li><a href="https://medium.com/mlworks/whats-new-with-openai-s-gpt5-6-551b3d8cc6b6">What’s New With OpenAI’s GPT 5 . 6 ? | by Mayur Jain | Medium</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-5.6`, `#AI models`, `#large language models`, `#multi-agent`

---

<a id="item-4"></a>
## [SGLang v0.5.15 发布：GLM-5.2 与 Spec V2 带来大幅性能提升](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

SGLang v0.5.15 带来了在 Blackwell 上针对生产环境调优的 GLM-5.2 NVFP4，默认启用 Spec V2 使吞吐量提升高达 11%，并新增 IndexShare MTP 将草稿步成本降低最多 1.9 倍。 这些优化显著提升了大规模语言模型推理的吞吐量和成本效率，惠及部署大规模 LLM 的开发者和企业。 IndexShare MTP 在草稿步之间重用索引器 top-k，Spec V2 使用 CUDA Graph 可编译的 DSA 草稿扩展消除不必要的同步。FlashInfer 自动调优现在覆盖草稿模型图。

github · Fridge003 · 7月10日 22:58

**背景**: SGLang 是一个开源的大语言模型推理引擎，以高性能著称。NVFP4 是 NVIDIA 的 4 位浮点格式，用于在 Blackwell GPU 上实现高效推理。推测性解码通过使用较小的草稿模型加速生成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>
<li><a href="https://huggingface.co/blog/zai-org/glm-52-blog">GLM-5.2: Built for Long-Horizon Tasks</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#performance optimization`, `#speculative decoding`, `#GPU serving`, `#sglang`

---

<a id="item-5"></a>
## [ClickHouse 团队将 PgBouncer 吞吐量提升 4 倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse Managed Postgres 团队通过使用 SO_REUSEPORT 进行套接字复用和一种对等机制进行高效的取消转发，将 PgBouncer 的吞吐量提升了 4 倍。 这一改进使 PgBouncer 能够利用多个 CPU 核心，克服其单线程瓶颈。它有利于具有高连接周转率和查询取消负载的 PostgreSQL 部署。 该设置需要在 pgbouncer.ini 中设置 so_reuseport=1，并配置 peer_id 和 [peers] 部分，以便将取消请求转发到正确的拥有进程。

hackernews · saisrirampur · 7月11日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是一个单线程的 PostgreSQL 连接池，因此只能使用一个 CPU 核心。使用 SO_REUSEPORT 运行多个进程可以让操作系统分配连接，但取消请求必须到达拥有该会话的确切进程。对等机制通过在取消键中编码 peer_id 并转发错发的取消来解决此问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres">How we scale PgBouncer in ClickHouse Managed Postgres</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>
<li><a href="https://deepwiki.com/pgbouncer/pgbouncer/7.3-peer-forwarding-and-cancel-requests">Peer Forwarding and Cancel Requests | DeepWiki</a></li>

</ul>
</details>

**社区讨论**: 评论者对对等设置表示兴趣，并提到了 Odyssey 和 pgdog 等替代方案。其他人分享了在 Kubernetes 上运行多个 PgBouncer 进程的经验。讨论具有建设性，涉及 so_reuseport 和对等配置的问题。

**标签**: `#PostgreSQL`, `#PgBouncer`, `#performance`, `#connection pooling`, `#scalability`

---

<a id="item-6"></a>
## [VultronRetriever 模型登顶 MTEB 排行榜](https://www.reddit.com/r/MachineLearning/comments/1utmxq8/vultronretriever_family_of_models_released_on/) ⭐️ 8.0/10

VultronRetriever 模型系列（Prime-8B、Core-4.5B、Flash-0.8B）在 HuggingFace 上发布，在 MTEB 排行榜上各自类别中夺得第一，其中 Prime-8B 成为全球总榜第一，并宣称索引存储减少 16 倍、吞吐量提升 12 倍。 此次发布显著提升了检索效率，使大规模嵌入和检索任务能够以极低的存储和延迟进行，并将最先进的检索能力带到 iPhone 等边缘设备上，实现完全离线使用。 这些模型采用 Hydra 架构实现后期交互检索，提供高精度且内存仅为同类模型的一半。它们使用 0% 交叉数据集重复和 0% 评估污染的数据集进行训练。

reddit · r/MachineLearning · /u/madkimchi · 7月11日 15:22

**背景**: MTEB（大规模文本嵌入基准）是评估嵌入模型在检索、分类、聚类等任务上表现的标准公开排行榜。后期交互检索（如 ColBERT 中使用）将查询和文档分开处理直到最后阶段，实现高效精确的检索。Hydra 架构在单个视觉语言模型中统一了检索和生成功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/spaces/mteb/leaderboard">MTEB Leaderboard - a Hugging Face Space by mteb</a></li>
<li><a href="https://arxiv.org/html/2603.28554">Hydra: Unifying Document Retrieval and Generation in a Single Vision-Language Model</a></li>
<li><a href="https://embeddings-benchmark.github.io/mteb/get_started/usage/leaderboard/">Run the Leaderboard - Massive Text Embedding Benchmark</a></li>

</ul>
</details>

**标签**: `#retrieval`, `#MTEB`, `#NLP`, `#AI`, `#model release`

---

<a id="item-7"></a>
## [苹果起诉 OpenAI 系统性窃取商业机密](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 8.0/10

苹果于 7 月 10 日在美国加州北区联邦法院起诉 OpenAI、两名前员工及 io Products，指控其系统性窃取苹果的产品设计、制造工艺及供应链机密，以加快消费级硬件研发。 这起两大科技巨头之间的诉讼突显了知识产权和人才挖角方面日益紧张的局势，可能重塑企业在 AI 和硬件领域保护商业机密的方式。 苹果指控前员工 Chang Liu 离职后仍访问内部网络并下载数十份硬件文件；OpenAI 硬件负责人 Tang Yew Tan 被指在离职前将供应商资料发送至个人邮箱，并要求求职者携带苹果零部件参加面试。苹果还表示，目前有超过 400 名前员工在 OpenAI 工作。

telegram · zaihuapd · 7月11日 03:14

**背景**: 苹果以对产品开发和硬件设计的严格保密而闻名。OpenAI 最初是非营利 AI 研究实验室，但近年日益转向消费级硬件的开发，包括传闻中的 AI 设备。商业机密诉讼常发生在员工跳槽至竞争对手时，但本案的规模和系统性窃取指控使其格外引人注目。

**标签**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#hardware`

---

<a id="item-8"></a>
## [U-Boot 引导程序存在六个漏洞，可在启动前执行代码](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

安全公司 Binarly 披露了 U-Boot 引导程序 FIT 签名验证代码中的六个漏洞，其中两个可导致任意代码执行，四个可造成设备崩溃，影响自 2013.07 版本以来的所有版本。 这些漏洞允许攻击者在操作系统和安全软件加载之前执行恶意代码，可能禁用固件防御并植入持久性固件恶意软件。对于支持远程固件更新的 BMC 等设备，无需物理接触即可利用。 这些漏洞（BRLY-2026-037 至 BRLY-2026-042）存在于 FIT 签名验证逻辑中。Binarly 已提交补丁并获得接受，但部署需要硬件厂商将修复集成到固件更新中，已停止支持的老旧设备将面临风险。

telegram · zaihuapd · 7月11日 08:32

**背景**: U-Boot 是一种广泛应用于嵌入式设备的开源引导程序。FIT（扁平化镜像树）是一种用于打包内核、设备树和其他镜像并附加密签名的格式。签名验证过程确保只加载可信固件。基板管理控制器（BMC）是专门用于系统监控和远程固件更新的微控制器，因此特别容易受到远程固件攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/u-boot-fit-signature-verification/">Six U - Boot FIT Signature Verification Flaws Enable Code Execution...</a></li>
<li><a href="https://docs.u-boot-project.org/en/latest/usage/fit/signature.html">U - Boot FIT Signature Verification — Das U - Boot unknown version...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#bootloader`, `#U-Boot`, `#firmware`

---

<a id="item-9"></a>
## [智谱创始人启动‘摸高计划’聚焦 AGI](https://mp.weixin.qq.com/s/3CQSkf_kBnXiCDgS4L-Cgg) ⭐️ 8.0/10

智谱创始人唐杰在一封内部信中宣布启动“摸高计划”，承诺专注于 AGI 研究而非短期商业变现。该计划指出了四项关键挑战：长程任务、自治智能体系统、完全自我训练和极致安全治理。 这标志着中国 AI 公司向长期 AGI 研究的战略转变，大量资源投入到安全性和可解释性方面，可能影响全球 AI 发展。智谱的开源策略和竞争性模型或可加速透明 AI 的进步。 智谱计划投入百亿级资源攻坚机械可解释性，推动黑盒模型透明化。其 GLM-5.2 模型已接近海外最前沿模型能力，并因其开源特性在技术社群中广受欢迎。

telegram · zaihuapd · 7月11日 13:59

**背景**: 机械可解释性是可解释人工智能的一个分支，旨在通过分析神经网络内部机制来理解其运作。智谱 AI 是一家中国 AI 公司，以其 GLM 系列模型闻名，这些模型开源且在研究和应用中广泛使用。“摸高计划”提出了一条通过四大支柱实现 AGI 的多年路线图。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability - Wikipedia</a></li>
<li><a href="https://www.scmp.com/tech/tech-trends/article/3359170/zhipu-ai-releases-harness-glm-52-model-chinese-firm-takes-aim-anthropic">Zhipu AI releases harness for GLM-5.2 model as Chinese firm takes aim at Anthropic | South China Morning Post</a></li>

</ul>
</details>

**标签**: `#AGI`, `#AI safety`, `#interpretability`, `#Zhipu AI`, `#GLM`

---

<a id="item-10"></a>
## [上海计划 2027 年前实现高质量脑控，脑机接口取得突破](https://t.me/zaihuapd/42501) ⭐️ 8.0/10

上海市科学技术委员会印发《上海市脑机接口未来产业培育行动方案（2025-2030 年）》，目标到 2027 年实现高质量脑控，半侵入式脑机接口产品在国内率先实现临床应用。 这标志着中国政府对脑机接口技术的大力推动，可能加速临床采用，并将上海打造为神经技术创新中心。 该计划还推动 5 款以上侵入式、半侵入式脑机接口产品完成医疗器械型式检验和临床试验，面向失语、瘫痪等患者实现部分语言和运动功能恢复。

telegram · zaihuapd · 7月11日 15:49

**背景**: 脑机接口（BCI）使大脑与外部设备直接通信。它们分为非侵入式（头皮电极）、半侵入式（电极置于颅骨下但位于大脑外）和侵入式（直接植入脑组织）。半侵入式 BCI（如 ECoG）在信号质量和手术风险之间取得平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Brain–computer_interface">Brain–computer interface - Wikipedia</a></li>
<li><a href="http://learn.neurotechedu.com/introtobci/">Intro to Brain Computer Interface - NeurotechEDU</a></li>
<li><a href="https://flcube.com/?p=26674">Shanghai's Ambitious Plan to Revolutionize Brain -Computer Interfaces</a></li>

</ul>
</details>

**标签**: `#brain-computer interface`, `#neurotechnology`, `#policy`, `#medical technology`, `#Shanghai`

---