---
layout: default
title: "Horizon Summary: 2026-07-20 (ZH)"
date: 2026-07-20
lang: zh
---

> 从 34 条内容中筛选出 13 条重要资讯。

---

1. [山姆·奥特曼泄露邮件揭示 OpenAI 计划发布本地 GPT-3 模型](#item-1) ⭐️ 9.0/10
2. [Hugging Face 披露 AI 智能体攻击，商业大模型拒绝协助取证](#item-2) ⭐️ 9.0/10
3. [Fastjson 1.x 曝无 gadget 高危 RCE 漏洞](#item-3) ⭐️ 9.0/10
4. [中国开放权重 AI 模型正在超越美国专有模型](#item-4) ⭐️ 8.0/10
5. [黑客清除罗马尼亚土地登记数据库](#item-5) ⭐️ 8.0/10
6. [测量 arXiv 上 AI 写作比例：2026 年达 39%](#item-6) ⭐️ 8.0/10
7. [完美不等于过度工程化](#item-7) ⭐️ 8.0/10
8. [AI 模型竞赛：Kimi K3、Qwen 3.8 与 Anthropic 的困境](#item-8) ⭐️ 8.0/10
9. [本·汤普森提议美国立法促进开放 AI 模型竞争](#item-9) ⭐️ 8.0/10
10. [特朗普政府或限制美企使用中国开放权重 AI 模型](#item-10) ⭐️ 8.0/10
11. [研究：三分之二美军应用含中俄代码](#item-11) ⭐️ 8.0/10
12. [欧盟拟以生物识别数据换取美免签](#item-12) ⭐️ 8.0/10
13. [智谱建成 1 吉瓦全国产芯片数据中心](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [山姆·奥特曼泄露邮件揭示 OpenAI 计划发布本地 GPT-3 模型](https://simonwillison.net/2026/Jul/20/sam-altman/#atom-everything) ⭐️ 9.0/10

2022 年 10 月 1 日，山姆·奥特曼在给 OpenAI 董事会的邮件中（该邮件在马斯克诉奥特曼案中被曝光）透露，OpenAI 计划发布一个可在消费级硬件上本地运行的 GPT-3 级语言模型，以抢占先机、阻止竞争对手，并增加新 AI 项目获得融资的难度。 这一爆料罕见地揭示了 OpenAI 的开源策略和竞争手段，引发了关于将开源发布作为防御性措施以抑制竞争而非造福公众的伦理质疑。 邮件明确表示，目的是‘阻止他人发布类似强大模型’并‘增加新项目获得融资的难度’，将本地发布定位为针对 Stability AI 等竞争对手的战略举措。

rss · Simon Willison · 7月20日 03:47

**背景**: 随着模型量化技术和 llama.cpp 等工具的发展，在消费级硬件上运行大型语言模型已变得越来越可行。量化通过降低模型精度来减少内存和计算需求，使得 GPT-3 级别的 LLaMA 等模型能够在笔记本电脑、手机甚至树莓派上运行。到 2024 年底，多个开源模型和框架已使本地 LLM 推理变得实用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arstechnica.com/information-technology/2023/03/you-can-now-run-a-gpt-3-level-ai-model-on-your-laptop-phone-and-raspberry-pi/">You can now run a GPT-3-level AI model on your laptop, phone, and Raspberry Pi - Ars Technica</a></li>
<li><a href="https://www.aimagicx.com/blog/on-device-ai-models-local-llm-guide-2026?trk=article-ssr-frontend-pulse_little-text-block">On-Device AI in 2026: Running LLMs Locally on Your... | AI Magicx</a></li>
<li><a href="https://newsletter.maartengrootendorst.com/p/a-visual-guide-to-quantization">A Visual Guide to Quantization - by Maarten Grootendorst</a></li>

</ul>
</details>

**标签**: `#ai-ethics`, `#sam-altman`, `#generative-ai`, `#open-source`, `#openai`

---

<a id="item-2"></a>
## [Hugging Face 披露 AI 智能体攻击，商业大模型拒绝协助取证](https://huggingface.co/blog/security-incident-july-2026) ⭐️ 9.0/10

Hugging Face 披露了 2026 年 7 月发生的一起安全事件，攻击者利用数据集处理流程中的两处代码执行漏洞，由自主 AI 智能体框架驱动，在周末期间入侵内部系统，窃取了部分内部数据集和服务凭证，并在多个内部集群间横向移动。 该事件揭示了一种新型的 AI 驱动网络攻击，并展现了商业大模型可能因安全护栏拒绝协助取证分析，迫使组织依赖本地开源模型如 GLM 5.2，凸显了 AI 安全与事件响应方面的新挑战。 攻击在周末期间执行了数万次操作，但 Hugging Face 确认面向公众的模型、数据集和 Spaces 未被篡改，软件供应链无异常。响应过程中，团队最初使用商业大模型 API 进行日志分析，但被安全护栏拦截；后改用本地部署的 GLM 5.2，成功分析了超过 1.7 万条攻击记录。

telegram · zaihuapd · 7月20日 10:41

**背景**: AI 智能体框架是允许自主智能体使用大语言模型执行任务和决策的系统，可能被武器化用于恶意目的。GLM 5.2 是由 Z.ai（原智谱 AI）开发的开源大语言模型，拥有 744B 总参数、40B 活跃参数、1M token 上下文窗口，在长周期任务上表现优异。商业大模型 API 的安全护栏旨在防止滥用，但也可能无意中阻止合法的取证活动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_5.2">GLM 5.2</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.2">zai-org/GLM-5.2 · Hugging Face</a></li>
<li><a href="https://juejin.cn/post/7514260735943065600">推荐当前流行的12个 AI 智 能 体 框 架 关于 AI ...</a></li>

</ul>
</details>

**标签**: `#网络安全`, `#AI安全`, `#Hugging Face`, `#大模型`, `#安全事件`

---

<a id="item-3"></a>
## [Fastjson 1.x 曝无 gadget 高危 RCE 漏洞](https://x.com/k_firsov/status/2078872293745570032) ⭐️ 9.0/10

Fastjson 1.x 版本 1.2.68 至 1.2.83 被曝存在高危远程代码执行漏洞，无需开启 autoTypeSupport 或依赖 classpath gadget 链即可利用。由于 Fastjson 1.x 已于 2024 年 10 月停止维护，官方极大概率不会发布安全补丁，唯一补救措施是升级至 Fastjson2 或启用 SafeMode。 该漏洞极其严重，因为 Fastjson 是 Java 应用中广泛使用的 JSON 库，且漏洞在多个 JDK 版本上均可利用，无需典型前提条件。使用受影响版本的组织必须立即迁移或应用缓解措施，以防远程代码执行攻击。 该漏洞无需开启 autoTypeSupport 或依赖 classpath 上的特定 gadget 类，且已在 JDK 8、17 和 21 上确认可利用。Fastjson 1.x 已于 2024 年 10 月生命周期结束，因此官方不会发布补丁；用户必须升级至 Fastjson2，或通过 JVM 参数或配置文件启用 SafeMode。

telegram · zaihuapd · 7月20日 14:32

**背景**: Fastjson 是阿里巴巴开发的 Java 高性能 JSON 库，广泛用于 Web 应用。反序列化漏洞常利用“gadget 链”——一系列类在反序列化时执行任意代码。Fastjson 的 autoTypeSupport 功能允许多态反序列化，但也是常见攻击向量；SafeMode 于 1.2.68 版本引入，可完全禁用 autoType。此漏洞的特别之处在于无需任何 gadget 链即可利用，因此更易被攻击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson/wiki/fastjson_safemode_en">fastjson _ safemode _en · alibaba/ fastjson Wiki · GitHub</a></li>
<li><a href="https://topic.alibabacloud.com/a/com-alibaba-fastjson-jsonexception-autotype-is-not-support-_1_27_32615398.html">Com. alibaba. fastjson . JSONException: autoType is not support</a></li>
<li><a href="https://www.huaweicloud.com/eu/notice/20220523153626935.html">Fastjson <= 1.2.80 Deserialization Remote Code Execution...</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#RCE`, `#Fastjson`, `#Java`

---

<a id="item-4"></a>
## [中国开放权重 AI 模型正在超越美国专有模型](https://werd.io/american-ai-is-locked-down-and-proprietary-its-losing/) ⭐️ 8.0/10

一篇文章指出，中国的开放权重 AI 模型由于成本更低、可及性更广，正在获得相对于美国专有模型的竞争优势，并在社区中引发高关注度。 这一趋势可能重塑全球 AI 格局，使强大的 AI 更实惠、更易获取，特别是对初创企业和发展中国家，同时挑战 OpenAI 和 Anthropic 等美国专有 AI 公司的主导地位。 中国的开放权重模型并非完全开源，但允许自由下载和微调，与基于 API 的专有模型相比成本更低。文章称 80%的初创企业现在使用中国模型，但评论中对此有争议。

hackernews · benwerd · 7月20日 14:21 · [社区讨论](https://news.ycombinator.com/item?id=48979269)

**背景**: 开放权重模型是指那些最终训练好的权重被公开发布的 AI 模型，允许任何人下载并在自己的基础设施上运行和定制。这与 GPT-4 或 Claude 等专有模型形成对比，这些模型只能通过付费 API 和严格的使用限制来访问。开放权重方法由 Meta 的 Llama 系列推广，但中国的 DeepSeek、阿里巴巴等模型正变得越来越有竞争力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>

</ul>
</details>

**社区讨论**: 评论普遍同意开放权重将超越专有模型，并类比历史上的转变如 PC vs 大型机或 Linux vs UNIX。但有人对‘80%的初创企业使用中国模型’的具体说法表示怀疑，指出他们亲身体验中使用的是美国模型，还有人指出开放权重并非真正的开源，限制了一些自由。

**标签**: `#AI`, `#Open Source`, `#China`, `#Large Language Models`, `#Industry Trends`

---

<a id="item-5"></a>
## [黑客清除罗马尼亚土地登记数据库](https://news.risky.biz/risky-bulletin-hacker-wipes-romanias-entire-land-registry-database/) ⭐️ 8.0/10

一名黑客清除了罗马尼亚的整个土地登记数据库，但离线备份可能减轻了损害；该机构正在迁移到政府云。 这一事件本可能因无法证明土地所有权而导致严重的社会混乱，凸显了关键基础设施面对网络攻击的脆弱性。 黑客被确认为来自阿尔及利亚的 Zakaria Mahdjoub，声称已删除备份，但据称该机构有离线副本。迁移到罗马尼亚政府云的工作正在进行中。

hackernews · speckx · 7月20日 13:28 · [社区讨论](https://news.ycombinator.com/item?id=48978605)

**背景**: 土地登记是政府记录财产所有权和边界的数据库，对房地产交易和法律纠纷至关重要。清空此类数据库可能会在房地产市场和法律体系中造成混乱。

**社区讨论**: 评论指出，离线备份可能防止了重大混乱，并推测 IT 合同中的腐败导致了漏洞。黑客的身份以及阿尔及利亚与罗马尼亚的引渡条约也被讨论。

**标签**: `#cybersecurity`, `#data breach`, `#critical infrastructure`, `#Romania`, `#hacker`

---

<a id="item-6"></a>
## [测量 arXiv 上 AI 写作比例：2026 年达 39%](https://unslop.run/blog/measuring-ai-writing-on-arxiv) ⭐️ 8.0/10

一项使用校准后的 AI 检测器对 arXiv 论文的分析发现，到 2026 年 1 月，所有论文中多达 39%、计算机科学论文中 65%被标记为 AI 写作，而数学论文仍接近 0.7%。 这揭示了自 ChatGPT 以来学术写作中 AI 辅助使用的急剧增加，引发了对检测方法可靠性及科学文献诚信度的担忧。 该检测器特意调校以避免误报，ChatGPT 之前的误报率仅为 0.4%，当论文的机器写作概率超过 42%时即被标记。

hackernews · dopamine_daddy · 7月20日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=48981206)

**背景**: arXiv 是一个广泛使用的科学论文预印本库，涵盖物理学、计算机科学、数学及相关领域。AI 文本检测器（如 GPTZero）利用统计和神经方法来识别大语言模型生成的文本，但其准确性仍存争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">arXiv - Wikipedia</a></li>
<li><a href="https://chromewebstore.google.com/detail/gptzero-ai-detection-writ/kgobeoibakoahbfnlficpmibdbkdchap">GPTZero: AI Detection & Writing Replay - Chrome Web Store</a></li>
<li><a href="https://www.emergentmind.com/topics/ai-text-detectors">AI Text Detectors : Methods & Challenges</a></li>

</ul>
</details>

**社区讨论**: 评论者对检测准确性表示怀疑；一位用户上传了自己 2016 年前的论文，却得到 27%-74%的 AI 评分，暗示可能存在误报。另一位则指出企业中 LLM 使用的博弈论动态：领导层鼓励 AI 生成的代码，尽管其质量影响尚不明确。

**标签**: `#AI writing detection`, `#arXiv`, `#academic integrity`, `#machine learning`, `#community discussion`

---

<a id="item-7"></a>
## [完美不等于过度工程化](https://var0.xyz/posts/perfection-is-not-over-engineering.html) ⭐️ 8.0/10

一位软件工程师认为，追求设计上的完美与过度工程化是不同的，不应被劝阻。 这种 nuanced 的观点有助于开发者区分严谨与浪费，鼓励更好的软件工艺。 作者指出，完美需要严格的需求；没有明确目标，就会沦为过度工程化。

hackernews · var0xyz · 7月20日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48979120)

**背景**: 在软件工程中，常有一句谚语“不要让完美成为优秀的敌人”，通常用来劝阻过度工程化。本文挑战了这一观点，区分了完美主义和过度工程化。

**社区讨论**: 评论者观点多样：一些人认为“完美与优秀”的对比被滥用，另一些人则提醒完美主义会导致自行车棚效应和情感包袱。有评论者指出，过度工程化通常是为不存在的约束进行优化。

**标签**: `#software engineering`, `#over-engineering`, `#perfectionism`, `#design philosophy`, `#development practices`

---

<a id="item-8"></a>
## [AI 模型竞赛：Kimi K3、Qwen 3.8 与 Anthropic 的困境](https://www.emergingtrajectories.com/lh/frontier-lab-economics/) ⭐️ 8.0/10

这些发布加剧了开源权重模型与专有模型之间的竞争，并引发了对 AI 能力是否接近瓶颈的讨论。社区还在探讨 ASIC 芯片如何改变 AI 经济，以及 Anthropic 的争议是否会威胁其市场地位。 Kimi K3 拥有 100 万 token 上下文窗口，专为长周期编程和知识工作设计。Qwen 3.8 是阿里巴巴 Qwen 模型家族的新成员，已在 Hugging Face 上发布。Anthropic 的 CPO 在 Claude Design 发布前数天从 Figma 董事会辞职，引发利益冲突猜测。

hackernews · cl42 · 7月20日 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48980019)

**背景**: 开源权重模型允许任何人下载和运行模型，而专有模型仅能通过 API 访问。ASIC（专用集成电路）是为特定任务（如 AI 推理）设计的定制芯片，比 GPU 效率更高。Anthropic 是一家以 Claude 模型闻名的领先 AI 实验室，但近期因产品策略和董事会道德问题面临争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(chatbot)">Kimi (chatbot) - Wikipedia</a></li>
<li><a href="https://platform.kimi.ai/docs/models">Model List - Kimi API Platform</a></li>
<li><a href="https://huggingface.co/collections/Qwen/qwen3">Qwen 3 - a Qwen Collection</a></li>
<li><a href="https://hashrateindex.com/blog/what-is-an-ai-asic-guide-ai-chips/">What Is an AI ASIC? The Complete Guide</a></li>

</ul>
</details>

**社区讨论**: 用户 LarsDu88 认为，最终赢家将是最快将模型烧录到 ASIC 上的公司，并提到 AI 已能辅助芯片设计。overgard 指出 Anthropic 的 Figma 争议可能构成对合作伙伴的背叛。bko 反驳称用户愿意为稍好的模型支付高价，而 port3000 注意到炒作周期正在缩短，暗示可能接近瓶颈。

**标签**: `#AI`, `#open source`, `#Anthropic`, `#model release`, `#industry analysis`

---

<a id="item-9"></a>
## [本·汤普森提议美国立法促进开放 AI 模型竞争](https://simonwillison.net/2026/Jul/20/afraid-of-chinese-models/#atom-everything) ⭐️ 8.0/10

本·汤普森提出一项美国法律，明确将收集数据用于 AI 训练视为合理使用，并禁止服务条款中禁止蒸馏，旨在帮助美国开放模型与中国模型竞争。 该提案可能重塑美国与中国 AI 模型之间的竞争格局，确保美国开放模型能够通过蒸馏合法地从现有模型中学习，解决中国模型通常更开放这一关键不对称问题。 汤普森还推测，阿里巴巴决定以开放权重发布 Qwen 3.8 Max，可能受到近期习近平鼓励开源、开放与合作共享的讲话影响。蒸馏在技术上几乎无法阻止，因此提议的政策转变具有务实性。

rss · Simon Willison · 7月20日 17:09

**背景**: 模型蒸馏是一种技术，较小的“学生”模型通过查询 API 等方式从较大的“教师”模型中学习。许多美国 AI 实验室在其服务条款中禁止蒸馏，而中国模型通常以开放权重发布，允许无限制蒸馏。美国关于 AI 训练数据的合理使用原则目前尚不明确，造成了法律不确定性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://prod-10c-www.netlify.app/blog/a-i/how-ai-model-distillation-helps-you-build-efficient-ai-models/">How AI Model Distillation Helps You Build Efficient AI Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen3.8-Max">Qwen3.8-Max</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open models`, `#distillation`, `#copyright`, `#Chinese AI`

---

<a id="item-10"></a>
## [特朗普政府或限制美企使用中国开放权重 AI 模型](https://www.axios.com/2026/07/20/ai-us-china-open-source-kimi) ⭐️ 8.0/10

据 Axios 报道，特朗普政府正考虑实施新限制，阻止美国企业使用中国的开放权重 AI 模型，特别是表现强劲且成本低廉的 Kimi K3 模型。 这一政策转变可能重塑全球 AI 竞争格局，迫使美国企业放弃价格更低、性能更强的中国模型，可能拖慢 AI 发展并增加成本，也凸显了中美科技紧张局势的升级。 限制措施可能并非直接封禁，而是通过采购规则、实体清单威胁和舆论压力等软性手段。白宫 AI 顾问 David Sacks 批评 OpenAI 和 Anthropi 试图借政府之手消灭开源竞争。

telegram · zaihuapd · 7月20日 11:49

**背景**: 开放权重模型（如 Kimi K3）会以 Apache 2.0 等许可协议发布已训练好的模型参数，允许他人下载、微调和部署。与完全开源不同，训练数据和代码通常不公开。Kimi K3 由 Moonshot AI 开发，在全球模型排行榜上名列前茅，与 GPT-5.6 和 Claude Fable 5 等闭源模型竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_K3">Kimi K3</a></li>
<li><a href="https://cdn.sputniknews.cn/20260720/1072397574.html">Kimi K 3 模 型 跻身全球前列，中国以“开源”重塑全球AI竞争格局</a></li>

</ul>
</details>

**标签**: `#AI政策`, `#Kimi K3`, `#开源模型`, `#中美竞争`, `#AI安全`

---

<a id="item-11"></a>
## [研究：三分之二美军应用含中俄代码](https://www.wired.com/story/apps-marketed-to-us-troops-are-shipping-chinese-and-russian-code/) ⭐️ 8.0/10

普渡大学一项研究显示，在面向美军人员推广的 220 余款应用中，近三分之二嵌入了来自中国、俄罗斯等国的第三方代码，其中包括被美国政府列为国家安全威胁的华为软件开发工具包（SDK）。 这引发了严重的国家安全担忧，因为嵌入的代码可能被用于监视或数据窃取，尤其考虑到美国国防部此前曾报告对手利用商业位置数据监视中东美军人员。 研究发现，虽然目前未观察到数据实际流向华为服务器，但该 SDK 可随时远程更新，潜伏代码存在被激活的风险。在 103 名军人关联受访者中，76%至 83%对应用包含中、俄、伊朗或朝鲜代码表示极度不安。

telegram · zaihuapd · 7月20日 13:42

**背景**: 供应链攻击利用第三方软件、硬件或服务中的漏洞，SolarWinds 事件就是一个著名例子。在这种情况下，面向美军推广的移动应用集成了来自被视为对手的国家的 SDK，创造了潜在的後門。美国国防部此前曾警告对手利用商业数据追踪军事人员。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://juejin.cn/post/7038800735856754725">为什么必须防止 供 应 链 攻 击 ?SolarWinds...</a></li>
<li><a href="https://www.buaq.net/go-168209.html">防止 供 应 链 攻 击 的9种 方 法</a></li>

</ul>
</details>

**标签**: `#国家安全`, `#供应链安全`, `#移动应用安全`, `#隐私`, `#第三方代码`

---

<a id="item-12"></a>
## [欧盟拟以生物识别数据换取美免签](https://edri.org/our-work/the-eu-is-about-to-sell-our-most-sensitive-data-to-the-us-for-visa-free-travel/) ⭐️ 8.0/10

欧盟委员会正与特朗普政府敲定一项“增强边境安全伙伴关系”（EBSP）框架协议，该协议要求欧盟向美国共享公民的生物识别数据和风险指标，以换取欧盟公民的免签赴美待遇。 该协议将为大规模监控和隐私侵犯树立危险先例，高度敏感的生物识别数据可能被系统性地传输给外国政府，可能压制政治异议和激进主义。 据泄露的 EBSP 草案显示，欧盟几乎全盘接受了美方对生物识别数据库的无限制访问要求。数据共享可能包括基于政治观点的“风险指标”，例如对跨性别权利的支持，引发了对身份定性的担忧。

telegram · zaihuapd · 7月20日 15:08

**背景**: “增强边境安全伙伴关系”（EBSP）是美国主导的倡议，旨在通过生物识别信息共享加强边境安全。欧盟免签证计划（VWP）目前允许欧盟公民免签赴美，但美国计划到 2027 年强制要求参与 EBSP。欧洲数字权利组织（EDRi）是欧洲领先的数字权利倡导组织。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://linux.do/t/topic/2621547">欧盟拟向美开放生物识别数据以换取免签待遇 - 前沿快讯 - LINUX DO</a></li>
<li><a href="https://hackernews.cc/archives/39702">HackerNews</a></li>

</ul>
</details>

**标签**: `#privacy`, `#biometric data`, `#data protection`, `#EU-US relations`, `#surveillance`

---

<a id="item-13"></a>
## [智谱建成 1 吉瓦全国产芯片数据中心](https://www.bloomberg.com/news/articles/2026-07-20/z-ai-completes-giant-data-center-with-chinese-chips-to-train-ai) ⭐️ 8.0/10

智谱 AI（Z.ai）建成了一座全部采用国产芯片的大型数据中心，功率达 1 吉瓦，已开始部分运营。该设施将用于支持 GLM 系列 AI 模型的训练。 这标志着中国在 AI 基础设施自主化方面取得了重要里程碑，减少了对英伟达等外国芯片供应商的依赖。它证明了中国 AI 实验室能够使用国产技术建设和运营大规模训练集群。 该数据中心功率达 1 吉瓦，足以同时为约 75 万户家庭供电。智谱运营多个各拥有超万枚芯片的计算集群，该设施是中国 AI 实验室建造的最大规模设施之一。

telegram · zaihuapd · 7月20日 15:43

**背景**: 智谱 AI 是中国领先的人工智能公司，开发了 GLM（通用语言模型）系列，包括开源权重的 ChatGLM 等模型。在美国对先进芯片实施出口限制的背景下，中国企业正加速采用华为、寒武纪等公司的国产替代方案，以维持 AI 发展的进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM_(AI)">GLM (AI)</a></li>

</ul>
</details>

**标签**: `#国产芯片`, `#数据中心`, `#AI训练`, `#GLM`, `#基础设施`

---