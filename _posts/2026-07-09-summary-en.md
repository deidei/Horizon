---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 40 items, 15 important content pieces were selected

---

1. [OpenAI Releases GPT-5.6 with Three Tiers, Sol Achieves ARC-AGI-3 SOTA](#item-1) ⭐️ 10.0/10
2. [Bun Rewritten from Zig to Rust with AI](#item-2) ⭐️ 9.0/10
3. [TypeScript 7.0 Released with Go Rewrite, Up to 12x Speed](#item-3) ⭐️ 9.0/10
4. [Ant Group Open-Sources LingBot-Video, First MoE Embodied Video Model](#item-4) ⭐️ 9.0/10
5. [EU Parliament Passes Chat Control 1.0 via Procedural Trick](#item-5) ⭐️ 8.0/10
6. [Postgres rewritten in Rust passes all regression tests](#item-6) ⭐️ 8.0/10
7. [US Army logistics vulnerabilities analyzed](#item-7) ⭐️ 8.0/10
8. [Meta launches Muse Spark 1.1 with commercial API](#item-8) ⭐️ 8.0/10
9. [AI content floods social media, especially LinkedIn](#item-9) ⭐️ 8.0/10
10. [OpenAI Launches GPT-Live Voice Mode with GPT-5.5 Delegation](#item-10) ⭐️ 8.0/10
11. [Meta's Superintelligence Update Reveals RL Startup and Compute Scaling](#item-11) ⭐️ 8.0/10
12. [IMGNet: Face Verification via Sign Patterns Replaces Cosine Similarity](#item-12) ⭐️ 8.0/10
13. [DJI EV50 drone reaches 8861m over Everest](#item-13) ⭐️ 8.0/10
14. [China's Supercomputing Internet Core Node Launches in Zhengzhou](#item-14) ⭐️ 8.0/10
15. [OpenAI and US War Dept to Ban AI for Citizen Surveillance](#item-15) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Releases GPT-5.6 with Three Tiers, Sol Achieves ARC-AGI-3 SOTA](https://openai.com/index/gpt-5-6/) ⭐️ 10.0/10

OpenAI announced the general availability of GPT-5.6, a family of three models: Luna, Terra, and Sol. The largest tier, Sol, sets a new state-of-the-art on the ARC-AGI-3 benchmark with a 7.8% score, becoming the first verified frontier model to solve an ARC-AGI-3 game. This release marks a significant leap in AI reasoning capabilities, especially with Sol's breakthrough on ARC-AGI-3, a benchmark designed to measure human-like interactive intelligence. The tiered pricing model (Luna, Terra, Sol) makes advanced AI more accessible while offering a premium option for demanding tasks, and the strong performance is likely to raise the bar for competitors. The three tiers are priced per 1M input/output tokens: Luna $1/$6, Terra $2.50/$15, Sol $5/$30. Sol consumes significant compute resources — a single complex query can use up to 95% of a 5-hour quota on the Plus plan. The model family also includes improved intent understanding and preserves original image dimensions.

hackernews · logickkk1 · Jul 9, 17:04 · [Discussion](https://news.ycombinator.com/item?id=48849066)

**Background**: GPT-5.6 is OpenAI's latest flagship model family, succeeding GPT-5. It comes in three sizes: Luna (fastest/cheapest), Terra (mid-range), and Sol (most capable). ARC-AGI-3 is an interactive reasoning benchmark that challenges AI agents to explore novel environments, infer goals, and plan effectively. The tiered pricing model follows a pattern also used by Anthropic and Google for their models.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT‑5.6 Sol: a next-generation model - OpenAI</a></li>
<li><a href="https://andrew.ooo/answers/gpt-5-6-sol-vs-terra-vs-luna-tiered-model-explained-july-2026/">GPT-5.6 Sol vs Terra vs Luna: OpenAI's New Tier Explained</a></li>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed but generally positive. Users noted the high quota consumption by Sol (ekzy reported 95% usage for one query) and shared practical tips from the developer guide. Some discussed comparisons with other models like Claude Code, and one commenter pointed out that OpenAI omitted comparisons with Fable 5 in certain benchmarks because it refused to answer questions. Overall, the release generated substantial engagement (939 points, 703 comments) confirming its importance.

**Tags**: `#GPT-5.6`, `#OpenAI`, `#AI`, `#large language models`, `#ARC-AGI`

---

<a id="item-2"></a>
## [Bun Rewritten from Zig to Rust with AI](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Jarred Sumner announced that Bun, the JavaScript runtime, has been rewritten from Zig to Rust using AI coding agents. The new Rust-based version is now live in Claude Code v2.1.181 since June 17, 2026, improving startup speed by 10% on Linux. This rewrite challenges the long-held belief that large-scale software rewrites are unwise, demonstrating that AI agents can make such projects feasible and cost-effective. It also improves Bun's reliability, addressing a large number of memory-related bugs, which benefits its extensive user base. The rewrite took 11 days, cost approximately $165,000 in AI API tokens, and used 5.9 billion uncached input tokens and 690 million output tokens. The Bun TypeScript test suite served as a conformance suite to validate the port, which involved over 1 million lines of code added.

rss · Simon Willison · Jul 8, 23:57

**Background**: Bun is an all-in-one JavaScript runtime and toolkit designed as a fast alternative to Node.js. It was originally written in Zig, a low-level systems programming language focused on robustness and performance. Rust, another systems language, provides memory safety guarantees through its ownership model, which helps prevent use-after-free and double-free bugs that plagued the Zig version.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language) - Wikipedia</a></li>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/bun: Incredibly fast JavaScript runtime, bundler, test runner, and package manager – all in one</a></li>

</ul>
</details>

**Tags**: `#Bun`, `#Rust`, `#Zig`, `#JavaScript runtime`, `#programming languages`

---

<a id="item-3"></a>
## [TypeScript 7.0 Released with Go Rewrite, Up to 12x Speed](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft has officially released TypeScript 7.0, which replaces the original JavaScript-based compiler with a complete rewrite in Go, enabling true multi-threaded compilation and delivering 8 to 12 times faster build speeds. Developers can now install it via npm, and mainstream editors support the new language server through LSP. This performance breakthrough drastically reduces compilation times for large TypeScript codebases, improving developer productivity and CI/CD pipeline efficiency. It also sets a precedent for rewriting core developer tools in lower-level languages for better performance. The new version introduces --checkers and --builders flags to customize parallelism, and provides a compatibility package to coexist with TypeScript 6. However, embedded language toolchains like Vue and Svelte are not yet supported due to unfinished APIs, so older versions are still needed for those ecosystems.

telegram · zaihuapd · Jul 9, 04:01

**Background**: TypeScript is a superset of JavaScript that adds static typing, and its compiler has historically been written in JavaScript itself. Rewriting the compiler in Go allows it to leverage native multi-threading and better memory management, resulting in dramatic speed improvements. The Language Server Protocol (LSP) standardizes communication between editors and language servers, enabling consistent support across all major IDEs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Language_Server_Protocol">Language Server Protocol - Wikipedia</a></li>
<li><a href="https://visualstudiomagazine.com/articles/2026/06/22/typescript-7-0-rc-moves-microsofts-go-rewrite-into-the-mainline-compiler.aspx">TypeScript 7.0 RC Moves Microsoft's Go Rewrite Into the Mainline Compiler -- Visual Studio Magazine</a></li>

</ul>
</details>

**Tags**: `#TypeScript`, `#compiler`, `#performance`, `#Microsoft`, `#Go`

---

<a id="item-4"></a>
## [Ant Group Open-Sources LingBot-Video, First MoE Embodied Video Model](https://www.qbitai.com/2026/07/446458.html) ⭐️ 9.0/10

Ant Group's LingBot has open-sourced LingBot-Video, the world's first embodied video foundation model based on Mixture-of-Experts (MoE) architecture, with 30 billion total parameters and only 3 billion activated during inference. This is a significant milestone for embodied AI and robotics, as it provides an open-source model that can generate task-oriented videos for robot manipulation, accelerating research in simulation, world models, and policy learning. LingBot-Video uses a DiT+MoE architecture, a data engine with 70,000 hours of embodied data, and a multi-dimensional reinforcement learning reward system focusing on physical plausibility and task completion.

telegram · zaihuapd · Jul 9, 04:30

**Background**: Mixture-of-Experts (MoE) is a neural network design that activates only a subset of parameters per input, enabling large models with efficient inference. Diffusion Transformer (DiT) adapts the Transformer architecture for diffusion-based generative models. Embodied AI aims to create models that understand and interact with the physical world, often for robotics applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://openaccess.thecvf.com/content/ICCV2023/papers/Peebles_Scalable_Diffusion_Models_with_Transformers_ICCV_2023_paper.pdf">Scalable Diffusion Models with Transformers William Peebles* UC Berkeley</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Embodied AI`, `#MoE`, `#Video Generation`, `#Open Source`

---

<a id="item-5"></a>
## [EU Parliament Passes Chat Control 1.0 via Procedural Trick](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

The European Parliament allowed Chat Control 1.0 to pass without an affirmative majority, enabling mass scanning of private messages on services like Gmail and Snapchat until 2028. This sets a dangerous precedent for EU digital rights, as legislation can be forced through procedural maneuvers, undermining democratic checks. It also threatens user privacy across major platforms. The law applies only to non-end-to-end encrypted services and was passed using an 'urgency procedure' requiring an absolute majority of all MEPs (361) to reject, despite 314 voting against and 276 in favor.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control refers to EU proposals to scan private messages for child sexual abuse material (CSAM). Critics argue the technology is unreliable and violates privacy. The law was rejected twice in March but revived via a Council-backed procedure.

<details><summary>References</summary>
<ul>
<li><a href="https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/">EU Parliament greenlights Chat Control 1.0 – Breyer: "Our children lose out"</a></li>
<li><a href="https://www.techtimes.com/articles/320010/20260709/eu-parliament-passes-chat-control-default-314-meps-couldnt-block-scanning-law.htm">EU Parliament Passes Chat Control by Default: 314 MEPs Couldn't Block Scanning Law</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control">Chat Control - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters express outrage over the procedural trick, calling it undemocratic and a step toward totalitarianism. One user notes that the vote was held before summer break when many MEPs were absent, allowing rejection to fail.

**Tags**: `#privacy`, `#surveillance`, `#EU`, `#legislation`, `#digital rights`

---

<a id="item-6"></a>
## [Postgres rewritten in Rust passes all regression tests](https://github.com/malisper/pgrust) ⭐️ 8.0/10

A project called pgrust uses large language models (LLMs) to rewrite PostgreSQL in Rust, and now passes 100% of the PostgreSQL regression tests. This demonstrates the potential of LLMs for large-scale code translation, but raises critical questions about code quality, architectural changes (e.g., threading), and license compatibility between the original PostgreSQL license and the new AGPL license. The project generated over 7100 commits in less than a month, making traditional code review via commit history impractical. The license was changed from the permissive PostgreSQL license to AGPL, which may raise compatibility issues with the original codebase.

hackernews · SweetSoftPillow · Jul 9, 06:18 · [Discussion](https://news.ycombinator.com/item?id=48841676)

**Background**: PostgreSQL is a widely used open-source relational database with a 30-year history. Rust is a systems programming language known for memory safety and performance. Regression tests are a suite of tests that ensure new changes don't break existing functionality. This project uses LLMs to automatically translate C code to Rust, which is a novel but controversial approach.

**Discussion**: The author explained they are experimenting with LLMs to build a better Postgres. Commenters noted that the 100% regression tests do not cover the threaded architecture change, making the achievement less comprehensive. Others raised concerns about the difficulty of reviewing LLM-generated code with over 7100 commits in a month, and the license change from PostgreSQL to AGPL, questioning its compatibility with the original source.

**Tags**: `#database`, `#rust`, `#postgres`, `#llm`, `#open-source`

---

<a id="item-7"></a>
## [US Army logistics vulnerabilities analyzed](https://mwi.westpoint.edu/the-glass-backbone-why-the-armys-logistics-will-break-in-the-next-war/) ⭐️ 8.0/10

A recent analysis from the Modern War Institute argues that the US Army's logistics are dangerously brittle due to misconceptions about the tooth-to-tail ratio, and will likely fail in future conflicts. This matters because logistics is critical to military success, and if the Army does not reform its logistics system, it risks losing future wars despite technological advantages. The article contends that the tooth-to-tail ratio—the proportion of combat troops to support personnel—is misunderstood, leading to underinvestment in logistics. It warns that modern warfare's speed and complexity will overwhelm the current logistics backbone.

hackernews · baud147258 · Jul 9, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48845442)

**Background**: The tooth-to-tail ratio is a military metric comparing combat forces to support units. Historically, logistics has been undervalued in budget priorities. The analysis draws on historical examples and current conflicts like Ukraine to highlight systemic risks.

**Discussion**: Comments show strong agreement with the analysis, with users drawing historical parallels (e.g., Fabian strategy against Hannibal) and noting the ongoing Ukraine war as evidence. One comment suggests technologies like SpaceX's StarFall could transform logistics, but others remain skeptical.

**Tags**: `#logistics`, `#military`, `#systems analysis`, `#strategic studies`, `#resilience`

---

<a id="item-8"></a>
## [Meta launches Muse Spark 1.1 with commercial API](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 8.0/10

Meta has released Muse Spark 1.1, a new version of their proprietary AI model, and introduced a commercial API for developers to access it via a paid subscription. This move signals Meta's entry into the commercial AI model market, potentially disrupting competitors like OpenAI and Anthropic with aggressive pricing and an open-weight strategy that could commoditize coding models. The model was evaluated on Terminal-Bench-2.1, but community members noted that resource caps (6 CPU cores, 8GB RAM) were overridden, questioning the validity of the results. Pricing is set at $1.25 per million input tokens and $4.5 per million output tokens, with cached input at $0.15.

hackernews · ot · Jul 9, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48846184)

**Background**: Muse Spark is a proprietary large language model developed by Meta Superintelligence Labs (MSL), first released on April 8, 2026. The commercial API allows developers to integrate the model into their applications for a fee. Meta's open-weight strategy releases model weights publicly, fostering community adoption but potentially reducing competitors' revenue.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Muse_Spark_AI_model">Muse Spark (AI model)</a></li>

</ul>
</details>

**Discussion**: Community feedback was mixed: some users praised the competitive pricing and performance, while others criticized the evaluation methodology as flawed due to resource limit overrides. There was debate over Meta's strategic role as a 'spoiler' commoditizing AI models versus competing head-to-head with frontier labs.

**Tags**: `#Meta AI`, `#Muse Spark`, `#open-source AI`, `#AI model evaluation`, `#commercial AI`

---

<a id="item-9"></a>
## [AI content floods social media, especially LinkedIn](https://www.pangram.com/blog/ai-in-your-feed) ⭐️ 8.0/10

A blog post on Pangram highlights the increasing prevalence of AI-generated content on social media, particularly LinkedIn, sparking debates about authenticity and the nature of online discourse. This trend threatens genuine human connection and discourse on professional networks, as AI-written posts may erode trust and devalue authentic voices, affecting how people network and share knowledge. The post scores 8.0/10 due to high community engagement, with 162 points and 141 comments reflecting diverse viewpoints, from skepticism about AI writing to observations of bots and mimicry of AI speech patterns.

hackernews · mukmuk · Jul 9, 15:50 · [Discussion](https://news.ycombinator.com/item?id=48847940)

**Background**: AI tools like GPT-4 can generate human-like text, making it easy to produce social media posts at scale. LinkedIn, a professional network, relies on authentic personal insights for meaningful interaction. The rise of AI content raises questions about the platform's value and the authenticity of its users' voices.

**Discussion**: Community comments show strong disagreement: some argue AI writing destroys personal voice and authenticity, while others note that LinkedIn has always had scripted content, and AI just accelerates it. A user also points out that people are increasingly mimicking AI speech patterns, even if not directly using AI.

**Tags**: `#AI`, `#social media`, `#content generation`, `#LinkedIn`, `#authenticity`

---

<a id="item-10"></a>
## [OpenAI Launches GPT-Live Voice Mode with GPT-5.5 Delegation](https://simonwillison.net/2026/Jul/8/introducing-gptlive/#atom-everything) ⭐️ 8.0/10

OpenAI introduced GPT-Live, an upgraded voice mode model for ChatGPT that can delegate complex tasks like web search and reasoning to GPT-5.5 while maintaining conversation flow. This update significantly improves the usefulness of ChatGPT voice mode, transforming it into a more capable brainstorming partner that can handle both conversational and complex reasoning tasks. GPT-Live replaces the previous GPT-4o era model and allows users to have long conversations—a full hour was tested—while it seamlessly delegates harder tasks to GPT-5.5 in the background.

rss · Simon Willison · Jul 8, 23:20

**Background**: GPT-5.5 is a large language model released by OpenAI on April 23, 2026, known by codename 'Spud'. It achieved notable benchmark scores on Terminal-Bench 2.0 and FrontierMath. OpenAI had previously used a GPT-4o era model for voice mode, which had a knowledge cut-off in 2024 and limited capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-Live`, `#ChatGPT`, `#Voice Mode`, `#AI`

---

<a id="item-11"></a>
## [Meta's Superintelligence Update Reveals RL Startup and Compute Scaling](https://newsletter.semianalysis.com/p/the-future-of-meta-superintelligence) ⭐️ 8.0/10

Meta's superintelligence initiative progress update reveals the emergence of a top-tier reinforcement learning environment startup and what is described as the most aggressive compute ramp ever seen, spanning over 2000 km. This indicates Meta is making rapid progress in superintelligence R&D, with significant implications for the AI industry and competitive dynamics, particularly for Google DeepMind. The update mentions a new reinforcement learning environment startup, unprecedented compute scaling across 2000+ km, and strategic advice for Google DeepMind, suggesting major infrastructure developments.

rss · Semianalysis · Jul 9, 19:16

**Background**: Superintelligence refers to artificial intelligence that surpasses human cognitive abilities in virtually all domains. Meta has been investing heavily in AI, particularly in reinforcement learning and large-scale compute infrastructure. The RL environment startup likely provides simulation platforms for training advanced AI agents.

**Tags**: `#Meta`, `#Superintelligence`, `#Reinforcement Learning`, `#Compute Scaling`, `#AI Progress`

---

<a id="item-12"></a>
## [IMGNet: Face Verification via Sign Patterns Replaces Cosine Similarity](https://www.reddit.com/r/MachineLearning/comments/1urxvxh/i_built_imgnet_a_face_verification_model_that/) ⭐️ 8.0/10

IMGNet introduces a face verification model that uses sliding window sign pattern matching instead of cosine similarity, achieving 96.27% on LFW with a 10.58 MB model trained on CASIA-WebFace. This work challenges the default use of cosine similarity in face verification by showing that sign pattern consistency can yield competitive results, potentially opening new directions for metric design in embedding-based recognition systems. The model includes a novel SW Block layer that computes multi-scale relational differences, and an IMG Sign MSE Loss defined purely over sign pattern agreement without amplitude dependency. When applied to ArcFace embeddings without retraining, the IMG Sign Score achieves 99.58% on LFW.

reddit · r/MachineLearning · /u/img-_- · Jul 9, 18:00

**Background**: Face verification typically uses neural networks to map faces into embedding vectors, then compares them using cosine similarity. Cosine similarity measures the angle between vectors, which is sensitive to global direction but ignores local sign patterns. IMGNet instead examines sign patterns across sliding windows, preserving relational structure.

**Tags**: `#face verification`, `#machine learning`, `#embeddings`, `#novel approach`

---

<a id="item-13"></a>
## [DJI EV50 drone reaches 8861m over Everest](https://www.163.com/dy/article/L1CUCV940514R9OJ.html) ⭐️ 8.0/10

DJI's unreleased EV50 vertical takeoff and landing (VTOL) drone participated in the 'Peak Mission' Everest scientific expedition, flying to 8,861 meters on the north slope, setting a record for the highest altitude in public testing among similar drones. This achievement demonstrates DJI's capability in high-altitude operations and low-altitude logistics, potentially impacting drone delivery and scientific research in extreme environments. The EV50 is a hybrid-wing drone that can take off and land vertically and switch to fixed-wing cruise. During the 12-day mission, it completed 32 sorties, climbed continuously for 3,730 meters, and still had 30% battery remaining on return.

telegram · zaihuapd · Jul 9, 06:00

**Background**: Vertical takeoff and landing (VTOL) drones combine the advantages of multirotors and fixed-wing aircraft, enabling operation in confined spaces while maintaining efficient long-range flight. High-altitude flights pose challenges due to thin air, cold temperatures, and strong winds. DJI is a leading drone manufacturer, and the EV50 is designed for cargo transport and low-altitude logistics.

**Tags**: `#无人机`, `#大疆`, `#珠峰`, `#航空科技`, `#物流`

---

<a id="item-14"></a>
## [China's Supercomputing Internet Core Node Launches in Zhengzhou](https://36kr.com/newsflashes/3887797387344387) ⭐️ 8.0/10

On July 9, 2026, the core node of China's National Supercomputing Internet officially launched in Zhengzhou, providing access to over 100,000 domestic AI computing cards. This marks a major milestone in China's national computing infrastructure, creating the largest single pool of domestic AI compute resources under the Supercomputing Internet platform, which will accelerate AI research and development across the country. The node acts as the core for operations management, resource scheduling, and also integrates supply-demand matching and industry incubation services, aiming to build a nationwide computing resource coordination system.

telegram · zaihuapd · Jul 9, 07:00

**Background**: The National Supercomputing Internet is a project to connect supercomputing centers and AI computing resources across China into a unified network. The core node in Zhengzhou is the largest single resource pool connected to this platform, providing massive domestic AI computing capacity.

**Tags**: `#supercomputing`, `#AI infrastructure`, `#domestic computing`, `#China tech`, `#national project`

---

<a id="item-15"></a>
## [OpenAI and US War Dept to Ban AI for Citizen Surveillance](https://t.me/zaihuapd/42459) ⭐️ 8.0/10

OpenAI and the US Department of War have agreed to revise their AI contract to explicitly prohibit the use of AI systems for monitoring US citizens, a move initiated by OpenAI CEO Sam Altman to address ethical concerns. This sets a significant precedent for ethical AI use in military contracts, potentially influencing other tech companies and government policies to protect civil liberties against AI-driven surveillance. The revised clause specifically bans intentional surveillance of US citizens and prohibits tracking or monitoring using personally identifiable information obtained commercially. The contract amendment has not been formally signed yet.

telegram · zaihuapd · Jul 9, 13:22

**Background**: OpenAI has been expanding its partnerships with US defense agencies, including the Department of War (formerly the Pentagon), raising ethical concerns about AI in warfare. Anthropic, another AI company, previously suspended a similar contract with the War Department due to controversy.

**Tags**: `#AI ethics`, `#OpenAI`, `#military AI`, `#surveillance`, `#AI regulation`

---