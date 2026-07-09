---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 36 items, 12 important content pieces were selected

---

1. [TypeScript 7.0 Rewritten in Go, Up to 12x Faster Builds](#item-1) ⭐️ 9.0/10
2. [John Deere Must Allow Right to Repair Under FTC Settlement](#item-2) ⭐️ 8.0/10
3. [OpenAI's Analysis Reveals Noise in Coding Benchmarks](#item-3) ⭐️ 8.0/10
4. [Bun Rewrites Runtime from Zig to Rust with AI Assistance](#item-4) ⭐️ 8.0/10
5. [SpaceXAI's Grok 4.5: Faster, Cheaper, Opus-Level AI Model](#item-5) ⭐️ 8.0/10
6. [Decoding the Obfuscated Bash Script on a Uniqlo T-Shirt](#item-6) ⭐️ 8.0/10
7. [Cloudflare Meerkat: First Production Asynchronous Consensus](#item-7) ⭐️ 8.0/10
8. [OpenAI Introduces GPT-Live, Upgrades ChatGPT Voice Mode](#item-8) ⭐️ 8.0/10
9. [LingBot-Video: Open-Source Sparse-MoE Video Diffusion Transformer](#item-9) ⭐️ 8.0/10
10. [Meituan OWL Model Conversations Suspected Leak on GitHub](#item-10) ⭐️ 8.0/10
11. [Smartphone apps identified via leaked radio signals with 99% accuracy](#item-11) ⭐️ 8.0/10
12. [LineageOS Releases Browser-Based Flashing Tool](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [TypeScript 7.0 Rewritten in Go, Up to 12x Faster Builds](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft has officially released TypeScript 7.0, a major version rewritten in Go, achieving up to 12x faster builds compared to TypeScript 6, with specific benchmarks showing a 125.7s build for vscode reduced to 10.6s. This performance improvement significantly reduces developer wait times for large codebases, making TypeScript more viable for massive projects and potentially accelerating CI/CD pipelines, while demonstrating the benefits of rewriting performance-critical compilers in lower-level languages. The new version introduces --checkers and --builders flags to customize parallelism, and provides a compatibility package for coexistence with TypeScript 6; however, toolchains for embedded languages like Vue and Svelte are not yet ready and still require the old version.

hackernews · DanRosenwasser · Jul 8, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48833715)

**Background**: TypeScript is a superset of JavaScript that adds static typing, helping developers catch errors early. Previously, the TypeScript compiler was written in TypeScript itself, which limited its performance for large codebases. Rewriting it in Go allows it to leverage native compilation and multi-threading, enabling the dramatic speed improvements seen in this release.

**Discussion**: Comments celebrate the team's achievement, with users sharing benchmark data and expressing excitement about the speed improvement. Some note their continued appreciation for JSDoc type syntax, while others joke about waiting for a Rust rewrite.

**Tags**: `#TypeScript`, `#performance`, `#Go`, `#compiler`, `#programming languages`

---

<a id="item-2"></a>
## [John Deere Must Allow Right to Repair Under FTC Settlement](https://apnews.com/article/john-deere-right-to-repair-agriculture-equipment-cb7514ffedb95c130a976af661f2bc02) ⭐️ 8.0/10

The Federal Trade Commission (FTC) has reached a settlement with John Deere requiring the company to allow farmers and independent repair shops to repair Deere equipment. The settlement ends years of practice where Deere restricted access to diagnostic software and repair tools. This settlement marks a major victory for the right-to-repair movement, empowering farmers to fix their own tractors and reducing their reliance on expensive dealer repairs. It could set a precedent for other industries, such as electronics and automotive, where similar restrictions exist. Deere must pay $1 million collectively to five states for antitrust enforcement costs and will be under compliance oversight for 10 years. The settlement specifically addresses software locks that prevented owners from diagnosing and fixing issues without dealer authorization.

hackernews · djoldman · Jul 8, 23:37 · [Discussion](https://news.ycombinator.com/item?id=48838876)

**Background**: Modern tractors contain sophisticated computer systems that control everything from engine timing to GPS navigation. Manufacturers like John Deere used digital rights management (DRM) to lock these systems, forcing farmers to use authorized dealers for repairs. This practice has led to farmers hacking their own equipment or buying illicit diagnostic tools from overseas.

<details><summary>References</summary>
<ul>
<li><a href="https://pirg.org/resources/john-deere-and-right-to-repair-over-the-years/">John Deere and Right to Repair over the years - pirg.org</a></li>
<li><a href="https://copperhilltech.com/blog/farmers-are-hacking-their-tractors-because-of-a-right-to-repair-ban/">Farmers Are Hacking Their Tractors Because of a Right to Repair Ban</a></li>

</ul>
</details>

**Discussion**: Comments praised activists like Louis Rossmann for their role in the right-to-repair movement. Some criticized the $1 million fine as trivial compared to Deere's profits, while others debated the broader implications for tech companies and consumer rights.

**Tags**: `#right-to-repair`, `#consumer rights`, `#agriculture technology`, `#FTC`, `#regulatory policy`

---

<a id="item-3"></a>
## [OpenAI's Analysis Reveals Noise in Coding Benchmarks](https://openai.com/index/separating-signal-from-noise-coding-evaluations/) ⭐️ 8.0/10

OpenAI published an analysis showing that the popular coding benchmark SWE-Bench Pro contains significant noise, with many tasks having incomplete or contradictory specifications, and they propose methods to improve evaluation reliability. Accurate coding evaluation is crucial for safely deploying AI models, and flawed benchmarks can mislead about model capabilities, potentially impacting development and safety decisions across the AI industry. OpenAI's team manually reviewed all 798 tasks in SWE-Bench Pro and found that 48% had issues, including missing tests, ambiguous requirements, or bugs in the ground-truth solutions, leading to inflated model performance.

hackernews · sk4rekr0w · Jul 8, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48837396)

**Background**: SWE-Bench Pro is a benchmark designed to evaluate AI models on real-world software engineering tasks, such as fixing bugs or implementing features. The signal-to-noise ratio concept, borrowed from engineering, describes the proportion of meaningful data (signal) versus irrelevant or misleading data (noise) in evaluation results.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/separating-signal-from-noise-coding-evaluations/">Separating signal from noise in coding evaluations - OpenAI</a></li>
<li><a href="https://judyailab.com/en/posts/ai-news-20260709-separating-signal-from-noise-in-coding-evaluations/">How to Distinguish Real Capability from Noise in Code Evaluations</a></li>
<li><a href="https://en.wikipedia.org/wiki/Signal-to-noise_ratio">Signal-to-noise ratio - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism, noting that benchmark flaws were known but undervalued, and called for new metrics that combine efficiency with intelligence, such as measuring accomplishments per API spend. Others highlighted issues like cheating and hardware configuration manipulation.

**Tags**: `#AI evaluation`, `#coding benchmarks`, `#OpenAI`, `#machine learning`, `#benchmark reliability`

---

<a id="item-4"></a>
## [Bun Rewrites Runtime from Zig to Rust with AI Assistance](https://bun.com/blog/bun-in-rust) ⭐️ 8.0/10

Bun, a popular JavaScript runtime, has rewritten its core runtime from Zig to Rust using AI-powered tools Fable and Claude Code, resulting in a 20% smaller binary, improved stability, and 5% better performance. This rewrite demonstrates the potential of AI-assisted code translation to reduce engineering costs and timeline significantly, while also sparking debate about language choice and the future of systems programming for high-performance runtimes. The project was executed by a single engineer using Fable (an automated translation pipeline) and Claude Code for code review and fixes, completing what would have taken a team of engineers a year in a much shorter time frame.

hackernews · afturner · Jul 8, 21:49 · [Discussion](https://news.ycombinator.com/item?id=48837877)

**Background**: Bun is a fast all-in-one JavaScript runtime that bundles, installs, and runs JavaScript and TypeScript. It was originally written in Zig, a systems programming language designed as an improvement to C. Rust is another systems language focused on memory safety and concurrency without garbage collection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/bun: Incredibly fast JavaScript runtime, bundler, test runner, and package manager – all in one</a></li>

</ul>
</details>

**Discussion**: Commenters debated the implications for Zig, with some noting that a naive rewrite away from Zig fixed memory leaks and improved stability, which is concerning for Zig's reputation. Others highlighted the cost-effectiveness of using AI instead of hiring engineers, while some criticized the handling of the transition, such as abandoning fixes for the Zig version.

**Tags**: `#Rust`, `#Zig`, `#AI-assisted development`, `#JavaScript runtime`, `#software engineering`

---

<a id="item-5"></a>
## [SpaceXAI's Grok 4.5: Faster, Cheaper, Opus-Level AI Model](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

SpaceXAI released Grok 4.5, a new AI model that delivers 4x better reasoning efficiency than Opus while costing only $2 per million input tokens and $6 per million output tokens. Grok 4.5's superior token efficiency and lower pricing could disrupt the AI market, but ethical concerns about xAI's trustworthiness may hinder its adoption in sensitive business applications. Grok 4.5 is an 'Opus-class model' that is faster and more token-efficient than competitors; it was trained on trillions of tokens of Cursor data capturing real-world developer interactions.

hackernews · BoumTAC · Jul 8, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48835111)

**Background**: Grok 4.5 is the latest model from xAI, founded by Elon Musk in 2023 and later acquired by SpaceX to become SpaceXAI. The model leverages data from Cursor, an AI coding startup acquired by SpaceXAI, to enhance coding and agentic tasks. Token efficiency refers to the model's ability to generate more useful output per token, reducing overall costs for users.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/news/grok-4-5">Introducing Grok 4.5 | SpaceXAI</a></li>
<li><a href="https://techcrunch.com/2026/07/08/spacexai-releases-grok-4-5-which-elon-describes-as-an-opus-class-model/">SpaceXAI releases Grok 4.5, which Elon describes as an 'Opus-class model' | TechCrunch</a></li>
<li><a href="https://www.axios.com/2026/07/08/spacexai-grok-new-model">Scoop: SpaceXAI launches new model, Grok 4.5</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise Grok 4.5's speed and cost-effectiveness, while others express distrust due to xAI's political alignment and ethical issues, such as insufficient moderation of CSAM content. Technical users compare it favorably against GPT and Opus on benchmarks.

**Tags**: `#AI`, `#LLM`, `#Grok`, `#xAI`, `#machine learning`

---

<a id="item-6"></a>
## [Decoding the Obfuscated Bash Script on a Uniqlo T-Shirt](https://tris.sherliker.net/blog/obfuscated-self-evaluating-bash-script-by-cdn-akamai-being-supplied-to-consumers-via-retail-stores/) ⭐️ 8.0/10

Tristan Sherliker's blog post decodes the obfuscated bash script printed on a Uniqlo t-shirt, revealing it to be a self-evaluating script that prints a mathematical formula when executed. This example showcases creative bash obfuscation, sparking community discussion about code aesthetics, typography, and the intersection of programming with fashion. The script uses self-evaluating techniques common in bash obfuscation, and the shirt's typography uses Roboto Mono font with optical kerning, making OCR difficult.

hackernews · speerer · Jul 8, 08:46 · [Discussion](https://news.ycombinator.com/item?id=48829312)

**Background**: Bash obfuscation involves making shell scripts intentionally hard to read, often by encoding, compressing, or using variable substitution. Self-evaluating scripts execute code that is constructed at runtime. The Uniqlo t-shirt, designed in collaboration with Akamai, features the script as a fashion statement.

<details><summary>References</summary>
<ul>
<li><a href="https://vuink.com/post/gevf-d-dfureyvxre-d-darg/blog/obfuscated-self-evaluating-bash-script-by-cdn-akamai-being-supplied-to-consumers-via-retail-stores">Obfuscated, self-evaluating bash script by CDN Akamai being ...</a></li>
<li><a href="https://github.com/Bashfuscator/Bashfuscator">GitHub - Bashfuscator/Bashfuscator: A fully configurable and ...</a></li>
<li><a href="https://www.baeldung.com/linux/bash-obfuscate-script">How to Obfuscate a Bash Script to Make It Unreadable - Baeldung</a></li>

</ul>
</details>

**Discussion**: Commenters praised the cleverness of the design. Some noted the font is Roboto Mono but the kerning is optical, breaking monospace consistency. Others linked to similar works like Martin Kleppe's Quine Clock. There was also discussion about the difficulty of OCR and curiosity whether an LLM wrote the original script.

**Tags**: `#obfuscation`, `#bash`, `#hackernews`, `#t-shirt`, `#Uniqlo`

---

<a id="item-7"></a>
## [Cloudflare Meerkat: First Production Asynchronous Consensus](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 8.0/10

Cloudflare Research launched Meerkat, a globally distributed consensus service based on the QuePaxa algorithm, which is the first production implementation of an asynchronous leaderless consensus protocol. The service aims to provide strong consistency and fault tolerance for key-value stores and other applications. This marks a significant milestone as asynchronous consensus, which does not rely on timeouts and can tolerate extreme network delays, moves from research to real-world deployment. It could improve reliability for globally distributed systems that struggle with leader-based protocols like Raft under adverse network conditions. Meerkat uses QuePaxa, which employs hedging—sending redundant proposals to multiple proposers—to achieve liveness without timeouts, enabling progress even during network partitions or delays. However, it requires global consensus for every read operation, which may increase read latency compared to systems that optimize for local reads.

hackernews · bobnamob · Jul 8, 13:18 · [Discussion](https://news.ycombinator.com/item?id=48831565)

**Background**: Most consensus algorithms in production, like Paxos and Raft, are partially synchronous: they rely on timeouts to detect failures and assume network delays are bounded. Asynchronous consensus algorithms like QuePaxa avoid timeouts entirely, making them robust to unbounded delays but historically too inefficient for practical use. QuePaxa, published at SOSP 2023, introduced techniques like adaptive hedging to achieve competitive performance in normal cases while maintaining resilience in worst-case scenarios.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/meerkat-introduction/">Introducing Meerkat: an experiment in global consensus</a></li>
<li><a href="https://bford.info/pub/os/quepaxa/quepaxa.pdf">QuePaxa: Escaping the Tyranny of Timeouts in Consensus QuePaxa: Escaping the Tyranny of Timeouts in Consensus GitHub - dedis/quepaxa: This is the code repository for ... QuePaxa: Escaping the Tyranny of Timeouts in Consensus Post by @cloudflare.social — Bluesky Artifact Review Summary: QuePaxa: Escaping the tyranny of ...</a></li>

</ul>
</details>

**Discussion**: Commenters noted that comparing Meerkat (leaderless) to Raft (leader-based) is confusing, and highlighted the novelty of QuePaxa being asynchronous. Some questioned the trade-off of consensus on every read, while others appreciated the value for messy networks where leader-based protocols suffer.

**Tags**: `#distributed systems`, `#consensus algorithms`, `#Cloudflare`, `#QuePaxa`, `#asynchronous consensus`

---

<a id="item-8"></a>
## [OpenAI Introduces GPT-Live, Upgrades ChatGPT Voice Mode](https://simonwillison.net/2026/Jul/8/introducing-gptlive/#atom-everything) ⭐️ 8.0/10

OpenAI has announced GPT-Live, a new model powering ChatGPT's voice mode that can delegate complex tasks to GPT-5.5 in the background while maintaining conversation flow. This upgrade significantly improves the usefulness of ChatGPT's voice mode, enabling real-time, natural conversations that can handle web search, reasoning, and other complex work without interruption. GPT-Live is currently available in the iPhone app and uses GPT-5.5 as its frontier model, with plans to continuously update as new models are released. A bug causing inappropriate laughter was reported and reportedly fixed.

rss · Simon Willison · Jul 8, 23:20

**Background**: ChatGPT's previous voice mode was based on an older GPT-4o era model with a knowledge cut-off in 2024, limiting its usefulness. GPT-Live represents a new generation of voice models designed for more natural human-AI interaction, capable of multitasking by offloading complex queries to a more powerful model like GPT-5.5.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT-Live | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT‑5.5 - OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-Live`, `#ChatGPT`, `#voice mode`, `#AI update`

---

<a id="item-9"></a>
## [LingBot-Video: Open-Source Sparse-MoE Video Diffusion Transformer](https://www.reddit.com/r/MachineLearning/comments/1ur0bxq/lingbotvideo_sparsemoe_video_diffusion/) ⭐️ 8.0/10

LingBot-Video is a 13B-parameter (1.4B active) sparse mixture-of-experts video diffusion transformer, post-trained with reinforcement learning using a VLM-graded physical plausibility reward. It is released as open source with weights, code, and a Diffusers/SGLang stack, and includes an action-to-video mode for robot rollout prediction. This model represents a significant step in open-source video generation for robotics, combining sparse MoE efficiency with RL-based physical plausibility rewards. However, it raises critical questions about whether VLM-graded rewards can reliably judge physics, and whether video generation alone qualifies as a true world model for robot policy evaluation. LingBot-Video uses a single-stream diffusion transformer with DeepSeek-V3-style sparse MoE (128 experts, top-8 routing). It is post-trained with six rewards including a physical-plausibility reward graded by a VLM from sampled frames, and they add real-video negatives to mitigate reward hacking.

reddit · r/MachineLearning · /u/Savings-Display5123 · Jul 8, 17:58

**Background**: Mixture of Experts (MoE) is a technique where a model uses multiple specialized sub-networks (experts) and a routing mechanism to activate only a subset per input, enabling larger total capacity with lower computational cost. Sparse MoE, as in DeepSeek-V3, activates only a fraction of experts per token. Action-conditioned world models predict future video frames given robot actions, serving as planners or evaluators in robotics. LingBot-Video is positioned as such a model, but only video generation results are shown, no closed-loop robot evaluations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://arxiv.org/abs/2606.04463">OSCAR: Omni-Embodiment Action-Conditioned World Model for ...</a></li>

</ul>
</details>

**Discussion**: The Reddit post author invites critique, specifically questioning whether a VLM can be a defensible judge of physics or if it leads to reward hacking, and where the line is between a video generator and a world model without closed-loop robot numbers. The author expresses genuine desire for community input on these issues.

**Tags**: `#video diffusion`, `#sparse MoE`, `#reinforcement learning`, `#world model`, `#open source`

---

<a id="item-10"></a>
## [Meituan OWL Model Conversations Suspected Leak on GitHub](https://github.com/gumusserv/ProducerBenchV2/blob/83cad6007ef3fe8df33386e8f43738fe62337e16/parsed_source_data/data/) ⭐️ 8.0/10

A suspected data leak of conversations from Meituan's free test OWL (LongCat) model was discovered on a GitHub repository, which has since been taken down. The leak was spotted by a Discord bot token scanner, prompting token resets. This incident highlights recurring security and privacy risks in deploying large language models, especially when user conversations are logged and exposed. It underscores the critical need for enterprises to protect sensitive data in AI workflows and for users to avoid sharing credentials or proprietary information with AI models. The repository was publicly accessible at least as of July 7, 2026, according to user screenshots. The leaked data reportedly included conversations from Meituan's OWL model, which is a test model on OpenRouter, and a Discord bot token scanner flagged the exposure.

telegram · zaihuapd · Jul 8, 13:35

**Background**: Meituan recently open-sourced LongCat-2.0, a 1.6 trillion-parameter MoE model with 48 billion active parameters per token, which powers the OWL model on OpenRouter. OpenRouter is a unified API platform providing access to hundreds of large language models from different providers. Similar data leaks have occurred with other AI providers like Google and DeepSeek, where user conversations are used for model improvement.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geopolitechs.org/p/longcat-20-chinas-most-unexpected">LongCat-2.0: China's Most Unexpected AI Model</a></li>
<li><a href="https://venturebeat.com/technology/meituan-open-sources-longcat-2-0-the-1-6t-near-frontier-agentic-coding-model-thats-been-leading-openrouter-trained-entirely-on-chinese-chips">Meituan open sources LongCat-2.0, the 1.6T, near-frontier agentic coding model that's been leading OpenRouter — trained entirely on Chinese chips | VentureBeat</a></li>

</ul>
</details>

**Tags**: `#data leak`, `#AI security`, `#privacy`, `#large language models`, `#Meituan`

---

<a id="item-11"></a>
## [Smartphone apps identified via leaked radio signals with 99% accuracy](https://www.scmp.com/news/china/science/article/3359688/chinese-researchers-find-peephole-any-smartphone-its-leaked-radio-signal) ⭐️ 8.0/10

Chinese researchers developed a non-contact technique that identifies smartphone apps by analyzing leaked low-frequency electromagnetic signals, achieving up to 99.07% accuracy on iPhone 15 Pro, Xiaomi 15 Pro, and OPPO Reno 13. This technique represents a novel side-channel attack that works even when the device is offline, in airplane mode, encrypted, or locked, posing significant privacy risks and offering new capabilities for digital forensics without physical access. The research tested apps including Douyin (TikTok), WeChat video calls, Baidu Maps, SMS, browser, camera, and cloud storage. The method requires no access to the operating system or stored data, relying solely on the unique electromagnetic signatures of each app.

telegram · zaihuapd · Jul 8, 16:05

**Background**: Side-channel attacks exploit physical emanations like electromagnetic radiation to infer sensitive information. Smartphones emit low-frequency electromagnetic signals during operation, and different apps generate distinct patterns. This non-contact digital forensics technique captures those signals from a distance, enabling app identification without touching the device.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ckhq.net/html/6c1af61946e47994a7d682373d5f7757.html">中国科研团队研发非接触式智能手机应用识别技术，准确率达99.07%</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/25590891831">什么是 Side Channel Attack（侧信道攻击）？ - 知乎</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#smartphone`, `#electromagnetic signals`, `#side-channel attack`

---

<a id="item-12"></a>
## [LineageOS Releases Browser-Based Flashing Tool](https://www.androidauthority.com/lineageos-summertime-update-2026-3685112/) ⭐️ 8.0/10

LineageOS has released Lineage Flash Tools, a web-based tool that allows users to flash custom ROMs directly from a browser without needing to install adb and fastboot locally. The team also announced that development of LineageOS 24 based on Android 17 has begun. This lowers the barrier for installing custom ROMs, making it more accessible to less technical users. The upcoming Android 17-based LineageOS 24 shows ongoing commitment to supporting the latest Android versions. The tool supports Fastboot, ADB, and Samsung's Odin protocol, and requires a WebUSB-capable browser like Chrome or Edge. It must be used in conjunction with device-specific Wiki installation guides and does not fully replace traditional flashing methods.

telegram · zaihuapd · Jul 9, 01:46

**Background**: WebUSB is a JavaScript API that allows web applications to communicate with USB devices securely, enabling browser-based flashing. Samsung devices typically use Odin protocol instead of fastboot for firmware flashing. A/B OTA streaming installation downloads only the needed parts of an update package to save space and speed up the process.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebUSB">WebUSB - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Odin_(firmware_flashing_software)">Odin (firmware flashing software) - Wikipedia</a></li>
<li><a href="https://source.android.com/docs/core/ota/ab">A/B (seamless) system updates | Android Open Source Project</a></li>

</ul>
</details>

**Tags**: `#LineageOS`, `#Android`, `#custom ROM`, `#WebUSB`, `#flashing`

---