---
layout: default
title: "Horizon Summary: 2026-07-08 (ZH)"
date: 2026-07-08
lang: zh
---

> 从 41 条内容中筛选出 14 条重要资讯。

---

1. [中国五年投入 2 万亿元建设全国算力网络](#item-1) ⭐️ 9.0/10
2. [潜伏 16 年的 KVM 漏洞允许虚拟机逃逸至宿主机](#item-2) ⭐️ 9.0/10
3. [中国拟限制顶尖 AI 模型出口](#item-3) ⭐️ 9.0/10
4. [Kokoro：可在 CPU 上运行的高质量文本转语音模型](#item-4) ⭐️ 8.0/10
5. [欧盟聊天控制提案：大规模监控加密信息](#item-5) ⭐️ 8.0/10
6. [欧盟强制新车安装驾驶员监控摄像头](#item-6) ⭐️ 8.0/10
7. [高技能人才为何离开德国](#item-7) ⭐️ 8.0/10
8. [微软裁掉 id Software 的 idTech 团队](#item-8) ⭐️ 8.0/10
9. [sqlite-utils 4.0 引入数据库模式迁移等新功能](#item-9) ⭐️ 8.0/10
10. [MIRA：为火箭联盟训练的 50 亿参数多人世界模型](#item-10) ⭐️ 8.0/10
11. [将微调约束到可信 LoRA 子空间可防止投毒攻击](#item-11) ⭐️ 8.0/10
12. [Anthropic 发布 Claude Sonnet 5，代理能力大幅提升](#item-12) ⭐️ 8.0/10
13. [英伟达 Blackwell 晶圆美国造，但需在台湾封装](#item-13) ⭐️ 8.0/10
14. [DeepSeek 自研 AI 推理芯片](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [中国五年投入 2 万亿元建设全国算力网络](https://t.me/zaihuapd/42399) ⭐️ 9.0/10

中国宣布计划在未来五年投入约 2 万亿元（2950 亿美元），建设全国互联数据中心网络，优先采用华为等本土 AI 芯片，目标占比不低于 80%，以减少对英伟达、AMD 等美企的依赖。 这是全球最大规模的计算基础设施投资之一，将重塑 AI 硬件供应链，加速中国技术自主，并可能对全球芯片市场产生深远影响。 该网络是中国“六网”基础设施计划的关键一环，由国有电信企业运营。中国电信、联通等已推出 token 套餐，将算力像移动数据一样打包销售。

telegram · zaihuapd · 7月7日 04:45

**背景**: 中国在第十五五规划中提出了“六网”基础设施计划，包括算力网络、卫星互联网、5G-Advanced/6G 等。算力网络旨在整合分散的计算资源，使企业和公共部门更易获得高性能计算。此外，中国已推出计算力 token，将绿色能源转化的计算能力标准化，降低 AI 应用成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.digitimes.com/news/a20260616VL212/infrastructure-technology-industrial-communications-water.html">China's six-network plan signals a long-term infrastructure and technology self-reliance push</a></li>
<li><a href="https://www.scmp.com/tech/big-tech/article/3353891/china-ramps-building-national-computing-power-network-ai-token-demand-surges">China ramps up building a national computing power network as AI token demand surges | South China Morning Post</a></li>
<li><a href="https://english.news.cn/20260522/74806708cbd64cd5adfaa1a8527f5ec7/c.html">China races to industrialize computing power with token factory, consumer token plans -Xinhua</a></li>

</ul>
</details>

**标签**: `#computing infrastructure`, `#AI chips`, `#China tech policy`, `#Huawei`, `#semiconductor`

---

<a id="item-2"></a>
## [潜伏 16 年的 KVM 漏洞允许虚拟机逃逸至宿主机](https://github.com/V4bel/Januscape) ⭐️ 9.0/10

安全研究人员公开了 Januscape（CVE-2026-53359），这是一个潜伏 16 年的 KVM/x86 漏洞，可以在 Intel 和 AMD 平台上实现虚拟机逃逸。概念验证（PoC）漏洞利用代码已发布，该漏洞此前曾被用作 Google kvmCTF 竞赛的 0-day 攻击。 这是首个已知的同时影响 Intel 和 AMD 系统的 KVM 虚拟机逃逸漏洞，对多租户云环境构成严重威胁。该漏洞打破了客户虚拟机与宿主机之间的隔离边界，可能允许攻击者攻陷整个宿主机及其他虚拟机。 该漏洞是 shadow MMU 模拟中的 use-after-free 缺陷，客户机可以通过内部操作破坏宿主机内核的 shadow page 表。在 RHEL 等发行版中，本地普通用户也可以利用该漏洞将权限提升至 root。

telegram · zaihuapd · 7月7日 10:14

**背景**: KVM 是基于内核的虚拟机，是 Linux 内核模块，允许宿主机运行多个虚拟机。Shadow MMU 负责在没有或无法使用硬件虚拟化支持（如 Intel EPT 或 AMD NPT）时为客户虚拟机管理页表。Use-after-free 漏洞发生在程序释放内存对象后仍继续使用该对象，可能导致内存损坏和任意代码执行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html">16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host on Intel and AMD x86 Systems</a></li>
<li><a href="https://securityaffairs.com/194868/security/januscape-16-year-old-linux-kvm-bug-enables-cloud-vm-escape-attacks.html">Januscape: 16-Year-Old Linux KVM Bug Enables Cloud VM Escape Attacks</a></li>
<li><a href="https://gbhackers.com/16-year-old-januscape-kvm-escape-vulnerability/">16-Year-Old Januscape KVM Escape Vulnerability Lets Attackers Compromise Linux Hosts</a></li>

</ul>
</details>

**标签**: `#security`, `#virtualization`, `#KVM`, `#vulnerability`, `#cloud`

---

<a id="item-3"></a>
## [中国拟限制顶尖 AI 模型出口](https://www.reuters.com/world/beijing-is-looking-curbing-overseas-access-chinas-top-ai-models-sources-say-2026-07-07/) ⭐️ 9.0/10

中国商务部已召集阿里巴巴、字节跳动及智谱等企业，讨论限制最先进的国产 AI 模型向海外提供访问，包括尚未发布的模型，并可能将技术泄露纳入刑事犯罪。 这标志着全球 AI 政策可能发生重大转变，将影响中国主要 AI 公司及国际领先 AI 模型的可得性，对 AI 产业和地缘政治具有深远影响。 限制范围可能仅适用于未来发布的新模型，目前仍在商讨中，尚未最终确定。会议还考虑限制境外资本投资国内 AI 初创企业。

telegram · zaihuapd · 7月7日 11:42

**背景**: AI 模型出口管制是更广泛国家安全措施的一部分。中国一直在开发先进的 AI 模型，如阿里巴巴的通义千问和字节跳动的豆包，政府日益关注技术泄露和地缘政治竞争。

**标签**: `#AI policy`, `#national security`, `#China`, `#export controls`, `#AI models`

---

<a id="item-4"></a>
## [Kokoro：可在 CPU 上运行的高质量文本转语音模型](https://ariya.io/2026/03/local-cpu-friendly-high-quality-tts-text-to-speech-with-kokoro/) ⭐️ 8.0/10

Kokoro 是一个开源的文本转语音（TTS）模型，拥有 8200 万个参数，可在 CPU 上高效运行，无需 GPU 即可实现高质量语音合成。 这对没有专用 GPU 的用户来说意义重大，使得高质量本地 TTS 可用于无障碍工具、播客生成等场景，推动了语音合成的普及。 Kokoro 支持 IPA 发音指南以纠正同形异义词，并已被集成到 Chrome 扩展中，用于朗读网页并高亮显示句子。

hackernews · speckx · 7月7日 18:24 · [社区讨论](https://news.ycombinator.com/item?id=48821576)

**背景**: 文本转语音（TTS）将书面文本转换为语音音频。许多高质量的 TTS 模型需要强大的 GPU，限制了其可及性。Kokoro 是一个轻量级模型（8200 万个参数），针对 CPU 推理进行了优化，适用于日常硬件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kokorottsai.com/">Kokoro TTS: Advanced AI Text-to-Speech Model with 82M parameters</a></li>
<li><a href="https://grokipedia.com/page/Kokoro_TTS">Kokoro TTS</a></li>

</ul>
</details>

**社区讨论**: 社区反馈非常积极，用户称赞 Kokoro 的 CPU 友好性和无障碍应用场景。一些人指出其在单字发音上的不足，并建议改进同形异义词的处理。有用户分享了一个 Chrome 扩展，以简化在网页上的使用。

**标签**: `#text-to-speech`, `#machine learning`, `#accessibility`, `#CPU`, `#open source`

---

<a id="item-5"></a>
## [欧盟聊天控制提案：大规模监控加密信息](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 8.0/10

欧盟的“聊天控制”提案（1.0 和 2.0）要求科技公司在用户设备上扫描所有私人消息以查找儿童性虐待材料，这实际上破坏了端到端加密。该计划因促成大规模监控而遭到隐私倡导者和技术专家的广泛批评。 如果实施，“聊天控制”将强制要求客户端扫描，破坏欧盟所有加密通信的安全性和隐私。这为大规模监控树立了危险先例，可能严重损害对数字通信和软件工程实践的信任。 “聊天控制 1.0”提供了《电子隐私指令》的临时豁免，允许自愿扫描，但已于 2024 年到期；然而 Meta、谷歌和微软等公司宣布将继续扫描。“聊天控制 2.0”则提议强制扫描所有消息，包括加密消息，无需授权或怀疑。

hackernews · gasull · 7月7日 14:23 · [社区讨论](https://news.ycombinator.com/item?id=48818311)

**背景**: 端到端加密（E2EE）确保只有发送者和接收者能阅读消息内容。客户端扫描（CSS）在用户设备上对消息进行扫描，在加密前（或解密后）与已知的儿童性虐待材料哈希数据库比对，而不向服务提供商透露内容——但实际上，它可以被绕过或扩展到扫描其他内容，带来隐私风险。欧盟的“聊天控制”提案旨在打击网络上的儿童性虐待，但被技术专家和人权组织广泛批评为大规模监控的一种形式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Regulation_to_Prevent_and_Combat_Child_Sexual_Abuse">Chat Control - Wikipedia</a></li>
<li><a href="https://www.eff.org/deeplinks/2026/04/eu-parliament-blocks-mass-scanning-our-chats-whats-next">EU Parliament Blocks Mass-Scanning of Our Chats—What's Next? | Electronic Frontier Foundation</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control: The EU's CSAM scanner proposal</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍反对该提案，认为这是一项以儿童保护为幌子的广泛监控工具。一位用户指出，虽然每个人都想阻止虐待儿童，但该法律过于宽泛，会影响所有用户。另一位指出欧盟声称保护隐私却推动这一监控的讽刺之处，还有一位提到欧洲议会甚至阻止了一个反对“聊天控制”的政党。

**标签**: `#privacy`, `#encryption`, `#surveillance`, `#EU legislation`, `#CSAM`

---

<a id="item-6"></a>
## [欧盟强制新车安装驾驶员监控摄像头](https://allaboutcookies.org/eu-mandatory-distracted-driver-system) ⭐️ 8.0/10

欧盟强制要求所有新售车辆必须配备驾驶员监控摄像头系统，以检测和预防分心驾驶行为。 这项规定将影响欧盟所有新车，可能减少因分心导致的事故，但也引发了驾驶员对隐私和用户体验的严重担忧。 该系统通常使用安装在转向柱上的红外摄像头，以高频率追踪驾驶员的面部和眼部运动，并可与其他安全功能（如车道保持辅助）集成。

hackernews · nickslaughter02 · 7月7日 20:50 · [社区讨论](https://news.ycombinator.com/item?id=48823557)

**背景**: 驾驶员监控系统（DMS）是一种高级驾驶辅助系统（ADAS），通过摄像头和传感器监测驾驶员的警觉状态，能够检测疲劳、分心或受损迹象。欧盟的强制要求与全球范围内新车强制配备 DMS 的趋势一致，类似法规在其他地区也已推行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Driver_monitoring_system">Driver monitoring system - Wikipedia</a></li>
<li><a href="https://www.edmunds.com/car-technology/driver-monitoring-system.html">Driver Monitoring Systems | Edmunds</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示出支持与批评并存。一些用户称赞福特 Blue Cruise 等系统的准确性，能有效捕捉分心行为；另一些用户则抱怨恼人的蜂鸣声、侵入性的用户体验（如沃尔沃的车道辅助）以及类似波音报警问题引发的隐私担忧。

**标签**: `#EU regulation`, `#driver monitoring`, `#privacy`, `#automotive`, `#safety`

---

<a id="item-7"></a>
## [高技能人才为何离开德国](https://www.dw.com/en/germany-migrants-skilled-workers-integration-labor-market-bureaucracy-language-housing/a-77853162) ⭐️ 8.0/10

一篇文章及 Hacker News 上的讨论揭示了高技能人才离开德国的原因，主要涉及官僚主义、文化融入困难和职业发展受限。 这之所以重要，是因为德国面临技能人才短缺问题，流失外国人才会削弱其经济竞争力和融合努力。 社区评论指出了具体问题：官僚主义效率低下、基础设施差、文化排外以及晋升机会缺乏，尤其是对不在跨国公司工作的人而言。

hackernews · theanonymousone · 7月7日 10:42 · [社区讨论](https://news.ycombinator.com/item?id=48815982)

**背景**: 德国为应对人口和劳动力短缺，积极从国外招募高技能人才。然而，由于签证流程复杂、语言障碍以及保守的社会文化，留住人才一直面临挑战。相关讨论反映了关于外籍人士融入和职业流动性的更广泛辩论。

**社区讨论**: 评论者分享了个人经历，感到不受欢迎且职业发展受限。一些人指出基础设施恶化、官僚主义等系统性问题，另一些人则分享了成功案例，但强调融入过程漫长。

**标签**: `#immigration`, `#skilled workers`, `#Germany`, `#career mobility`, `#culture`

---

<a id="item-8"></a>
## [微软裁掉 id Software 的 idTech 团队](https://gamefromscratch.com/microsoft-fire-idtech-team-at-id-software/) ⭐️ 8.0/10

微软裁掉了 id Software 的整个 idTech 引擎开发团队，实质性地停止了该专有游戏引擎的内部开发。 此举可能迫使未来 id Software 的游戏依赖虚幻引擎等第三方引擎，减少引擎多样性，并可能削弱 id 游戏独特的技术特色。 此次裁员是微软游戏部门更大规模裁员的一部分，但微软或 id Software 尚未官方确认。idTech 引擎曾驱动《毁灭战士》和《雷神之锤》等经典系列。

hackernews · bauc · 7月7日 15:33 · [社区讨论](https://news.ycombinator.com/item?id=48819244)

**背景**: idTech 是 id Software 开发的专有游戏引擎，以率先采用实时射线投射和虚拟纹理等先进图形技术而闻名。微软于 2021 年通过收购 ZeniMax Media 获得了 id Software。游戏引擎是游戏开发的基础工具，维护专有引擎需要内部拥有专业化技术人才。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech">id Tech - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech_5">id Tech 5 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech_6">id Tech 6 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论中既有批评也有怀疑。一些人认为微软为了成本效益牺牲了技术独特性，可能强化 Epic Games 的引擎垄断。另一些人则质疑 idTech 团队是否真的被裁，指出文章缺乏直接证据。

**标签**: `#Microsoft`, `#id Software`, `#game engines`, `#layoffs`, `#game development`

---

<a id="item-9"></a>
## [sqlite-utils 4.0 引入数据库模式迁移等新功能](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0 已发布，新增数据库模式迁移、通过新 `db.atomic()` 方法实现的嵌套事务以及对复合外键的支持。这是自 2020 年 11 月 3.0 以来首次重大版本更新。 此次更新响应了开发者长期以来的需求，为这个广泛使用的 SQLite Python 库增加了模式迁移支持，让数据库变更管理更加便捷。嵌套事务和复合外键的添加进一步提升了库在处理复杂数据库操作时的实用性。 迁移通过 Python 文件使用 `Migrations` 类和 `table.transform()` 方法定义，该方法实现了 SQLite 推荐的重新创建表模式，从而允许高级模式更改。库的 `migrate` 命令会应用未完成的迁移，并在专用表中记录它们。

rss · Simon Willison · 7月7日 19:32

**背景**: sqlite-utils 是一个用于操作 SQLite 数据库的 Python 库和命令行工具，由 Simon Willison 创建。模式迁移是一种对数据库模式进行版本控制和增量更改的方法，对于不断演进的应用程序非常重要。在 4.0 之前，用户需要手动处理模式更改，通常使用原生 SQL 或外部迁移工具。

**标签**: `#sqlite-utils`, `#SQLite`, `#Python`, `#schema migrations`, `#database`

---

<a id="item-10"></a>
## [MIRA：为火箭联盟训练的 50 亿参数多人世界模型](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 8.0/10

General Intuition、Kyutai 与 Epic Games 的研究人员发布了 MIRA，这是一个在 10,000 小时合成火箭联盟游戏数据上训练的 50 亿参数多人世界模型，可在单个 NVIDIA B200 GPU 上以 20fps 支持 4 名玩家运行，同时发布了可玩演示、技术论文和 1000 小时数据集。 MIRA 代表了向多智能体环境中大规模交互式世界模型迈出的重要一步，能够实时模拟和规划复杂游戏。其开源发布（代码、演示、数据集）加速了世界模型、强化学习和游戏 AI 的研究，潜在应用远超游戏领域。 该模型拥有 50 亿参数，在 NVIDIA B200 GPU 上可实现四名玩家 20 帧每秒的运行速度。它使用从火箭联盟回放生成的合成数据进行训练，发布的数据集包含 1000 小时的四人游戏数据。

reddit · r/MachineLearning · /u/MasterScrat · 7月7日 07:59

**背景**: 世界模型是一种机器学习系统，学习环境的内部表示并预测其如何响应动作而演变，使智能体无需持续与现实交互即可进行规划和推理。火箭联盟是一款基于物理的高速多人游戏，为多智能体世界模型提供了具有挑战性的试验场。MIRA 建立在交互式视频生成和世界模型的前期工作之上，但解决了多个交互智能体的额外复杂性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence)</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/world-models/">What Is a World Model? | NVIDIA Glossary</a></li>
<li><a href="https://www.notboring.co/p/world-models">World Models: Computing the Uncomputable</a></li>

</ul>
</details>

**标签**: `#world models`, `#multi-agent`, `#reinforcement learning`, `#game AI`, `#Rocket League`

---

<a id="item-11"></a>
## [将微调约束到可信 LoRA 子空间可防止投毒攻击](https://www.reddit.com/r/MachineLearning/comments/1uq68li/what_if_a_model_could_only_learn_what_trusted/) ⭐️ 8.0/10

一篇新论文提出将微调限制在从可信 LoRA 适配器学习的子空间中，使得某些恶意更新在几何上不可达。 这种防御方法通过从根本上限制模型可以学习的内容，而不是检测攻击，来应对微调中日益增长的投毒威胁。它可以保护个性化助手和用户适配模型等应用免受隐藏后门的影响。 该方法在 196 个公开的 LoRA 适配器上进行了测试，包括专门为绕过防御而设计的自适应攻击，结果显示攻击成功率显著下降，同时在覆盖的任务上保留了有用的适应能力。

reddit · r/MachineLearning · /u/Bright_Warning_8406 · 7月7日 20:00

**背景**: LoRA（低秩适应）是一种通过向现有权重添加轻量级低秩矩阵来微调大型模型的技术，避免了完全重新训练。该论文提出将微调更新限制在由可信 LoRA 适配器池张成的子空间中，使得新的适应必须是已验证行为的组合。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LoRA_(machine_learning)">LoRA (machine learning) - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/lora">What is LoRA (Low-Rank Adaption)? | IBM</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#AI safety`, `#fine-tuning`, `#LoRA`, `#adversarial defense`

---

<a id="item-12"></a>
## [Anthropic 发布 Claude Sonnet 5，代理能力大幅提升](https://t.me/zaihuapd/42404) ⭐️ 8.0/10

Anthropic 发布了 Claude Sonnet 5，这是迄今为止代理能力最强的 Sonnet 模型，能够规划、使用浏览器和终端等工具并自主运行。它在推理、工具使用、编码和知识工作方面优于 Sonnet 4.6，性能接近 Opus 4.8，但价格更低。 此次发布使先进的代理式 AI 能力更加普及和实惠，有望加速在自动化、软件开发和科研等领域的应用。同时也加剧了 AI 模型市场的竞争，尤其是与 GPT-4 和 Gemini 等模型的竞争。 Claude Sonnet 5 即日起在所有套餐中可用，并成为 Free 和 Pro 等级的默认模型。定价为每百万输入 token 2 美元，限时优惠截至 2026 年 8 月 31 日，使其对高使用量场景更具成本效益。

telegram · zaihuapd · 7月7日 09:02

**背景**: Anthropic 的 Claude 模型系列包括 Sonnet（中等规模、平衡型）和 Opus（大规模、高性能）。代理能力指模型能自主规划并使用浏览器和代码终端等外部工具执行任务，模拟人机交互。

**标签**: `#AI`, `#Claude`, `#Anthropic`, `#model release`, `#agent`

---

<a id="item-13"></a>
## [英伟达 Blackwell 晶圆美国造，但需在台湾封装](https://www.tomshardware.com/tech-industry/nvidia-and-intel-tout-chips-built-in-america-but-every-arizona-made-blackwell-die-is-still-packaged-in-taiwan) ⭐️ 8.0/10

英伟达的 Blackwell 晶圆现已在台积电亚利桑那州 Fab 21 工厂使用定制 4NP 工艺量产，但生产出的晶粒仍需运往 7000 英里外的台湾进行先进 CoWoS-L 封装。 这凸显了美国芯片制造对台湾先进封装的持续依赖，揭示了美国本土封装基础设施的缺口及其对供应链韧性的战略影响。 晶圆采用台积电为英伟达定制的 4NP 工艺节点，封装步骤包括切割、堆叠和 CoWoS-L 集成。美国目前没有量产或封装 HBM 的设施，完整的本土供应链预计最早要到 2028–2029 年才能形成。

telegram · zaihuapd · 7月7日 09:47

**背景**: 先进封装（如台积电的 CoWoS-L）对 Blackwell 等高性能 AI 芯片至关重要，因为它能将多个芯片（如 GPU 和 HBM 内存）集成到单个封装中，实现高密度互连。美国专注于推进逻辑芯片制造，但在封装产能方面落后，导致依赖亚洲供应链。Amkor、台积电和 SK 海力士等公司正在美国建设封装厂，但尚未投产。

**标签**: `#semiconductor`, `#nvidia`, `#supply chain`, `#geopolitics`

---

<a id="item-14"></a>
## [DeepSeek 自研 AI 推理芯片](https://www.reuters.com/world/china/chinas-deepseek-developing-its-own-ai-chip-sources-say-2026-07-07/) ⭐️ 8.0/10

据三位知情人士透露，中国 AI 公司 DeepSeek 正在自研 AI 推理芯片，以减少对英伟达和华为芯片的依赖。该项目始于约一年前，目前仍处于早期阶段。 此举意义重大，可能减少 DeepSeek 受美国出口管制的风险，并重塑中国 AI 硬件格局。若成功，可能激励其他中国 AI 公司寻求芯片自主。 该芯片专注于推理而非训练，即用于运行已训练模型以响应用户查询。DeepSeek 已开始与芯片设计、代工和存储公司接洽，近几个月来私下大量招募芯片设计工程师。

telegram · zaihuapd · 7月7日 11:08

**背景**: DeepSeek 此前依赖英伟达 H800 和华为昇腾芯片运行其模型。美国出口管制限制了中国获取先进 AI 芯片，促使国内企业开发替代品。创始人梁文锋在 2024 年一次罕见采访中承认芯片管制构成挑战。

**标签**: `#AI chips`, `#DeepSeek`, `#China`, `#semiconductor`, `#inference`

---