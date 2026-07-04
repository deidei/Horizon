---
layout: default
title: "Horizon Summary: 2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> 从 47 条内容中筛选出 8 条重要资讯。

---

1. [欧盟议会间谍软件调查员遭 Pegasus 黑客攻击](#item-1) ⭐️ 9.0/10
2. [PostgreSQL 与 OOM 杀手：为何使用严格内存过量提交](#item-2) ⭐️ 8.0/10
3. [CDD 仅从 LLM 逻辑值恢复微调数据原文](#item-3) ⭐️ 8.0/10
4. [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](#item-4) ⭐️ 8.0/10
5. [华为发布搭载昇腾 950PR 的 Atlas 350 AI 加速卡](#item-5) ⭐️ 8.0/10
6. [阿里巴巴下令全员卸载 Claude 产品](#item-6) ⭐️ 8.0/10
7. [NASA 发射救援卫星拯救垂危的雨燕望远镜](#item-7) ⭐️ 8.0/10
8. [腾讯玄武阿图因 AI 在 CyberGym 测试中超越 Mythos](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [欧盟议会间谍软件调查员遭 Pegasus 黑客攻击](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 9.0/10

公民实验室发现，欧洲议会间谍软件调查委员会的一名成员的 iPhone 在 2022 年 10 月和 2023 年 3 月两次被 Pegasus 间谍软件感染。 这一突破表明，间谍软件正被用于对付调查者本人，暗示了跨多个欧盟国家的授权，并危及敏感信息。它引发了关于欧洲议会内部监控主权和设备安全政策的紧迫问题。 第一次感染与针对俄罗斯和白俄罗斯流亡记者的 Pegasus 行动重叠，暗示存在获得多国授权的客户。被感染的手机同时包含个人医疗信息和政府机密文件，凸显了工作和个人设备缺乏隔离的问题。

hackernews · ledoge · 7月3日 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: Pegasus 是以色列 NSO 集团开发的商业间谍软件，被政府用于秘密监控记者和活动人士等目标。公民实验室是一个网络安全监督机构，曝光了多起 Pegasus 感染事件。欧洲议会设有调查成员国间谍软件滥用的委员会。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://therecord.media/international-spyware-agreement-new-members">Finland, Germany, Ireland, Japan, Poland, South Korea added to US-led spyware agreement | The Record from Recorded Future News</a></li>

</ul>
</details>

**社区讨论**: 评论者强调了希腊、波兰和意大利持续的间谍软件丑闻，有人认为这次黑客攻击是希腊国内行动而非针对欧盟议会的攻击。其他人指出多个欧盟国家曾使用 Pegasus，并对议会的设备隔离政策提出质疑。

**标签**: `#Pegasus`, `#spyware`, `#cybersecurity`, `#European Parliament`, `#espionage`

---

<a id="item-2"></a>
## [PostgreSQL 与 OOM 杀手：为何使用严格内存过量提交](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud 发布了一篇博客文章，解释了他们为何对 PostgreSQL 使用严格内存过量提交（vm.overcommit_memory=2），以避免 OOM 杀手问题，并提升大规模数据库的可靠性。 这意义重大，因为许多 PostgreSQL 运维人员在默认启发式过量提交下会因 OOM 杀手遭遇不稳定，而严格过量提交为生产环境提供了一个经过验证的替代方案。 严格过量提交（模式 2）会拒绝超出可用内存的内存分配，这可以防止 OOM 杀手事件，但若未仔细调整可能导致 fork 失败；文章建议在部署前进行彻底测试。

hackernews · furkansahin · 7月3日 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48774509)

**背景**: Linux 内存过量提交有三种模式：启发式（0）、始终（1）和严格（2）。默认的启发式模式允许进程基于内部启发式过量提交内存，但在内存压力下，OOM 杀手可能会杀死进程（包括 PostgreSQL），导致可靠性问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@amerather_9719/how-linux-kernel-manages-application-memory-27c23ac94177">How Linux Kernel Manages Application Memory | by Amer... | Medium</a></li>
<li><a href="https://kernel-internals.org/mm/overcommit/">Memory Overcommit - Linux Kernel Internals</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-03-02-optimize-memory-vm-swappiness-overcommit-ubuntu/view">How to Optimize Memory (vm.swappiness, overcommit ) on Ubuntu</a></li>

</ul>
</details>

**社区讨论**: 评论提醒，虽然严格过量提交避免了 OOM 杀手，但可能阻止 fork()调用，需要仔细测试，特别是在调整过量提交比例时。一位评论者分享了在 Go 应用程序与 PostgreSQL 一起分配虚拟内存时遇到的问题。

**标签**: `#PostgreSQL`, `#Linux memory management`, `#OOM killer`, `#database reliability`, `#sysadmin`

---

<a id="item-3"></a>
## [CDD 仅从 LLM 逻辑值恢复微调数据原文](https://www.reddit.com/r/MachineLearning/comments/1umn2dk/contrastive_decoding_diffing_cdd_recovering/) ⭐️ 8.0/10

对比解码差分（CDD）仅通过灰盒逻辑值访问，无需模型权重或激活，就能从窄微调的大型语言模型中恢复原文内容。在四个模型家族的 20 个生物体×模型对中，有 19 个达到了 4/5 以上的原文恢复评分。 该方法显著推进了模型差分和安全领域，因为它无需白盒访问就能从 LLM 中提取精确的微调数据。它还揭示了一个意外的数据污染问题：来自合成数据生成的虚构科学家角色在不同微调领域中反复出现。 CDD 直接对比基座模型和微调模型的逻辑值，使用单一默认配置，无需逐物种校准或层选择。先前的白盒方法——激活差异透镜（ADL）——在同等基准测试中从未超过 3/5 的恢复评分，尽管它需要完全的权重访问。

reddit · r/MachineLearning · /u/CebulkaZapiekana · 7月3日 19:01

**背景**: 模型差分旨在揭示 LLM 版本或微调模型之间的系统性行为差异。近期研究表明，微调会在基座模型和微调模型的激活差异中留下可检测的痕迹，但该方法需要完整的权重访问。对比解码是一种通过对比不同模型输出来选择令牌的技术，而 CDD 则将该思想应用于恢复训练数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2602.10371">Simple LLM Baselines are Competitive for Model Diffing</a></li>
<li><a href="https://aiwiki.ai/wiki/contrastive_decoding">Contrastive decoding | AI Wiki</a></li>
<li><a href="https://www.geeksforgeeks.org/nlp/contrastive-decoding-in-natural-language-processing/">Contrastive Decoding in Natural Language... - GeeksforGeeks</a></li>

</ul>
</details>

**标签**: `#LLM security`, `#model diffing`, `#contrastive decoding`, `#machine learning`, `#finetuning`

---

<a id="item-4"></a>
## [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic 致信美国参议院银行委员会，指控阿里巴巴策划了迄今为止已知最大规模的“蒸馏攻击”，利用近 2.5 万个欺诈账户，在 2026 年 4 月 22 日至 6 月 5 日期间与 Claude 进行了超过 2880 万次交互。 这一事件凸显了通过蒸馏攻击窃取模型这一日益严重的威胁，可能削弱 AI 公司的知识产权和竞争优势，并可能促使整个行业采取更严格的监管和防御措施。 Anthropic 表示，此次攻击涉及阿里巴巴的 AI 实验室 Qwen，是针对该公司规模最大的此类攻击，检测工作揭示了这些欺诈账户和巨大的交互量。蒸馏技术允许较弱的模型通过学习较强模型的输出来模仿其能力。

telegram · zaihuapd · 7月3日 06:21

**背景**: 模型蒸馏是一种技术，通过训练较小、能力较弱的模型来复制较大、更强大模型的行为。蒸馏攻击是指对手滥用公共 API 在未经授权的情况下收集这些训练数据。Anthropic 开发了检测和预防此类攻击的方法，但强调需要全行业合作才能大规模解决这个问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI security`, `#model distillation`, `#intellectual property`, `#Anthropic`, `#Alibaba`

---

<a id="item-5"></a>
## [华为发布搭载昇腾 950PR 的 Atlas 350 AI 加速卡](https://t.me/zaihuapd/42329) ⭐️ 8.0/10

在华为中国合作伙伴大会 2026 上，华为正式发布并上市了搭载全新昇腾 950PR 处理器的 AI 推理加速卡 Atlas 350，声称其单卡算力达到英伟达 H20 的 2.87 倍，并且是国内首款支持 FP4 低精度推理的加速卡。 这一发布增强了华为在 AI 加速卡市场（尤其是推理工作负载）的地位，并在贸易限制持续的情况下为中国市场提供了英伟达产品的替代方案。FP4 支持可显著降低大语言模型的模型大小和延迟。 Atlas 350 配备 112 GB HBM 内存，采用华为自研高带宽内存，支持单卡加载 70B 参数模型，MXFP4 精度下算力达 2 PFLOPS。与前代相比，该卡提升了向量算力和 2.5 倍的互联带宽。

telegram · zaihuapd · 7月3日 08:35

**背景**: FP4 是一种 4 位浮点精度格式，通过减少内存占用和计算量来加速 AI 推理，同时保持可接受的精度。昇腾 950PR 是华为最新的 AI 处理器，针对推理和推荐任务进行了优化，其 CANN 框架现已实现超过 95%的 CUDA 代码兼容性，便于从英伟达平台迁移。H20 是英伟达为符合美国出口管制而设计的一款面向中国市场的低端 GPU。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eetrend.com/content/2025/100594934.html">华 为 昇 腾 950 /960/970炸裂发布！ 还首发了自研HBM内存！ 昇 腾 950 ...</a></li>
<li><a href="https://www.omniyq.com/sys-nd/500.html">昇 腾 950 ：国产算力的一个里程碑 - 云擎天下-超高性价比AI算力服务平台</a></li>
<li><a href="https://www.cfi.cn/p20260421002039.html">DeepSeek启动首轮外部融资 有望助推国产算力生态全面铺开- CFi.CN...</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#AI accelerator`, `#hardware`, `#deep learning`, `#inference`

---

<a id="item-6"></a>
## [阿里巴巴下令全员卸载 Claude 产品](https://t.me/zaihuapd/42334) ⭐️ 8.0/10

阿里巴巴内部下令要求所有员工立即卸载 Anthropic 的 Claude 产品，包括 Sonnet、Opus、Fable 等模型以及 Claude Code 智能体工具，禁令于 7 月 10 日生效。此前 Anthropic 指控阿里在 4 月 22 日至 6 月 5 日期间使用约 2.5 万个虚假账号与 Claude 进行了超过 2800 万次交互。 这一事件凸显了中国大型科技公司与西方 AI 提供商在使用政策和安全方面日益紧张的局势。它可能导致企业内部对 AI 的管控更加严格，并影响中国公司获取先进 AI 模型的方式。 阿里巴巴此前曾报销员工使用 Claude、GPT、Gemini 等外部模型的费用。禁令不仅涵盖聊天模型，还包括 Claude Code 这类基于终端的 AI 编程助手智能体产品。

telegram · zaihuapd · 7月3日 13:00

**背景**: Claude 是由美国 AI 公司 Anthropic 开发的一系列大语言模型，其模型从 Haiku 到 Fable 能力递增、成本逐级上升。阿里巴巴被指控利用虚假账户绕过使用限制，促使 Anthropic 加强了风控策略，进而引发了此次内部禁令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://claude.com/resources/tutorials/choosing-the-right-claude-model">Choosing the right Claude model : Haiku, Sonnet , Opus , or Fable</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>

</ul>
</details>

**标签**: `#Alibaba`, `#Claude`, `#Anthropic`, `#enterprise AI`, `#security`

---

<a id="item-7"></a>
## [NASA 发射救援卫星拯救垂危的雨燕望远镜](https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a) ⭐️ 8.0/10

此次任务展示了商业卫星维护能力，可延长昂贵太空资产的寿命并减缓太空碎片问题，有望彻底改变老化卫星的管理方式。 LINK 航天器将用机械臂抓住雨燕，然后通过推进器将其抬升约 240 公里，最快可使雨燕于 9 月恢复观测，并将其运行寿命延长至 2026 年以后。

telegram · zaihuapd · 7月3日 15:43

**背景**: 轨道衰变是指卫星因大气阻力（尤其在太阳活动高峰期）逐渐降低轨道的过程。雨燕天文台于 2004 年发射，用于研究伽马射线暴，目前高度持续下降；若不干预，最快可能在 2025 年 10 月坠入大气层烧毁。利用机械臂进行卫星维护是一个新兴领域，DARPA 和商业公司正在开发在轨维修、加油和重新定位的技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a">Rescue mission is launched to save an aging NASA telescope ...</a></li>
<li><a href="https://www.reuters.com/business/aerospace-defense/space-startup-katalyst-launches-orbital-rescue-mission-aging-nasa-observatory-2026-07-03/">Space startup Katalyst launches orbital rescue mission for ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Swift_rescue_mission">Swift Boost Mission - Wikipedia</a></li>

</ul>
</details>

**标签**: `#space`, `#NASA`, `#satellite rescue`, `#astronomy`

---

<a id="item-8"></a>
## [腾讯玄武阿图因 AI 在 CyberGym 测试中超越 Mythos](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 8.0/10

腾讯玄武实验室宣布，其阿图因 AI 在加州大学伯克利分校主导的 CyberGym 网络安全基准测试中获得 84.0%的得分，超越 Anthropic 的 Claude Mythos Preview。该工具基于开源模型 GLM-5.1 构建，消耗的预算不到 Mythos 的 0.1%。 这一成就表明，低成本的开源 AI 模型可以在真实漏洞发现中超越强大的专有模型，可能使先进的网络安全能力更加普及。同时，它也凸显了 AI 在自动漏洞分析领域的重大进展。 阿图因 AI 在 curl、gnark、OpenSSL、Python cryptography、Java bc-java 等项目中发现了多个 Mythos 未检出的高危逻辑漏洞，最高评分达 9.3。在伯克利 BVI 真实世界漏洞榜单中，阿图因 AI 的严重漏洞严重程度排名第一，总数排名第五。

telegram · zaihuapd · 7月3日 16:12

**背景**: CyberGym 是一个大规模网络安全基准测试，用于评估 AI 代理在真实漏洞分析任务上的表现，包含来自 188 个开源项目的 1,507 个历史漏洞。Claude Mythos 是 Anthropic 开发的先进但未公开发布的 AI 模型，以其漏洞发现能力著称，后来推出了公开版本 Claude Fable 5。GLM-5.1 是智谱 AI（Z.AI）发布的开源语言模型，采用 MIT 许可证，专为长时间自主任务设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cybergym.io/cybergym/">CyberGym: Evaluating AI Agents' Real-World Cybersecurity ...</a></li>
<li><a href="https://arxiv.org/abs/2506.02548">[2506.02548] CyberGym: Evaluating AI Agents' Real-World ... CyberGym Leaderboard - llm-stats.com CyberGym Benchmark 2026: 9 model averages | BenchLM.ai Defense at AI speed: Microsoft’s new multi-model agentic ... CyberGym-E2E: Scalable Real-World Benchmark for AI Agents ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>

</ul>
</details>

**标签**: `#网络安全`, `#AI`, `#漏洞挖掘`, `#基准测试`

---