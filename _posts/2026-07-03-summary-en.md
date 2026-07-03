---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 40 items, 9 important content pieces were selected

---

1. [Commerce Department Bans Differential Privacy in Census Data](#item-1) ⭐️ 9.0/10
2. [Immich 3.0: Major Update to Self-Hosted Photo Platform](#item-2) ⭐️ 9.0/10
3. [ECTC 2026: Intel EMIB-T, HBM4, Microfluidic Cooling, Photonic Interconnects Advances](#item-3) ⭐️ 9.0/10
4. [crustc: Entire Rust Compiler Translated to C](#item-4) ⭐️ 8.0/10
5. [PeerTube: Decentralized Video Platform Gains Attention](#item-5) ⭐️ 8.0/10
6. [Podman v6.0.0 Introduces Major Network Improvements and Quadlet](#item-6) ⭐️ 8.0/10
7. [Postgres Transactions as Distributed Systems Superpower](#item-7) ⭐️ 8.0/10
8. [Using DSPy to Optimize Datasette Agent's SQL Prompts](#item-8) ⭐️ 8.0/10
9. [Anthropic in Early Talks with Samsung for Custom AI Chip](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Commerce Department Bans Differential Privacy in Census Data](https://scottaaronson.blog/?p=9902) ⭐️ 9.0/10

On June 4, 2026, the U.S. Secretary of Commerce issued Directive DAO 216-26, banning differential privacy and noise infusion in Census Bureau statistical products, restricting disclosure avoidance to coarsening only. This policy shift threatens the privacy of individuals in census data and could degrade the accuracy of public data used for critical decisions like resource allocation and redistricting. The directive explicitly forbids 'noise infusion' and differential privacy, which are central to modern disclosure avoidance, and only permits coarsening techniques such as rounding and aggregation.

hackernews · flowercalled · Jul 3, 00:01 · [Discussion](https://news.ycombinator.com/item?id=48768992)

**Background**: Differential privacy is a mathematical framework introduced in 2006 that ensures statistical releases do not reveal information about any individual. Noise infusion adds random noise to data to protect privacy. Coarsening reduces precision but may not provide strong privacy guarantees. The Census Bureau had been using differential privacy for the 2020 Census data, and this directive reverses that approach.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Differential_privacy">Differential privacy - Wikipedia</a></li>
<li><a href="https://privacytools.seas.harvard.edu/differential-privacy">Differential Privacy | Harvard University Privacy Tools Project</a></li>
<li><a href="https://desfontain.es/blog/banning-noise.html">Banning noise will be a disaster for statistical data products - Ted is writing things</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern about the political motives behind the directive and its potential to destroy useful public data. Some called for contacting legislators to oppose the order, while others questioned the effectiveness of coarsening compared to noise infusion.

**Tags**: `#privacy`, `#differential privacy`, `#census`, `#data protection`, `#government policy`

---

<a id="item-2"></a>
## [Immich 3.0: Major Update to Self-Hosted Photo Platform](https://github.com/immich-app/immich/discussions/29439) ⭐️ 9.0/10

Immich 3.0 has been released as a major version update to the open-source, self-hosted photo and video management platform. The release brings significant improvements and new features, as detailed in the GitHub discussion announcement. This release reinforces Immich's position as a leading self-hosted alternative to proprietary services like Google Photos and Apple Photos, offering users greater control over their personal media. The strong community engagement and high upvote count reflect the project's popularity and the demand for privacy-focused photo management solutions. While specific new features are not listed in the summary, the update is described as a major version release, indicating substantial under-the-hood changes and user-facing enhancements. Community comments highlight ongoing discussions around features such as better support for external image sources and end-to-end encryption.

hackernews · hashier · Jul 2, 14:13 · [Discussion](https://news.ycombinator.com/item?id=48761944)

**Background**: Immich is a free, open-source platform for self-hosting photo and video backups, designed as a privacy-respecting alternative to cloud services like Google Photos. It allows users to manage, search, and organize their media on their own hardware, with features similar to commercial offerings but without data leaving the user's control. The project has gained significant traction in the self-hosting community since its inception.

<details><summary>References</summary>
<ul>
<li><a href="https://immich.app/">Immich</a></li>

</ul>
</details>

**Discussion**: The community response is largely positive, with many users praising Immich as a no-brainer replacement for Apple Photos or Google Photos when combined with a VPN like Tailscale. However, some users express a desire for better support for external image sources and note that the lack of end-to-end encryption is a drawback, with some choosing alternatives like Ente Photos for that feature. Overall, the discussion reflects high engagement and a mix of feature requests and appreciation.

**Tags**: `#self-hosting`, `#photography`, `#open-source`, `#photo management`, `#version release`

---

<a id="item-3"></a>
## [ECTC 2026: Intel EMIB-T, HBM4, Microfluidic Cooling, Photonic Interconnects Advances](https://newsletter.semianalysis.com/p/ectc2026) ⭐️ 9.0/10

At ECTC 2026, Intel, TSMC, SK Hynix, Samsung, Micron, Marvell, Lightmatter, and Microsoft presented breakthroughs in advanced packaging including Intel's EMIB-T technology, custom HBM, HBM4 packaging challenges, microfluidic cooling, and photonic interconnects. These innovations address critical thermal, power, and bandwidth bottlenecks in AI and high-performance computing hardware, enabling continued scaling of chiplet architectures and heterogeneous integration. Intel's EMIB-T adds through-silicon vias to the embedded bridge, enabling HBM4-class power delivery and large package scaling, with production fab rollout expected in 2026. Microfluidic cooling can handle heat densities exceeding hundreds of watts per square centimeter, while photonic interconnects aim to replace electrical links for higher bandwidth and lower latency.

rss · Semianalysis · Jul 2, 17:25

**Background**: Advanced packaging techniques like EMIB (Embedded Multi-Die Interconnect Bridge) are crucial for integrating multiple chips in a single package, as traditional monolithic scaling slows. EMIB-T enhances this with TSVs for better power delivery. Microfluidic cooling uses liquid flow through microchannels to remove heat efficiently, and photonic interconnects use light for data transfer, reducing energy and increasing speed. These technologies are key for next-generation AI accelerators and HBM memory stacks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/cpus/intel-details-new-advanced-packaging-breakthroughs-emib-t-paves-the-way-for-hbm4-and-increased-ucie-bandwidth">Intel details new advanced packaging breakthroughs — EMIB-T paves the way for HBM4 and increased UCIe bandwidth | Tom's Hardware</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/intels-emib-t-heads-for-fab-rollout-this-year">Intel's EMIB-T packaging technology set for fab rollout this year — as TSMC CoWoS capacity remains limited, EMIB-T is preparing for advanced AI accelerator designs | Tom's Hardware</a></li>
<li><a href="https://medium.com/no-time/microfluidic-cooling-the-silent-revolution-in-high-performance-semiconductor-c713d1089630">Microfluidic Cooling : The Silent Revolution In... | Medium</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#packaging`, `#HBM`, `#photonics`, `#AI hardware`

---

<a id="item-4"></a>
## [crustc: Entire Rust Compiler Translated to C](https://github.com/FractalFir/crustc) ⭐️ 8.0/10

A project called crustc has successfully translated the entirety of the Rust compiler (rustc) into C, enabling Rust code to be compiled on platforms that lack LLVM or GCC support. This opens up Rust to a vast range of legacy and obscure hardware that only supports C compilers, potentially expanding Rust's adoption in embedded and retro computing. It also addresses the bootstrapping problem, allowing Rust to be built from C without relying on an existing Rust compiler. The project translates rustc, the Rust compiler, into C rather than generating C code from Rust source, making it a full transpilation of the compiler itself. This is the 14th known attempt, according to community comments, and the author spent three years on it.

hackernews · Philpax · Jul 2, 22:57 · [Discussion](https://news.ycombinator.com/item?id=48768464)

**Background**: Bootstrapping is the process of writing a compiler in the language it compiles, which creates a chicken-and-egg problem: you need a compiler to compile the compiler. Creating a Rust compiler written in C would allow building Rust from source on any platform with a C compiler, eliminating the need for an existing Rust binary. This has been a longstanding goal for improving portability and verifiability of the Rust ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/FractalFir/crustc">crustc: entirety of `rustc`, translated to C - GitHub</a></li>
<li><a href="https://gab.ae/news/crustc-entirety-of-rustc-translated-to-c-2026">crustc: entirety of `rustc`, translated to C | GAB adventures</a></li>
<li><a href="https://en.wikipedia.org/wiki/Compiler_bootstrapping">Compiler bootstrapping</a></li>

</ul>
</details>

**Discussion**: The community is largely positive, praising the dedication and originality, with comments noting the potential for bootstrapping verification and security (e.g., diverse double-compiling). Some discuss the difficulty and previous attempts, while others express curiosity about the implementation details.

**Tags**: `#rust`, `#compiler`, `#transpilation`, `#bootstrapping`, `#C`

---

<a id="item-5"></a>
## [PeerTube: Decentralized Video Platform Gains Attention](https://github.com/Chocobozzz/PeerTube) ⭐️ 8.0/10

PeerTube is a free, open-source, decentralized video platform that uses ActivityPub federation and WebTorrent for peer-to-peer streaming, offering an alternative to centralized services like YouTube. PeerTube represents a significant step towards a decentralized web, empowering creators and users to avoid corporate control over video content. PeerTube relies on ActivityPub for federation across instances and on WebTorrent for distributing playback load among viewers, but it lacks built-in monetization or advanced content discovery features.

hackernews · doener · Jul 2, 11:17 · [Discussion](https://news.ycombinator.com/item?id=48759634)

**Background**: The Fediverse is a collection of decentralized social networks that communicate via open protocols like ActivityPub. PeerTube is a video platform within this ecosystem. WebTorrent is a JavaScript library that enables peer-to-peer streaming directly in web browsers, reducing server load.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fediverse">Fediverse</a></li>
<li><a href="https://en.wikipedia.org/wiki/ActivityPub">ActivityPub</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebTorrent">WebTorrent</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted the lack of monetization as a major obstacle for professional YouTubers, while others noted that PeerTube currently has limited content and audience, especially outside niche topics like open source software.

**Tags**: `#decentralization`, `#video hosting`, `#fediverse`, `#open source`, `#peer-to-peer`

---

<a id="item-6"></a>
## [Podman v6.0.0 Introduces Major Network Improvements and Quadlet](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0, a major version release, introduces significant network improvements and the Quadlet feature for declarative container management with systemd. This release strengthens Podman's position as a leading Docker alternative, offering enhanced networking and simplified container orchestration via systemd, which could accelerate migration from Docker. Quadlet allows users to run containers declaratively using systemd unit files, similar to Kubernetes or Compose, and network improvements include better performance and configuration options.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is an open-source container engine that provides a Docker-compatible command-line interface and API. Unlike Docker, Podman is daemonless and can run containers rootlessly. Quadlet is a feature that integrates Podman with systemd, enabling declarative container management without external orchestration tools.

<details><summary>References</summary>
<ul>
<li><a href="https://www.redhat.com/en/blog/quadlet-podman">Make systemd better for Podman with Quadlet</a></li>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-quadlet.1.html">podman-quadlet — Podman documentation</a></li>

</ul>
</details>

**Discussion**: Community comments highlight strong praise for Podman's ease of migration and Quadlet, with many users preferring it over Docker. However, some users report issues on macOS, such as random crashes and architecture differences, suggesting that cross-platform support remains a challenge.

**Tags**: `#podman`, `#containers`, `#docker-alternative`, `#devops`, `#open-source`

---

<a id="item-7"></a>
## [Postgres Transactions as Distributed Systems Superpower](https://www.dbos.dev/blog/co-locating-workflow-state-with-your-data) ⭐️ 8.0/10

An article advocates using Postgres transactions to co-locate workflow state with application data in a central database, simplifying distributed system design by leveraging atomic operations. This approach reduces the complexity of workflow orchestration by eliminating the need for separate message queues or state stores, making systems easier to build and maintain. It challenges common patterns like the outbox pattern and appeals to practitioners seeking simplicity. The DBOS Transact open-source library implements this pattern, where each workflow step becomes a database commit unit, simplifying idempotency and atomicity. However, this tightly couples the database to the workflow, making later architectural separation difficult.

hackernews · KraftyOne · Jul 2, 18:38 · [Discussion](https://news.ycombinator.com/item?id=48765639)

**Background**: Distributed systems often use separate components like message queues or workflow engines to manage state across services, adding complexity. By co-locating workflow state in a single Postgres database, developers can use ACID transactions to ensure atomic updates, simplifying coordination. This concept is central to the DBOS project, which provides tools for durable workflow orchestration.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dbos.dev/">DBOS | Durable Workflow Orchestration</a></li>
<li><a href="https://www.geeksforgeeks.org/system-design/comparison-centralized-decentralized-and-distributed-systems/">Centralized vs. Decentralized vs. Distributed Systems</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some praise the atomicity benefits and share similar in-house solutions, while others question whether this is truly a distributed system or just a centralized mutex with tight coupling. There is debate about the trade-off between simplicity and future flexibility.

**Tags**: `#Postgres`, `#distributed systems`, `#transactions`, `#workflow orchestration`, `#database`

---

<a id="item-8"></a>
## [Using DSPy to Optimize Datasette Agent's SQL Prompts](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 8.0/10

Simon Willison used the DSPy framework to evaluate and iteratively improve the system prompts for Datasette Agent's SQL query generation, identifying specific weaknesses like column-name guessing. He automated the optimization process via Claude Code and DSPy, testing with GPT-4.1 mini and nano models. This demonstrates a practical, repeatable methodology for automatically improving AI agent prompts using programmatic optimization rather than manual trial-and-error. It could significantly enhance the reliability of SQL-generating agents and similar LLM-based tools. One discovered improvement was to include column names in the schema listing to prevent the model from guessing columns and entering error-retry loops. The research used DSPy's optimization algorithms to test prompt variants against a defined metric.

rss · Simon Willison · Jul 2, 18:25

**Background**: DSPy is a Python framework that enables programmatic optimization of language model prompts and weights by expressing tasks as structured signatures. Datasette Agent is an AI assistant for Datasette that can write and execute SQL queries to answer user questions about data. Traditionally, improving prompts requires manual iteration; DSPy automates this by compiling programs with built-in optimizers.

<details><summary>References</summary>
<ul>
<li><a href="https://dspy.ai/">DSPy</a></li>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp/dspy: DSPy: The framework for ... GitHub - isaka/DSPy: DSPy: The framework for programming—not ... What Is DSPy? How It Works, Use Cases, and Resources Tutorials Overview - DSPy Programming, Not Prompting: A Hands-On Guide to DSPy DSPy Framework — Programmatic Prompt Optimization (2026)</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent : an AI assistant for Datasette to help explore and...</a></li>

</ul>
</details>

**Tags**: `#DSPy`, `#prompt engineering`, `#SQL`, `#LLM`, `#Datasette`

---

<a id="item-9"></a>
## [Anthropic in Early Talks with Samsung for Custom AI Chip](https://www.theinformation.com/articles/anthropic-talks-samsung-manufacture-custom-ai-chip) ⭐️ 8.0/10

Anthropic has started developing its own custom AI chip and is in early-stage talks with Samsung Electronics for manufacturing, aiming to gain more control over the compute infrastructure for its Claude models. This move reduces Anthropic's reliance on third-party hardware providers like NVIDIA, similar to OpenAI's custom chip initiative, and signals a broader trend of AI labs verticalizing their hardware to optimize performance and cost. The project is still in early stages, and Anthropic is entering the custom chip space later than competitors like OpenAI and Google. Samsung's foundry offers advanced nodes (e.g., 3nm GAA), which could be leveraged for the chip.

telegram · zaihuapd · Jul 2, 15:57

**Background**: Custom AI chips are purpose-built processors designed to accelerate AI workloads, such as inference for large language models, offering better performance and efficiency than general-purpose GPUs. Companies like OpenAI have developed their own inference chips (e.g., 'Jalapeño') to optimize for their models. Samsung Foundry is a major semiconductor manufacturer with advanced process technologies, making it a potential partner for custom chip production.

<details><summary>References</summary>
<ul>
<li><a href="https://www.partgenie.ai/insights/openai-s-jalape-o-will-be-spicy-but-the-real-sizzle-is-its-chip-design-ai-1">OpenAI's Custom Jalapeño AI Inference Chip Signals Vertical...</a></li>
<li><a href="https://semiconductor.samsung.com/foundry/about-samsung-foundry/company-info/">Company Info | About Samsung Foundry | Samsung Semiconductor ...</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#Anthropic`, `#Samsung`, `#custom chip`, `#AI infrastructure`

---