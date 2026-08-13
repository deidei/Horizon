---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> 从 32 条内容中筛选出 8 条重要资讯。

---

1. [谷歌发布 Gemini 3.7 Flash，其最智能的"工作马"模型](#item-1) ⭐️ 9.0/10
2. [DRAM“意大利面化”攻击在 AMD CPU 上获取 Ring-0 权限](#item-2) ⭐️ 9.0/10
3. [Cerebras 与 OpenAI 推出 GPT-5.6 Sol Ultrafast，推理速度快 7 倍](#item-3) ⭐️ 8.0/10
4. [选择无聊技术，明智使用创新令牌](#item-4) ⭐️ 8.0/10
5. [DeepSeek Harness 开发者预览版发布：开源智能体框架](#item-5) ⭐️ 8.0/10
6. [像素指标无法区分世界模型性能；新工具“worldproof”诊断原因](#item-6) ⭐️ 8.0/10
7. [DeepMind 推手语转文字模型 SL2T，Pixel 11 首次落地](#item-7) ⭐️ 8.0/10
8. [谷歌发布 Gemini 3.6 Flash，透露 Gemini 4 已开始预训练](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌发布 Gemini 3.7 Flash，其最智能的"工作马"模型](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 9.0/10

谷歌发布了 Gemini 3.7 Flash，这是一款基于 Gemini 3.6 Flash 的新多模态模型，在视觉和编码任务上表现出色。该模型现在也为 160 多个国家的 Google AI Pro 和 Ultra 订阅者的 Gemini Spark 提供支持。 这一发布突显了谷歌快速的迭代节奏——三周前刚推出 Gemini 3.6 Flash——以及其提供廉价、可靠、适用于日常 AI 工作负载的"工作马"模型的目标。它也使 Gemini 3.7 Flash 与 Opus 5、Luna 等竞争对手在价格和视觉/编码基准上的竞争更加激烈。 Gemini 3.7 Flash 基于 Gemini 3.6 Flash，并在推理、编码、智能体工具调用、多模态、多语言和长上下文等基准上接受了评估。据社区消息，其首发价格计划于 2026 年 12 月 31 日翻倍。

hackernews · thisisauserid · 8月13日 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**背景**: Gemini 是 Google DeepMind 开发的多模态大语言模型家族，于 2023 年 12 月 6 日发布，并用于 Gemini 聊天机器人。Flash 系列被设计为快速、低成本的"工作马"模型，适用于总结、解析、格式化等高容量、以文本为主的使用场景。Gemini 3.7 Flash 是该系列的最新版本，仅在三周前发布过 Gemini 3.6 Flash。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-7-flash/">Gemini 3 . 7 Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3 . 7 Flash : our most intelligent workhorse model</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_2.5_Flash_Image">Gemini 2.5 Flash Image</a></li>

</ul>
</details>

**社区讨论**: 社区反应褒贬不一：jjcm 认为 Gemini 3.7 Flash 在图像转 HTML 任务上表现出色，且价格合理，但 Opus 5 仍是同类最佳。simonw 称其首发定价"很奇怪"，并质疑如此紧凑的发布节奏。Alifatisk 认为 GPT-5.6 Luna (Max) 在 DeepSWE 1.1 上仍然更强且更便宜；wxw 也表示，既然 Luna 价格更低，何必再用 Flash。

**标签**: `#AI`, `#Google Gemini`, `#LLM`, `#Model Release`, `#Machine Learning`

---

<a id="item-2"></a>
## [DRAM“意大利面化”攻击在 AMD CPU 上获取 Ring-0 权限](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

Christopher Domas 发布了名为“skitter-creek-bath-salts”的硬件安全项目，通过“意大利面化”DRAM 来获取 ring-0 特权，并将在 Black Hat 上发表演讲。该技术已在 AMD Family 16h CPU 上开发并测试。 这是一项具有开创性的 DRAM 漏洞研究，因为它暴露了操作系统之下的隐藏攻击面，可能绕过所有软件安全机制。它可能影响游戏主机等封闭系统，并凸显了未公开的 DRAM 控制器行为带来的危险。 根据 README，该攻击适用于 AMD Jaguar（Family 16h），其数据手册记载 DRAM 控制器的转换寄存器且无法被锁定。较新的 CPU（如 Zen 3）已改变内存控制器的基址，因此其他处理器家族是否受影响仍是未解问题。

hackernews · matt_d · 8月13日 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**背景**: DRAM 控制器使用内部寄存器进行内存地址转换；如果能够重新编程这些寄存器，攻击者就可以重映射内存并获取特权访问。“意大利面化”一词来自天体物理学，描述物体在极端引力下被拉伸和压缩，这里借喻对 DRAM 地址转换的操纵。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49286341">Spaghettifying DRAM | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spaghettification">Spaghettification - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞 Christopher Domas 的演讲风格，并期待 Black Hat 演讲。有人指出 DRAM 的复杂度已大幅增加，形成了巨大的攻击面；也有人质疑除了老的 AMD Family 16h 之外，该攻击到底影响哪些现代 CPU。

**标签**: `#hardware-security`, `#DRAM`, `#exploitation`, `#low-level`, `#security-research`

---

<a id="item-3"></a>
## [Cerebras 与 OpenAI 推出 GPT-5.6 Sol Ultrafast，推理速度快 7 倍](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras 与 OpenAI 宣布推出 GPT-5.6 Sol Ultrafast，这一前沿模型版本在准确率与标准模型相当的同时，运行速度快了近 7 倍。在评估中，它用约 11 小时回答了全部 2500 道 HLE 问题，而 Claude Fable 5 则耗时超过 78 小时。 这标志着前沿 AI 推理速度大幅提升的一个重要里程碑，有望支持实时应用以及更多迭代、更高质量的推理。Cerebras 与 OpenAI 的合作表明，定制硬件可以在大模型服务领域挑战以 GPU 为主导的格局。 Ultrafast 模式运行在 Cerebras 晶圆级硬件上；据 Artificial Analysis 报道的速度，它比 Claude Fable 5 快 11 倍，比 Fast 模式下的 Opus 4.8 快 5 倍。目前尚未公布定价信息，Cerebras 还表示到 2027 年底将扩展至 200MW 的 AI 算力容量。

hackernews · pr337h4m · 8月13日 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**背景**: Cerebras 打造了全球最大的 AI 处理器——晶圆级引擎（Wafer-Scale Engine），其中 WSE-3 芯片面积达 46,225 平方毫米，包含 4 万亿个晶体管，专为快速训练和推理设计。传统的大模型推理优化包括量化、蒸馏和批处理等技术，而 Cerebras 的目标是通过专门构建的超大芯片而非渐进式软件优化来加速 AI。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者总体上对这次合作感到兴奋，有人认为更快的推理能够支持迭代式思考，从而提升推理质量。但也有不少人持怀疑态度，指出 OpenAI 和 Cerebras 并未明确确认与标准 GPT-5.6 Sol 的性能完全一致，并且没有公布任何定价细节。

**标签**: `#AI`, `#LLM`, `#Inference`, `#Cerebras`, `#OpenAI`

---

<a id="item-4"></a>
## [选择无聊技术，明智使用创新令牌](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

Dan McKinley 在 2015 年发表的文章《选择无聊技术》主张，组织应优先采用成熟可靠的技术，并通过有限的“创新令牌”来规划新技术的采纳。这篇文章近期在 Hacker News 上重新引发讨论，仍能激发深入思考。 这篇文章为工程领导者在创新与风险之间权衡提供了实用框架，其“创新令牌”概念已成为被广泛引用的思维模型。它能帮助团队避免工具蔓延，并将创新精力集中在能创造真正业务价值的领域。 文章的核心比喻是每家公司大约拥有三个“创新令牌”，用来采纳新技术，需要谨慎使用。文章强调，无聊（成熟）的技术具有可预测的失败模式，能让团队把解决问题的精力集中在真正的产品领域上。

hackernews · tosh · 8月13日 17:48 · [社区讨论](https://news.ycombinator.com/item?id=49289512)

**背景**: 这篇文章的作者是 Dan McKinley，他曾任 Etsy 和 Stripe 的软件工程师。文章针对初创公司普遍追逐新框架、新语言的现象，指出这种倾向会带来不必要的复杂性和风险。“创新令牌”把技术采纳视为一种需要精打细算的有限资源。多年来，这篇文章已成为讨论务实技术选型时的经典参考。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lessannoyingbusiness.com/post/innovation-tokens">Innovation Tokens - When to break from the status quo</a></li>
<li><a href="https://ilearnt.com/blog/innovationtokens/">Innovation tokens</a></li>
<li><a href="https://www.morbe.online/post/boring-technology-why-less-hype-can-lead-to-more-productivity">Boring technology : Why less hype can lead to more productivity</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论总体持正面态度，许多读者称这是他们最喜欢的文章，并称赞“创新令牌”框架非常有助于解释取舍。但也有反对者认为“新”或“新颖”只是弱代理指标，工程师应直接评估需求、风险和权衡。还有人将其与 AI 智能体时代联系起来，建议公司应把创新令牌花在智能体上，其余技术保持成熟稳定。

**标签**: `#technology strategy`, `#software engineering`, `#innovation`, `#boring technology`, `#engineering leadership`

---

<a id="item-5"></a>
## [DeepSeek Harness 开发者预览版发布：开源智能体框架](https://deepseek.com/harness/en/) ⭐️ 8.0/10

DeepSeek 发布了 DeepSeek Harness，作为早期开源开发者预览版，所有智能体能力均以插件实现，并提供完全可追踪的会话日志。源代码已以 MIT 许可证公开。 这一发布意义重大，因为它来自主要 AI 实验室，直击智能体开发中的可观测性和可扩展性两大痛点。它可能影响开发者构建和调试多步骤智能体系统的方式，同时给限制模型轨迹访问的美国实验室带来竞争压力。 该框架采用插件架构，所有能力都可替换或重新组合，并通过 Cordis v4 支持热重载和动态启用/禁用。会话日志为追加写入，记录系统提示、推理过程、工具调用、子智能体调度和上下文注入；Trajectory 视图支持恢复、分叉、搜索和回放。

hackernews · bjin · 8月13日 12:58 · [社区讨论](https://news.ycombinator.com/item?id=49285244)

**背景**: AI 智能体框架为开发者提供构建自主系统的抽象和运行时，使其能够调用工具、管理上下文并协调子智能体，例如 LangChain、Microsoft Agent Framework 和 AutoGen。DeepSeek Harness 是一种“智能体 harness”，即协调智能体循环、插件和会话状态的运行时层。其架构遵循“一切皆是插件”的模式，并利用 Cordis v4 插件系统，该系统可以在不重启进程的情况下加载/卸载组件并回滚副作用。该早期预览版采用 MIT 许可证，明确尚未达到生产就绪状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://deepseek-code.com/">DeepSeek Harness: Open-Source AI Agent Framework</a></li>
<li><a href="https://www.langchain.com/resources/ai-agent-frameworks">The best AI agent frameworks in 2026</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极但有所保留。评论者称赞追加写入、可回放的会话日志是“杀手级功能”，并认为美国模型的加密轨迹无法与之相比；一位作者澄清这只是早期粗糙预览。持怀疑态度的人认为其用处有限，并表达了对“插件疲劳”的担忧，还有人强调 Cordis v4 热重载和副作用回滚的重要性。

**标签**: `#AI agents`, `#open-source`, `#developer tools`, `#DeepSeek`, `#agent framework`

---

<a id="item-6"></a>
## [像素指标无法区分世界模型性能；新工具“worldproof”诊断原因](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 8.0/10

作者发布了开源诊断工具 worldproof，用于诊断世界模型，并发现 SSIM 和 PSNR 等像素指标在真实机器人视频上无法对世界模型进行排序，因为一个简单的“最后一帧”基线就已获得接近完美的分数（在 SO-101 机械臂记录上达到 0.983 SSIM 和 53.9 dB PSNR）。误差不随预测步数增长，因此所有模型得分接近，评估缺乏区分度。 这是世界模型社区面临的一个关键评估陷阱：依赖像素指标的基准在真实数据上可能给出错误信心或完全无法区分模型。该开源诊断工具也为研究者提供了实用价值，使其能够在自己数据上测量有效的评估步数范围。 作者使用每组 64 条轨迹，并采用四分位均值与分层自助置信区间，在 DROID（15fps）上测量了“最后一帧”基线，发现存在三个区间：第 1–3 步接近完美且无法区分，第 4–24 步指标单调快速下降、模型可分离，第 28 步之后分数在 0.20 SSIM 附近触底振荡、预测与真实情况完全不相关。需要注意的是，LPIPS 无法区分这两个数据集，且在掩码变体上指向相反方向；另外，在帧率较高时，把第 0 步纳入计算会抬高所有汇总指标，因为复制基线几乎免费获得第一步。

reddit · r/MachineLearning · /u/georgia_bucea · 8月13日 19:58

**背景**: 世界模型是一类从数据中学习环境动态的神经网络，通常通过根据动作预测未来帧来工作；它们被用于机器人和规划领域，使智能体能够“想象”结果。SSIM（结构相似性）和 PSNR（峰值信噪比）是常见的像素级图像质量指标，用于将预测帧与真实帧进行比较，但它们不一定反映语义或任务相关的准确性。“最后一帧”基线——即简单地预测画面不变——是一个平凡的下限，但在慢速或高帧率视频上可能已经获得很高分数，从而暴露出评估设置缺乏区分度的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Structural_similarity">Structural similarity index measure - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio">Peak signal-to-noise ratio - Wikipedia</a></li>

</ul>
</details>

**标签**: `#world-models`, `#evaluation-metrics`, `#robotics`, `#machine-learning`, `#diagnostics`

---

<a id="item-7"></a>
## [DeepMind 推手语转文字模型 SL2T，Pixel 11 首次落地](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

DeepMind 发布了大规模多语言手语转文字模型 SL2T，首次在 Pixel 11 的 Gboard 和实时字幕（Live Transcribe）中落地，支持美国手语转英语，并在 FLEURS-ASL 上取得零样本 70 BLEURT 的成绩。 这是无障碍领域的一次重要进展，手语 AI 从研究走向消费产品。同时，该模型仅使用姿态关键点而非原始视频，展示了隐私保护的多模态模型的潜力。 该模型使用超过 10 万小时、50 多种手语的数据训练，仅处理手部和身体姿态关键点以保护隐私，未来将扩展到更多设备和语言，而不只是美国手语转英语。

telegram · zaihuapd · 8月13日 08:55

**背景**: FLEURS-ASL 是将 FLORES/FLEURS 基准扩展到美国手语的版本，用于评估手语翻译。BLEURT 是一种基于 BERT 的学习型评估指标，衡量译文的流畅度和语义保真度。DeepMind 的 SL2T 表明，手语翻译可以直接从身体坐标完成，而非依赖原始视频，这是一种不同于传统视频方法的技术路线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/">Putting sign language AI into users’ hands — Google DeepMind</a></li>
<li><a href="https://arxiv.org/html/2408.13585">FLEURS - ASL : Including American Sign Language in Massively...</a></li>
<li><a href="https://arxiv.org/abs/2004.04696">[2004.04696] BLEURT: Learning Robust Metrics for Text Generation</a></li>

</ul>
</details>

**标签**: `#AI`, `#accessibility`, `#DeepMind`, `#sign language`, `#multimodal model`

---

<a id="item-8"></a>
## [谷歌发布 Gemini 3.6 Flash，透露 Gemini 4 已开始预训练](https://t.me/zaihuapd/43177) ⭐️ 8.0/10

谷歌发布了 Gemini 3.6 Flash，声称相比 Gemini 3.5 Flash 可减少 17% 的输出 Token，并用更少的推理步骤和工具调用完成多步任务。同时，谷歌透露下一代模型 Gemini 4 已启动预训练。 此次发布表明谷歌正在快速迭代 Gemini 系列，以明显的效率提升和更具竞争力的定价策略，可能改变开发者在 LLM API 市场上的选择。确认 Gemini 4 启动预训练，也预示着下一代前沿模型的发展方向。 Gemini 3.6 Flash 在代码生成、知识工作和计算机操作能力上均有提升，知识截止日期更新至 2026 年 3 月。其 API 定价为每百万输入 Token 1.5 美元、每百万输出 Token 7.5 美元；谷歌还推出了面向高吞吐、低延迟场景的 Gemini 3.5 Flash。

telegram · zaihuapd · 8月13日 17:32

**背景**: LLM 推理通过分词、带自注意力机制的 Transformer 层以及自回归 Token 生成，将文本提示转换为回复。工具调用允许语言模型直接调用外部函数或 API 来协助回答，而计算机操作能力则让 AI 代理能像人类用户一样操作软件界面。这些概念是理解 Gemini 3.6 Flash 效率与能力变化的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arpitbhayani.me/blogs/how-llm-inference-works/">How LLM Inference Works</a></li>
<li><a href="https://blog.solega.co/how-to-implement-tool-calling-with-gemma-4-and-python/">How to Implement Tool Calling with Gemma 4 and Python - Solega Blog</a></li>
<li><a href="https://openai.com/index/computer-using-agent/">Computer-Using Agent | OpenAI</a></li>

</ul>
</details>

**标签**: `#Gemini`, `#Google`, `#AI模型`, `#大语言模型`, `#技术发布`

---