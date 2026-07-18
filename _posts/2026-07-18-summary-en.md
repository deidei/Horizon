---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 37 items, 12 important content pieces were selected

---

1. [Kimi K3: Chinese AI Model Rivals Frontier Labs at Lower Cost](#item-1) ⭐️ 9.0/10
2. [GPT-5.6 Solves 30-Year Convex Optimization Conjecture](#item-2) ⭐️ 8.0/10
3. [LG monitors silently install software via Windows Update](#item-3) ⭐️ 8.0/10
4. [What AI did to Stack Overflow in a graph](#item-4) ⭐️ 8.0/10
5. [PHK Reflects on Bikeshedding and Says Goodbye](#item-5) ⭐️ 8.0/10
6. [Claude Fable 5 Made Permanent on Subscriptions](#item-6) ⭐️ 8.0/10
7. [DeepMind/Kaggle Grand Prize Winner Accused of AI Slop](#item-7) ⭐️ 8.0/10
8. [Doubao Phone shifts from GUI to MCP, stockpiles hundreds of thousands](#item-8) ⭐️ 8.0/10
9. [Meta in Talks to Lease AI Compute to Anthropic for $10B](#item-9) ⭐️ 8.0/10
10. [SpaceX in Talks with Pentagon for Multibillion-Dollar AI Compute Deal](#item-10) ⭐️ 8.0/10
11. [TSMC A14 Process to Enter Production in 2028](#item-11) ⭐️ 8.0/10
12. [Trump Administration Considers FINRA-like Watchdog for Top AI Models](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Kimi K3: Chinese AI Model Rivals Frontier Labs at Lower Cost](https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/) ⭐️ 9.0/10

Chinese startup Moonshot AI released Kimi K3, a 2.8 trillion parameter model that achieves performance comparable to GPT-5.6 and Opus 4.8 at lower API prices. This milestone challenges US dominance in AI and raises debates about knowledge distillation ethics and national security, as open-weight frontier models become more accessible and affordable. Kimi K3 has a 1M-token context window and costs $3/$15 per million input/output tokens, compared to $5/$25-$30 for comparable US models, though some users report it consuming more compute time on complex tasks.

hackernews · sbochins · Jul 18, 17:32 · [Discussion](https://news.ycombinator.com/item?id=48960218)

**Background**: Knowledge distillation is a technique where a smaller model is trained to emulate a larger, more powerful model, often used to create cheaper, faster models. Frontier AI models are the most advanced general-purpose systems. Kimi K3 is reported to have 2.8 trillion parameters, putting it in the same league as top US models like GPT-5.6 and Opus 4.8.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/17/moonshot-ai-kimi-k3-model-openai-anthropic-china.html">China's Moonshot AI unveils Kimi K3 that rivals OpenAI, Anthropic</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation</a></li>

</ul>
</details>

**Discussion**: Comments highlight that distillation is an inevitable progression, with one user noting it was always going to happen. Another user found Kimi K3 slower and more expensive in usage than expected, while a third raised concerns about national security implications and possible criminalization of using such models.

**Tags**: `#AI`, `#distillation`, `#frontier models`, `#national security`, `#cost efficiency`

---

<a id="item-2"></a>
## [GPT-5.6 Solves 30-Year Convex Optimization Conjecture](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 8.0/10

OpenAI's GPT-5.6 large language model used a single prompt to produce a proof that resolves a 30-year-old open conjecture in convex optimization, marking a significant AI contribution to mathematical research. This demonstrates that LLMs can tackle long-standing theoretical problems in mathematics and theoretical computer science, potentially accelerating research and shifting how mathematicians approach open problems. It also raises questions about the future role of human researchers in solving such conjectures. The conjecture concerns upper bounds on the time complexity of solving convex optimization problems over convex Lipschitz functions, specifically on a spherical domain (which can be generalized to any bounded domain via variable transformation). The proof was produced by GPT-5.6's Sol Pro variant, not the more capable Ultra variant.

hackernews · mbustamanter · Jul 18, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48957779)

**Background**: Convex optimization is a subfield of mathematical optimization that minimizes convex objective functions over convex sets, with many problems solvable in polynomial time. GPT-5.6 is OpenAI's large language model released in July 2026, available in three variants: Luna, Terra, and Sol. The Sol variant is designed for enterprise work, coding, and scientific research, with Sol Pro being a more advanced version capable of orchestrating multi-step reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization">Convex optimization</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6</a></li>

</ul>
</details>

**Discussion**: Commenters noted that while the solved conjecture is more niche than the cyclic double cover conjecture from OpenAI, it represents a real contribution. There was discussion about whether LLMs could target impenetrable proofs like Mochizuki's abc conjecture proof, and observations that AI can apply enormous brute force to problems. Some questioned the difference between GPT-5.6 variants and the implications for junior researchers.

**Tags**: `#AI`, `#mathematics`, `#convex optimization`, `#LLM`, `#research`

---

<a id="item-3"></a>
## [LG monitors silently install software via Windows Update](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent) ⭐️ 8.0/10

Connecting certain LG monitors to a Windows PC automatically installs software, including a McAfee subscription promoter, via Windows Update without user consent. This automatic installation undermines user control over their systems and poses security and privacy risks, as arbitrary third-party software can gain full system and internet access. The software installs immediately when a monitor is connected via HDMI, runs on every system boot, and is not sandboxed, affecting both new and previously connected LG monitors.

hackernews · baranul · Jul 18, 10:21 · [Discussion](https://news.ycombinator.com/item?id=48956688)

**Background**: Windows Update has a feature that automatically downloads and installs recommended device drivers and associated software from hardware vendors. While intended for convenience and compatibility, this mechanism can be exploited by vendors to push unwanted applications without user interaction.

<details><summary>References</summary>
<ul>
<li><a href="https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent">LG monitors silently install software through Windows Update ...</a></li>
<li><a href="https://support.microsoft.com/en-US/Windows/Hardware/Drivers/automatically-get-recommended-and-updated-hardware-drivers">Automatically get recommended and updated hardware drivers</a></li>
<li><a href="https://www.fingerlakes1.com/2026/07/18/lg-monitor-software-now-installs-through-windows-update-and-many-users-did-not-expect-it/">LG Monitor Software Now Installs Through Windows Update and ...</a></li>

</ul>
</details>

**Discussion**: Community comments describe the behavior as malware-like, highlighting that it occurs without any user action and grants full system access. Users share workarounds via Group Policy or device installation settings to block automatic downloads, and some blame Microsoft for not vetting such software before distribution.

**Tags**: `#security`, `#privacy`, `#windows`, `#drivers`, `#windows-update`

---

<a id="item-4"></a>
## [What AI did to Stack Overflow in a graph](https://data.stackexchange.com/stackoverflow/query/1953768#graph) ⭐️ 8.0/10

A graph from Stack Exchange Data Explorer shows a sharp decline in Stack Overflow activity, which community members attribute to both the rise of large language models (LLMs) and the site's exclusionary policies. This trend underscores how AI-driven tools and governance decisions can reshape online knowledge communities, pushing developers toward faster AI-generated answers over traditional Q&A platforms. The graph reveals Stack Overflow's activity peaked in 2014, long before LLMs became mainstream, and the decline accelerated after the site's acquisition by Prosus in 2021 and the release of ChatGPT in 2022.

hackernews · secretslol · Jul 18, 11:12 · [Discussion](https://news.ycombinator.com/item?id=48956949)

**Background**: Stack Overflow is a popular Q&A platform for programmers, where users ask and answer technical questions. Large language models (LLMs) like GPT-4 can generate code and explanations, reducing the need to visit the site. The graph is created using the Stack Exchange Data Explorer, which allows custom queries of site data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters widely agree that Stack Overflow's strict moderation and hostility toward new users drove people away even before AI became a factor. Some note that the decline started well before LLMs, pointing to the 2014 peak and the negative impact of the Prosus acquisition.

**Tags**: `#Stack Overflow`, `#AI impact`, `#community decline`, `#LLMs`, `#Q&A platforms`

---

<a id="item-5"></a>
## [PHK Reflects on Bikeshedding and Says Goodbye](https://queue.acm.org/detail.cfm?id=3818307) ⭐️ 8.0/10

Poul-Henning Kamp, who popularized the term 'bikeshedding' in open source, published a farewell article in ACM Queue reflecting on the phenomenon and its impact on community dynamics. This reflective piece from a founding figure provides valuable insight for open source maintainers and participants, highlighting a persistent communication pitfall. The high engagement (166 points, 174 comments) underscores its resonance with the community. The article revisits Kamp's famous 1999 essay 'Why Should I Care What Color the Bikeshed Is?' and discusses how bikeshedding continues to affect decision-making in open source projects. It is published in ACM Queue, a respected computer science magazine.

hackernews · Ygg2 · Jul 18, 17:27 · [Discussion](https://news.ycombinator.com/item?id=48960155)

**Background**: Bikeshedding, also known as Parkinson's law of triviality, describes the tendency to spend disproportionate time on trivial issues while neglecting more complex ones. The term was coined by C. Northcote Parkinson in 1957 and popularized in software development by Poul-Henning Kamp in 1999. In open source, this can lead to endless debates over minor features while core design problems remain unresolved.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bikeshedding">Bikeshedding</a></li>
<li><a href="https://en.wikipedia.org/wiki/Law_of_triviality">Law of triviality - Wikipedia</a></li>
<li><a href="https://thedecisionlab.com/biases/bikeshedding">Bikeshedding - The Decision Lab</a></li>

</ul>
</details>

**Discussion**: Comments show a mix of appreciation and critique. One user suggests using reversible decisions to quickly resolve trivial issues, while another highlights PHK's contributions like MD5crypt. Some disagree with Kamp's skepticism about LLM-assisted code review, arguing it's already a major disruptor.

**Tags**: `#bikeshedding`, `#open source`, `#software engineering`, `#community dynamics`

---

<a id="item-6"></a>
## [Claude Fable 5 Made Permanent on Subscriptions](https://simonwillison.net/2026/Jul/18/claude-make-fable-5-permanent/#atom-everything) ⭐️ 8.0/10

Anthropic has reversed its decision to remove Claude Fable 5 from subscription plans, announcing that starting July 20, 2026, the model will be included in Max and Team Premium plans at 50% of limits, with Pro and Team Standard users receiving access via usage credits and a one-time $100 credit. This move responds to competitive pressure from OpenAI's GPT-5.6 Sol and Kimi's Kimi 3, ensuring that Anthropic's best model remains accessible to subscribers and maintaining the value of its premium plans in a rapidly evolving market. The original plan to make Fable 5 API-only was driven by compute capacity concerns, but strong competition made the subscription-exclusion untenable. The $20/month plan still does not include Fable 5 access.

rss · Simon Willison · Jul 18, 06:00

**Background**: Claude Fable 5 is Anthropic's most advanced 'Mythos' model, featuring a 1-million-token context window and high API pricing ($10/M input, $50/M output). GPT-5.6 Sol, released July 9, 2026, is OpenAI's frontier model with strong capabilities in coding and science, while Kimi 3 boasts 2.8 trillion parameters and native vision. Anthropic had announced Fable 5 would be withdrawn from subscriptions, but competitive pressure forced a reversal.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Claude`, `#Anthropic`, `#pricing`, `#competition`

---

<a id="item-7"></a>
## [DeepMind/Kaggle Grand Prize Winner Accused of AI Slop](https://www.reddit.com/r/MachineLearning/comments/1uzyf66/did_blatant_ai_slop_just_win_a_25k_usd_deepmind/) ⭐️ 8.0/10

A Reddit user alleges that the $25,000 grand prize winner of the Google DeepMind and Kaggle 'Measuring Progress Toward AGI' competition submitted nonsensical, unvetted content that failed to meet the competition's requirements. This controversy raises serious questions about the integrity of the review process in high-stakes AI competitions and could undermine trust in benchmark standards for AGI research. The winning entry reportedly generated random numbers and contained unfounded claims, being ten times the requested submission length with evidence of minimal review by authors or judges.

reddit · r/MachineLearning · /u/TheWerkmeister · Jul 18, 15:10

**Background**: The Google DeepMind-sponsored Kaggle challenge 'Measuring Progress Toward AGI - Cognitive Abilities' asked participants to design new cognitive-science-based AI benchmarks. The competition offered a $200,000 prize pool with $25,000 for the grand prize, aiming to evaluate AI beyond standard benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kaggle.com/competitions/kaggle-measuring-agi/overview/how-to-get-25-bonus-on-the-assignment">Measuring Progress Toward AGI - Cognitive Abilities - Kaggle</a></li>
<li><a href="https://www.mindstudio.ai/blog/google-agi-benchmark-10-cognitive-dimensions">How Google's New AGI Benchmark Measures Intelligence Across 10 Cognitive Dimensions | MindStudio</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#Kaggle`, `#DeepMind`, `#research ethics`, `#AGI benchmarks`

---

<a id="item-8"></a>
## [Doubao Phone shifts from GUI to MCP, stockpiles hundreds of thousands](https://www.latepost.com/news/dj_detail?id=3648) ⭐️ 8.0/10

Doubao Phone has abandoned its previous strategy of using GUI automation to directly read screens and simulate clicks on top apps, instead requiring major apps like Alibaba and Tencent to provide MCP services and open data/control permissions for integration. Its stockpile has been increased from 30,000 units to hundreds of thousands. This strategic pivot from GUI automation to native MCP integration signals a major shift in AI phone design, potentially reshaping the AI agent ecosystem by pushing super apps to adopt open protocols. It could accelerate industry adoption of MCP-like frameworks, as seen with Apple and Google's similar moves. The Doubao Phone first released a technical preview in December 2025, but its GUI automation capabilities were disabled after being blocked by apps like WeChat and Taobao. The shift to MCP requires each super app to proactively implement and expose MCP servers, granting controlled access to data and functions.

telegram · zaihuapd · Jul 18, 00:29

**Background**: GUI automation refers to technology that simulates human interactions by reading screen pixels and issuing clicks or gestures, often used for testing. However, it is brittle and often blocked by apps. The Model Context Protocol (MCP) is an open standard that allows AI agents to securely access external services (e.g., calendars, databases) through structured APIs, providing a more reliable and permission-based integration method. Doubao Phone's previous approach relied on GUI automation, which led to conflicts with super apps; MCP offers a negotiated alternative.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>
<li><a href="https://dl.acm.org/doi/10.1145/3611643.3613885">Appaction: Automatic GUI Interaction for Mobile Apps via Holistic Widget Perception | Proceedings of the 31st ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering</a></li>

</ul>
</details>

**Tags**: `#AI agent`, `#MCP`, `#mobile strategy`, `#AI ecosystem`, `#product shift`

---

<a id="item-9"></a>
## [Meta in Talks to Lease AI Compute to Anthropic for $10B](https://www.nytimes.com/2026/07/17/technology/meta-anthropic-ai-computing-power.html) ⭐️ 8.0/10

Meta is in early negotiations to lease AI computing power to Anthropic, with a potential deal valued at $10 billion over two years. This deal highlights the severe scarcity of AI compute resources and could allow Meta to monetize its massive data center investments while providing Anthropic with critical infrastructure. Anthropic proposed the deal in June 2026; if finalized, Anthropic would pay monthly with both sides able to exit early. Talks are early and may not result in an agreement.

telegram · zaihuapd · Jul 18, 01:14

**Background**: AI compute, especially for training large models, has become a bottleneck for many AI startups. Meta has invested heavily in data centers, with planned spending of up to $145 billion this year, partly to address its own AI needs. Leasing out spare capacity could help Meta justify these expenditures to investors.

**Tags**: `#AI`, `#Meta`, `#Anthropic`, `#compute`, `#cloud computing`

---

<a id="item-10"></a>
## [SpaceX in Talks with Pentagon for Multibillion-Dollar AI Compute Deal](https://www.wsj.com/tech/ai/spacex-in-talks-to-provide-computing-power-for-pentagons-ai-push-15e752e4) ⭐️ 8.0/10

SpaceX is negotiating a multibillion-dollar deal with the U.S. Department of Defense to provide data center computing power for running AI models, according to sources familiar with the talks. If finalized, this deal would mark SpaceX's entry into defense cloud computing, challenging incumbents like Amazon and Microsoft, and could accelerate AI adoption across military operations. The negotiations are ongoing and could still fall apart; SpaceX has recently signed similar compute deals with Anthropic and Google, and is expanding its cloud computing business.

telegram · zaihuapd · Jul 18, 01:44

**Background**: The Pentagon is rapidly acquiring cloud computing capacity to support AI applications in national security and daily operations. SpaceX has transformed its Colossus data center into a commercial computing platform, securing deals with AI companies like Anthropic and Google. This potential contract would deepen SpaceX's existing relationship with the military.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/06/22/spacex-ai-colossus-data-center-reflection.html">SpaceX signs computing power deal with open-source AI startup ... SpaceX Is in Talks on a Multibillion Dollar Defense Contract ... SpaceX signs $920m monthly cloud deal with Google ahead of IPO Musk's SpaceX in talks to supply the Pentagon with computing ... SpaceX lands Google AI compute deal after Anthropic pact ... Google and SpaceX: $11B Deal for Cloud Computing in Space</a></li>
<li><a href="https://www.fool.com/investing/2026/07/18/spacex-is-in-talks-on-a-multibillion-dollar-defense-contract-here-is-what-it-means-for-investors/">SpaceX Is in Talks on a Multibillion Dollar Defense Contract ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#defense`, `#SpaceX`, `#cloud computing`, `#infrastructure`

---

<a id="item-11"></a>
## [TSMC A14 Process to Enter Production in 2028](https://t.me/zaihuapd/42643) ⭐️ 8.0/10

TSMC announced that its next-generation A14 process technology will begin production in 2028, delivering up to 15% faster speed or 30% lower power compared to the N2 process, along with over 20% higher logic density. This announcement underscores TSMC's commitment to maintaining its leadership in advanced semiconductor manufacturing, providing a clear roadmap for AI and high-performance computing applications that demand ever-increasing transistor density and energy efficiency. The A14 process is TSMC's 1.4nm-class node, using second-generation GAAFET transistors, and follows the A16 node (expected in 2026). TSMC is also introducing NanoFlex Pro, an evolution of its standard cell architecture for better performance and flexibility.

telegram · zaihuapd · Jul 18, 05:00

**Background**: Semiconductor process nodes refer to the manufacturing technology used to create integrated circuits, with smaller nodes generally offering better performance and power efficiency. TSMC's N2 process, which uses GAAFET transistors for the first time, is set to enter volume production later this year. The A14 node represents a full-node advancement beyond N2, targeting further improvements in speed, power, and density critical for next-generation chips.

<details><summary>References</summary>
<ul>
<li><a href="https://pr.tsmc.com/english/news/3228">TSMC Unveils Next-Generation A14 Process at North America Technology Symposium|Taiwan Semiconductor Manufacturing Company Limited</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/tsmcs-2nm-n2-process-node-enters-production-this-year-a16-and-n2p-arriving-next-year">TSMC's 2nm N2 process node enters production this year, A16 and N2P arriving next year | Tom's Hardware</a></li>

</ul>
</details>

**Tags**: `#TSMC`, `#semiconductor`, `#A14`, `#chip manufacturing`

---

<a id="item-12"></a>
## [Trump Administration Considers FINRA-like Watchdog for Top AI Models](https://www.bloomberg.com/news/articles/2026-07-17/us-considers-creating-finra-like-watchdog-to-vet-top-ai-models) ⭐️ 8.0/10

The Trump administration is exploring the creation of an independent AI watchdog agency modeled after FINRA to review the safety of cutting-edge AI models. The proposal is led by Treasury Secretary Scott Bessent and is under review by Chief of Staff Susie Wiles. This marks a significant potential shift in AI governance, aiming to address industry concerns about ad-hoc government interventions. If implemented, it could establish a more structured and industry-participatory regulatory framework for AI safety. The proposal aligns with a suggestion from Google DeepMind CEO Demis Hassabis for an industry-funded independent regulator. Notably, President Trump has not yet reviewed the plan, and the framework remains under discussion.

telegram · zaihuapd · Jul 18, 05:45

**Background**: FINRA (Financial Industry Regulatory Authority) is a non-profit self-regulatory organization that oversees securities firms and enforces rules to ensure market fairness. The proposed AI watchdog would similarly be an independent agency funded by the industry, reporting to a federal body like the SEC. This model aims to balance government oversight with industry expertise.

<details><summary>References</summary>
<ul>
<li><a href="https://brokercheck.finra.org/">brokercheck. finra .org</a></li>

</ul>
</details>

**Tags**: `#AI监管`, `#政策`, `#特朗普政府`, `#FINRA`, `#大模型`

---