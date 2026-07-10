---
layout: default
title: "Horizon Summary: 2026-07-10 (ZH)"
date: 2026-07-10
lang: zh
---

> 从 36 条内容中筛选出 12 条重要资讯。

---

1. [GPT-5.6 Sol Ultra 证明图论循环双覆盖猜想](#item-1) ⭐️ 10.0/10
2. [开源射频相机 QuadRF 可穿透墙壁探测无人机和 WiFi](#item-2) ⭐️ 9.0/10
3. [长征十号乙完成全球首次网系回收](#item-3) ⭐️ 9.0/10
4. [OpenAI、谷歌通过新加坡向黑名单中国公司提供 AI](#item-4) ⭐️ 9.0/10
5. [sglang v0.5.15：Blackwell 与推测解码性能提升](#item-5) ⭐️ 8.0/10
6. [纽约市禁止欺骗性订阅行为](#item-6) ⭐️ 8.0/10
7. [成功公司患上制度性失明](#item-7) ⭐️ 8.0/10
8. [为什么 ML 没有限制每位作者的投稿数量？](#item-8) ⭐️ 8.0/10
9. [马斯克盛赞 Anthropic，承诺 400 亿美元合同不中断服务](#item-9) ⭐️ 8.0/10
10. [腾讯洽购 AI 公司 Manus，拟从 Meta 手中回购](#item-10) ⭐️ 8.0/10
11. [欧盟因成瘾设计对 Meta 罚款 120 亿美元](#item-11) ⭐️ 8.0/10
12. [OpenAI 将 Codex 和 Atlas 整合进 ChatGPT 桌面应用](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GPT-5.6 Sol Ultra 证明图论循环双覆盖猜想](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf) ⭐️ 10.0/10

2026 年 7 月 10 日，OpenAI 宣布其 GPT-5.6 Sol Ultra 模型生成了图论中长期未解的循环双覆盖猜想的一个证明。证明和使用的提示词均以 PDF 形式公开发布。 这标志着 AI 驱动数学发现的一个重要里程碑，表明大型语言模型能够解决数学中的深层开放问题。它可能改变数学家处理猜想的方式，并加速证明生成。 该证明非常简洁，暗示了之前专家们忽略的一个巧妙技巧。模型被提供了一个包含背景和指令的提示，并在大约一小时内生成了证明。

hackernews · scrlk · 7月10日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=48863490)

**背景**: 循环双覆盖猜想由 W. T. Tutte 等人提出，询问是否每个无桥无向图都有一个环的集合覆盖每条边恰好两次。这是图论中的一个核心问题，与图嵌入相关。此前只有部分结果，该猜想几十年来一直未被解决。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://www.openproblemgarden.org/op/cycle_double_cover_conjecture">Cycle double cover conjecture | Open Problem Garden</a></li>

</ul>
</details>

**社区讨论**: 社区对此印象深刻，评论强调这是一个证明而非反例，并且提示词的发布受到赞赏。一些人注意到证明极其简洁，引发了对是否利用了某个技巧的疑问，并讨论了 AI 在数学中的影响，包括对理论构建证明的需求。

**标签**: `#AI`, `#mathematics`, `#graph theory`, `#breakthrough`, `#OpenAI`

---

<a id="item-2"></a>
## [开源射频相机 QuadRF 可穿透墙壁探测无人机和 WiFi](https://www.jeffgeerling.com/blog/2026/quadrf-can-spot-drones-and-see-wifi-through-my-wall/) ⭐️ 9.0/10

QuadRF 是一个开源射频成像平台，结合了树莓派 5、软件定义无线电和相控阵天线，演示中成功实时探测到大疆 Phantom 4 无人机以及穿墙的 WiFi 信号。 该工具将先进的射频感知能力开放给爱好者和研究人员，可能催生无人机探测、安全审计和隐私研究等新应用，同时也引发关于监控能力的伦理问题。 该系统采用 4x4 MIMO SDR 和相控阵波束成形，基于树莓派 5 运行，部分开源（RF 核心受保护）。演示视频实时显示了无人机和墙后 WiFi 接入点的可视化图像。

hackernews · speckx · 7月10日 15:59 · [社区讨论](https://news.ycombinator.com/item?id=48861717)

**背景**: 无线电波能穿透多种建筑材料，但探测和定位信号需要专用硬件。软件定义无线电（SDR）提供灵活的信号处理，但相控阵定向传统上价格高昂。QuadRF 将这些功能整合为一个相对低成本的开源套件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/dustinbowers/QuadRF">GitHub - dustinbowers/QuadRF</a></li>
<li><a href="https://www.hackster.io/news/quadrf-the-open-source-rf-camera-that-lets-you-see-wi-fi-signals-141ad91f2a2d">QuadRF: The Open Source RF Camera That Lets You See Wi-Fi ...</a></li>
<li><a href="https://www.opensourceforu.com/2026/07/rf-imaging-platform-visualises-wi-fi-signals/">RF Imaging Platform Visualises Wi-Fi Signals - Open Source ...</a></li>

</ul>
</details>

**社区讨论**: 创作者（mrtnmcc）与社区互动，表示正在根据反馈改进用户界面。评论者讨论了诸如声音源定位、隐私问题以及与智能眼镜集成等潜在用途。有人指出，类似能力早已存在于政府监控工具中。

**标签**: `#RF detection`, `#open-source`, `#drone detection`, `#WiFi security`, `#SDR`

---

<a id="item-3"></a>
## [长征十号乙完成全球首次网系回收](https://weibo.com/7340734455/R814of1Ki) ⭐️ 9.0/10

2026 年 7 月 10 日，长征十号乙运载火箭从海南商业航天发射场升空，其第一级通过海上平台的网系回收系统成功回收，这是中国首次实现运载火箭一子级可控回收，也是全球首次运载火箭网系回收。 这一突破大幅降低了发射成本，推动了中国可重复使用火箭技术的发展，展示了独立于 SpaceX 着陆腿方式的回收新路径。 网系回收依靠回收船井字形阻拦索挂住火箭挂钩，无需着陆支腿即可实现回收。长征十号乙由此成为中国首型成功回收的重复使用运载火箭。

telegram · zaihuapd · 7月10日 04:36

**背景**: 火箭回收是实现可重复使用的关键，可以降低单次发射成本。现有方法如 SpaceX 的垂直着陆腿需要精确的发动机点火并增加额外重量。网系回收通过缆绳捕获火箭，有望减轻重量和降低复杂度。此前中国尚未实现运载火箭一子级海上回收。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.guancha.cn/kegongliliang/2026_07_10_823277.shtml">长10乙 回 收 成功：美国人做了和没做的事，我们都要做-科工力量</a></li>
<li><a href="http://www.ce.cn/xwzx/gnsz/gdxw/202607/t20260710_3080704.shtml">ce.cn/xwzx/gnsz/gdxw/202607/t20260710_3080704.shtml</a></li>

</ul>
</details>

**标签**: `#航天`, `#火箭回收`, `#中国航天`, `#长征十号乙`, `#网系回收`

---

<a id="item-4"></a>
## [OpenAI、谷歌通过新加坡向黑名单中国公司提供 AI](https://www.ft.com/content/5d6aafa1-5d47-4585-aa95-6ec06a6cd20f) ⭐️ 9.0/10

据《金融时报》报道，OpenAI 和谷歌一直在向阿里巴巴、百度和腾讯的新加坡子公司提供先进 AI 服务，而这三家公司的母公司均被列入五角大楼的 1260H 名单（中国军方关联实体清单）。 该报道揭示了美国 AI 出口管制的一个潜在漏洞——中国公司可通过海外子公司获取先进模型，这重新引发了要求加强监管的呼声，可能影响全球 AI 治理和国家安全。 OpenAI 最近在发现疑似“模型蒸馏”（一种将知识从大模型转移到小模型的技术）行为后，暂停了阿里巴巴关联用户的 API 访问权限。相比之下，Anthropic 采取了更严格的政策，全面禁止中国公司及其海外实体访问其前沿 AI 模型。

telegram · zaihuapd · 7月10日 09:59

**背景**: 1260H 名单根据《国防授权法》设立，列出据称与中国军方有关联的中国公司，并对其实施特定制裁。模型蒸馏是一种利用先进模型的输出来训练较小模型、使其性能接近大模型的技术。这些中国科技巨头通过新加坡子公司运营，可能规避了仅适用于中国大陆实体的出口限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1260H_list">1260H list</a></li>
<li><a href="https://www.wilmerhale.com/en/insights/client-alerts/20260611-pentagon-adds-65-new-entities-to-the-1260h-list-of-chinese-military-companies">Pentagon Adds 65 New Entities to the 1260H List of Chinese Military Companies</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#export controls`, `#OpenAI`, `#Google`, `#China`

---

<a id="item-5"></a>
## [sglang v0.5.15：Blackwell 与推测解码性能提升](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

sglang v0.5.15 发布了针对 Blackwell GPU 优化的 GLM-5.2 NVFP4 生产版本，在 8 块 B300 上达到 500+ tok/s/user，默认启用 Spec V2 实现端到端 TPS 提升 11%，并推出 IndexShare MTP 将 draft-step 成本降低最多 1.9 倍。 该版本显著提升了大型语言模型在 NVIDIA 最新 Blackwell GPU 上的推理吞吐量，并增强了推测解码效率，直接有利于延迟敏感的生产部署并降低运营成本。 关键优化包括针对 Blackwell 的 GEMM 路由器（含形状专用 JIT 和 CuteDSL BF16 内核）、面向 draft-model 图的 FlashInfer 自动调优，以及默认启用 breakable CUDA Graph。新增模型支持包括 Hunyuan 3、Qwen3.6 NVFP4 等。

github · Fridge003 · 7月10日 22:58

**背景**: sglang 是一个开源的大语言模型推理引擎。Blackwell 是 NVIDIA 最新的 GPU 架构，拥有 2080 亿晶体管并采用 4nm 工艺。NVFP4 是一种 4 位浮点量化格式。推测解码通过使用草稿模型预测多个令牌来加速生成；MTP（多令牌预测）是一种变体，其中主模型本身通过轻量级草稿头预测未来令牌。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/nvidia/GLM-5.2-NVFP4">nvidia/ GLM - 5 . 2 - NVFP 4 · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://docs.vllm.ai/en/stable/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>

</ul>
</details>

**标签**: `#sglang`, `#LLM inference`, `#GPU optimization`, `#speculative decoding`, `#release`

---

<a id="item-6"></a>
## [纽约市禁止欺骗性订阅行为](https://www.theguardian.com/us-news/2026/jul/10/new-york-city-deceptive-subscriptions-ban) ⭐️ 8.0/10

纽约市市长 Mamdani 宣布了一项具有里程碑意义的“一键取消”消费者保护规则，禁止欺骗性的订阅行为，并要求公司提供简单的取消选项。 这项规定通过让取消订阅与注册一样容易，加强了消费者权益，可能迫使公司提高透明度，并减少数百万居民不必要的扣费。 该规则专门针对“垃圾费用”和欺骗性自动续费行为，与加州法律不同，纽约市的规则据报不包含针对餐馆的豁免，这可能会堵住一个常见的漏洞。

hackernews · randycupertino · 7月10日 18:26 · [社区讨论](https://news.ycombinator.com/item?id=48863464)

**背景**: 订阅模式通常依赖使取消变得困难来留住客户，这种做法被称为“暗模式”。“一键取消”运动旨在要求取消方式与注册方式相同，防止公司强迫客户打电话或亲自到场取消。

**社区讨论**: 评论强调了对执法力度的怀疑，指出加州也有类似规定但存在餐馆豁免削弱效果。一些用户赞赏这项消费者保护，而另一些则分享了多次取消失败的个人经历，表明需要更强有力的执法。

**标签**: `#consumer protection`, `#subscriptions`, `#regulation`, `#NYC`, `#tech policy`

---

<a id="item-7"></a>
## [成功公司患上制度性失明](https://ianreppel.org/how-successful-companies-go-blind/) ⭐️ 8.0/10

Ian Reppel 的文章《成功公司如何变盲》指出，随着公司成功壮大，官僚惯性、风险规避和部门竖井导致制度性失明，抑制创新。 这种模式解释了为何许多行业领导者无法适应颠覆性变化，影响员工、投资者和整体经济。 文章强调，制度性失明并非能力问题，而是系统性问题；即使在厚重的官僚体制中，有才华的人也会变得无效。

hackernews · speckx · 7月10日 13:31 · [社区讨论](https://news.ycombinator.com/item?id=48859678)

**背景**: 制度性失明指组织因根深蒂固的流程和文化而忽视明显问题的倾向。官僚惯性是官僚机构延续既定程序的趋势，而部门竖井管理则指各部门孤立运作。这些因素共同压制创新，导致组织衰退。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.researchgate.net/publication/400224729_The_implications_of_organizational_blindness_on_employees_and_organizations_A_bibliometric_perspective">(PDF) The implications of organizational blindness on employees and organizations: A bibliometric perspective</a></li>
<li><a href="https://hrzone.com/glossary/what-is-bureaucratic-inertia/">What is Bureaucratic Inertia ? - HRZone</a></li>
<li><a href="https://procfopartners.com/insights/business-strategy/the-dangers-of-siloed-leadership/">The Dangers of Siloed Leadership - ProCFO</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了个人经历：一位来自老牌防务公司的评论者指出缺乏创新财务激励，另一位描述了长期任职但未提升技能的管理层导致停滞。第三位评论者认为这是情境问题而非能力问题，有才华的人在糟糕系统中也会变得无效。

**标签**: `#organizational behavior`, `#company culture`, `#innovation`, `#bureaucracy`, `#management`

---

<a id="item-8"></a>
## [为什么 ML 没有限制每位作者的投稿数量？](https://www.reddit.com/r/MachineLearning/comments/1usq43t/why_doesnt_the_ml_research_community_limit_the/) ⭐️ 8.0/10

一位 Reddit 用户指出，与安全（CCS）和计算机体系结构（DAC）等领域不同，机器学习研究社区没有限制每位作者的投稿数量，这加剧了审稿人过载以及在 ACL Rolling Review（ARR）等场合中观察到的质量问题。 实施每位作者的投稿数量限制可以减轻审稿负担，提高评审质量，并鼓励更深入、更有影响力的工作，而非大量投稿，从而有可能推动 ML 研究文化走向可持续。 发帖者指出，其他领域多年来已成功使用投稿限制，例如 CCS（安全）和 DAC（计算机体系结构）。这个问题凸显了 ML 中的文化差异，即尽管审稿系统压力日益增大，但无限投稿仍是常态。

reddit · r/MachineLearning · /u/alafaya101 · 7月10日 14:59

**背景**: 机器学习会议如 NeurIPS、ICML 和 ACL 的投稿数量激增，给同行评审过程带来了压力。ACL Rolling Review（ARR）是 NLP 领域的集中审稿平台，旨在简化评审流程但依然面临瓶颈。相比之下，其他一些计算机科学社区对每位作者设置投稿上限，以更均匀地分配工作量。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://aclrollingreview.org/">ACL Rolling Review – A peer review platform for the Association for Computational Linguistics</a></li>
<li><a href="https://2026.aclweb.org/calls/main_conference_papers/">Main Conference - ACL 2026</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#research community`, `#conference submissions`, `#review quality`, `#academic publishing`

---

<a id="item-9"></a>
## [马斯克盛赞 Anthropic，承诺 400 亿美元合同不中断服务](https://x.com/i/status/2075278580955685036) ⭐️ 8.0/10

埃隆·马斯克一改此前对 Anthropic 的批评，称其为当前 AI 领域的领导者，并承诺即使存在竞争也不会切断其服务。他透露 Anthropic 已成为 SpaceX 最大客户，签署了价值约 4000 亿美元的合同，租用整个 Colossus 1 数据中心。 这笔交易凸显了 AI 计算基础设施的巨大需求，以及马斯克的 xAI 与 Anthropic 之间尽管存在竞争却建立的战略关系。这标志着 AI 行业联盟的重大转变，以及训练前沿模型所需资本的巨大规模。 Anthropic 购买了 300 兆瓦的算力，包下了 xAI 位于田纳西州孟菲斯附近 Colossus 1 数据中心的全部产能，每月支付 12.5 亿美元直至 2029 年 5 月，总额约 4000 亿美元。马斯克还表示，目前没有其他公司推出过可与 Anthropic 的 Mythos/Fable 系列相比的模型。

telegram · zaihuapd · 7月10日 02:02

**背景**: Anthropic 是一家 AI 安全与研究公司，以开发 Claude 模型系列而闻名，包括先进的 Mythos 和 Fable 系列。Colossus 1 数据中心由 xAI（马斯克的 AI 公司）建造，拥有 22 万个 NVIDIA GPU，是世界上最强大的 AI 超级计算机之一。每月 12.5 亿美元的租赁费凸显了训练和运行尖端 AI 模型的极端成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/05/20/anthropic-will-pay-xai-1-25-billion-per-month-for-compute/">Anthropic will pay xAI $1.25B per month for compute</a></li>
<li><a href="https://www.buildmvpfast.com/blog/anthropic-xai-colossus-1-gpu-data-center-compute-deal-2026">Anthropic xAI Colossus 1 GPU Deal: 220K GPUs, 300 MW</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Elon Musk`, `#business`, `#contracts`

---

<a id="item-10"></a>
## [腾讯洽购 AI 公司 Manus，拟从 Meta 手中回购](https://www.reuters.com/technology/tencent-talks-become-ai-start-up-manus-largest-shareholder-ft-reports-2026-07-10/) ⭐️ 8.0/10

腾讯正在谈判收购 AI 初创公司 Manus，计划从 Meta 手中回购股份成为最大股东。此前，北京要求 Meta 放弃其对 Manus 的 20 亿美元收购交易。 这笔交易反映了中美在 AI 领域日益加剧的地缘政治紧张局势，并可能重塑全球 AI 初创企业的竞争格局。 腾讯将与现有投资者真格基金和 HSG 联手，以至少 20 亿美元的价格从 Meta 手中回购 Manus。该消息由《金融时报》率先报道，相关方均未置评。

telegram · zaihuapd · 7月10日 06:45

**背景**: Manus 是一家 AI 初创公司，吸引了 Meta 的兴趣，但中国的监管干预阻止了 Meta 的收购。如今，中国科技巨头腾讯介入收购，凸显了 AI 技术的战略重要性以及政府政策对跨境科技交易的影响。

**标签**: `#AI`, `#acquisitions`, `#Tencent`, `#Meta`, `#Manus`

---

<a id="item-11"></a>
## [欧盟因成瘾设计对 Meta 罚款 120 亿美元](https://www.theverge.com/policy/963872/meta-eu-addictive-design-200b-fine-risk-digital-services-act-dsa) ⭐️ 8.0/10

欧盟委员会初步认定，Meta 旗下的 Facebook 和 Instagram 因采用无限滚动、自动播放和个性化推荐等成瘾性设计，违反了《数字服务法》。Meta 可能面临高达 120 亿美元的罚款，约占其全球年营收的 6%。 这是欧盟根据《数字服务法》采取的最严厉监管行动之一，直接针对损害用户福祉的设计实践。它为平台责任开创了先例，可能迫使 Meta 及其他科技巨头从根本上重新设计核心功能以降低成瘾性。 欧盟批评 Meta 现有的限时工具形同虚设，要求默认关闭成瘾性功能、设置有效的屏幕休息时间，并弱化以参与度为导向的推荐算法。最终裁决可能要求 Meta 彻底重新设计其应用。

telegram · zaihuapd · 7月10日 14:47

**背景**: 《数字服务法》（DSA）是欧盟自 2022 年起生效的法规，对数字平台（尤其是拥有超过 4500 万欧盟用户的超大型在线平台）施加严格义务。成瘾性设计模式利用心理脆弱性驱动强迫性使用，导致用户花费过多时间或金钱。DSA 旨在保护用户免受此类有害行为侵害，并要求平台对其设计选择负责。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act">Digital Services Act</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/policies/digital-services-act">The Digital Services Act | Shaping Europe’s digital future</a></li>

</ul>
</details>

**标签**: `#Meta`, `#EU Regulation`, `#Digital Services Act`, `#Addictive Design`, `#Big Tech`

---

<a id="item-12"></a>
## [OpenAI 将 Codex 和 Atlas 整合进 ChatGPT 桌面应用](https://t.me/zaihuapd/42482) ⭐️ 8.0/10

OpenAI 发布了新版 ChatGPT 桌面应用，将 Codex、ChatGPT Work 智能体和浏览器功能整合到同一应用中。独立桌面浏览器 Atlas 将于 2025 年 8 月 9 日停止提供。 此次整合将代码辅助、网页浏览和 AI 智能体统一到一个工具中，简化了开发者工作流程，减少了上下文切换。这也表明 OpenAI 致力于构建综合性桌面平台，而非维持多个独立产品。 Chrome 用户仍可通过插件使用 ChatGPT 和 Codex，无需更换浏览器。新版桌面应用取代了早先独立的 Codex 应用和 Atlas 浏览器（后者是专为 macOS 推出的 ChatGPT 驱动浏览器）。

telegram · zaihuapd · 7月10日 19:51

**背景**: Codex 是 OpenAI 的 AI 编码智能体，帮助工程团队处理拉取请求、代码审查和自动化任务，包含在 ChatGPT Plus、Pro 等计划中。Atlas 是一款内置 ChatGPT 的独立桌面浏览器，用户可以直接在任何页面上获取摘要和智能网页帮助。将这些功能整合到 ChatGPT 桌面应用中，OpenAI 旨在为开发和一般网页任务提供统一体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-chatgpt-atlas/">Introducing ChatGPT Atlas - OpenAI</a></li>
<li><a href="https://developers.openai.com/codex/app">App – Codex | OpenAI Developers</a></li>
<li><a href="https://help.openai.com/en/articles/12628461-setting-up-the-atlas-browser">Setting up the Atlas browser - OpenAI Help Center</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#Codex`, `#desktop app`, `#integration`

---