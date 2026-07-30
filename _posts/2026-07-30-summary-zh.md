---
layout: default
title: "Horizon Summary: 2026-07-30 (ZH)"
date: 2026-07-30
lang: zh
---

> 从 38 条内容中筛选出 16 条重要资讯。

---

1. [GitHub 推出堆叠 PR 公开预览](#item-1) ⭐️ 9.0/10
2. [Gemini Robotics 2：为机器人赋予全身智能](#item-2) ⭐️ 9.0/10
3. [OpenAI 将 GPT-5.6 Luna 成本降低 80%](#item-3) ⭐️ 9.0/10
4. [Kimi K3 以创新工程实现前沿性能](#item-4) ⭐️ 9.0/10
5. [Anthropic AI 发现 NIST 后量子候选算法 HAWK 严重弱点](#item-5) ⭐️ 9.0/10
6. [警示：廉价流媒体棒存在安全风险](#item-6) ⭐️ 8.0/10
7. [欧足联及 55 个足协拒绝参加 FIFA 赛事](#item-7) ⭐️ 8.0/10
8. [谷歌通过新 API 在全球 Android 上扩展年龄验证](#item-8) ⭐️ 8.0/10
9. [重构的经济效益与 AI 辅助的局限性](#item-9) ⭐️ 8.0/10
10. [GCC 指导委员会通过 AI 生成贡献政策](#item-10) ⭐️ 8.0/10
11. [Schneier：使用 AI 写作削弱批判性思维](#item-11) ⭐️ 8.0/10
12. [助理教授因会议审稿流程流失三名潜在博士生](#item-12) ⭐️ 8.0/10
13. [MLVC：面向跨平台部署的学习型视频编解码器](#item-13) ⭐️ 8.0/10
14. [俄罗斯指控 Telegram 创始人杜罗夫协助恐怖活动](#item-14) ⭐️ 8.0/10
15. [Google DeepMind 解散 AlphaFold 团队，核心成员加入 Anthropic](#item-15) ⭐️ 8.0/10
16. [欧盟启动 AI 超级工厂招标 拟撬动约 300 亿欧元投资](#item-16) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GitHub 推出堆叠 PR 公开预览](https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/) ⭐️ 9.0/10

GitHub 宣布了堆叠式拉取请求（Stacked PRs）的公开预览，这是一种工作流程，允许开发者将多个相互依赖的拉取请求作为有序栈来管理。该功能旨在将大型变更分解为更小、可审查的拉取请求。 这是一项重大工作流程变革，有望提高代码审查效率，并实现大型功能上的更细粒度协作。它可能成为标准实践，尤其对于使用主干开发的团队而言。 该功能处于公开预览阶段，存在已知问题；例如，合并整个堆栈在很多情况下是损坏的，而压缩合并（squash-and-merge）需要重新审批栈中的每个拉取请求。还提供了 CLI 工具 gh-stack。

hackernews · tomzorz · 7月30日 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49112232)

**背景**: 堆叠式拉取请求将一个大变更分解为一系列较小、逻辑有序的拉取请求，每个请求基于前一个构建。这与单个包含多个提交的大拉取请求不同。该工作流程受到 Linux 内核等大型开源项目中使用的实践的启发，补丁以系列形式发送。GitHub 的实现包括 CLI 和 UI 集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/">Stacked pull requests are now in public preview - GitHub Changelog</a></li>
<li><a href="https://github.github.com/gh-stack/">GitHub Stacked PRs | GitHub Stacked PRs</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：开发者 Steve Klabnik 称赞这是重大变革，而用户 matharmin 则报告了严重错误，对预览的不稳定性感到沮丧。GitHub 团队的 Sameenkarim 征求反馈并指出这是 GitHub 最大规模的发布之一。总体而言，对概念感到兴奋，但对执行存在担忧。

**标签**: `#GitHub`, `#stacked PRs`, `#development workflow`, `#pull requests`, `#version control`

---

<a id="item-2"></a>
## [Gemini Robotics 2：为机器人赋予全身智能](https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/) ⭐️ 9.0/10

Google DeepMind 发布了 Gemini Robotics 2，这是一个新的模型系列，赋予机器人全身智能，实现从脚到指尖的协调控制、高级灵巧操作以及多机器人协作。 这代表了机器人 AI 的重大飞跃，可能使机器人在现实环境中更自然、更自适应地运行，从而加速工业和家庭的自动化进程。 Gemini Robotics 2 基于 Gemini 2.0 大语言模型，是一种视觉-语言-动作模型。目前仅限受信任的测试者使用，包括 Agile Robots、Agility Robotics、Boston Dynamics 和 Enchanted Tools。

hackernews · ai2027 · 7月30日 15:15 · [社区讨论](https://news.ycombinator.com/item?id=49111237)

**背景**: 传统机器人由感知、规划和控制的独立模块控制。Gemini Robotics 2 将这些整合到一个单一的 AI 模型中，能够理解自然语言、感知环境并生成全身动作。这种方法旨在使机器人更有能力处理复杂的非结构化任务，而无需针对特定任务编程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/">Gemini Robotics 2 brings whole body intelligence to robots</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_Robotics">Gemini Robotics</a></li>
<li><a href="https://deepmind.google/models/gemini-robotics/vla/">Gemini Robotics 2 — Google DeepMind</a></li>

</ul>
</details>

**社区讨论**: 社区评论既兴奋又怀疑。一位 DeepMind 研究员赞扬了实验室工作的广度。一些用户将 Google 的努力与 Anthropic 和 OpenAI 相比持正面态度，而另一些用户则因执行器限制而对人形机器人的实用性持怀疑态度。总体情绪是谨慎乐观。

**标签**: `#robotics`, `#deepmind`, `#AI`, `#gemini`, `#whole-body intelligence`

---

<a id="item-3"></a>
## [OpenAI 将 GPT-5.6 Luna 成本降低 80%](https://openai.com/index/advancing-the-price-performance-frontier-with-gpt-5-6/) ⭐️ 9.0/10

OpenAI 宣布推出 GPT-5.6 Luna，其最快且最实惠的模型，成本降低 80%，并在 token 生成效率方面有显著提升。 这一巨大的性价比提升使高质量 AI 推理变得更加普及，可能重塑竞争格局，并支持此前因成本过高而无法实现的新应用。 据社区讨论，80% 的成本降低归功于内核级优化（服务成本降低 20%）以及将 token 生成效率提升超过 15% 的实验。

hackernews · tedsanders · 7月30日 17:15 · [社区讨论](https://news.ycombinator.com/item?id=49112867)

**背景**: GPT-5.6 是 OpenAI 于 2026 年 7 月发布的一个模型系列，包括 Sol（旗舰）、Terra（平衡型）和 Luna（高性价比）。Luna 本就便宜且强大，此次更新使其价格进一步降低至原来的五分之一。该模型可通过 OpenAI API 使用，并设有不同的速率限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/models/gpt-5.6-luna">GPT-5.6 Luna Model | OpenAI API</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>
<li><a href="https://techjournal.org/openai-gpt-5-6-sol-terra-luna">GPT-5.6 Explained: Sol, Terra & Luna (July 2026)</a></li>

</ul>
</details>

**社区讨论**: 社区成员对降价幅度表示惊讶，有人将其比作从拨号上网到宽带的转变。用户指出，区分简单和复杂任务以选择模型仍然是一个难题，而成本节省可以使运行更多并行代理成为可能。

**标签**: `#AI`, `#GPT`, `#cost reduction`, `#performance`, `#OpenAI`

---

<a id="item-4"></a>
## [Kimi K3 以创新工程实现前沿性能](https://www.reddit.com/r/MachineLearning/comments/1vaysjf/how_kimi_k3_engineered_its_way_to_the_frontier_r/) ⭐️ 9.0/10

Moonshot AI 发布了开放权重的 Kimi K3 模型，在 Artificial Analysis 的 580 个模型中排名第四，仅次于 Claude Opus 5、Fable 5 和 GPT-5.6 Sol。该模型引入了 Kimi Delta Attention、Quantile Balancing 和 AgentENV，大幅提升了效率。 Kimi K3 表明，通过创新工程，开放权重模型可以媲美专有的前沿模型，可能使顶级 AI 的获取更加民主化。其在注意力机制、负载均衡和训练基础设施方面的创新可能影响未来的大语言模型设计。 Kimi Delta Attention 在 93 层中的 69 层用每个头的 128x128 矩阵替代了 KV 缓存，将 100 万 token 上下文的显存占用从 104.6 GiB 降至 27.2 GiB。Quantile Balancing 通过单批次的 router 分数裕度使每层 896 个专家负载均衡，取代了固定步长的偏置调节。

reddit · r/MachineLearning · /u/noninertialframe96 · 7月30日 16:37

**背景**: 大型语言模型通常使用注意力机制，需要缓存键值对，这在长上下文下会占用大量显存。混合专家模型将 token 路由到不同专家，但负载不均会影响效率。基于人类反馈的强化学习通常依赖沙盒环境来安全训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://openathena.ai/blog/quantile-balancing/">Mixture of Experts Quantile Balancing: Validated at 32B-A5B (1e22 FLOPs) Scale | Open Athena</a></li>
<li><a href="https://github.com/kvcache-ai/AgentENV">GitHub - kvcache-ai/AgentENV: AgentENV (AENV) is a ...</a></li>

</ul>
</details>

**标签**: `#model architecture`, `#attention mechanism`, `#open-weight`, `#LLM`, `#training infrastructure`

---

<a id="item-5"></a>
## [Anthropic AI 发现 NIST 后量子候选算法 HAWK 严重弱点](https://startupfortune.com/claude-mythos-broke-hawk-and-the-nist-post-quantum-timeline-may-not-survive-it/) ⭐️ 9.0/10

Anthropic 的 Claude Mythos Preview 模型在约 60 小时内发现了 NIST 后量子候选算法 HAWK-256 的严重弱点，将其安全边际从 2^64 降至 2^38，耗费约 10 万美元 API 费用。 这一 AI 驱动的密码分析演示表明，大语言模型能够发现人类专家多年来未察觉的细微密码学缺陷，可能加速后量子密码学过渡，并强调密码灵活性的必要性。 该攻击不是多项式时间攻击，因此更大密钥仍安全，且 HAWK 尚未被 NIST 撤回。研究还包括对七轮 AES-128 的改进攻击，但完整的十轮 AES-128 不受影响。

telegram · zaihuapd · 7月30日 05:47

**背景**: NIST 正在标准化能够抵御未来量子计算机攻击的后量子密码算法。HAWK 是 NIST 后量子数字签名第三轮筛选中的候选算法。安全边际表示破解算法所需的计算量；从 2^64 降到 2^38 意味着该算法比之前认为的弱得多。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arstechnica.com/security/2026/07/mythos-uncovers-crypto-weaknesses-that-went-unknown-for-years/">Mythos attack on 3rd-round PQC algorithm candidate puts it ...</a></li>
<li><a href="https://www.nist.gov/pqc">Post-quantum cryptography | NIST</a></li>
<li><a href="https://csrc.nist.gov/csrc/media/Projects/pqc-dig-sig/documents/round-1/spec-files/hawk-spec-web.pdf">HAWK Specification Document - NIST Computer Security Resource ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#cryptanalysis`, `#post-quantum cryptography`, `#NIST`, `#Anthropic`

---

<a id="item-6"></a>
## [警示：廉价流媒体棒存在安全风险](https://krebsonsecurity.com/2026/07/read-this-before-you-buy-that-tv-streaming-stick/) ⭐️ 8.0/10

Krebs on Security 发布警告称，许多廉价电视流媒体棒预装了用于住宅代理欺诈和广告欺诈的恶意软件和广告软件。 这将导致消费者隐私受到侵犯，家庭网络变成网络犯罪工具，而大型零售商仍在继续销售这些有风险的设备。 这些设备通常运行过时的 Android 版本且无安全补丁，甚至可能被故意配置用于恶意代理服务，使其容易受到远程攻击。

hackernews · speckx · 7月30日 17:04 · [社区讨论](https://news.ycombinator.com/item?id=49112744)

**背景**: 住宅代理欺诈是指通过合法的家庭 IP 地址路由互联网流量以隐藏犯罪活动。廉价的流媒体棒和电视盒常被植入恶意软件，利用所有者的网络连接作为代理，从而实现广告欺诈或其他诈骗行为。尽管多次警告，这些设备仍在主要电商平台出售。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fraudlogix.com/glossary/what-is-a-residential-proxy/">Residential Proxy: Detection Evasion & Fraud Prevention | Fraudlogix</a></li>
<li><a href="https://www.trendmicro.com/vinfo/us/security/news/cybercrime-and-digital-threats/the-rise-of-residential-proxies-and-its-impact-on-cyber-risk-exposure-management">The Rise of Residential Proxies as a Cybercrime Enabler | Trend Micro (US)</a></li>
<li><a href="https://spur.us/platform/residential-proxy-detection">Residential Proxy Detection – Expose Automation & Abuse | Spur</a></li>

</ul>
</details>

**社区讨论**: 评论者就零售商的问责制进行辩论，一些人认为亚马逊和百思买应承担部分责任。用户分享了廉价设备上广告软件的真实经历，许多人指出低价本应是一个危险信号。还有人担心自己的网络连接被用于代理服务。

**标签**: `#security`, `#privacy`, `#streaming devices`, `#malware`, `#consumer alerts`

---

<a id="item-7"></a>
## [欧足联及 55 个足协拒绝参加 FIFA 赛事](https://www.uefa.com/news-media/news/02a7-213a92896eb0-54dfbf454e3b-1000--statement-on-behalf-of-uefa-and-its-55-national-associations/) ⭐️ 8.0/10

欧足联及其 55 个成员协会联合声明，拒绝参加国际足联主办的赛事，理由是担忧贪污、财务动机以及足球商业化日益严重。 这一史无前例的抵制可能重塑全球足球治理结构，有可能催生竞争赛事，并挑战国际足联作为这项运动管理机构的垄断地位。 这一决定是对国际足联提议将世界杯扩军至 64 支球队以及主席因凡蒂诺领导下涉嫌腐败的回应。

hackernews · dickfickling · 7月30日 18:40 · [社区讨论](https://news.ycombinator.com/item?id=49113929)

**背景**: 国际足联是国际足球管理机构，主办世界杯等重大赛事。欧足联是欧洲足球管理机构，负责欧洲俱乐部和国家队。由于国际足联的商业化运作和治理争议，双方关系一直紧张。

**社区讨论**: 评论者普遍支持欧足联的立场，批评国际足联的腐败和商业化。有人建议欧足联自行组织世界杯，也有人担心对球员和球迷的影响。讨论突显了足球治理中的深刻分歧。

**标签**: `#football`, `#FIFA`, `#UEFA`, `#sports governance`, `#corruption`

---

<a id="item-8"></a>
## [谷歌通过新 API 在全球 Android 上扩展年龄验证](https://android-developers.googleblog.com/2026/07/google-play-age-signals-api-safer-experiences.html) ⭐️ 8.0/10

谷歌宣布通过 Play Age Signals API 在全球范围内扩展 Android 上的年龄检查，截至 2026 年底，该 API 允许应用在家长通过 Family Link 同意后请求用户的年龄范围。 此举对隐私、监管和开发者具有重要意义，因为它允许在不要求完整身份验证的情况下提供适龄内容，可能为平台级年龄限制设定新标准。 Age Signals API 目前处于测试阶段，返回年龄范围（例如 0-12、13-15、16-17、18+），需要 Android 6.0 或更高版本；在全球全面推出前已在巴西进行测试。

hackernews · dmantis · 7月30日 10:13 · [社区讨论](https://news.ycombinator.com/item?id=49107950)

**背景**: 年龄验证一直是一个有争议的话题，通常需要账户或身份证上传。谷歌的方法试图通过 Family Link 的家长控制来平衡隐私和安全，让家长分享孩子的年龄范围而不透露确切出生日期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/google/play/age-signals/overview">Play Age Signals overview | Android Developers</a></li>
<li><a href="https://developer.android.com/google/play/age-signals/use-age-signals-api">Use Play Age Signals API (beta) - Android Developers</a></li>
<li><a href="https://cybernews.com/tech/android-developers-age-verification-tool-google/">What is Google’s Android Age Signals API tool? | Cybernews</a></li>

</ul>
</details>

**社区讨论**: 社区评论情绪复杂：有人反对强制创建账户和垄断效应，也有人担心复杂性和不完整的解决方案，有用户讽刺地建议对老年人也进行年龄限制以防范诈骗。

**标签**: `#android`, `#age verification`, `#privacy`, `#regulation`, `#google play`

---

<a id="item-9"></a>
## [重构的经济效益与 AI 辅助的局限性](https://martinfowler.com/articles/exploring-gen-ai/refactoring-economic-benefit.html) ⭐️ 8.0/10

Martin Fowler 的文章定量分析了重构的经济效益，特别探讨了 AI 工具如何提供帮助，但仍需要人类监督以维护代码质量和安全。 这很重要，因为它为 AI 辅助重构提供了基于证据的切实视角，帮助开发者和管理者在投资此类实践时做出明智决策。 文章利用实证测量表明，虽然 AI 可以通过使代码更紧凑来减少令牌消耗，但人类监督对于防止引入错误或丢失概念完整性至关重要。

hackernews · javaeeeee · 7月30日 15:10 · [社区讨论](https://news.ycombinator.com/item?id=49111176)

**背景**: 重构是在不改变外部行为的前提下重组现有代码，以改善非功能属性的过程。大型语言模型等 AI 工具可以提出重构建议，但缺乏对更广泛项目上下文的理解，因此人类审查对安全性至关重要。

**社区讨论**: 评论者赞扬文章具体且量化，'whats_a_quasar'指出这是 AI 评论应有的写作方式。一些人争论 AI 与人类实践的角色，'firasd'强调人在回路中对于理解项目全局上下文不可或缺。

**标签**: `#refactoring`, `#AI`, `#software engineering`, `#economics`, `#best practices`

---

<a id="item-10"></a>
## [GCC 指导委员会通过 AI 生成贡献政策](https://lwn.net/Articles/1086041/) ⭐️ 8.0/10

GCC 指导委员会宣布了一项针对 AI 生成贡献的新政策，要求贡献者证明他们已审查并对任何由生成式 AI 辅助产生的代码负责。 该政策为大型开源项目管理 AI 生成的提交树立了重要先例，旨在维持代码质量和社区信任，同时避免疏远贡献者。 该政策要求披露 AI 使用情况并提供人工审查证明；它还明确欢迎尚未遵守该政策的贡献者，并引导他们合规。

hackernews · arto · 7月30日 11:45 · [社区讨论](https://news.ycombinator.com/item?id=49108685)

**背景**: GCC（GNU 编译器套件）是基石性的开源编译器套件。随着像 GitHub Copilot 这样的生成式 AI 工具普及，维护者面临区分真正的人类贡献与自动化低质量或垃圾提交的挑战，这促使制定明确政策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/niccrane_maintaining-open-source-in-the-age-of-generative-activity-7437947698504249346-CHV8">AI - generated contributions in open source : Challenges... | LinkedIn</a></li>
<li><a href="https://groundy.com/articles/are-ai-generated-prs-killing-open-source/">Are AI - Generated PRs Killing Open Source ? | Groundy</a></li>
<li><a href="https://ai.plainenglish.io/building-community-contributing-to-open-source-projects-with-ai-4e9597afcf50">Building Community: Contributing to Open - Source Projects with AI</a></li>

</ul>
</details>

**社区讨论**: 社区评论显示了广泛的观点：有人赞扬该政策的欢迎语气，有人批评其可执行性，一个令人印象深刻的引用强调了 AI 造成的经济不对称。总体情绪投入但存在分歧。

**标签**: `#GCC`, `#AI policy`, `#open source`, `#software engineering`, `#community discussion`

---

<a id="item-11"></a>
## [Schneier：使用 AI 写作削弱批判性思维](https://simonwillison.net/2026/Jul/30/bruce-schneier/#atom-everything) ⭐️ 8.0/10

Bruce Schneier 认为，使用人工智能完成像政策备忘录这样的写作作业会损害批判性思维技能的发展，因为这些任务被设计成用于思维锻炼的‘健身任务’。 这一观点意义重大，因为它质疑了 AI 在教育和职业培训中的广泛采用，并指出了对学生和员工可能产生的长期认知后果。 Schneier 区分了‘健身任务’（用于技能发展）和‘工作任务’（用于产出），并指出雇主已经注意到毕业生批判性思维的下降。

rss · Simon Willison · 7月30日 18:25

**背景**: Bruce Schneier 是一位知名的安全技术专家和作家，经常撰写关于技术社会影响的文章。他用‘健身任务’的比喻来描述那些主要目的是进行思维锻炼而非产出成果的作业，强调写作过程本身培养批判性思维技能。

**标签**: `#AI`, `#education`, `#critical thinking`, `#Bruce Schneier`, `#writing`

---

<a id="item-12"></a>
## [助理教授因会议审稿流程流失三名潜在博士生](https://www.reddit.com/r/MachineLearning/comments/1vawwb8/i_have_lost_three_and_a_half_potential_phd/) ⭐️ 8.0/10

一位助理教授报告称，已有三名半潜在博士生因对顶级机器学习会议论文投稿过程的负面体验而放弃读博，尽管这些论文获得了正面评审意见。 这凸显了机器学习学术界的一个系统性问题：同行评审流程的高随机性和反复重投令有才华的本科生望而却步，可能阻碍下一代研究人才的培养。 该教授指出，没有明显缺陷的论文在每次重投后会招致越来越随机的评审意见，甚至一篇获得四票弱接受的论文最终也被拒稿。

reddit · r/MachineLearning · /u/AffectionateLife5693 · 7月30日 15:30

**背景**: 顶级机器学习会议如 NeurIPS、ICML 和 ICLR（常被称为'三巨头'）采用同行评审流程，论文由志愿者审阅。该流程因高方差和有时武断的决定而受到批评，催生了'彩票式投稿'这一说法，指那些希望碰运气被接收的低投入论文。这篇帖子说明了该流程如何挫败甚至高质量的论文，并阻碍年轻研究者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.roboflow.com/ai-computer-vision-conferences/">Top AI & Computer Vision Conferences in 2026</a></li>
<li><a href="https://research.com/conference-rankings/computer-science/machine-learning">World's Best Computer Science - Machine Learning & Artificial intelligence Conferences: H-Index Computer Science - Machine Learning & Artificial intelligence Conferences Ranking 2026 | Research.com</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#academia`, `#peer review`, `#PhD`, `#conference review`

---

<a id="item-13"></a>
## [MLVC：面向跨平台部署的学习型视频编解码器](https://www.reddit.com/r/MachineLearning/comments/1vb3xwd/mlvc_multiplatform_learned_video_codec_for/) ⭐️ 8.0/10

研究人员推出了 MLVC，一种多平台学习型视频编解码器，它通过超先验传输熵模型尺度参数，克服了跨平台数值不一致问题，从而在不同 NPU 上实现可靠的解码。 这项工作解决了神经视频编解码器在实际部署中的关键障碍：异构硬件上缺乏位精确计算。通过在 100 FPS 下实现跨 NPU 兼容性，MLVC 使学习型编解码器更接近视频流和通信的实际应用。 MLVC 在消费级 NPU 上实现了 360p/540p 视频约 100 FPS 的编码/解码速度。它通过超先验显式发送熵模型尺度参数，避免了要求神经网络位精确执行，从而确保跨平台的熵解码一致性。

reddit · r/MachineLearning · /u/tanelai · 7月30日 19:40

**背景**: 神经视频编解码器利用深度学习压缩视频，性能可能超越传统手工编解码器（如 H.264/H.265）。然而，其部署受到高功耗和跨平台数值不一致的阻碍：不同 NPU（如 Apple 与 Intel）之间的细微运算差异可能导致熵解码失败。神经处理单元（NPU）是一种专门用于 AI 推理的加速器，但当前 NPU 工具链缺乏标准化的定点运算，导致结果无法位精确。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neural_processing_unit">Neural processing unit - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/neural-processing-unit">What is a neural processing unit (NPU)? - IBM</a></li>

</ul>
</details>

**标签**: `#video codec`, `#machine learning`, `#neural networks`, `#NPU`, `#cross-platform`

---

<a id="item-14"></a>
## [俄罗斯指控 Telegram 创始人杜罗夫协助恐怖活动](https://t.me/zaihuapd/42859) ⭐️ 8.0/10

7 月 29 日，俄罗斯联邦安全局（FSB）依据《刑法》第 205.1 条第 1.1 款指控 Telegram 创始人帕维尔·杜罗夫协助恐怖活动，并将其列入国际通缉名单。 这标志着俄罗斯对科技平台的打压显著升级，开创了因内容审核不力而对科技领袖个人追究责任的先例，并可能进一步加剧数字治理领域的国际紧张关系。 FSB 指控 Telegram 管理层拒不删除被乌克兰情报机构及恐怖组织用于协调破坏、袭击和诈骗的频道、群组和机器人，造成多人伤亡和数十亿卢布损失。

telegram · zaihuapd · 7月30日 03:45

**背景**: FSB 是俄罗斯的主要安全机构，负责反间谍和反恐。Telegram 是一款广泛使用的即时通讯应用，以加密和内容审核宽松著称。俄罗斯当局此前曾因数据合规问题对 Telegram 处以罚款，但此次刑事指控史无前例。

**标签**: `#Telegram`, `#Pavel Durov`, `#FSB`, `#cybercrime`, `#geopolitics`

---

<a id="item-15"></a>
## [Google DeepMind 解散 AlphaFold 团队，核心成员加入 Anthropic](https://www.ft.com/content/61b2953d-ee0d-45de-af6e-a9c1cf524b33?syn-25a6b1a6=1) ⭐️ 8.0/10

Google DeepMind 已解散曾获诺贝尔奖的 AlphaFold 团队，大部分成员被调往其他项目，而三名核心研究人员 John Jumper、Jonas Adler 和 Alexander Pritzel 已离开并加入竞争对手 Anthropic。 此举表明 DeepMind 的战略重心从基础生物学研究转向大型语言模型等其他 AI 应用，同时 Anthropic 获得了重要人才，加强了与 OpenAI 和 Google 在 AI 领域的竞争。 近四分之一的原 AlphaFold 论文作者已完全离开公司，其余人内部转岗至 Gemini、酶设计、核聚变和基因组学等项目，或加入 Alphabet 旗下药物研发公司 Isomorphic Labs。

telegram · zaihuapd · 7月30日 07:45

**背景**: AlphaFold 是 DeepMind 开发的 AI 系统，能够从氨基酸序列预测蛋白质的三维结构，在 2020 年的 CASP14 竞赛中取得了突破性精度。2024 年，Demis Hassabis 和 John Jumper 因 AlphaFold 的工作获得了一半的诺贝尔化学奖。该团队的解散反映了 DeepMind 转向更商业化 AI 项目（如 Gemini）的战略调整。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AlphaFold">AlphaFold</a></li>
<li><a href="https://alphafold.com/">AlphaFold Protein Structure Database</a></li>

</ul>
</details>

**标签**: `#DeepMind`, `#AlphaFold`, `#Anthropic`, `#AI research`, `#protein folding`

---

<a id="item-16"></a>
## [欧盟启动 AI 超级工厂招标 拟撬动约 300 亿欧元投资](https://www.wsj.com/world/europe/eu-opens-call-for-creation-of-local-ai-gigafactories-c286213d) ⭐️ 8.0/10

欧盟启动 AI 超级工厂招标，旨在撬动约 300 亿欧元投资，以增强本地 AI 能力。

telegram · zaihuapd · 7月30日 11:50

**标签**: `#AI infrastructure`, `#European Union`, `#investment`, `#policy`

---