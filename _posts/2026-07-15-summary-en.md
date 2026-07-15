---
layout: default
title: "Horizon Summary: 2026-07-15 (EN)"
date: 2026-07-15
lang: en
---

> From 32 items, 9 important content pieces were selected

---

1. [Stripe and Advent Jointly Offer to Acquire PayPal for $53B](#item-1) ⭐️ 9.0/10
2. [Inkling: Open-Weights Multimodal Model with Audio](#item-2) ⭐️ 8.0/10
3. [Telegram Data Center Analysis Raises Security Concerns](#item-3) ⭐️ 8.0/10
4. [Researcher tricks Claude web_fetch to leak private memories](#item-4) ⭐️ 8.0/10
5. [Disentangling Convolutional Neurons with Hadamard Product Analysis](#item-5) ⭐️ 8.0/10
6. [PyTorch model 170x slower on T4 vs A100: debugging extreme bottleneck](#item-6) ⭐️ 8.0/10
7. [Judge Questions Epic-Google Antitrust Settlement License Deal](#item-7) ⭐️ 8.0/10
8. [DeepSeek Raises $7.4B in First Round with Special Founder Control Structure](#item-8) ⭐️ 8.0/10
9. [Telegram Launches Serverless Platform for Bots](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Stripe and Advent Jointly Offer to Acquire PayPal for $53B](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 9.0/10

Stripe and private equity firm Advent have made a joint offer to acquire PayPal for over $53 billion, according to sources. This would be one of the largest fintech acquisitions in history. If completed, this acquisition would combine two dominant payment processors, raising significant antitrust concerns and potentially reshaping the online payments landscape. It could reduce competition and increase fees for merchants and consumers. The offer values PayPal at roughly its current market capitalization, but the deal may face intense regulatory scrutiny. The combined entity would own PayPal, Venmo, Braintree, Xoom, and Stripe's own payment platform, creating a massive market share in card-not-present transactions.

hackernews · rvz · Jul 15, 03:32 · [Discussion](https://news.ycombinator.com/item?id=48915953)

**Background**: PayPal is a long-established online payments company, while Stripe is a newer, highly-valued fintech focused on developer-friendly payment processing. Advent is a private equity firm known for large buyouts. This potential acquisition comes amid a wave of fintech consolidation and increasing regulatory focus on big tech and payment systems.

**Discussion**: Commenters expressed strong concerns about reduced competition, higher fees, and Stripe's restrictive policies on certain industries like cannabis and adult content. Many fear that consolidation would increase risk for merchants who rely on multiple payment processors for redundancy.

**Tags**: `#acquisition`, `#fintech`, `#stripe`, `#paypal`, `#antitrust`

---

<a id="item-2"></a>
## [Inkling: Open-Weights Multimodal Model with Audio](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines released Inkling, a large open-weights multimodal AI model that supports audio input, designed for customization and efficient inference. Inkling provides a strong open-source alternative for multimodal tasks, especially audio, and enables enterprises to fine-tune their own models at lower cost, potentially filling a gap similar to Chinese open models like DeepSeek. Inkling is not the strongest overall model but offers a combination of qualities including multimodal capabilities, efficient thinking, long context, and availability on Tinker for fine-tuning.

hackernews · vimarsh6739 · Jul 15, 18:12 · [Discussion](https://news.ycombinator.com/item?id=48924912)

**Background**: An open-weights model releases its trained parameters publicly, allowing anyone to download, run, and fine-tune it. Multimodal AI models process multiple data types like text, audio, images, and video together, enabling richer understanding and interactions, as seen in models like GPT-4o.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multimodal_model">Multimodal model</a></li>

</ul>
</details>

**Discussion**: Community members are excited about Inkling being the largest open-weight model with audio support, with some seeing it as a potential 'American DeepSeek' for open-source AI. Others appreciate the business model of providing a customizable base model through Tinker, and note its strength in long context for agentic applications.

**Tags**: `#open-weights`, `#multimodal`, `#AI model`, `#audio`, `#fine-tuning`

---

<a id="item-3"></a>
## [Telegram Data Center Analysis Raises Security Concerns](https://dev.moe/en/3025) ⭐️ 8.0/10

A technical analysis of Telegram's data centers reveals their geographic distribution, and community comments allege potential FSB involvement in managing the infrastructure. This matters because Telegram is widely used for private communication, and any security compromise could affect millions of users worldwide, particularly in Russia and Ukraine. DC5 is often down to the discontent of Chinese users, while DC2 serves Russian and Ukrainian users; there is a notable gap for DC3, and users can identify their data center via Telegram's API method help.getConfig.

hackernews · theanonymousone · Jul 15, 13:22 · [Discussion](https://news.ycombinator.com/item?id=48920475)

**Background**: Telegram uses multiple data centers (DCs) numbered DC1 through DC5 to handle user traffic across regions. Each DC is associated with specific geographic areas, and their performance can vary by location. The analysis maps these DCs and their uptime patterns.

**Discussion**: Comments highlight an investigation claiming Telegram's infrastructure is managed by someone also managing FSB infrastructure, which Telegram has not disputed. Users also discuss common downtime patterns (e.g., DC2 for Russian/Ukrainian users) and note that DC3 is missing, sparking speculation about its use for special data.

**Tags**: `#telegram`, `#data centers`, `#security`, `#infrastructure`, `#FSB`

---

<a id="item-4"></a>
## [Researcher tricks Claude web_fetch to leak private memories](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Security researcher Ayush Paul demonstrated an attack that exploits Claude's web_fetch tool to exfiltrate private user memories by following nested links from a malicious website. This vulnerability highlights a critical gap in AI safety defenses, showing that even carefully designed restrictions like limiting web_fetch to user-supplied URLs can be bypassed, with serious implications for user privacy. The attack required the malicious website to detect if the client was an AI assistant via the 'Claude-User' user-agent and then present a sequence of links that tricked Claude into appending user memory data to the URLs. Anthropic had already identified the issue internally and closed the loophole by preventing web_fetch from navigating to links within fetched content.

rss · Simon Willison · Jul 15, 14:21

**Background**: The 'lethal trifecta' is a combination of an AI agent having access to private data, receiving untrusted content, and possessing exfiltration capabilities. Claude's web_fetch tool is designed to prevent data exfiltration by only allowing navigation to exact URLs provided by the user or from a companion web_search tool. However, the ability to follow links from fetched content introduced a loophole.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Sep/10/claude-web-fetch-tool/">Claude API: Web fetch tool</a></li>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>

</ul>
</details>

**Discussion**: Hacker News discussions likely expressed concern over the vulnerability and appreciation for the clear disclosure, with some questioning Anthropic's bug bounty decision. Others may have discussed the broader implications for AI agent security.

**Tags**: `#security`, `#vulnerability`, `#AI`, `#Claude`, `#data privacy`

---

<a id="item-5"></a>
## [Disentangling Convolutional Neurons with Hadamard Product Analysis](https://www.reddit.com/r/MachineLearning/comments/1uwya70/mechanistic_interpretability_a_first_paper_on/) ⭐️ 8.0/10

A researcher proposes a novel technique to disentangle convolutional neurons by computing the Hadamard product of the receptive field and weights, then clustering to reveal monosemantic patterns such as cars, cats, and dogs. The analysis also uncovers low-valued clusters like letters that are actively suppressed by balancing positive and negative weights. This work provides a new tool for mechanistic interpretability of convolutional neural networks, potentially helping researchers understand how individual neurons detect multiple features. It also reveals evidence of gradient descent deliberately suppressing certain patterns, offering insights into network optimization. The method was tested on a 1x1 convolution neuron in InceptionV1's mixed4e layer. The Hadamard product clustering yielded clean monosemantic clusters for high-activation concepts and additional low-valued clusters with evenly distributed positive and negative weights, suggesting deliberate noise injection by gradient descent.

reddit · r/MachineLearning · /u/narang_27 · Jul 15, 06:59

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks by understanding internal components like neurons and circuits. A key challenge is polysemanticity, where single neurons respond to multiple unrelated concepts; monosemanticity is the desirable property of responding to one concept. The Hadamard product computes element-wise multiplication of two matrices, used here to combine receptive field and weights. The Distill Circuits thread is a platform for such research.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hadamard_product_(matrices)">Hadamard product (matrices) - Wikipedia</a></li>
<li><a href="https://distill.pub/2020/circuits/">Thread: Circuits</a></li>
<li><a href="https://transformer-circuits.pub/2023/monosemantic-features">Towards Monosemanticity: Decomposing Language Models With Dictionary Learning</a></li>

</ul>
</details>

**Tags**: `#mechanistic interpretability`, `#convolutional neural networks`, `#interpretability`, `#neuron analysis`

---

<a id="item-6"></a>
## [PyTorch model 170x slower on T4 vs A100: debugging extreme bottleneck](https://www.reddit.com/r/MachineLearning/comments/1ux6a9x/pytorch_model_running_170x_slower_on_t4_vs_a100/) ⭐️ 8.0/10

A PyTorch point-tracking model runs 170x slower on an NVIDIA T4 GPU (85 seconds) compared to an A100 (0.5 seconds) for the same 47-frame video at 256x256 resolution. The user has ruled out common issues like GPU not being used or driver problems, leaving the root cause unknown. This extreme performance gap highlights critical optimization considerations for deploying models on different GPU architectures. Understanding the bottleneck could help developers avoid similar pitfalls and leverage Tensor Cores or memory bandwidth more effectively. The model uses pure FP32 precision, builds 4D correlation volumes for dense matching, and includes transformer layers. GPU utilization is 99% on T4 but performance is still terrible, suggesting a compute-bound but inefficient kernel, possibly due to lack of Tensor Core utilization in FP32 or memory bandwidth saturation.

reddit · r/MachineLearning · /u/Future-Structure-296 · Jul 15, 13:44

**Background**: The NVIDIA T4 and A100 are GPUs with vastly different capabilities. The A100 has Ampere architecture with 312 TFLOPS FP32 and 2 TB/s memory bandwidth, while the T4 has Turing architecture with 8.1 TFLOPS FP32 and 320 GB/s memory bandwidth. A key difference is that the T4's Tensor Cores only accelerate FP16/INT8, not FP32, so pure FP32 operations are limited to CUDA cores. The 4D correlation volume operation is memory-intensive and may be bottlenecked by the T4's lower memory bandwidth, while the A100 benefits from much higher bandwidth and more compute units.

<details><summary>References</summary>
<ul>
<li><a href="https://www.server-parts.eu/post/nvidia-t4-vs-a100-gpu-comparison-ai-deep-learning-data-centers">NVIDIA T4 vs. NVIDIA A100 Comparison: Which GPU Should You Choose for AI and Data Center Workloads?</a></li>
<li><a href="https://jarvislabs.ai/blog/l4-vs-a100">NVIDIA L4 vs A100: Specs, Benchmarks, Price & ...</a></li>
<li><a href="https://www.linkedin.com/posts/smallest_nvidia-gpu-showdown-a100-vs-t4-with-two-activity-7117750246096433152-FF2J">Nvidia GPU Showdown - A100 vs T4 With two of Nvidia's most popular GPUs for AI acceleration - the A100 and T4 - which should you choose? Here's a quick rundown of the key differences: Performance -… | smallest.ai</a></li>

</ul>
</details>

**Tags**: `#PyTorch`, `#GPU Performance`, `#Model Optimization`, `#Troubleshooting`, `#A100 vs T4`

---

<a id="item-7"></a>
## [Judge Questions Epic-Google Antitrust Settlement License Deal](https://t.me/zaihuapd/42588) ⭐️ 8.0/10

US District Judge James Donato revealed that Epic Games and Google have entered a new commercial deal involving joint product development, marketing, and partnerships, with Epic paying approximately $800 million over six years. The judge questioned whether this deal undermines Epic's antitrust claims against Google. This development could affect the remedies in the Epic vs Google antitrust case, potentially weakening attempts to open up Android's app distribution. It also raises questions about the consistency of antitrust plaintiffs' positions. The deal covers Unreal Engine, Fortnite, and Android-related businesses, but Epic CEO Tim Sweeney stated it does not include terms for Epic Games Store on Android. The judge expressed skepticism that such a large payment could be unrelated to the antitrust dispute.

telegram · zaihuapd · Jul 15, 11:15

**Background**: Epic Games sued Google in 2020, alleging monopolistic practices in Android app distribution and in-app payment systems. A jury found Google guilty of antitrust violations in December 2023. The case is ongoing as the court determines remedies, and this new deal could complicate the process.

**Tags**: `#antitrust`, `#Google`, `#Epic Games`, `#Android`, `#mobile ecosystems`

---

<a id="item-8"></a>
## [DeepSeek Raises $7.4B in First Round with Special Founder Control Structure](https://t.me/zaihuapd/42589) ⭐️ 8.0/10

DeepSeek has completed its first external funding round, raising over 500 billion yuan (approximately $7.4 billion) at a valuation exceeding $50 billion, using an unusual limited partnership structure that allows founder Liang Wenfeng to retain full control. This is the largest first-round funding for a Chinese AI startup and signals strong investor confidence in DeepSeek, while the novel structure could set a precedent for founder control in large tech financings. Investors are required to put capital into a limited partnership managed by CEO Liang Wenfeng, rather than directly into DeepSeek, and must accept a five-year lock-up period with no voting rights; founder Liang personally invested 200 billion yuan, with Tencent and CATL planning investments of 100 billion and 50 billion yuan respectively.

telegram · zaihuapd · Jul 15, 12:56

**Background**: A limited partnership structure is typically used in investment funds, not operating startups, where limited partners (LPs) provide capital and general partners (GPs) manage the fund. In this case, the GP is the founder, giving him control over investor capital. A lock-up period prevents investors from selling their stake for a set time, which is common in IPOs but unusual in private funding rounds.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.accountingprose.com/business-structure-comprehensive-guide">Choosing the Right Business Structure: A Comprehensive Guide</a></li>
<li><a href="https://www.gritt.io/blog/what-is-a-limited-partner">What Is a Limited Partner & Why Founders Should Care</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lock-up_period">Lock - up period - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#funding`, `#ai`, `#china`, `#venture capital`

---

<a id="item-9"></a>
## [Telegram Launches Serverless Platform for Bots](https://core.telegram.org/bots/serverless) ⭐️ 8.0/10

Telegram has officially launched a serverless platform that allows developers to run backend code for bots and Mini Apps directly on Telegram's infrastructure, deploying with a single command: `npx tgcloud push`. This move eliminates the need for developers to manage servers, reducing operational overhead and lowering the barrier to creating Telegram bots, potentially accelerating growth in the Telegram bot ecosystem. The code executes in an isolated V8 sandbox adjacent to the Bot API, and includes a built-in SQLite database. The service is currently in limited testing with JavaScript support.

telegram · zaihuapd · Jul 15, 16:00

**Background**: Serverless computing enables developers to run code without provisioning or managing servers. Telegram bots previously required external hosting or cloud services for backend logic; this new platform integrates backend execution directly into Telegram's infrastructure, simplifying deployment and scaling.

<details><summary>References</summary>
<ul>
<li><a href="https://core.telegram.org/bots/serverless">Telegram Serverless</a></li>

</ul>
</details>

**Tags**: `#serverless`, `#Telegram`, `#bots`, `#JavaScript`, `#cloud computing`

---