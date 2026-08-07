---
layout: default
title: "Horizon Summary: 2026-08-07 (EN)"
date: 2026-08-07
lang: en
---

> From 35 items, 11 important content pieces were selected

---

1. [DeepSeek V4 Flash 0731: Fast, Cheap, and Capable Model Update](#item-1) ⭐️ 8.0/10
2. [Assembly Hall of Shame: A Curated Collection of Extremely Slow x86 Instructions](#item-2) ⭐️ 8.0/10
3. [Why Everyone in Tech So Sad: Losing Faith in the Industry](#item-3) ⭐️ 8.0/10
4. [Oracle's OpenJDK Bans AI-Generated Code Contributions](#item-4) ⭐️ 8.0/10
5. [pgrust Rewrites Postgres in Rust, Claiming 300x Faster Analytics](#item-5) ⭐️ 8.0/10
6. [2027 HBM Capacity Sold Out, Squeezing DRAM Supply](#item-6) ⭐️ 8.0/10
7. [Fighting Scrapers: A Year-Long Battle on a 1.5 Million-Page Website](#item-7) ⭐️ 8.0/10
8. [New Mexico Court Orders Meta to Pay $567M Over Children's Mental Health Harms](#item-8) ⭐️ 8.0/10
9. [Gemini Stumbles, Google Cloud Profits](#item-9) ⭐️ 8.0/10
10. [US Reviews China's Offshore Access to Nvidia Chips After AI Breakthroughs](#item-10) ⭐️ 8.0/10
11. [Critical OAuth flaw in sub2api allows account takeover via email only](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Flash 0731: Fast, Cheap, and Capable Model Update](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 8.0/10

DeepSeek released the updated V4 Flash 0731 model, an efficiency-optimized Mixture-of-Experts LLM with 284B total parameters and 13B activated parameters. It delivers faster inference, lower cost, and stronger debugging and data-analysis abilities compared with the earlier preview. This release gives developers a compelling open-weight option that combines top-tier coding performance with very low inference costs, narrowing the gap with leading closed-source models. It is particularly relevant for teams building agentic or reasoning-heavy applications on a budget. The model uses a Mixture-of-Experts architecture with 284B total parameters, only 13B activated per token, and supports a 1M-token context window. The 07/31 build is a substantial update over the earlier preview, and a separate V4 Flash-Max variant offers reasoning close to the Pro version with more thinking time.

hackernews · tosh · Aug 7, 17:56 · [Discussion](https://news.ycombinator.com/item?id=49214008)

**Background**: DeepSeek is an AI lab that releases open-weight large language models, competing with both open and proprietary systems. Mixture-of-Experts (MoE) models keep total parameter counts large but activate only a small subset per token, which cuts compute and cost. V4 Flash is the efficiency-oriented member of the DeepSeek-V4 series, aimed at fast, low-cost inference.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash">DeepSeek V 4 Flash - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://ollama.com/library/deepseek-v4-flash">deepseek - v 4 - flash</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, with users praising the low cost (spending around $5/day or under $100/month) and high speed, including strong local performance on RTX Pro 6000 Blackwell GPUs. Several users note it is now good enough for almost everything, while one off-topic comment mentions a Claude account ban.

**Tags**: `#AI`, `#DeepSeek`, `#LLM`, `#Model Release`, `#Benchmark`

---

<a id="item-2"></a>
## [Assembly Hall of Shame: A Curated Collection of Extremely Slow x86 Instructions](https://github.com/xoreaxeaxeax/asm-hall-of-shame) ⭐️ 8.0/10

The GitHub repository 'Assembly Hall of Shame' curates notoriously slow x86 instructions and provides methods for timing them, exposing surprising hardware performance pitfalls. It includes benchmark results such as a 12 ms write to an ACPI IO port, which currently sits at position 8 on the leaderboard. This project highlights that instruction-level performance on modern x86 CPUs is not intuitive and can be off by orders of magnitude, which matters for low-level developers, OS engineers, and security researchers. It also sparked discussion about abusing such slow paths, for example to trigger or break System Management Mode (SMM). The repository enforces a rule that trapped, emulated, or virtualized instructions may only time the trap itself, not the handler, in order to keep measurements meaningful. However, some commenters suspect that the 12 ms write to an ACPI IO port might actually be handled by SMM, which would blur that distinction.

hackernews · piotrgrabowski · Aug 7, 18:01 · [Discussion](https://news.ycombinator.com/item?id=49214098)

**Background**: x86 processors include many instructions whose execution time varies wildly depending on the operand, addressing mode, and microarchitectural state. Timing is usually done with the Time Stamp Counter (TSC) via the RDTSC instruction, but pitfalls such as out-of-order execution, frequency scaling, and SMM interrupts can distort measurements. Agner Fog's instruction tables and dedicated timing guides document latencies and throughputs for AMD and Intel processors. The project builds on this tradition by collecting real-world examples of instructions that are surprisingly slow.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Time_Stamp_Counter">Time Stamp Counter - Wikipedia</a></li>
<li><a href="https://www.agner.org/optimize/instruction_tables.pdf">Introduction Page 1 4. Instruction tables By Agner Fog</a></li>
<li><a href="https://wassenberg.dreamhosters.com/articles/timing_pitfalls.pdf">Timing Pitfalls and Solutions</a></li>

</ul>
</details>

**Discussion**: The comments reflect broad interest and humor: one user jokes that NOP is infinitely slow relative to what it does, and another connects the project to the Core War game. A more serious exchange questions whether the ACPI port write traps into SMM, linking to a related project that abuses slow instructions to break SMI. Another comment laments how much compute is wasted on abstraction layers, echoing the repo's theme.

**Tags**: `#assembly`, `#x86`, `#performance`, `#low-level`, `#hardware`

---

<a id="item-3"></a>
## [Why Everyone in Tech So Sad: Losing Faith in the Industry](https://www.noemamag.com/why-is-everyone-in-tech-so-sad/) ⭐️ 8.0/10

In a new essay for Noema Magazine, "Why Is Everyone in Tech So Sad?" explores the widespread sadness and loss of faith among technology workers, drawing parallels to the decline of skilled trades such as printing. The author contends that the once-bright promise of a tech career has dimmed, leaving many feeling betrayed by their own industry. This matters because it articulates a widespread burnout and disillusionment that is rarely examined in depth for a group as influential as tech workers. The historical comparison with printers suggests that today's tech professionals may face structural disruption, prompting critical conversations about career longevity and the future of knowledge work. The essay uses the history of printers—a respected craft that was ultimately eliminated by technological change—as a cautionary tale. It also touches on how the very innovations that created modern tech roles may now be devaluing them, leaving workers without a clear sense of direction.

hackernews · RickJWagner · Aug 7, 12:42 · [Discussion](https://news.ycombinator.com/item?id=49209539)

**Background**: The tech industry has long been perceived as a realm of limitless opportunity, where skilled workers enjoyed high pay and meaningful innovation. In recent years, however, a wave of layoffs, burnout, and declining purpose has given rise to what some call a "tech malaise." By invoking historical parallels like the printing trade, the essay frames today's anxiety not as a personal failure but as part of a larger pattern of industries being upended by their own success.

**Discussion**: Community comments strongly resonate with the essay's themes. One user compares tech workers to printers, noting how that trade vanished entirely; others point to the toxicity of the online world and a general erosion of work ethic. Many express personal disillusionment—one veteran of over twenty years says he now daydreams about being homeless, underscoring the depth of dissatisfaction.

**Tags**: `#tech culture`, `#burnout`, `#mental health`, `#software engineering`, `#industry analysis`

---

<a id="item-4"></a>
## [Oracle's OpenJDK Bans AI-Generated Code Contributions](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 8.0/10

The OpenJDK project has published an interim policy banning or restricting AI-generated code contributions, as announced in a post on openjdk.org/legal/ai. Oracle's lawyers are still drafting the final version of this policy. This is a significant policy shift for one of the world's most important open-source projects, affecting how Java contributors work and shaping debate on AI provenance in open source. It also highlights the irony that Oracle (led by Larry Ellison) heavily promotes AI while refusing AI-generated code from outside. The policy is explicitly positioned as a risk-management measure, focused on legal provenance rather than purely code quality. The final version is still being written by Oracle's legal team, so the interim rules may change.

hackernews · delduca · Aug 7, 17:36 · [Discussion](https://news.ycombinator.com/item?id=49213754)

**Background**: OpenJDK is the open-source reference implementation of the Java platform, maintained by Oracle and a community of developers. AI-generated code can carry uncertain copyright provenance because models may be trained on licensed or copyrighted code, creating legal risk for projects that accept such contributions. Oracle has a long history of aggressive copyright enforcement around Java, including lawsuits over the Java API.

**Discussion**: Commenters generally understood the decision as a legal/risk-management move, though many noted the irony with Oracle's own AI push. Some expressed skepticism about the final policy, while others pointed out that the burden on human reviewers is a real concern.

**Tags**: `#OpenJDK`, `#Oracle`, `#AI-generated code`, `#open source policy`, `#software licensing`

---

<a id="item-5"></a>
## [pgrust Rewrites Postgres in Rust, Claiming 300x Faster Analytics](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 8.0/10

The blog post 'Making Postgres 300x faster for analytics' introduces pgrust, a Rust-based reimplementation of PostgreSQL that achieves up to 300x speedups on analytical queries via batching, operator fusion, and SIMD. The project is also compiled to WebAssembly, allowing it to run in the browser. This is significant because it challenges the assumption that PostgreSQL's query engine is near its performance ceiling, and shows how modern techniques can deliver order-of-magnitude gains. It could influence future Postgres development and spark broader adoption of adaptive planning and vectorized execution in traditional databases. The speedup comes from three techniques: batching rows to reduce per-tuple overhead, fusing operators to avoid materializing intermediate results, and using SIMD instructions to process multiple values at once. The author emphasizes correctness as the top priority, using formal verification and differential fuzz testing to prove 1,000+ functions match Postgres's logic.

hackernews · poly2it · Aug 7, 11:00 · [Discussion](https://news.ycombinator.com/item?id=49208535)

**Background**: PostgreSQL is a widely used open-source relational database, but its row-at-a-time executor is slower on analytical workloads than columnar and vectorized systems like ClickHouse. pgrust is an experimental rewrite in Rust meant to show what Postgres could look like if built today; it can compile to WebAssembly and run queries in the browser. Batching, operator fusion, and SIMD are proven techniques in database engines, used by systems like DuckDB, to reduce per-row overhead and better utilize modern CPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/pgrust: Postgres rewritten in Rust, now faster than Postgres and Clickhouse · GitHub</a></li>
<li><a href="https://pgrust.com/">pgrust — postgres, rewritten in rust</a></li>

</ul>
</details>

**Discussion**: Author comments state that correctness is top priority, with formal verification and differential fuzz testing proving over 1,000 functions match Postgres. Some commenters question whether a critical database can gain trust outside the official Postgres team, while others are excited about adaptive planning, a feature long resisted by the Postgres core team.

**Tags**: `#postgres`, `#query-engine`, `#rust`, `#performance`, `#simd`

---

<a id="item-6"></a>
## [2027 HBM Capacity Sold Out, Squeezing DRAM Supply](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

Memory industry reports that HBM (High Bandwidth Memory) capacity for 2027 is fully sold out, driven by surging AI demand. This leaves less wafer capacity for commodity DRAM, tightening overall memory supply. This marks a multi-year supply constraint for memory, affecting not just AI accelerators but also consumer electronics like PCs, consoles, and phones. Prices for DRAM and devices could rise, and AI hardware production may be bottlenecked. HBM consumes roughly three times the wafer supply of standard DDR5 to produce the same number of bits on a given technology node, because HBM dies are larger. Since HBM is prioritized, non-HBM DRAM output growth will be limited.

hackernews · inigyou · Aug 7, 07:58 · [Discussion](https://news.ycombinator.com/item?id=49207236)

**Background**: HBM is a 3D-stacked DRAM interface used with GPUs and accelerators, developed by Samsung, AMD, and SK Hynix. It provides much higher bandwidth than regular DRAM by stacking dies vertically and connecting them via through-silicon vias to a logic die. AI model training and inference demand enormous memory bandwidth, making HBM critical.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://medium.com/the-low-end-disruptor/the-great-wall-of-high-bandwidth-memory-hbm-4d19b9f48549">The Great Wall of High Bandwidth Memory ( HBM ) | Medium</a></li>
<li><a href="https://acepcba.com/what-is-hbm-memory-why-does-ai-hardware-need-it/">What Is HBM Memory and Why Does AI Hardware Depend on It ?</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern about broader market effects: one noted HBM capacity 'sold out' means fewer wafers for DDR5, another worried about inflation for consumer products, and one user described an urge to stockpile microcontrollers. Some also reflected on the user-level impact, with one saying AI's memory/storage pressure makes them hesitant to use AI.

**Tags**: `#HBM`, `#memory`, `#semiconductors`, `#supply chain`, `#AI`

---

<a id="item-7"></a>
## [Fighting Scrapers: A Year-Long Battle on a 1.5 Million-Page Website](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

A website owner of a 1.5‑million‑page site published a detailed retrospective of a year spent defending against scrapers and bots, revealing that a single bad month caused hosting costs to jump roughly 500% from a baseline of about $90. The post covers the strategies used, including Cloudflare challenges, and the practical and philosophical costs of fighting bot traffic. This account matters because it quantifies the real operational and financial burden that AI scrapers and bots impose on independent web publishers. It also feeds into the broader industry debate about centralized bot protection (Cloudflare) versus self‑hosted alternatives, and who ultimately controls access to public web content. The site runs on Cloudflare Workers and D1, a serverless SQLite database; a single 'bad spike month' drove the monthly bill from about $90 to roughly 500% higher. The author also acknowledges that the site itself scrapes public documents, noting the irony of a scraper complaining about scrapers.

hackernews · petercooper · Aug 7, 14:51 · [Discussion](https://news.ycombinator.com/item?id=49211386)

**Background**: Web scraping is the automated extraction of website data, and for site owners it can overwhelm servers and inflate bills when bots consume bandwidth and database queries. Many websites rely on Cloudflare's bot protection, which includes Turnstile, a CAPTCHA‑alternative challenge platform. The rise of AI crawlers such as OpenAI's GPTBot has intensified the volume and sophistication of scraping, making this a growing concern for independent publishers.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Cloudflare_Turnstile">Cloudflare Turnstile</a></li>
<li><a href="https://datadome.co/bots/gptbot/">What is the GPTBot?</a></li>

</ul>
</details>

**Discussion**: Commenters largely sympathize with the author but split on solutions: some warn against relying on Cloudflare's centralized control and recommend self‑hosted proof‑of‑work tools like Anubis, while others suggest moving off D1 to a static site to cut costs. Several share their own scraper‑related numbers — one notes Claude‑searchbot fetched 205,000 pages in 72 hours while sending just one referral — and highlight the irony that the author's site itself scrapes public documents.

**Tags**: `#web scraping`, `#bot protection`, `#Cloudflare`, `#website security`, `#AI crawlers`

---

<a id="item-8"></a>
## [New Mexico Court Orders Meta to Pay $567M Over Children's Mental Health Harms](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta) ⭐️ 8.0/10

A New Mexico state court ordered Meta to pay $567 million for harming children's mental health through its social media platforms, and to make changes for underage users. The judgment stems from a lawsuit alleging Meta violated public-nuisance law by designing addictive features that harmed minors. This is one of the largest state-level judgments against a major social media company over youth mental health, and could set a precedent for other states and jurisdictions pursuing similar claims. It pressures Meta and the broader industry to rethink algorithmic design and child-safety protections. The ruling leverages New Mexico's public-nuisance law, NMSA 1978 § 30-8-1, rather than federal Section 230 protections. Reports differ on the total amount: Reuters and The Guardian cite $567 million for a teen mental health fund, while The Wall Street Journal reports a $942 million total judgment.

hackernews · boplicity · Aug 7, 00:06 · [Discussion](https://news.ycombinator.com/item?id=49204352)

**Background**: Social media companies have faced growing scrutiny over the impact of their platforms on young users' mental health, with studies linking heavy use to anxiety and depression. New Mexico's lawsuit, filed by the state attorney general, sought to hold Meta accountable under state public-nuisance law, an approach that bypasses the federal immunity that protects platforms from being treated as publishers of third-party content.

**Discussion**: Commenters noted that while $567 million or even $942 million is a small fraction of Meta's global revenue, it is a massive penalty when apportioned to New Mexico's 2.1 million residents. One user pointed to the specific public-nuisance statute and the applicable section, while others analogized Instagram Reels and TikTok to addictive substances and urged Meta to change its algorithms.

**Tags**: `#social-media`, `#regulation`, `#mental-health`, `#meta`, `#legal`

---

<a id="item-9"></a>
## [Gemini Stumbles, Google Cloud Profits](https://newsletter.semianalysis.com/p/gemini-is-cooked-but-gcp-is-cooking) ⭐️ 8.0/10

A SemiAnalysis article argues that DeepMind's difficulties with its Gemini AI models will paradoxically boost Google Cloud Platform's short-term growth. The analysis reframes DeepMind's long-term challenges as a short-term tailwind for GCP's cloud infrastructure business. This matters because it highlights a strategic split inside Google between DeepMind's long-term AI ambitions and GCP's commercial momentum. It suggests that even if Google's frontier models fall behind, its cloud arm could still capture significant revenue from the broader AI boom. The core claim is a timing mismatch: DeepMind's long-term failure becomes GCP's short-term gain because demand for AI compute and cloud revenue keeps growing regardless of model quality. The article focuses on business strategy and market dynamics rather than technical benchmarks or specific product releases.

rss · Semianalysis · Aug 7, 02:32

**Background**: Google DeepMind is Google's AI research unit responsible for the Gemini family of large language models, which compete with OpenAI's GPT series. Google Cloud Platform (GCP) sells cloud computing and AI infrastructure services to external customers. The article's argument rests on the observation that a company's own model quality and its cloud infrastructure revenue can diverge, especially when external demand for AI compute is strong.

**Tags**: `#AI`, `#Google Cloud`, `#DeepMind`, `#Strategy`, `#Cloud Computing`

---

<a id="item-10"></a>
## [US Reviews China's Offshore Access to Nvidia Chips After AI Breakthroughs](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 8.0/10

The US Commerce Department's Bureau of Industry and Security (BIS) has launched a systematic review of how Chinese AI companies obtain and use Nvidia chips abroad, including via remote access to overseas computing resources. The review was triggered in part by the recent release of Moonshot AI's Kimi K3 model, which a White House official accused of being powered by illegally obtained Nvidia chips accessed remotely from Thailand. This review could expand US export controls beyond hardware sales to cover cloud-based remote computing, directly affecting Nvidia and other US tech companies' ability to serve global customers. It also signals a new front in US-China tech competition, potentially reshaping how AI firms worldwide access advanced chips. BIS is compiling two lists: one of black-market locations suspected of smuggling restricted chips into China, and another of countries where Chinese companies remotely rent chips. The report also alleges that Alibaba, through a Singapore shell company controlled by a Cayman entity, uses Nvidia chips in Malaysia via Megaspeed, a company already under US investigation.

telegram · zaihuapd · Aug 7, 11:18

**Background**: The US has restricted exports of advanced AI chips to China since 2022, but Chinese companies have sought to circumvent these controls by leasing computing power from data centers in other countries. Remote access to chips is not inherently illegal, and it is unclear whether BIS has authority to restrict such cloud computing arrangements. The US House has passed a bipartisan bill to explicitly grant that power, though it is expected to face opposition from Nvidia and other tech companies.

**Tags**: `#US-China tech policy`, `#export controls`, `#AI hardware`, `#Nvidia`, `#cloud computing`

---

<a id="item-11"></a>
## [Critical OAuth flaw in sub2api allows account takeover via email only](https://github.com/Wei-Shaw/sub2api/issues/5350) ⭐️ 8.0/10

A critical OAuth vulnerability (CVSS 8.8) in sub2api v0.1.171 and earlier allows attackers to take over any account knowing only the victim's email address, without password, captcha, or user interaction. The flaw leverages the pending session flow's existingUser branch to bind an attacker's OAuth identity to the victim's account. This vulnerability enables full account takeover, giving attackers control over API keys, billing balance, and subscription quotas. Since OAuth is widely used, this highlights the importance of verifying identity binding steps in OAuth flows. The exploit targets the pending session flow's existingUser branch, which fails to verify password or captcha when binding an OAuth identity. After binding, every subsequent OAuth login by the attacker resolves to the victim's account.

telegram · zaihuapd · Aug 7, 14:59

**Background**: OAuth 2.0 is a widely used framework that lets users log in to sites using social media accounts. Common OAuth vulnerabilities include redirect URI manipulation, weak CSRF protection, and missing PKCE, but this case stems from an insecure account-binding logic in sub2api. Account takeover occurs when an attacker links their own identity to a victim's existing account, gaining full access.

<details><summary>References</summary>
<ul>
<li><a href="https://portswigger.net/web-security/oauth">OAuth 2.0 authentication vulnerabilities | Web Security Academy</a></li>
<li><a href="https://outpost24.com/blog/common-oauth-vulnerabilities-mitigations/">7 common OAuth vulnerabilities (plus mitigations)</a></li>

</ul>
</details>

**Tags**: `#security`, `#oauth`, `#vulnerability`, `#account-takeover`, `#sub2api`

---