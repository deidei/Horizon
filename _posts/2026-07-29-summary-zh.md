---
layout: default
title: "Horizon Summary: 2026-07-29 (ZH)"
date: 2026-07-29
lang: zh
---

> 从 42 条内容中筛选出 11 条重要资讯。

---

1. [Claude 共享链接被搜索引擎索引致用户数据泄露](#item-1) ⭐️ 9.0/10
2. [开源引擎在 M 系列 Mac 上以 2GB 内存运行 Gemma 4 26B](#item-2) ⭐️ 8.0/10
3. [Mitchell Hashimoto 创立 Superlogical，基于 libghostty](#item-3) ⭐️ 8.0/10
4. [Kimi 推出 K3-256k：半价长上下文 AI 模型](#item-4) ⭐️ 8.0/10
5. [LLM 难以可靠遵循长政策文档](#item-5) ⭐️ 8.0/10
6. [AI 蠕虫利用 Microsoft Copilot 在 Word 中自我传播](#item-6) ⭐️ 8.0/10
7. [英伟达通知 AIC 合作伙伴显卡涨价，厂商暂停出货](#item-7) ⭐️ 8.0/10
8. [俄联邦安全局指控 Telegram 创始人杜罗夫协助恐怖活动](#item-8) ⭐️ 8.0/10
9. [Hugging Face 被滥用于生成深度伪造裸照](#item-9) ⭐️ 8.0/10
10. [月之暗面寻求 20 亿美元融资，估值 300 亿美元，计划香港上市](#item-10) ⭐️ 8.0/10
11. [中国反网络暴力法草案针对 AI 网暴](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Claude 共享链接被搜索引擎索引致用户数据泄露](https://t.me/zaihuapd/42830) ⭐️ 9.0/10

Anthropic 的 Claude AI 出现隐私漏洞，导致大量共享对话链接被 Google 等搜索引擎索引，暴露了 API 密钥、加密货币钱包和个人信息等敏感数据。 此次事件暴露的敏感数据可能导致身份盗窃、财务损失或企业间谍活动，并凸显了 AI 聊天服务中反复出现的安全漏洞——而 ChatGPT 等竞争对手已修复了类似问题。 该漏洞源于共享聊天页面缺少 'noindex' 元标签，导致搜索引擎可以抓取和索引这些页面。ChatGPT 在大约一年前发现类似漏洞并已修复，但 Anthropic 尚未解决此问题。

telegram · zaihuapd · 7月29日 02:40

**背景**: Claude 的“共享对话”功能允许用户生成对话的公开链接，本意是供特定人员查看。当页面缺少 'noindex' 标签时，Google 等搜索引擎可能会将其编入索引，使内容可被公开搜索。这是网络隐私中常见的疏忽，正确使用 robots.txt 或 noindex 标签可以防止索引。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://overcentral.com/en/claude-ai-shared-chats-leak/">Claude AI Privacy Leak: Shared Conversations Indexed by Google</a></li>
<li><a href="https://news.aibase.com/news/29922">Anthropic Claude's Shared Chat Function Exposes Privacy Risks...</a></li>
<li><a href="https://www.zdnet.com/article/claude-ai-shared-chats-indexed-by-google/">Claude AI shared chats indexed by Google - see if your... | ZDNET</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#Claude`, `#AI`, `#vulnerability`

---

<a id="item-2"></a>
## [开源引擎在 M 系列 Mac 上以 2GB 内存运行 Gemma 4 26B](https://github.com/drumih/turbo-fieldfare) ⭐️ 8.0/10

TurboFieldfare 是一个用 Swift 和 Metal 编写的全新开源推理引擎，它通过从 SSD 流式传输路由专家，使得在任何 M 系列 Mac 上，仅需 2GB RAM 即可运行 4 位量化的 Gemma 4 26B-A4B-IT 模型。 这一突破大幅降低了本地运行大型语言模型的硬件门槛，使内存受限的 Mac 用户也能使用强大的设备端 AI。它展示了一种实用的方法，通过将专家卸载到 SSD 来运行超出可用 RAM 的模型，可能影响未来推理引擎的设计。 该模型的 4 位量化权重约为 14GB，但引擎仅使用约 2GB RAM，通过将共享层和 KV 缓存保留在内存中，同时从 SSD 流式传输路由专家（使用小型缓存和有界并行 pread）来实现。在 8GB M2 MacBook Air 上达到 5-6 tok/s，在 M5 MacBook Pro 上达到 31-35 tok/s，并包含一个实验性的兼容 OpenAI 的服务器，支持流式输出和工具调用。

hackernews · gitpusher42 · 7月29日 15:05 · [社区讨论](https://news.ycombinator.com/item?id=49098510)

**背景**: 像 Gemma 4 26B 这样的大型语言模型通常过大，无法完全装入消费级设备内存。混合专家（MoE）架构包含许多专门的“专家”子网络，但每个 token 仅激活少数几个，从而实现条件计算。4 位量化降低权重精度以节省空间，KV 缓存存储先前 token 状态以加速生成。该引擎巧妙地利用 MoE 稀疏性，仅从 SSD 加载所需的专家。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/mixture-of-experts-moe-layers">Mixture of Experts ( MoE ) Layers</a></li>
<li><a href="https://medium.com/@minh.hoque/understanding-kv-caching-in-transformers-729271c9b74a">Understanding KV Caching in Transformers - Medium</a></li>
<li><a href="https://arxiv.org/abs/1810.05723">[1810.05723] Post-training 4-bit quantization of convolution ... True 4-Bit Quantized Convolutional Neural Network Training on ... 4-Bit Model Quantization - emergentmind.com Post training 4-bit quantization of convolutional networks ... Post training 4-bit quantization of convolutional networks ... Post training 4-bit quantization of convolutional networks ... 4-bit CNN Quantization Method With Compact LUT-Based ... Images</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极且参与度高。一些用户质疑这与 llama.cpp 中的 mmap 相比如何，作者指出主要区别在于将 SSD 读取与推理同步。少数用户提供了针对旧版 macOS 的编译提示，并建议在 DiffusionGemma 等相关项目上进行合作。

**标签**: `#inference engine`, `#on-device AI`, `#LLM`, `#Mac`, `#Metal`

---

<a id="item-3"></a>
## [Mitchell Hashimoto 创立 Superlogical，基于 libghostty](https://www.superlogical.com/) ⭐️ 8.0/10

Mitchell Hashimoto 宣布成立新公司 Superlogical，将基于开源终端库 libghostty 构建商业产品。他还计划将 Ghostty 终端模拟器的所有权转让给一个非营利组织。 这代表了一种新颖的开源商业模式：将核心项目交给非营利组织，而公司则将其库作为公共依赖进行构建。这可能启发其他开发者分离库和产品的所有权，促进可持续生态系统的发展。 Superlogical 将完全按照 libghostty 的设计使用它，消费所有用户都可用的相同 MIT 许可组件，并计划将共享的终端改进上游推送。Ghostty 是一个快速、GPU 加速的跨平台终端模拟器，附带 C 兼容库 libghostty。

hackernews · yan · 7月29日 15:41 · [社区讨论](https://news.ycombinator.com/item?id=49098965)

**背景**: Ghostty 是一个使用平台原生 UI 和 GPU 加速的终端模拟器，其库 libghostty 允许将终端嵌入第三方项目。Mitchell Hashimoto 是 Ghostty 的创建者，也是 HashiCorp 的创始人。该公告详细说明了将 Ghostty 所有权转让给非营利组织以确保其独立性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.</a></li>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>
<li><a href="https://ghostty.org/">Ghostty</a></li>

</ul>
</details>

**社区讨论**: 评论者赞扬所有权转移模型是将核心开源项目与商业实体分离的聪明方法。有人将其与 OLE/COM 等传统技术相提并论，而一名用户批评标题过于隐晦，倾向于更信息化的标题。总体情绪积极，参与度很高。

**标签**: `#open-source`, `#terminal`, `#business model`, `#software engineering`

---

<a id="item-4"></a>
## [Kimi 推出 K3-256k：半价长上下文 AI 模型](https://www.kimi.com/code/docs/en/kimi-code/models) ⭐️ 8.0/10

Kimi（月之暗面）发布了 K3-256k 模型，提供 256k token 的上下文窗口，价格仅为现有 1M token 版本的一半。 这一价格使长上下文 AI 对通常使用不到 256k 上下文的开发者和用户更加可及，可能加速大上下文模型在编码和知识工作中的应用。 根据社区用户 wxw 的评论，在 256k 上下文内，K3-256k 提供与 1M 版本相同的结果，但仅使用约一半的配额。该模型可通过 Kimi 的 API 和平台使用。

hackernews · monneyboi · 7月29日 19:25 · [社区讨论](https://news.ycombinator.com/item?id=49101852)

**背景**: Kimi 是月之暗面（Moonshot AI）开发的中国 AI 聊天机器人和大语言模型系列，以其长上下文能力著称。原始 K3 模型支持 1M token 的上下文窗口，属于最大之一。新的 K3-256k 变体降低了成本，同时保持了大多数用例的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(chatbot)">Kimi (AI) - Wikipedia</a></li>
<li><a href="https://platform.kimi.ai/docs/models">Model List - Kimi API Platform</a></li>
<li><a href="https://codingscape.com/blog/llms-with-largest-context-windows">LLMs with largest context windows</a></li>

</ul>
</details>

**社区讨论**: 社区反应普遍积极。用户 timcobb 指出 256k 对大多数任务足够，1M 往往过度。madihaa 喜欢较低的成本，因为他们通常保持在 200k 上下文以下。xyzsparetimexyz 称降价'巨大'。MangoCoffee 评论说大语言模型正迅速成为商品，美国 AI 实验室可能失去护城河。

**标签**: `#LLM`, `#AI`, `#pricing`, `#context-length`, `#Kimi`

---

<a id="item-5"></a>
## [LLM 难以可靠遵循长政策文档](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

这一发现挑战了 LLM 能通过长篇指令治理 AI 代理的假设，凸显了在现实任务中部署代理的关键安全风险。 论文表明，即使声称拥有 100 万 token 上下文窗口的模型，在处理长政策时性能也会显著下降，且随文档长度增加而恶化。

hackernews · spIrr · 7月29日 13:01 · [社区讨论](https://news.ycombinator.com/item?id=49096969)

**背景**: 大型语言模型使用带有注意力机制的 Transformer 架构处理文本，注意力机制为输入的不同部分分配相关性。上下文窗口限制了模型一次能考虑的文本量。尽管最新模型宣称拥有百万级 token 窗口，但实际效果受限于记忆和注意力约束。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.plainenglish.io/context-window-in-llms-198e8079d3c8">Context Window in LLMs. In this article, I will try to simplify</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transformer_(deep_learning)">Transformer (deep learning) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者同意这一发现，指出即使使用 CLAUDE.md 文件，像 Claude 这样的模型也会在大约 10 分钟后忽略早期指令。有人认为'代理 AI'是一种合成训练能力，如果没有针对特定手册进行后训练就会失败。

**标签**: `#LLM`, `#AI safety`, `#long-context`, `#agents`, `#benchmark`

---

<a id="item-6"></a>
## [AI 蠕虫利用 Microsoft Copilot 在 Word 中自我传播](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 8.0/10

研究人员演示了一种新型 AI 蠕虫，它通过在文档中嵌入恶意的提示注入指令，利用 Microsoft Copilot for Word 自我传播，导致 Copilot 自动修改并将感染扩散到新文档。 这一漏洞揭示了 AI 代理无法区分用户指令与数据内容的根本性安全缺陷，对 AI 工具拥有广泛文档和邮件访问权限的企业环境构成严重风险。 该蠕虫利用间接提示注入，通过文档中隐藏的对抗性提示（如使用白色文字）欺骗 Copilot 执行命令，例如将受感染文档转发给新联系人。目前尚无可靠的缓解措施。

hackernews · Canopy9560 · 7月29日 11:44 · [社区讨论](https://news.ycombinator.com/item?id=49096188)

**背景**: 提示注入攻击允许攻击者在文本中嵌入隐藏指令，大语言模型可能将这些指令解读为合法命令。Microsoft Copilot for Word 将 LLM 功能直接集成到文档编辑体验中，使 AI 能够读取和修改文档内容。当用户打开特制文档时，Copilot 可能被欺骗执行发送邮件或修改其他文档等操作，从而使蠕虫得以传播。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**社区讨论**: 社区反应表达了担忧，认为只要 AI 混淆指令与数据，这类漏洞从根本上就无法修复。一些用户已卸载 Copilot，另一些则强调现有技术如白色文字仍可用于注入提示。

**标签**: `#AI security`, `#prompt injection`, `#Copilot`, `#LLM vulnerabilities`, `#cybersecurity`

---

<a id="item-7"></a>
## [英伟达通知 AIC 合作伙伴显卡涨价，厂商暂停出货](https://t.me/zaihuapd/42834) ⭐️ 8.0/10

英伟达已通知所有 AIC 合作伙伴显卡涨价，涉及搭载 GDDR7 显存的 Blackwell 旗舰产品线和搭载 GDDR6 显存的 GeForce 消费级产品线。各大显卡品牌代工厂已封仓并暂停对外出货，供应量从 7 月下旬起进一步收紧。 此次涨价信号表明消费者将面临更高成本，可能影响整个 GPU 市场，因为英伟达将不断上涨的内存成本转嫁给合作伙伴。这也可能引发全线产品定价和供货的调整。 涨价覆盖 GDDR7 显存的 Blackwell 旗舰产品线和 GDDR6 显存的 GeForce 消费级产品线。供应链消息称，8GB、12GB 和 16GB 显卡的显存成本分别增加约 76 美元、114 美元和 152 美元。RTX 50 SUPER 系列也受影响。

telegram · zaihuapd · 7月29日 03:54

**背景**: 英伟达的 AIC（附加卡）合作伙伴是像华硕、微星、技嘉等制造商，它们从英伟达购买 GPU 芯片并制造成品显卡。Blackwell 架构是英伟达最新的 GPU 微架构，继 Hopper 和 Ada Lovelace 之后，面向数据中心和游戏。GDDR7 是最新一代图形内存，比 GDDR6 提供更高带宽。此次涨价是由于 GDDR7 内存成本上升，英伟达此前吸收但现转嫁给合作伙伴。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techpowerup.com/news-tags/AIC">News Posts matching 'AIC' | TechPowerUp</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#GPU`, `#price increase`, `#hardware`, `#supply chain`

---

<a id="item-8"></a>
## [俄联邦安全局指控 Telegram 创始人杜罗夫协助恐怖活动](https://www.interfax.ru/russia/1106228) ⭐️ 8.0/10

俄罗斯联邦安全局宣布对 Telegram 创始人帕维尔·杜罗夫提起刑事指控，依据刑法第 205.1 条第 1.1 款（协助恐怖活动），并将其列入国际通缉名单。 此举加剧了俄罗斯与主要加密消息平台之间的紧张关系，引发对隐私、加密和平台责任的担忧。可能为政府如何追究科技领袖对用户内容的责任树立先例。 俄联邦安全局指控 Telegram 管理层拒绝删除被乌克兰情报机构和恐怖组织用于策划袭击的频道和机器人，造成包括妇女儿童在内的多人死亡和数十亿卢布损失。

telegram · zaihuapd · 7月29日 05:56

**背景**: Telegram 是由帕维尔·杜罗夫创立的加密消息应用。它因托管与恐怖主义和极端主义相关的内容而一直存在争议。俄罗斯此前曾在 2018 年试图封锁 Telegram，但后来解除了禁令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nodeseek.com/post-846558-1">快讯•俄罗斯通缉TG创始人杜罗夫</a></li>
<li><a href="https://www.guancha.cn/internation/2026_07_29_825460.shtml">俄国家安全局：通缉“电报”创始人杜罗夫</a></li>

</ul>
</details>

**标签**: `#Telegram`, `#privacy`, `#regulation`, `#national security`, `#surveillance`

---

<a id="item-9"></a>
## [Hugging Face 被滥用于生成深度伪造裸照](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

AI Forensics 于 7 月 28 日发布报告称，Hugging Face 被广泛用于生成非自愿深度伪造（Deepfake）色情内容，包括儿童裸照，尽管平台有禁止此类内容的政策。 该报告揭示了 AI 安全与伦理方面的重大问题，暴露了平台政策与实际执行之间的差距。这对 AI 治理、平台责任以及保护弱势群体（特别是女性和儿童）具有重要影响。 测试显示，Hugging Face 排名前九的图像编辑模型中有七个能通过简单提示轻易为女性“脱衣”。研究人员设置的蜜罐在 7 天内收到超过 1000 条请求，其中 73%涉及性内容，近 7%针对儿童。

telegram · zaihuapd · 7月29日 08:20

**背景**: Hugging Face 是一家公司和开源平台，机器学习社区在此协作开发模型、数据集和应用程序。深度伪造（Deepfake）技术利用 AI（如生成式对抗网络 GAN）创建高度逼真的虚假图像或视频。报告称 Hugging Face 在平台层面几乎未实施防护措施来阻止其工具生成有害内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.ibm.com/think/topics/hugging-face">What is Hugging Face? | IBM</a></li>
<li><a href="https://baike.baidu.com/item/深度伪造/56522542">深度伪造_百度百科</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#deepfakes`, `#Hugging Face`, `#ethics`, `#non-consensual content`

---

<a id="item-10"></a>
## [月之暗面寻求 20 亿美元融资，估值 300 亿美元，计划香港上市](https://t.me/zaihuapd/42845) ⭐️ 8.0/10

月之暗面正寻求新一轮至多 20 亿美元的融资，目标估值 300 亿美元，这已是其六个月内第三轮融资，同时筹备香港上市。 估值从 40 亿美元飙升至 300 亿美元的速度，凸显了市场对 Kimi 聊天机器人和大语言模型的需求激增，显示出对中国 AI 初创企业的高度信心。 公司 4 月年度经常性收入已突破 2 亿美元，由 Kimi 聊天机器人和大模型需求推动，并推出了桌面 AI 代理 Kimi Work，用于自主工作流。

telegram · zaihuapd · 7月29日 10:12

**背景**: 月之暗面（Moonshot AI）是中国 AI 初创公司，旗下有 Kimi 聊天机器人。该公司迅速扩张，前几轮融资由美团领投。像 Kimi Work 这样的 AI 代理是基于大语言模型的软件程序，能够自主执行任务、使用工具并与系统交互。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/products/kimi-work">Kimi Work: Next-Gen Desktop AI Agent for Knowledge Workers</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>

</ul>
</details>

**标签**: `#AI`, `#funding`, `#Moonshot AI`, `#startup`, `#valuation`

---

<a id="item-11"></a>
## [中国反网络暴力法草案针对 AI 网暴](https://mp.weixin.qq.com/s/PrzKFhbwjgFEGBPADvFD6Q) ⭐️ 8.0/10

2026 年 7 月 29 日，国家互联网信息办公室公布反网络暴力法征求意见稿，首次纳入专门规制利用 AI 技术制作、传播网络暴力信息的条款，并强化平台的监测与保护责任。 该草案直接针对 AI 生成的网络暴力行为，是中国网络治理的重要一步，可能为其他国家规制 AI 滥用提供先例。 草案共 60 条，明确网络暴力的定义，要求平台建立监测识别机制，并引入人格权侵害禁令和精神损害赔偿等司法保护措施。

telegram · zaihuapd · 7月29日 10:59

**背景**: AI 网络暴力是指利用深度伪造、自动骚扰或 AI 驱动的虚假信息等手段侵害他人的行为。中国民法典已有人格权保护规定，但此次专门针对网络环境和 AI 工具作出细化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.bitig.info/blog/ai-generated-cyber-attacks-weapon/">How AI - Generated Cyber Attacks Became a Weapon | Bitig</a></li>
<li><a href="https://natlawreview.com/article/china-s-new-civil-law-adds-right-publicity">China’s New Civil Law Adds Right of Publicity</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#cyber law`, `#platform liability`, `#China`, `#tech policy`

---