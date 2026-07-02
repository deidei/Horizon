---
layout: default
title: "Horizon Summary: 2026-07-02 (EN)"
date: 2026-07-02
lang: en
---

> From 40 items, 11 important content pieces were selected

---

1. [First Synthetic Cell That Grows and Divides Created](#item-1) ⭐️ 10.0/10
2. [Box3D: A New Open Source 3D Physics Engine from Box2D Creator](#item-2) ⭐️ 9.0/10
3. [MOTHRAG: Graph-Free Multi-Hop Retrieval Outperforms Graph-Based Systems](#item-3) ⭐️ 9.0/10
4. [Claude Code 2.1.91 accused of covert telemetry via prompt encoding](#item-4) ⭐️ 9.0/10
5. [Sony to End Physical Disc Production for New PlayStation Games by 2028](#item-5) ⭐️ 8.0/10
6. [Interactive Deep Dive into Internal Combustion Engine Mechanics](#item-6) ⭐️ 8.0/10
7. [Cloudflare Monetization Gateway Enables Pay-Per-Request via x402](#item-7) ⭐️ 8.0/10
8. [Hamiltonian Neural Networks via Differential Geometry and Noether's Theorem](#item-8) ⭐️ 8.0/10
9. [NVIDIA Cuts DeepSeek V4 Inference Cost by 5x on Blackwell](#item-9) ⭐️ 8.0/10
10. [Visa, Mastercard and 140+ Firms Launch Open Standard Stablecoin Network](#item-10) ⭐️ 8.0/10
11. [ChatGPT Weekly Users Double to 200 Million in Under a Year](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [First Synthetic Cell That Grows and Divides Created](https://www.quantamagazine.org/for-the-first-time-a-cell-built-from-scratch-grows-and-divides-20260701/) ⭐️ 10.0/10

Scientists led by Dr. Kate Adamala at the University of Minnesota created SpudCell, a synthetic cell built from lifeless chemicals that can grow, replicate its DNA, and divide, completing the full cell cycle for the first time. This breakthrough demonstrates that life-like functions can be achieved from non-living components, marking a paradigm shift in synthetic biology and opening possibilities for engineered cells in biotechnology and medicine. SpudCell lacks a cytoskeleton and uses an alternative division mechanism, bypassing a major hurdle that had stalled the field. The initial paper was rejected by Cell after a reviewer called SpudCells 'not real biology', but it is now publicly available.

hackernews · defrost · Jul 1, 14:20 · [Discussion](https://news.ycombinator.com/item?id=48747304)

**Background**: Synthetic biology aims to construct artificial cells from scratch to understand life's principles and create useful systems. Previous synthetic cells could grow and replicate DNA but could not divide, as division requires complex cytoskeletal reorganization. The SpudCell team circumvented this by designing a division process without a cytoskeleton, achieving the complete cell cycle.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SpudCell">SpudCell - Wikipedia</a></li>
<li><a href="https://www.nytimes.com/2026/07/01/science/spud-cell-what-to-know.html">SpudCell: Scientists Made a Cell With Most of the Hallmarks of Life. Here’s What to Know. - The New York Times</a></li>
<li><a href="https://www.theguardian.com/science/2026/jul/01/synthetic-life-lab-made-dna-spudcells-scientists">‘Beautiful blobs’: synthetic life a step closer as scientists make cells using lab-made DNA | Science | The Guardian</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the paper's rejection by Cell and the controversy over whether SpudCells are 'real biology'. Some users discuss the mechanism of division and the chirality of amino acids, while others praise the achievement and note the lead researcher's prior work on synthetic cells.

**Tags**: `#synthetic biology`, `#spudcell`, `#cell division`, `#synthetic cells`, `#bioengineering`

---

<a id="item-2"></a>
## [Box3D: A New Open Source 3D Physics Engine from Box2D Creator](https://box2d.org/posts/2026/06/announcing-box3d/) ⭐️ 9.0/10

Erin Catto has announced Box3D, an open source 3D physics engine that builds on the legacy of the widely-used Box2D library. Box3D is poised to become a foundational tool for game development, robotics simulation, and machine learning environments, given its author's legendary status and the proven impact of Box2D. Box3D is a new library with no immediate support for determinism or GPU acceleration, but it promises high-quality rigid body simulation with convex decomposition and hand-tuned solvers.

hackernews · makepanic · Jul 1, 12:12 · [Discussion](https://news.ycombinator.com/item?id=48745445)

**Background**: Box2D is a 2D physics engine created by Erin Catto that has been used in thousands of games and simulation projects, including Angry Birds. It also underpins many reinforcement learning environments like OpenAI Gym's Lunar Lander. A 3D successor has been anticipated for years.

**Discussion**: The community expressed excitement and gratitude, with comments highlighting Box2D's role in indie games and ML research. Requests for deterministic simulation and concerns about the complexity of 3D physics were also noted.

**Tags**: `#physics engine`, `#open source`, `#game development`, `#simulation`, `#box2d`

---

<a id="item-3"></a>
## [MOTHRAG: Graph-Free Multi-Hop Retrieval Outperforms Graph-Based Systems](https://www.reddit.com/r/MachineLearning/comments/1ukotww/p_mothretrieval_graphfree_multihop_retrieval_via/) ⭐️ 9.0/10

MOTHRAG, a graph-free multi-hop retrieval framework using query-time orchestration, was open-sourced and achieves state-of-the-art results on HotpotQA (78.1% accuracy), outperforming GraphRAG by 9.5 points and HippoRAG by 2.6 points. This is significant because it eliminates the need for costly offline knowledge graph construction and re-indexing, making multi-hop RAG practical for frequently changing data. It also reduces computational requirements by running on commodity APIs without GPUs. MOTHRAG uses a graph-free dense index with query-time orchestration, and the reported cost is about $0.03 per query on commodity APIs. It uses an embed-and-append update strategy, avoiding full rebuilds, but underperforms on the MuSiQue dataset (50.5 vs 52.6) compared to NeocorRAG.

reddit · r/MachineLearning · /u/Annual-Commercial563 · Jul 1, 15:26

**Background**: Multi-hop retrieval-augmented generation (RAG) requires retrieving information from multiple documents to answer complex questions. Traditional approaches like GraphRAG build a knowledge graph offline, which is accurate but expensive to update when data changes. MOTHRAG avoids this by using a dense vector index and orchestrating retrieval at query time, similar to how query-time orchestration tools schedule workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/yixuantt/MultiHop-RAG/">GitHub - yixuantt/MultiHop-RAG: Repository for "MultiHop-RAG: A Dataset for Evaluating Retrieval-Augmented Generation Across Documents" (COLM 2024) · GitHub</a></li>
<li><a href="https://arxiv.org/abs/2401.15391">[2401.15391] MultiHop-RAG: Benchmarking Retrieval-Augmented Generation for Multi-Hop Queries</a></li>

</ul>
</details>

**Tags**: `#RAG`, `#multi-hop retrieval`, `#knowledge graph`, `#NLP`, `#open-source`

---

<a id="item-4"></a>
## [Claude Code 2.1.91 accused of covert telemetry via prompt encoding](https://t.me/zaihuapd/42285) ⭐️ 9.0/10

A reverse engineering analysis revealed that Claude Code 2.1.91, released in April 2026, covertly checks for proxy and timezone settings (specifically Asia/Shanghai or Asia/Urumqi) and encodes the results into system prompts sent to Anthropic's API. This raises significant privacy and trust concerns for users of a widely-used AI coding tool, as it suggests undisclosed surveillance of user environment and potential targeting of users in specific regions. The technique involves encoding proxy URL and timezone information by altering the date format and Unicode apostrophe in the 'Today's date is' prompt, effectively steganographing data into the API prompt.

telegram · zaihuapd · Jul 1, 04:42

**Background**: Telemetry is commonly used in software for diagnostics, but covert collection without user consent is controversial. Claude Code is an AI-powered coding assistant that uses Anthropic's API. The reverse engineering specifically targeted version 2.1.91 released in April 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/monitoring-usage">Monitoring - Claude Code Docs</a></li>
<li><a href="https://github.com/lainra/claude-code-telemetry">GitHub - lainra/claude-code-telemetry: Claude Code Telemetry is a lightweight bridge that captures telemetry data from Claude Code and forwards it to Langfuse for visualization, with a secure local turnkey installation under a minute. · GitHub</a></li>
<li><a href="https://www.elastic.co/security-labs/claude-code-cowork-monitoring-otel-elastic">Claude Code/Cowork monitoring at scale with Otel & Elastic — Elastic Security Labs</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#telemetry`, `#AI`, `#Claude Code`, `#reverse engineering`

---

<a id="item-5"></a>
## [Sony to End Physical Disc Production for New PlayStation Games by 2028](https://blog.playstation.com/2026/07/01/physical-disc-production-ending-in-january-2028-for-new-games-releasing-on-playstation-consoles/) ⭐️ 8.0/10

Sony announced that starting January 2028, it will cease production of physical discs for new games releasing on PlayStation consoles, transitioning to an all-digital distribution model. This marks a major industry shift toward digital-only gaming, raising concerns about digital ownership, DRM restrictions, and long-term game preservation for consumers and collectors. The move applies only to new game releases; existing physical games and those released before the cutoff will still be produced. Sony emphasized that this decision aligns with market trends toward digital downloads.

hackernews · Tiberium · Jul 1, 12:13 · [Discussion](https://news.ycombinator.com/item?id=48745456)

**Discussion**: Community reaction is overwhelmingly negative, with commenters highlighting Sony's recent removal of purchased digital movies as evidence that digital content is rented, not owned. Others warn this could lead to a 'dark age' of gaming where titles become unplayable when servers shut down, and note that physical copies often remain cheaper than digital prices years after release.

**Tags**: `#gaming`, `#digital ownership`, `#Sony`, `#physical media`, `#game preservation`

---

<a id="item-6"></a>
## [Interactive Deep Dive into Internal Combustion Engine Mechanics](https://ciechanow.ski/internal-combustion-engine/) ⭐️ 8.0/10

The article provides an in-depth, interactive visual exploration of the internal combustion engine, covering its history, components, and operating principles. It serves as an excellent educational resource for understanding a technology that powers most vehicles, despite the rise of electric propulsion. The interactive diagrams allow readers to see and manipulate engine parts, demonstrating four-stroke cycles, valve timing, and lubrication. The article also discusses the evolution of control systems from carburetors to electronic fuel injection.

hackernews · StefanBatory · Jul 1, 13:04 · [Discussion](https://news.ycombinator.com/item?id=48746076)

**Background**: An internal combustion engine (ICE) is a heat engine that burns fuel inside a combustion chamber to produce mechanical work. The most common type is the four-stroke engine, which cycles through intake, compression, power, and exhaust strokes. Key components include pistons, cylinders, valves, spark plugs, and a crankshaft. Over decades, ICE technology has been refined for efficiency and emissions reduction, but the fundamental design remains largely unchanged since the mid-20th century.

**Discussion**: Commenters highlighted the static nature of engine design over 50 years, with evolution happening mainly in control systems and emissions hardware. Specific observations include the firing order of a 4-cylinder engine, the role of oil in hydrodynamic lubrication (notable in Ford engines with auto start/stop), and the perceived loss of elegance in modern engines due to added complexity like overhead cams and variable valve timing.

**Tags**: `#internal combustion engine`, `#mechanical engineering`, `#interactive article`, `#technology deep-dive`

---

<a id="item-7"></a>
## [Cloudflare Monetization Gateway Enables Pay-Per-Request via x402](https://blog.cloudflare.com/monetization-gateway/) ⭐️ 8.0/10

Cloudflare announced the Monetization Gateway, allowing developers to charge for any web resource (APIs, datasets, web pages, MCP tools) using the HTTP 402 status code and the x402 open protocol, with payments settled in stablecoins. This enables instant, low-cost micropayments without requiring user accounts or complex payment infrastructure, potentially transforming how bots and AI agents pay for web resources and how creators monetize content. The gateway is an extension of Cloudflare's existing network and is currently on a waitlist. It repurposes the historically underused HTTP 402 'Payment Required' status code.

hackernews · soheilpro · Jul 1, 13:59 · [Discussion](https://news.ycombinator.com/item?id=48746914)

**Background**: HTTP 402 is a reserved status code for 'Payment Required' but has never been widely adopted. The x402 protocol is an open standard that leverages stablecoins for settlement. Cloudflare operates a global edge network that can proxy requests and handle the payment logic at the edge.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/monetization-gateway/">Announcing the Monetization Gateway: charge for ... - The Cloudflare Blog</a></li>
<li><a href="https://byteiota.com/cloudflare-monetization-gateway-charge-apis-via-x402/">Cloudflare Monetization Gateway: Charge APIs via x402 - byteiota</a></li>
<li><a href="https://www.cryptoninjas.net/news/cloudflare-unveils-stablecoin-monetization-gateway-unlocking-instant-x402-payments-for-any-api/">Cloudflare Unveils Stablecoin Monetization Gateway, Unlocking Instant ...</a></li>

</ul>
</details>

**Discussion**: Comments reflect both excitement and skepticism. Some see it as the fulfillment of microtransaction dreams for agents, while others worry about legal complexities (invoicing, VAT) and the risk of spam/low-quality content. There's also concern that it doesn't solve the problem of distinguishing bots from humans for free experiences.

**Tags**: `#monetization`, `#Cloudflare`, `#microtransactions`, `#HTTP 402`, `#web infrastructure`

---

<a id="item-8"></a>
## [Hamiltonian Neural Networks via Differential Geometry and Noether's Theorem](https://www.reddit.com/r/MachineLearning/comments/1ukzdnj/hamiltonian_neural_networks_from_a_differential/) ⭐️ 8.0/10

A blog post introduces a differential geometry perspective on Hamiltonian Neural Networks (HNNs), emphasizing Noether's theorem to link conservation laws with symmetries and generalization in machine learning. This novel viewpoint clarifies why HNNs generalize well by grounding them in fundamental physics, potentially inspiring more robust physics-informed neural networks and improved inductive biases. The post is math-heavy but includes interactive visuals to ease understanding, focusing on how Noether's theorem provides a principled connection between symmetries and conserved quantities in HNN training.

reddit · r/MachineLearning · /u/FlameOfIgnis · Jul 1, 21:55

**Background**: Hamiltonian Neural Networks are a class of neural networks that learn Hamiltonian dynamics directly, conserving energy and respecting physical laws. Noether's theorem states that every continuous symmetry of a physical system corresponds to a conservation law. Differential geometry offers a geometric framework to understand these symmetries and conservation laws, providing deeper insight into model behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Noether's_theorem">Noether's theorem</a></li>
<li><a href="https://arxiv.org/abs/1906.01563">[1906.01563] Hamiltonian Neural Networks</a></li>
<li><a href="https://greydanus.github.io/2019/05/15/hamiltonian-nns/">Hamiltonian Neural Networks</a></li>

</ul>
</details>

**Tags**: `#Hamiltonian Neural Networks`, `#Differential Geometry`, `#Noether's Theorem`, `#Physics-Informed Machine Learning`, `#Symmetry`

---

<a id="item-9"></a>
## [NVIDIA Cuts DeepSeek V4 Inference Cost by 5x on Blackwell](https://blogs.nvidia.com/blog/inference-software-lowest-token-cost/) ⭐️ 8.0/10

NVIDIA's inference software stack on Blackwell platform reduced the per-token cost for DeepSeek V4 to one-fifth of its previous level within one month, achieving 5x throughput improvement from ~2,200 to ~11,200 tokens/second/GPU using the SGLang engine. This dramatic cost reduction makes large-scale deployment of DeepSeek V4 significantly more affordable, enabling wider adoption of state-of-the-art AI models in production. It also demonstrates NVIDIA's continued dominance in inference optimization, with a roadmap for up to 20x further improvements. The optimization leverages kernel and runtime improvements including fusion, memory compression, quantization precision paths, improved memory budgeting, interruptible compute graphs, and inference stability fixes. Future advanced optimizations like disaggregated serving, new floating-point precision, and multi-token prediction could push system throughput up to 20x.

telegram · zaihuapd · Jul 1, 10:36

**Background**: DeepSeek V4 is a Mixture-of-Experts (MoE) language model with up to 1.6 trillion parameters, requiring massive compute for inference. SGLang is an open-source high-performance inference engine widely deployed on over 400,000 GPUs. The NVIDIA Blackwell architecture and its ultra variant provide enhanced AI compute and memory bandwidth critical for such large models.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/sgl-project/sglang">GitHub - sgl-project/ sglang : SGLang is a high-performance serving...</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#DeepSeek`, `#inference optimization`, `#AI infrastructure`, `#cost reduction`

---

<a id="item-10"></a>
## [Visa, Mastercard and 140+ Firms Launch Open Standard Stablecoin Network](https://www.reuters.com/business/consortium-including-visa-mastercard-jointly-launch-new-global-stablecoin-2026-06-30/) ⭐️ 8.0/10

On June 30, 2026, a consortium of over 140 companies including Visa, Mastercard, and Coinbase announced the launch of Open Standard, a new stablecoin network, and will issue a dollar-pegged stablecoin called Open USD later this year. This initiative aims to address key barriers to enterprise stablecoin adoption by offering a free-to-mint/redeem model that shares reserve revenue with partners, potentially transforming global payments and accelerating the use of stablecoins in mainstream commerce. Open USD will charge no mint or redeem fees and will distribute most of its reserve income back to partners after deducting management fees, positioning itself as neutral, open infrastructure. The network is collectively governed by the consortium and aims to become an open standard for payments.

telegram · zaihuapd · Jul 1, 11:06

**Background**: Stablecoins are cryptocurrencies pegged to a stable asset like the US dollar, designed to reduce volatility. Currently, they are mainly used in crypto trading and have not achieved widespread adoption in everyday payments due to cost, complexity, and lack of open infrastructure. The GENIUS Act, signed into US law in 2026, provides a federal regulatory framework for payment stablecoins, aiming to foster innovation and adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/christiancatalini/2026/06/30/why-an-open-standard-will-win-the-stablecoin-race/">Why An Open Standard Will Win The Stablecoin Race</a></li>
<li><a href="https://www.theblock.co/post/406736/visa-stripe-coinbase-join-open-usd-stablecoin-shares-reserve-revenue">Visa, Stripe, Coinbase and more join Open USD stablecoin that shares reserve revenue | The Block</a></li>
<li><a href="https://www.thestreet.com/crypto/markets/aptos-visa-and-blackrock-among-140-firms-launching-new-stablecoin">Aptos, Visa and BlackRock among 140 firms launching new stablecoin - TheStreet Crypto: Bitcoin and cryptocurrency news, advice, analysis and more</a></li>

</ul>
</details>

**Tags**: `#stablecoin`, `#blockchain`, `#payments`, `#fintech`, `#consortia`

---

<a id="item-11"></a>
## [ChatGPT Weekly Users Double to 200 Million in Under a Year](https://t.me/zaihuapd/42298) ⭐️ 8.0/10

OpenAI announced that ChatGPT now has over 200 million weekly active users, doubling from 100 million in November 2023. Additionally, 92% of Fortune 500 companies use OpenAI products, and API usage doubled following the release of the GPT-4o Mini model. This milestone demonstrates rapid AI adoption among consumers and enterprises, with ChatGPT maintaining its lead despite competition from Google, Microsoft, and Meta. The growth signals strong demand for AI-powered tools and could attract further investment from companies like Apple and Nvidia. The GPT-4o Mini model, described as faster and cheaper, contributed to a doubling of API usage. Fortune 500 adoption reached 92%, indicating deep enterprise penetration. Rumors suggest Apple and Nvidia may invest in OpenAI's next funding round.

telegram · zaihuapd · Jul 1, 13:01

**Background**: ChatGPT is a conversational AI chatbot developed by OpenAI, first launched in November 2022. It gained rapid popularity, reaching 100 million monthly users within months. OpenAI has since released multiple model updates, including GPT-4 and the more efficient GPT-4o Mini. The GPT-4o Mini is a cost-effective small model designed for focused tasks, offering lower pricing and faster performance while still supporting text and image inputs.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-4o-mini-advancing-cost-efficient-intelligence/">GPT-4o mini: advancing cost-efficient intelligence | OpenAI</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-4o-mini">GPT-4o mini Model | OpenAI API</a></li>
<li><a href="https://openrouter.ai/openai/gpt-4o-mini">GPT-4o-mini - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#ChatGPT`, `#OpenAI`, `#AI`, `#user growth`, `#industry news`

---