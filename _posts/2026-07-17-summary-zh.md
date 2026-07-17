---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> 从 33 条内容中筛选出 10 条重要资讯。

---

1. [Firefox 被编译为 WebAssembly 并在浏览器中运行](#item-1) ⭐️ 9.0/10
2. [首次在宜居带岩石系外行星发现大气层](#item-2) ⭐️ 8.0/10
3. [Kimi K3 与鹈鹕基准测试：揭示分词不一致性](#item-3) ⭐️ 8.0/10
4. [开源 AI 崛起威胁闭源模型主导地位](#item-4) ⭐️ 8.0/10
5. [AI 提交与 AI 评委破坏 Kaggle 竞赛公正性](#item-5) ⭐️ 8.0/10
6. [Stereo2Spatial：开源扩散模型实现立体声转双耳空间音频](#item-6) ⭐️ 8.0/10
7. [Truth Social 将向华尔街销售特朗普帖子的快速访问权限](#item-7) ⭐️ 8.0/10
8. [特斯拉 Cybercab 在北美启动量产](#item-8) ⭐️ 8.0/10
9. [华为昇腾 950 超节点首次亮相，自称算力达英伟达 6.7 倍](#item-9) ⭐️ 8.0/10
10. [美议员推动禁止中国存储芯片进入盟友供应链](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Firefox 被编译为 WebAssembly 并在浏览器中运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter 将整个 Firefox 浏览器（包括 Gecko 引擎）编译为 WebAssembly，使其能够在 Chrome 等另一个浏览器中运行。该项目使用 Claude Opus 和 Fable 模型进行 AI 辅助开发，预估消耗了价值 25,000 美元的 token，但借助订阅计划实际成本大幅降低。 这是一项突破性的技术成就，展示了 WebAssembly 在运行复杂、全尺寸应用（而非简单游戏或工具）方面日益增强的能力。它可能催生新的浏览器虚拟化、边缘计算和安全测试形式，并凸显了 AI 辅助编程在应对大规模移植项目上的潜力。 编译后的 Firefox 使用 Wisp 协议将所有网络流量通过 Puter 的服务器代理到 WebSocket 上，因为基于浏览器的代码无法直接打开任意 TCP/UDP 连接。该演示对 HTTPS 流量实现了端到端加密，gecko.wasm 二进制文件大小为 233MB。

rss · Simon Willison · 7月16日 23:34

**背景**: WebAssembly (Wasm) 是一种可移植的二进制格式，能在浏览器中高性能地执行代码，最初设计用于补充 JavaScript。Wisp 协议是一种轻量级协议，用于在单个 WebSocket 连接上代理多个 TCP 和 UDP 套接字。Firefox 的 Gecko 引擎因其强大的单进程支持而被选中，这简化了移植到 Wasm 的过程。Claude Fable 是 Anthropic 近期推出的、用于代码生成任务的 AI 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**标签**: `#WebAssembly`, `#Firefox`, `#Browser Virtualization`, `#AI-Assisted Development`, `#Technical Feat`

---

<a id="item-2"></a>
## [首次在宜居带岩石系外行星发现大气层](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

首次在距离 48 光年的红矮星宜居带内岩石系外行星 LHS 1140b 上探测到大气层。该探测利用 JWST 的发射光谱仪，在行星经过恒星后方时进行分析。 这标志着系外行星大气层表征的里程碑，此前对类地行星的大气探测非常有限。但由于红矮星强烈的恒星活动可能逐步剥蚀大气，该行星的“类地”性质仍存在争议。 LHS 1140b 是超级地球，质量约为地球的 5.6 倍，半径大 70%，每 24.7 天绕恒星一周。探测到的气体是氦气，对于小行星而言不寻常，曾引发该行星可能是处于沸腾状态的迷你海王星的猜测，但本次研究的 JWST 数据排除了这一假设。

hackernews · neversaydie · 7月17日 14:06 · [社区讨论](https://news.ycombinator.com/item?id=48947560)

**背景**: 系外行星大气探测通常使用掩星光谱法，分析穿过行星大气层的星光。红矮星因温度较低且宜居带很近，其强烈的耀斑活动可能剥蚀行星大气，对宜居性构成挑战。LHS 1140b 于 2017 年由 MEarth 项目发现，一直是宜居性研究的关键目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140">LHS 1140 - Wikipedia</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - Science@NASA</a></li>

</ul>
</details>

**社区讨论**: 评论围绕“类地”标签展开争议：有用户认为红矮星活动使大气留存极不可能，但另一用户引用 arXiv 预印本指出 JWST 光谱已排除迷你海王星。其他用户讨论了未来探测器的推进方式，并指出探测到的氦气暗示该行星可能并非真正的类地行星。

**标签**: `#exoplanet`, `#atmosphere`, `#astronomy`, `#JWST`, `#red dwarf`

---

<a id="item-3"></a>
## [Kimi K3 与鹈鹕基准测试：揭示分词不一致性](https://simonwillison.net/2026/Jul/16/kimi-k3/) ⭐️ 8.0/10

Simon Willison 分析了 Kimi K3 在鹈鹕基准测试上的表现，发现分词不一致性：提示语'生成一只骑自行车的鹈鹕的 SVG'在 Kimi K3 中占用 95 个令牌，而在 OpenAI 的分词器中仅 10 个。他主张应评估模型的代理工具调用能力，而非静态图像生成。 这一讨论揭示了当前 LLM 评估实践中的关键局限性：基准测试结果可能因分词问题而失真。它推动社区转向更现实的评估方式，例如多轮代理工具调用，这更能反映实际使用场景。 鹈鹕基准测试要求生成骑自行车的鹈鹕的 SVG，但 Simon 指出该测试未涉及代理能力。社区成员注意到 Kimi K3 异常高的令牌数暗示存在 85 个令牌的隐藏系统提示，可能用于推理努力。

hackernews · droidjj · 7月17日 14:21 · [社区讨论](https://news.ycombinator.com/item?id=48947717)

**背景**: 鹈鹕基准测试由 Simon Willison 于 2024 年底创建，是一个非正式测试，用于比较 LLM 从简单提示生成 SVG 代码的能力。分词是将文本拆分为令牌的过程；不同模型可能对相同文本有不同分词方式，影响令牌计数和潜在性能。Kimi K3 是 Moonshot AI 发布的 2.8 万亿参数开放权重模型，支持 100 万令牌上下文窗口，专为长程编码和知识工作设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openlm.ai/kimi-k3/">Kimi K3 - openlm.ai</a></li>
<li><a href="https://grokipedia.com/page/Pelican_on_a_bicycle_AI_benchmark">Pelican on a bicycle (AI benchmark)</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>

</ul>
</details>

**社区讨论**: 社区评论引发了数据污染担忧（OsrsNeedsf2P），指出了分词异常和可能的隐藏系统提示（devttyeu），并提出将代理任务与鹈鹕式中断相结合的新基准（btown）。其他人分享了成本/速度比较（michaelbuckbee）和替代性 SVG 基准测试（ianberdin）。

**标签**: `#LLM`, `#benchmark`, `#tokenization`, `#AI evaluation`, `#Kimi K3`

---

<a id="item-4"></a>
## [开源 AI 崛起威胁闭源模型主导地位](https://stateofopensource.ai/) ⭐️ 8.0/10

Mozilla 的一份新报告及社区数据显示，开源 AI 模型市场份额迅速增长，在 OpenRouter 上，开源模型日处理量从四个月前的 8880 亿个 token 增至现在的 4.19 万亿个 token。 这一转变可能威胁 OpenAI 和 Anthropic 等闭源 AI 公司，因为开源模型更具成本效益且被广泛采用，有望重塑 AI 行业格局。 报告指出，超大规模云服务商可以无许可费地运行开源模型，而苹果等公司可将其优化用于设备端部署，但同时前沿闭源模型训练和维护成本依然高昂。

hackernews · rellem · 7月17日 14:31 · [社区讨论](https://news.ycombinator.com/item?id=48947825)

**背景**: 开源 AI 模型以宽松许可证公开提供，允许任何人使用、修改和分发。这与闭源模型形成对比，后者底层代码和权重是专有的。市场份额变化通过 OpenRouter 等平台追踪，该平台聚合了各种模型的 API 使用情况。

**社区讨论**: 社区评论显示普遍认为开源模型正在超越闭源模型，用户 GodelNumbering 提供数据显示开源模型 token 处理量四个月内增长了 5 倍。部分用户批评报告由 AI 生成且缺乏实质内容，而另一些人则认为开源模型成本优势将使闭源模型过时。

**标签**: `#open source`, `#AI`, `#machine learning`, `#LLM`, `#industry trends`

---

<a id="item-5"></a>
## [AI 提交与 AI 评委破坏 Kaggle 竞赛公正性](https://www.kaggle.com/competitions/kaggle-measuring-agi/discussion/724918#3498423) ⭐️ 8.0/10

Kaggle 上一个高赞讨论揭示了大量证据，表明 AI 生成的提交和基于 AI 的评判正在损害平台竞赛的公平性和完整性。 这破坏了 Kaggle 作为 AI/ML 技能基准的信任，可能贬低竞赛结果的价值，并阻碍真正的人类参与。 社区成员报告称参与者将思考过程外包给 AI，且 AI 评委可能被操纵，例如通过提示注入来宣布获胜者。

hackernews · twerkmeister · 7月17日 11:30 · [社区讨论](https://news.ycombinator.com/item?id=48946010)

**背景**: Kaggle 是谷歌旗下的数据科学竞赛平台，参与者构建模型以解决实际问题。传统上，人类技能和模型透明度受到重视，但大语言模型的兴起使得完全由 AI 生成的流程成为可能。该平台本身也在尝试 AI 评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kaggle">Kaggle - Wikipedia</a></li>
<li><a href="https://www.kaggle.com/">Kaggle: The World's AI Proving Ground</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了对 AI 破坏公平竞争的沮丧；有人指出暴力方法一直存在，但 AI 放大了问题。对 Kaggle 的声誉以及竞赛是否曾产生可靠研究表示怀疑。

**标签**: `#AI`, `#Machine Learning`, `#Kaggle`, `#Competition Integrity`, `#Ethics`

---

<a id="item-6"></a>
## [Stereo2Spatial：开源扩散模型实现立体声转双耳空间音频](https://www.reddit.com/r/MachineLearning/comments/1uzevbg/stereo2spatial_convert_stereo_music_tracks_to/) ⭐️ 8.0/10

开发者发布了 Stereo2Spatial，这是一个流匹配扩散模型，可将立体声音乐转换为空间化双耳混音，并附带 Windows 桌面应用和训练/推理代码，采用 Apache 2.0 许可证。 该项目解决了现有立体声音乐缺乏高质量空间混音的问题，提供了一个开源工具，使消费者和创作者无需昂贵的多声道设备即可进行空间音频创作，从而推动空间音频的普及。 该模型最初使用基于 EAR-VAE 的潜在空间方法，但为了修复质量问题转而采用原始波形建模，并借鉴 WavFlow 论文中的振幅提升技术来稳定训练。模型在 2 块 A6000 GPU 上训练了 20 天，使用了 7,669 首曲目。

reddit · r/MachineLearning · /u/kittenkrazy · 7月17日 22:55

**背景**: 空间音频再现三维声场，提供沉浸感；双耳音频通过头相关传输函数在耳机上模拟这种效果。变分自编码器将音频压缩到紧凑的潜在空间，而流匹配扩散模型通过学习从噪声到数据的连续变换来生成高质量样本。振幅提升技术将音频信号缩放到固定的 RMS 级别，以避免训练不稳定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Eps-Acoustic-Revolution-Lab/EAR_VAE">Eps-Acoustic-Revolution-Lab/EAR_VAE - GitHub</a></li>
<li><a href="https://arxiv.org/abs/2601.12950">[2601.12950] ImmersiveFlow: Stereo-to-7.1.4 spatial audio ... ImmersiveFlow: Stereo-to-7.1.4 spatial audio generation with ... ImmersiveFlow: Stereo-to-7.1.4 spatial audio generation with ... Xuzhou Ye - catalyzex.com Figure 3 from ImmersiveFlow: Stereo-to-7.1.4 spatial audio ... ImmersiveFlow: Stereo-to-7.1.4 spatial audio generation with ...</a></li>

</ul>
</details>

**标签**: `#Machine Learning`, `#Audio Processing`, `#Spatial Audio`, `#Diffusion Models`, `#VAE`

---

<a id="item-7"></a>
## [Truth Social 将向华尔街销售特朗普帖子的快速访问权限](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

特朗普媒体科技集团宣布推出 Truth API，这是一个付费数据订阅服务，从 8 月 1 日起向机构客户提供 Truth Social 上排名前十账号的实时帖子，访问速度为毫秒级。 此举直接将总统的社交媒体活动与高频交易挂钩，引发了对市场操纵和利益冲突的担忧，因为特朗普经常使用 Truth Social 宣布政策决定和宣传股票。 该 API 专门针对算法交易者，为其提供信息优势；定价尚未公开。特朗普关于关税、伊朗和霍尔木兹海峡的帖子此前曾多次引发股市和油市剧烈波动。

telegram · zaihuapd · 7月17日 01:02

**背景**: Truth Social 是美国前总统唐纳德·特朗普创立的社交媒体平台。高频交易利用算法在毫秒级时间内基于市场数据执行交易。API（应用程序编程接口）允许软件实时通信和访问数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hindustantimes.com/world-news/us-news/trump-media-launches-truth-api-to-give-banks-faster-access-to-truth-social-posts-101784225959242.html">Trump Media launches Truth API to give banks... | Hindustan Times</a></li>

</ul>
</details>

**标签**: `#Truth Social`, `#API`, `#high-frequency trading`, `#market manipulation`, `#politics`

---

<a id="item-8"></a>
## [特斯拉 Cybercab 在北美启动量产](https://t.me/zaihuapd/42621) ⭐️ 8.0/10

特斯拉已于 2026 年 2 月在北美工厂启动 Cybercab 的量产，这款全自动驾驶电动车取消了方向盘和踏板。 这标志着自动驾驶汽车部署的重要里程碑，使特斯拉更接近推出 Robotaxi 服务，并可能改变城市交通方式。 Cybercab 是一款专为无人驾驶设计的双座车，完全依赖特斯拉的 FSD 系统进行行驶控制。

telegram · zaihuapd · 7月17日 03:06

**背景**: 特斯拉 Cybercab 于 2024 年 10 月首次以概念车形式亮相，当时有 20 辆原型车为参会者提供短途试乘。该车旨在成为特斯拉 Robotaxi 网络的一部分，这是一个车主可以部署用于网约车的自动驾驶车队。车辆取消了方向盘和踏板等传统控制装置，强调其全自动驾驶设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Cybercab">Tesla Cybercab - Wikipedia</a></li>
<li><a href="https://www.bbc.com/news/articles/cm29x5ke9jdo">Tesla robotaxi: Cybercab unveiled by Elon Musk</a></li>
<li><a href="https://www.tesla.com/robotaxi">Robotaxi - Tesla</a></li>

</ul>
</details>

**标签**: `#autonomous driving`, `#Tesla`, `#electric vehicles`, `#Robotaxi`

---

<a id="item-9"></a>
## [华为昇腾 950 超节点首次亮相，自称算力达英伟达 6.7 倍](https://www.ithome.com/0/978/019.htm) ⭐️ 8.0/10

华为在 2026 世界人工智能大会上首次公开亮相昇腾 950 超节点，声称其总算力达到英伟达 NVL144 系统的 6.7 倍，该设备支持 1024 卡集群，提供 1 EFLOPS FP8 和 2 EFLOPS FP4 算力。 这可能显著改变 AI 硬件格局，为中国提供英伟达主导地位的国产替代方案，有望加速 AI 发展并减少对外国芯片的依赖。 该超节点采用华为自研的灵衢互联协议和超节点架构，实现 1024 卡规模和 256 TB 全局统一内存，并在 FP8 和 FP4 精度级别上给出了具体的算力数据。

telegram · zaihuapd · 7月17日 10:27

**背景**: 超节点（SuperPoD）是一种构建大规模 AI 算力集群的架构，最早由英伟达提出，通过高速互联将多个计算节点紧密耦合形成一个逻辑上的单一系统。华为的灵衢协议专为这种大规模场景设计，旨在与英伟达的 NVLink 竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nbd.com.cn/articles/2025-09-18/4065524.html">突破大规模超节点 互 联 技术 华 为 发布 互 联 协 议 “ 灵 衢 ” | 每经网</a></li>
<li><a href="https://baike.baidu.com/item/超节点/67393838">超节点（构建大规模算力集群的技术架构）_百度百科</a></li>
<li><a href="https://server.it168.com/a2025/1017/6901/000006901416.shtml">灵 衢 ： 华 为 重构算力底座的“超级 协 议 ”-服务器专区</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#Huawei`, `#Ascend`, `#SuperPoD`, `#Compute Comparison`

---

<a id="item-10"></a>
## [美议员推动禁止中国存储芯片进入盟友供应链](https://www.tomshardware.com/pc-components/dram/lawmakers-want-us-government-to-ban-memory-chips-from-china-even-in-allied-supply-chains-citing-unacceptable-risk-to-national-economic-and-supply-chain-security) ⭐️ 8.0/10

美国众议院中国委员会主席 John Moolenaar 和议员 George Whitesides 致信商务部长 Howard Lutnick，要求禁止美国公司采购中国存储芯片，并将长鑫存储（CXMT）列入实体清单，对长江存储（YMTC）施加额外限制。 如果实施，这将扰乱全球半导体供应链，尤其影响依赖存储芯片的 AI 基础设施，并可能迫使西方与中国存储供应商进行战略性脱钩。 议员们指出，苹果等美国科技公司正寻求采购中国存储芯片，采购可能资助解放军军民两用技术发展。他们还敦促与日本、韩国和欧盟协调，防止中国制造商在盟友供应链中扎根。

telegram · zaihuapd · 7月17日 14:00

**背景**: 长鑫存储（CXMT）是一家总部位于安徽合肥的中国 DRAM 制造商。长江存储（YMTC）是一家中国 NAND 闪存生产商。两者都曾受美国出口限制，被认为是中国半导体自给自足的关键。美国实体清单限制向被视为国家安全风险的中国实体出口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.mofcom.gov.cn/zwgk/zcfb/art/2025/art_e4f474d3aeba4672913db1042d845d78.html">不可靠 实 体 清 单 工作机制关于将斯凯迪奥公司等11...</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#geopolitics`, `#supply chain`, `#AI hardware`, `#trade policy`

---