---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 41 items, 7 important content pieces were selected

---

1. [Keyv and Related npm Packages Hit by Active Shai-Hulud Supply Chain Attack](#item-1) ⭐️ 9.0/10
2. [Waymo Opens Driverless Ride-Hail to Everyone in Dallas](#item-2) ⭐️ 8.0/10
3. [DeepSeek V4 Flash Runs on a Single AMD MI300X](#item-3) ⭐️ 8.0/10
4. [Lilian Weng: Harness Engineering as New Frontier for Self-Improving Agents](#item-4) ⭐️ 8.0/10
5. [Huawei unveils Tao's Law, a time-scaling alternative to Moore's geometric scaling](#item-5) ⭐️ 8.0/10
6. [Google Builds $200B Wall Street Financing Machine for Anthropic AI Chips](#item-6) ⭐️ 8.0/10
7. [China's First Mandatory L3/L4 Autonomous Driving Standard Approved, Effective 2027](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Keyv and Related npm Packages Hit by Active Shai-Hulud Supply Chain Attack](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 9.0/10

A new wave of the Shai-Hulud worm has compromised the widely used npm package Keyv and hundreds of other packages, using preinstall scripts to steal credentials and self-propagate across writable npm packages and GitHub repositories. Because Keyv is a widely adopted key-value storage library with more than 1,700 dependent projects, this attack can cascade through the JavaScript ecosystem, exposing developer credentials, cloud secrets, and downstream repositories to theft and further compromise. It underscores how a single compromised dependency can severely undermine trust in open-source software. The malicious release uses a preinstall script that harvests repository, registry, cloud, and private-key credentials, then leverages available npm publishing access to poison more packages. The Keyv repository also retained separate Claude Code and VS Code workspace hooks that execute the payload once a developer trusts the workspace.

hackernews · cimi_ · Aug 4, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49166874)

**Background**: Shai-Hulud is a self-replicating npm worm that first came to light in September 2025 and has since compromised hundreds of packages. It typically spreads by stealing maintainer credentials and publishing malicious versions of legitimate packages. npm packages frequently use pre- and post-install scripts to run code during installation, which attackers abuse to execute malware on developer and CI machines before any audit occurs. Because packages depend on many transitive dependencies, one compromised package can quickly poison thousands of projects.

<details><summary>References</summary>
<ul>
<li><a href="https://research.jfrog.com/post/shai-hulud-is-back-august/">Major Shai Hulud campaign strikes npm again, affecting keyv and 400+ packages - JFrog Security Research</a></li>
<li><a href="https://thehackernews.com/2026/08/keyv-linked-npm-worm-poisons-hundreds.html">Keyv-Linked npm Worm Poisons Hundreds of Packages, Plants Claude Code and VS Code Hooks</a></li>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem | CISA</a></li>

</ul>
</details>

**Discussion**: Commenters reacted with alarm and frustration, calling for a moratorium on pre/post-install hooks and treating any newly introduced install hook with extreme suspicion. Some shared practical mitigations, such as setting npm's min-release-age=5 in .npmrc, while others asked for commands to scan node_modules and pnpm stores. Several also lamented the fragility of the dependency system and the difficulty of cleaning up knock-on compromises.

**Tags**: `#security`, `#npm`, `#supply chain attack`, `#open source`, `#malware`

---

<a id="item-2"></a>
## [Waymo Opens Driverless Ride-Hail to Everyone in Dallas](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 8.0/10

Waymo announced that its driverless ride-hailing service is now open to everyone in Dallas, Texas. This makes Dallas the latest major metro area where anyone can hail a fully autonomous vehicle. This expansion brings commercial autonomous vehicles to a large, car-dependent, low-density metro area, offering an alternative to limited public transit. It could also influence urban policy, with some arguing driverless cars could reduce parking demand and support affordable housing. The service is available via the Waymo app, and a Google support page shows the Dallas service area. Waymo is a subsidiary of Alphabet, formerly the Google self-driving car project.

hackernews · xnx · Aug 4, 18:29 · [Discussion](https://news.ycombinator.com/item?id=49172836)

**Background**: Waymo is an autonomous vehicle company and the leading commercial operator of robotaxis in the United States. It began as Google's self-driving car project and already operates in cities such as Phoenix, San Francisco, and Los Angeles. Dallas-Fort Worth is among the top five U.S. metroplexes, but it is extremely low density and car-centric, with few public transit options, making it a significant new testing ground.

<details><summary>References</summary>
<ul>
<li><a href="https://waymo.com/">Waymo - Self-Driving Cars - Autonomous Vehicles - Ride-Hail</a></li>
<li><a href="https://builtin.com/articles/waymo-robotaxis">Waymo Explained: Alphabet’s Autonomous Vehicle Company | Built In</a></li>

</ul>
</details>

**Discussion**: Commenters shared positive hands-on experiences, noting Waymos have become normal and cause fewer incidents than human drivers, while some mentioned occasional stuck situations. One commercial real estate professional argued driverless cars are an effective affordable housing policy, while another expressed surprisingly low hype despite Waymo being advanced consumer-interactive robots.

**Tags**: `#autonomous vehicles`, `#Waymo`, `#transportation`, `#urban policy`, `#AI`

---

<a id="item-3"></a>
## [DeepSeek V4 Flash Runs on a Single AMD MI300X](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

A technical guide and benchmark demonstrates DeepSeek V4 Flash running on a single AMD MI300X GPU with good performance, exceeding 150 tokens per second, while reducing the context window from the original 1 million tokens to 256K tokens. This matters because it shows that a large Mixture-of-Experts model can be deployed on a single AMD accelerator, lowering hardware barriers and offering a practical tradeoff analysis for inference. It also underscores AMD's growing presence in AI inference and the importance of balancing model quantization and context length. The benchmark preserves the model's full inference weights without aggressive quantization and still achieves over 150 tokens per second, with the main sacrifice being the context window reduced to 256K tokens. The MI300X is an OAM module with 192GB of HBM3 memory, while the lower-memory PCIe-based MI350P (144GB) should also fit the model because its 256 Mixture-of-Experts (MoE) experts use native MXFP4 quantization.

hackernews · zhoutong · Aug 4, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49166386)

**Background**: DeepSeek V4 Flash is a Mixture-of-Experts (MoE) large language model with 284 billion total parameters, part of the DeepSeek V4 family that also includes the 1.6-trillion-parameter V4-Pro. The model was trained for a 1M-token context window and serves as a cost-efficient alternative to the larger Pro model; an updated checkpoint significantly improved its agentic capabilities. The AMD Instinct MI300X is AMD's flagship data-center accelerator, featuring 192GB of HBM3 memory at 5.3 TB/s bandwidth and available through cloud providers like RunPod. Quantization techniques such as MXFP4 reduce memory footprint, enabling large models to fit on a single GPU while sometimes trading off performance on long-context tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek V 4 Explained: V 4 -Pro 1.6T vs V 4 - Flash 284B (2026)</a></li>
<li><a href="https://canitrun.dev/gpus/mi300x/">AMD Instinct MI 300 X — 192 GB VRAM: Which LLMs... — CanItRun</a></li>
<li><a href="https://www.remio.ai/post/deepseek-v4-flash-reportedly-outperforms-its-larger-sibling-on-agent-tasks">DeepSeek V 4 Flash Reportedly Outperforms Its Larger Sibling on...</a></li>

</ul>
</details>

**Discussion**: Commenters were largely positive, praising the honest tradeoff analysis: the configuration retains full-precision weights and delivers over 150 tokens per second, with only the context window shrinking from 1M to 256K. Hardware concerns were raised, noting that the MI300X is typically sold as an 8-GPU server costing around €250K, while the PCIe-based MI350P with 144GB should also run the model thanks to native MXFP4 quantization. Others pointed to prior art like DwarfStar that uses even less memory and recommended renting MI300X instances via HotAisle for experimentation.

**Tags**: `#deepseek`, `#amd`, `#mi300x`, `#llm-inference`, `#quantization`

---

<a id="item-4"></a>
## [Lilian Weng: Harness Engineering as New Frontier for Self-Improving Agents](https://lilianweng.github.io/posts/2026-07-04-harness/) ⭐️ 8.0/10

Lilian Weng's blog post introduces harness engineering—the practice of optimizing the tools, skills, prompts, and scaffolding around an AI agent—as a fresh direction for enabling agents to self-improve. The post reframes self-improvement as a problem of optimizing the harness, not just the model weights. As model capabilities plateau, improving the harness can deliver significant gains in agent performance, cost efficiency, and reliability. This shift may reshape how organizations scale AI coding agents and how the field approaches self-improvement beyond weight training. The concept of harness engineering originates from software testing, where a test harness controls and observes a system; in agents, it covers the entire operating environment. Practitioners highlight levers such as building fitness functions for codebases, using production traces to find real issues, letting agents write their own tools (e.g., cutting context loading from 20k tokens across 15 calls to 800 tokens in a single call), and applying eval/test splits to avoid reward hacking.

hackernews · tosh · Aug 4, 06:17 · [Discussion](https://news.ycombinator.com/item?id=49164896)

**Background**: Harness engineering is an emerging discipline that designs, builds, and maintains the infrastructure orchestrating AI agents at scale, including prompts, tools, skills, and evaluation loops. It differs from prompt engineering, which optimizes a single exchange, and context engineering, which manages the context window, by instead building the world the agent operates in. The term 'harness' is borrowed from software engineering, where test harnesses control and observe a system under test.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/harness-engineering-discipline-decides-how-smart-your-parag-patil-uqhzf">Harness Engineering : The Discipline That Decides How Smart Your...</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-harness-engineering-beyond-prompt-context-engineering">How Stripe Ships 1,300 AI PRs a Week: Harness Engineering</a></li>
<li><a href="https://outcomeschool.com/blog/harness-engineering-in-ai">In this blog, we will learn about Harness Engineering in AI .</a></li>

</ul>
</details>

**Discussion**: Practitioner comments show strong hands-on interest: one shares that automating harness research with production traces proved surprisingly powerful, while another calls for a generic, accurate fitness function for codebases to enable agent-driven self-optimization. Others see a paradigm shift from training weights toward training prompts and code, and one asks when harnesses will generate their own RLHF/DPO training data for LoRA fine-tuning. A lighter comment jokes about the ongoing 'quest for Torment Nexus.'

**Tags**: `#AI engineering`, `#LLM agents`, `#self-improvement`, `#harness optimization`

---

<a id="item-5"></a>
## [Huawei unveils Tao's Law, a time-scaling alternative to Moore's geometric scaling](https://t.me/zaihuapd/42966) ⭐️ 8.0/10

At the 2026 International Symposium on Circuits and Systems (ISCAS 2026) in Shanghai, Huawei semiconductor chief He Tingbo formally proposed "Tao's Law" (τ law), which replaces geometric scaling with time scaling as a new guiding principle for semiconductor advancement. Huawei claims it has designed and mass-produced 381 chips under this principle over the past six years, and will release a new Kirin chip using logic folding technology this autumn. Tao's Law presents a potential paradigm shift for the semiconductor industry as Moore's Law approaches physical and economic limits, offering an alternative path that does not rely solely on shrinking transistor dimensions. If validated, it could reshape chip design strategies and industry competition, particularly for Huawei and China's semiconductor ecosystem under export restrictions. Tao's Law targets systematically reducing the time constant (τ) through techniques such as logic folding, which compresses signal propagation delay and thereby increases effective transistor density. Huawei projects that high-end chips based on this law could reach transistor density equivalent to a 1.4nm process by 2031, and He Tingbo also published a detailed paper, "A Time Scaling Theory for Multi-Layer Electronic Systems," on a Chinese Academy of Sciences preprint platform.

telegram · zaihuapd · Aug 4, 08:04

**Background**: Moore's Law has driven semiconductor progress for over half a century by shrinking transistor geometries, but it is now approaching physical limits where further miniaturization becomes extremely costly and difficult. "Time scaling" instead compresses the time constant of signal propagation across device, circuit, chip, and system levels, aiming to continue performance and density gains without aggressive lithographic scaling. Logic folding is one such technique that optimizes signal paths, reuses logic modules, and reduces latency.

<details><summary>References</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260525/herald/1573642c437a5e4e76a15fc1c40f0a35.html">华为提出的“韬定律”是什么？跟摩尔定律有什么不同？ - 21经济网</a></li>
<li><a href="https://www.guancha.cn/economy/2026_05_25_818313.shtml">何庭波万字论文，详述华为“韬定律”-观察者网</a></li>
<li><a href="https://caifuhao.eastmoney.com/news/20260525164059876078810">从非系统观下的“几何压缩”到系统观下的“时间压缩”：什么是半导体的“逻辑折叠技术”？_财富号_东方财富网</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#Huawei`, `#chip design`, `#scaling`, `#logic folding`

---

<a id="item-6"></a>
## [Google Builds $200B Wall Street Financing Machine for Anthropic AI Chips](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

The Financial Times reports that Google has quietly assembled one of the largest infrastructure financing structures ever, involving roughly $200 billion in contracts to deliver over $150 billion in AI chips to Anthropic. Participants include Broadcom, Apollo, Blackstone, Morgan Stanley, and several crypto miners. This financial engineering could reshape how AI compute is funded, moving massive hardware investments off balance sheets and spreading risk across Wall Street institutions. It highlights the enormous capital needed to scale frontier AI and may influence how other hyperscalers finance AI infrastructure. In June, the special purpose vehicle Compute SPV completed its first transactions, buying about $35 billion in hardware, roughly 1 gigawatt of compute or 1 million TPUs. The structure resembles vendor financing used by Boeing and GE: Google guarantees data centers, Broadcom buys and helps finance chips, and Apollo and Blackstone purchase hardware to lease back to Anthropic.

telegram · zaihuapd · Aug 4, 10:52

**Background**: A special purpose vehicle (SPV) is a separate legal entity used to isolate financial risk, common in large infrastructure projects. Tensor Processing Units (TPUs) are Google's custom application-specific integrated circuits (ASICs) designed to accelerate machine learning workloads. Because Anthropic has no credit rating, the deal spreads risk across multiple investors instead of placing hundreds of billions of dollars on any single balance sheet.

<details><summary>References</summary>
<ul>
<li><a href="https://www.investopedia.com/terms/s/spv.asp">investopedia.com/terms/s/ spv .asp</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tensor_Processing_Unit">Tensor Processing Unit - Wikipedia</a></li>
<li><a href="https://345tool.com/news/apollo-and-blackstone-raise-36b-to-lease-google-tpus-for-anthropic-in-largest-ch-2">Apollo and Blackstone Raise $36B to Lease Google... | 345tool News</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#Anthropic`, `#Google`, `#financing`, `#cloud computing`

---

<a id="item-7"></a>
## [China's First Mandatory L3/L4 Autonomous Driving Standard Approved, Effective 2027](https://t.me/zaihuapd/42972) ⭐️ 8.0/10

China's Ministry of Industry and Information Technology (MIIT) has completed and submitted the draft of the mandatory national standard 'Safety Requirements for Intelligent Connected Vehicle Autonomous Driving Systems.' The draft, open for public comment from June 17, proposes implementation on July 1, 2027. This is a major regulatory milestone that shifts China's autonomous driving oversight from vague concept-level encouragement to enforceable safety requirements. It will force automakers to rigorously prove safety via a Safety Case mechanism, affecting L3/L4 vehicle development, AI safety validation, and industry practices. The standard applies to M- and N-category vehicles equipped with L3 and L4 systems, but excludes automated parking systems. It introduces a Safety Case dossier mechanism (claim-argument-evidence) and sets distinct requirements for L3 human-machine handover and L4 autonomous risk handling.

telegram · zaihuapd · Aug 4, 13:06

**Background**: L3 (conditionally automated) and L4 (highly automated) driving are defined by the SAE levels of driving automation, where the system handles driving tasks under specific conditions. Historically China lacked a mandatory national safety standard for these levels, relying on voluntary guidelines and group standards. Accidents involving autonomous vehicles globally, such as those by Waymo and Uber, have highlighted that demonstrating functionality is not the same as demonstrating safety, prompting regulators to adopt structured safety assurance approaches like Safety Case.

<details><summary>References</summary>
<ul>
<li><a href="https://www.autohome.com.cn/news/202608/1316205.html">autohome.com.cn/news/202608/1316205.html</a></li>
<li><a href="https://www.163.com/dy/article/L01347E80547KOTE.html">163.com/dy/article/L01347E80547KOTE.html</a></li>
<li><a href="https://m.163.com/dy/article/K1BTJR1H0514R9KQ.html">m.163.com/dy/article/K1BTJR1H0514R9KQ.html</a></li>

</ul>
</details>

**Tags**: `#autonomous-driving`, `#regulation`, `#safety-standards`, `#AI`, `#automotive`

---