---
layout: default
title: "Horizon Summary: 2026-07-27 (EN)"
date: 2026-07-27
lang: en
---

> From 32 items, 12 important content pieces were selected

---

1. [vLLM v0.26.0 Released with Inkling Model and DeepSeek-V4 Optimizations](#item-1) ⭐️ 9.0/10
2. [Anthropic Calls for Safety Testing of Open-Weights Models](#item-2) ⭐️ 9.0/10
3. [Moonshot AI Releases 3T Parameter Open-Weight Kimi-K3](#item-3) ⭐️ 9.0/10
4. [Fastjson 1.x critical RCE without autoType or gadgets](#item-4) ⭐️ 9.0/10
5. [SMIC Tests China's First Domestic DUV Lithography Machine](#item-5) ⭐️ 9.0/10
6. [Moonshot AI to Open-Source Kimi-K3, 3T-Parameter Model](#item-6) ⭐️ 9.0/10
7. [Judge Rejects Google's DMCA Claim to Block Scraping](#item-7) ⭐️ 8.0/10
8. [Libsm64: Turning Super Mario 64 into a Reusable Library](#item-8) ⭐️ 8.0/10
9. [Bun's Rust Rewrite Progress and v1.4 Delay](#item-9) ⭐️ 8.0/10
10. [CXMT Soars 471.59% on STAR Market Debut, Largest IPO Ever](#item-10) ⭐️ 8.0/10
11. [AI-Driven Price Hikes Strain Huawei-CXMT Relations](#item-11) ⭐️ 8.0/10
12. [Google Reveals Gemini 4, Its Most Ambitious Pretraining Project, Expected Late 2026](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 Released with Inkling Model and DeepSeek-V4 Optimizations](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 introduces the new Inkling model family with full support stack, significant performance optimizations for DeepSeek-V4 (including a specialized routing kernel achieving 2.94% E2E TPOT improvement), fp32 lm_head support, flexible attention backends, and maturity for KV offloading and tiered secondary storage. This release significantly improves inference performance and flexibility for cutting-edge models like DeepSeek-V4 and the new Inkling family, solidifying vLLM's position as a top-tier open-source LLM inference engine. The community-driven nature with 411 commits from 212 contributors highlights the active ecosystem. Key technical details include piecewise CUDA graph support for the Inkling model, Hopper FA4 relative attention, MTP=1 speculative decoding, LoRA support, and standard ModelOpt NVFP4 quantization. For DeepSeek-V4, optimizations include fused_topk_bias (1.5-2x kernel speedup) and redundant repeat/copy removal (1.8% E2E TPOT).

github · khluu · Jul 27, 01:06

**Background**: vLLM is a high-throughput, memory-efficient inference engine for large language models, widely used in production and research. The new Inkling model is an open-weights generalist multimodal model released by Thinking Machines Lab under Apache 2.0 license. Flash Attention 4 (FA4) is the latest version of the efficient attention algorithm optimized for Hopper GPUs, improving over FA3 with CuTeDSL support.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/cuda_graphs/">CUDA Graphs - vLLM</a></li>
<li><a href="https://pytorch.org/blog/flexattention-flashattention-4-fast-and-flexible/">FlexAttention + FlashAttention-4: Fast and Flexible – PyTorch</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#model optimization`, `#open source`, `#GPU`

---

<a id="item-2"></a>
## [Anthropic Calls for Safety Testing of Open-Weights Models](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 9.0/10

Anthropic published a policy statement arguing that open-weights AI models should not be banned, but should undergo mandatory safety testing for all sufficiently capable models, both open and closed. This position from a leading AI company directly addresses the tension between open-source AI and safety regulation, potentially influencing future policy decisions and industry practices. Anthropic specifically supports measures such as banning chip sales to China and cracking down on smuggling, which critics argue could effectively function as a ban on open-weights models due to prohibitive testing costs.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open-weights models are AI models whose trained parameters are publicly released, allowing anyone to download, run, and modify them. Unlike closed models, they enable widespread access but raise safety concerns about misuse, such as generating harmful content or enabling malicious applications.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Discussion**: Community commenters broadly criticize Anthropic's stance as a de facto ban, arguing that mandatory safety testing could be prohibitively expensive or administratively gamed. Some see it as a business move to protect Anthropic's proprietary models from competition, while others question the consistency of opposing bans yet supporting hardware restrictions on China.

**Tags**: `#AI safety`, `#open-weights`, `#regulation`, `#Anthropic`, `#open-source AI`

---

<a id="item-3"></a>
## [Moonshot AI Releases 3T Parameter Open-Weight Kimi-K3](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 9.0/10

Moonshot AI has released Kimi-K3, a 3 trillion parameter open-weight model, on HuggingFace along with a technical report. This is one of the largest openly available models to date. This release pushes the boundary of open-weight models, enabling researchers and startups to access a model of unprecedented scale. It could democratize access to frontier AI capabilities and spur innovation in customization and fine-tuning. The model uses mxfp4 native precision, requiring approximately 1.5TB of VRAM to host, necessitating high-end hardware like 8x B200 or more. The license includes revenue-based restrictions for model-as-a-service businesses exceeding $20 million in revenue.

hackernews · nateb2022 · Jul 27, 06:18 · [Discussion](https://news.ycombinator.com/item?id=49065752)

**Background**: An open-weight model means the trained parameters are publicly released, allowing anyone to download and run the model locally, study its behavior, and fine-tune it for specific tasks. However, open-weight models are not fully open-source as they often lack training data and code. Moonshot AI is a Beijing-based AI company known for developing large language models like the Kimi series.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Discussion**: Community comments highlight three main themes: pricing, customization, and hardware requirements. There is also a note about the model initially introducing itself as 'Claude', which raised questions.

**Tags**: `#AI/ML`, `#large language model`, `#open-source`, `#model release`, `#HuggingFace`

---

<a id="item-4"></a>
## [Fastjson 1.x critical RCE without autoType or gadgets](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

Security researcher Kirill Firsov disclosed a high-risk remote code execution vulnerability in Fastjson 1.x versions 1.2.68 through 1.2.83. The exploit does not require enabling autoTypeSupport or any classpath gadget chains and works on JDK 8, 17, and 21. This vulnerability is critical because Fastjson is widely used in Java applications, and the exploit requires neither autoType enablement nor specific gadget chains, making it easier to exploit. Since Fastjson 1.x reached end-of-life in October 2024, no official patch will be released, forcing users to upgrade to Fastjson 2 urgently. The vulnerability affects Fastjson 1.2.68 to 1.2.83 inclusive, without requiring the attacker to enable autoType or have specific gadgets on the classpath. Fastjson 1.x maintenance ended in October 2024, so no security update will be provided by Alibaba.

telegram · zaihuapd · Jul 27, 10:31

**Background**: Fastjson is a popular JSON parsing library for Java developed by Alibaba. Deserialization vulnerabilities often rely on enabling autoType (which allows deserialization of arbitrary classes) and using pre-existing 'gadget chains'—sequences of method calls that lead to code execution. This new vulnerability bypasses both requirements, making it more dangerous. Fastjson 2 is the recommended replacement, with active maintenance and better security defaults.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson2/blob/main/docs/autotype_en.md">fastjson 2/docs/autotype_en.md at main · alibaba/ fastjson 2 · GitHub</a></li>
<li><a href="https://github.com/frohoff/ysoserial">GitHub - frohoff/ysoserial: A proof-of-concept tool for ... Gadget chains in Java: how unsafe deserialization leads to ... Developing a custom gadget chain for Java deserialization ... Lab: Developing a custom gadget chain for Java deserialization Java Deserialization Attacks: From Gadget Chains to RCE</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#fastjson`, `#RCE`, `#java`

---

<a id="item-5"></a>
## [SMIC Tests China's First Domestic DUV Lithography Machine](https://t.me/zaihuapd/42800) ⭐️ 9.0/10

SMIC is trial-running China's first domestically developed advanced deep ultraviolet (DUV) lithography machine, created by Shanghai startup Yuliangsheng. The company is using it to produce 28nm chips and attempting to extend to 7nm and potentially 5nm nodes via multiple patterning, albeit with low yields. This development marks a critical milestone in China's semiconductor self-sufficiency amid escalating export restrictions. If successful, it could reduce reliance on Dutch ASML equipment and reshape global chip supply chains. Most components of the DUV machine are domestically sourced, but some remain imported. Industry insiders estimate it will take one to two years to achieve stable yields for mass production, and the machine is unlikely to compete with ASML's offerings until at least 2027.

telegram · zaihuapd · Jul 27, 14:10

**Background**: Deep ultraviolet (DUV) lithography uses 193nm wavelength light to pattern circuits on silicon wafers, and is widely used for producing chips down to 7nm when combined with multiple patterning techniques. Multiple patterning involves splitting a single layer into multiple exposures to overcome resolution limits. In contrast, extreme ultraviolet (EUV) lithography uses 13.5nm light and is required for advanced nodes below 7nm. China currently relies on ASML's DUV tools for its most advanced chips, while EUV sales to China are banned under US export controls.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Multiple_patterning">Multiple patterning - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Extreme_ultraviolet_lithography">EUV lithography - Wikipedia</a></li>
<li><a href="https://www.semi.org/en/changes-and-challenges-abound-multi-patterning-lithography">Changes and Challenges Abound in Multi-patterning Lithography | SEMI</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#lithography`, `#SMIC`, `#DUV`, `#China chips`

---

<a id="item-6"></a>
## [Moonshot AI to Open-Source Kimi-K3, 3T-Parameter Model](https://t.me/zaihuapd/42802) ⭐️ 9.0/10

Moonshot AI announced it will open-source Kimi-K3, a 2.8T-parameter model (referred to as 3T-class) featuring Kimi Delta Attention and Attention Residuals, with native agentic capabilities and a 1-million-token context window. The model weights are expected to be released on July 27, 2026 on Hugging Face. This marks the first time a frontier-scale model (3T parameters) is openly released, potentially democratizing access to state-of-the-art AI capabilities. The novel architecture may influence future LLM designs, promoting efficient linear attention and agentic workflows. The model uses a hybrid MoE architecture with 3 KDA layers per 1 full attention layer, and the context window supports up to 1 million tokens. Despite being called 3T-class, the actual parameter count is 2.8T.

telegram · zaihuapd · Jul 27, 15:15

**Background**: Large language models (LLMs) typically use full attention mechanisms that scale quadratically with sequence length, making long contexts expensive. Kimi Delta Attention (KDA) is a linear attention variant that improves efficiency while maintaining expressivity. Agentic capabilities refer to the model's ability to use tools, plan, and execute multi-step tasks autonomously. Moonshot AI (月之暗面) is a Chinese AI company known for the Kimi model series.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture GitHub - MoonshotAI/Kimi-Linear Kimi-Linear A arXiv:2510.26692v2 [cs.CL] 1 Nov 2025 Images hwilner/kimi-delta-attention - GitHub Linear Attention: Kimi Delta Attention | Jianyu Huang Kimi K3 Tech Blog: Open Frontier Intelligence KDA (Kimi Delta Attention) | fla-org/flash-linear-attention ...</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#large language model`, `#attention mechanism`, `#Moonshot AI`

---

<a id="item-7"></a>
## [Judge Rejects Google's DMCA Claim to Block Scraping](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

A U.S. judge ruled that Google cannot use the Digital Millennium Copyright Act (DMCA) to stop third parties from scraping its search results, because the factual data in those results lacks the originality required for copyright protection. This ruling sets a significant legal precedent for web scraping and data access, potentially limiting large tech companies' ability to use copyright law to control publicly available information. It could empower smaller competitors and researchers who rely on scraping for innovation and accountability. Google had argued that its search engine results pages (SERPs) are copyrightable compilations, but the judge found they lack creative selection or arrangement. The case was brought against SerpAPI, a service that scrapes Google results for clients.

hackernews · cdrnsf · Jul 27, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49073513)

**Background**: The Digital Millennium Copyright Act (DMCA) is a U.S. law that provides a framework for copyright holders to protect their works online, but it does not cover factual data. Web scraping, the automated extraction of data from websites, often operates in a legal gray area. Tools like web scrapers and proxy services are commonly used to extract public data, which this case centers on.

<details><summary>References</summary>
<ul>
<li><a href="https://webscraper.io/">Web Scraper Cloud | Enterprise Web Scraping Platform</a></li>
<li><a href="https://llanj.org/wiki/how-to-crawl-webpages-requiring-login">How To Crawl Webpages Requiring Login - Llanj</a></li>
<li><a href="https://thunderbit.com/">Thunderbit: AI Web Scraper - Scrape any website in 2 clicks</a></li>

</ul>
</details>

**Discussion**: Commenters noted the irony of Google, a company built on scraping the open web, now trying to prevent others from scraping its results. Some pointed out that Google's deprecation of its search API forced users to rely on third-party scrapers, creating the very demand Google is suing over. Others discussed legal differences between US and EU copyright law regarding databases.

**Tags**: `#legal`, `#web scraping`, `#Google`, `#DMCA`, `#API`

---

<a id="item-8"></a>
## [Libsm64: Turning Super Mario 64 into a Reusable Library](https://github.com/libsm64/libsm64) ⭐️ 8.0/10

Libsm64 is a software library that extracts Super Mario 64's movement and rendering code into a reusable API, allowing developers to integrate Mario characters and mechanics into other game engines like Unity or Source. This enables novel cross-game integrations and creative reuse of classic game code, demonstrating the potential of decompilation projects to extend game assets beyond their original context without relying on proprietary metaverse concepts. The library is built on the full decompilation of Super Mario 64 (SM64) from the n64decomp/sm64 project, providing a clean C interface for movement and rendering. As of the news, there are example integrations like Mario in Half-Life 2 and a demo video showing basic functionality.

hackernews · klaussilveira · Jul 27, 10:04 · [Discussion](https://news.ycombinator.com/item?id=49067352)

**Background**: Super Mario 64 is a landmark 1996 platformer for the Nintendo 64. In 2019, a community-driven decompilation project produced fully readable C source code from the original machine code, enabling modifications and ports. Libsm64 takes this further by packaging the game's core logic into a library for external use.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm 64 / libsm 64 : Mario 64 as a library for use in external...</a></li>
<li><a href="https://github.com/n64decomp/sm64">GitHub - n64decomp/sm64: A Super Mario 64 decompilation, brought to you by a bunch of clever folks. · GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters reacted enthusiastically, calling it a 'favorite library' and noting it embodies the promise of interoperable game assets without crypto hype. One user asked about demo videos and another listed an awesome-libsm64 repository for interesting projects.

**Tags**: `#reverse engineering`, `#game development`, `#open source`, `#emulation`

---

<a id="item-9"></a>
## [Bun's Rust Rewrite Progress and v1.4 Delay](https://lockwood.dev/ai/2026/07/27/how-is-the-bun-rewrite-in-rust-going.html) ⭐️ 8.0/10

Bun's Rust rewrite has been quietly deployed in Claude Code over a month ago, with the v1.4 release delayed until a specific number of newly passing Node.js tests are met. This rewrite is significant for the JavaScript ecosystem as it promises improved performance and compatibility for Bun, a popular Node.js alternative. The use of LLMs in the translation also highlights new approaches to large-scale codebase rewrites. Bun creator Jarred stated that the Rust rewrite shipped in Claude Code without widespread notice, but v1.4 is held back until the promised Node.js test pass count is achieved. Community discussions also mention a competing Zig-based fork achieving sub-second build times.

hackernews · tomlockwood · Jul 27, 11:12 · [Discussion](https://news.ycombinator.com/item?id=49067854)

**Background**: Bun is a fast all-in-one JavaScript runtime originally written in Zig, designed as a drop-in replacement for Node.js. The decision to rewrite in Rust aims to leverage Rust's safety and performance, and the transition was partly assisted by LLMs. Claude Code is an AI-powered coding tool by Anthropic that helps developers understand and edit codebases.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/ bun : Incredibly fast JavaScript runtime , bundler...</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed sentiment: Jarred provides transparent update on the rewrite and delay; some users praise LLM-assisted translation while others question its long-term maintainability; a comparison with a Zig-based fork that claims faster builds sparks debate on the necessity of the rewrite.

**Tags**: `#Bun`, `#Rust`, `#JavaScript Runtime`, `#Rewrite`, `#Performance`

---

<a id="item-10"></a>
## [CXMT Soars 471.59% on STAR Market Debut, Largest IPO Ever](https://www.stcn.com/article/detail/4042119.html) ⭐️ 8.0/10

ChangXin Memory Technologies (CXMT) made its trading debut on Shanghai's STAR Market on July 27, with shares opening at 49.5 yuan, a 471.59% surge from the IPO price of 8.66 yuan. The IPO raised approximately 57.9 billion yuan, making it the largest IPO on the STAR Market, surpassing SMIC's previous record of 53.2 billion yuan. This debut underscores the rapid growth of China's domestic memory chip industry and strong investor appetite for semiconductor companies on the STAR Market. CXMT's massive valuation and profitability forecast signal China's progress in reducing reliance on foreign DRAM suppliers like Samsung and SK Hynix. CXMT's IPO includes an over-allotment option that could bring total proceeds to 66.6 billion yuan. The company forecasts net profit of 50-57 billion yuan for the first half of 2026, a significant turnaround from previous losses.

telegram · zaihuapd · Jul 27, 01:29

**Background**: The STAR Market, officially the Shanghai Stock Exchange Science and Technology Innovation Board, was launched in 2019 to support innovative tech companies with more flexible listing rules, often compared to Nasdaq. CXMT, founded in 2016, is China's largest DRAM manufacturer and roughly the world's fourth-largest by capacity, producing DDR4, DDR5, and LPDDR memory chips.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Shanghai_Stock_Exchange_STAR_Market">Shanghai Stock Exchange STAR Market - Wikipedia</a></li>
<li><a href="https://www.cxmt.com/en/">About cxmt - cxmt</a></li>
<li><a href="https://chinaidb.com/companies/cxmt/">CXMT ( ChangXin Memory ) — China AI Index</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#IPO`, `#memory chip`, `#CXMT`, `#Chinese tech`

---

<a id="item-11"></a>
## [AI-Driven Price Hikes Strain Huawei-CXMT Relations](https://t.me/zaihuapd/42788) ⭐️ 8.0/10

AI data center demand has driven up storage chip prices, giving CXMT stronger bargaining power. Huawei asked CXMT to ease procurement costs but was refused; in June, engineers from Huawei-linked equipment maker Xinkailai were ordered to leave CXMT's core R&D area and have not been allowed to return. This reveals growing friction within China's semiconductor supply chain as AI demand reshapes market dynamics, potentially affecting Huawei's access to critical memory chips. CXMT, now the world's fourth-largest DRAM maker, may prioritize other clients over Huawei, impacting Huawei's AI infrastructure plans. CXMT has become the fourth-largest DRAM manufacturer globally, and its products are in tight supply due to AI data center buildout. The Xinkailai incident highlights the strategic tension: Huawei wanted cost relief, but CXMT pushed through price increases even for its major customer.

telegram · zaihuapd · Jul 27, 03:17

**Background**: CXMT (Changxin Memory Technologies) is a Chinese DRAM chipmaker that has made technical breakthroughs despite US sanctions. Xinkailai (SiCarrier Technologies) is a Shenzhen-based semiconductor equipment company backed by the Shenzhen government and closely tied to Huawei, providing front-end process equipment. The incident occurred at CXMT's Hefei R&D center, reflecting the delicate balance between Huawei's need for stable chip supply and CXMT's profit motives amid AI-driven demand.

<details><summary>References</summary>
<ul>
<li><a href="http://chip.com.cn/cxmt.html">长 鑫 存 储 ( CXMT ) - Glochip.com</a></li>
<li><a href="https://gaohaojun.cn/Blog/2026/01/21/红色内存潮流长鑫存储的战略分析和围绕DRAM的地缘政治斗争/">内 存 的赤色潮流： 长 鑫 存 储 （ CXMT ... - Gao Haojun</a></li>
<li><a href="https://en.wikipedia.org/wiki/SiCarrier">SiCarrier - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#storage chips`, `#Huawei`, `#CXMT`, `#AI data centers`, `#supply chain`

---

<a id="item-12"></a>
## [Google Reveals Gemini 4, Its Most Ambitious Pretraining Project, Expected Late 2026](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 8.0/10

Google CEO Sundar Pichai announced during Alphabet's Q2 2026 earnings call that Gemini 4, their next-generation large language model, has entered training as the company's most ambitious pretraining project to date. He expressed excitement about internal progress and indicated a release by late 2026. This announcement signals Google's intensified commitment to advancing large language models and artificial general intelligence (AGI) research. The release of Gemini 4 could significantly impact the competitive landscape of AI, potentially influencing product capabilities across Google's ecosystem and the broader industry. Pichai emphasized that compute resources will be prioritized for cutting-edge AGI development to ensure Gemini 4 remains at the forefront upon launch. Additionally, the Gemini 3.x Flash series will continue with near-monthly updates, focusing on improved coding abilities.

telegram · zaihuapd · Jul 27, 04:06

**Background**: Large language models (LLMs) like Gemini are typically pretrained on vast text datasets to predict the next word, then fine-tuned for specific tasks. Gemini is a family of multimodal LLMs developed by Google DeepMind, succeeding LaMDA and PaLM 2, and includes variants like Gemini Pro and Flash. Pretraining is the most computationally intensive phase, making ambitious pretraining projects a major strategic investment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_(AI_model)">Gemini (AI model)</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Gemini`, `#large language models`, `#announcement`

---