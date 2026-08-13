---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 32 items, 8 important content pieces were selected

---

1. [Google unveils Gemini 3.7 Flash, its most intelligent workhorse model](#item-1) ⭐️ 9.0/10
2. [DRAM 'Spaghettifying' Attack Achieves Ring-0 on AMD CPUs](#item-2) ⭐️ 9.0/10
3. [Cerebras and OpenAI Launch GPT-5.6 Sol Ultrafast, 7x Faster Inference](#item-3) ⭐️ 8.0/10
4. [Choose Boring Technology and Spend Innovation Tokens Wisely](#item-4) ⭐️ 8.0/10
5. [DeepSeek Harness Developer Preview Launches as Open-Source Agent Framework](#item-5) ⭐️ 8.0/10
6. [Pixel Metrics Fail to Rank World Models; New Tool 'worldproof' Diagnoses Why](#item-6) ⭐️ 8.0/10
7. [DeepMind's SL2T Brings Sign Language-to-Text AI to Pixel 11](#item-7) ⭐️ 8.0/10
8. [Google Launches Gemini 3.6 Flash, Reveals Gemini 4 Pretraining](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Google unveils Gemini 3.7 Flash, its most intelligent workhorse model](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 9.0/10

Google has unveiled Gemini 3.7 Flash, a new multimodal model built on Gemini 3.6 Flash with strong vision and coding performance. The model now also powers Gemini Spark for Google AI Pro and Ultra subscribers in over 160 countries. This release underscores Google's fast iteration cycle — Gemini 3.6 Flash launched just three weeks prior — and its aim to provide a cheap, reliable 'workhorse' model for everyday AI workloads. It also intensifies competition with rivals like Opus 5 and Luna on both price and vision/coding benchmarks. Gemini 3.7 Flash is based on Gemini 3.6 Flash and was evaluated across reasoning, coding, agentic tool use, multimodal, multilingual, and long-context benchmarks. Its introductory pricing is scheduled to double on December 31, 2026, according to community reports.

hackernews · thisisauserid · Aug 13, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49289112)

**Background**: Gemini is a family of multimodal large language models developed by Google DeepMind, announced on December 6, 2023, and used by the Gemini chatbot. The Flash series is designed as fast, cost-efficient 'workhorse' models for high-volume, mostly text-based use cases such as summarization, parsing, and formatting. Gemini 3.7 Flash is the latest iteration, following 3.6 Flash just three weeks earlier.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-7-flash/">Gemini 3 . 7 Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/">Gemini 3 . 7 Flash : our most intelligent workhorse model</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_2.5_Flash_Image">Gemini 2.5 Flash Image</a></li>

</ul>
</details>

**Discussion**: Community reactions were mixed but engaged: jjcm found Gemini 3.7 Flash impressive for image-to-HTML work and competitive at its price point, though Opus 5 remained best-in-class. simonw called the introductory pricing 'really weird' and questioned the tight release cadence. Alifatisk argued GPT-5.6 Luna (Max) still outperforms it on DeepSWE 1.1 and is cheaper; wxw similarly wondered whether Flash is necessary when Luna undercuts it on price.

**Tags**: `#AI`, `#Google Gemini`, `#LLM`, `#Model Release`, `#Machine Learning`

---

<a id="item-2"></a>
## [DRAM 'Spaghettifying' Attack Achieves Ring-0 on AMD CPUs](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

Christopher Domas released a hardware security project called 'skitter-creek-bath-salts' that 'spaghettifies' DRAM to gain ring-0 privileges, accompanied by a Black Hat talk. The technique was developed and tested on AMD Family 16h CPUs. This is groundbreaking DRAM exploitation research because it exposes a hidden attack surface below the operating system, potentially bypassing all software security mechanisms. It could affect game consoles and other locked-down systems, and highlights the dangers of undocumented DRAM controller behavior. According to the README, the attack works on AMD Jaguar (Family 16h), whose datasheets document the DRAM controller's translation registers as unlockable. Newer CPUs like Zen 3 have moved the memory controller base address, leaving open the question of which other families are affected.

hackernews · matt_d · Aug 13, 14:17 · [Discussion](https://news.ycombinator.com/item?id=49286341)

**Background**: DRAM controllers translate memory addresses using internal registers; if these can be reprogrammed, an attacker can remap memory and gain privileged access. 'Spaghettification' borrowed from astrophysics describes how an object is stretched and compressed by extreme forces, here used as a metaphor for manipulating DRAM address translation.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49286341">Spaghettifying DRAM | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spaghettification">Spaghettification - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters praised Christopher Domas's presentation style and looked forward to the Black Hat talk. Some noted that DRAM complexity has grown enormous, creating a large attack surface, while others questioned which modern CPUs are actually affected beyond the old AMD Family 16h.

**Tags**: `#hardware-security`, `#DRAM`, `#exploitation`, `#low-level`, `#security-research`

---

<a id="item-3"></a>
## [Cerebras and OpenAI Launch GPT-5.6 Sol Ultrafast, 7x Faster Inference](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

Cerebras and OpenAI announced GPT-5.6 Sol Ultrafast, a version of the frontier model that achieves comparable accuracy to standard models but runs nearly 7 times faster. In evaluations, it answered all 2,500 HLE questions in about 11 hours, versus more than 78 hours for Claude Fable 5. This marks a major milestone in making frontier-level AI inference dramatically faster, which could enable real-time applications and more iterative, higher-quality reasoning. The Cerebras-OpenAI collaboration shows that custom hardware can challenge GPU-based dominance in LLM serving. Ultrafast mode runs on Cerebras wafer-scale hardware; according to Artificial Analysis reported speeds, it runs 11x faster than Claude Fable 5 and 5x faster than Opus 4.8 in Fast mode. No pricing information has been released yet, and Cerebras says it is scaling to 200MW of AI compute capacity by 2027.

hackernews · pr337h4m · Aug 13, 18:10 · [Discussion](https://news.ycombinator.com/item?id=49289844)

**Background**: Cerebras builds the Wafer-Scale Engine, the world's largest AI processor, with the WSE-3 measuring 46,225 mm² and containing 4 trillion transistors, designed for fast training and inference. Traditional LLM inference optimization includes techniques like quantization, distillation, and batching, but Cerebras aims to speed up AI through a purpose-built, ultra-large chip rather than incremental software optimizations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters are generally excited about the collaboration, with some arguing that faster inference enables iterative thinking and better reasoning quality. However, several express skepticism that OpenAI and Cerebras have not explicitly confirmed exact performance parity with the standard GPT-5.6 Sol, and note that no pricing details were shared.

**Tags**: `#AI`, `#LLM`, `#Inference`, `#Cerebras`, `#OpenAI`

---

<a id="item-4"></a>
## [Choose Boring Technology and Spend Innovation Tokens Wisely](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

Dan McKinley's 2015 essay 'Choose Boring Technology' argues that organizations should prefer well-understood, reliable technologies and budget the adoption of new ones using a fixed supply of 'innovation tokens.' The essay resurfaced on Hacker News and continues to provoke thoughtful discussion. This essay offers a practical framework for engineering leaders weighing innovation against risk, and its 'innovation tokens' concept has become a widely cited mental model. It helps teams avoid tool sprawl and focus their innovative energy on areas that create real business value. The central metaphor is that each company gets about three 'innovation tokens' for adopting new technology, and they should be spent sparingly. The essay emphasizes that boring technology has predictable failure modes, allowing teams to concentrate their problem-solving skills on their actual product domain.

hackernews · tosh · Aug 13, 17:48 · [Discussion](https://news.ycombinator.com/item?id=49289512)

**Background**: The essay was written by Dan McKinley, a software engineer who previously worked at Etsy and Stripe. It responds to the common tendency among startups to chase the newest frameworks and languages, which introduces unnecessary complexity and risk. The 'innovation tokens' idea frames technology adoption as a finite resource that must be budgeted deliberately. Over the years, this essay has become a classic reference in discussions about pragmatic technology choices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lessannoyingbusiness.com/post/innovation-tokens">Innovation Tokens - When to break from the status quo</a></li>
<li><a href="https://ilearnt.com/blog/innovationtokens/">Innovation tokens</a></li>
<li><a href="https://www.morbe.online/post/boring-technology-why-less-hype-can-lead-to-more-productivity">Boring technology : Why less hype can lead to more productivity</a></li>

</ul>
</details>

**Discussion**: The Hacker News comments are largely positive, with many readers calling the essay a favorite and praising the innovation tokens framework as highly useful for explaining tradeoffs. However, some dissenters argue that 'new' or 'novel' is a weak proxy and that engineers should evaluate requirements, risks, and tradeoffs directly. Others tie the framework to the age of AI agents, suggesting companies should spend their innovation tokens on agents while keeping everything else boring.

**Tags**: `#technology strategy`, `#software engineering`, `#innovation`, `#boring technology`, `#engineering leadership`

---

<a id="item-5"></a>
## [DeepSeek Harness Developer Preview Launches as Open-Source Agent Framework](https://deepseek.com/harness/en/) ⭐️ 8.0/10

DeepSeek released DeepSeek Harness as an early open-source developer preview, with all agent capabilities implemented as plugins and fully traceable session logs. The source code is available now under the MIT license. This release matters because it comes from a major AI lab and directly targets two pain points in agent development: observability and extensibility. It could shape how developers build and debug multi-step agentic systems, while putting competitive pressure on US labs that restrict access to model traces. The framework uses a plugin architecture where every capability can be swapped or recomposed, and it supports hot-reload and dynamic enable/disable via Cordis v4. Session logs are append-only and record system prompts, reasoning, tool calls, subagent scheduling, and context injections; the Trajectory view supports resume, fork, search, and replay.

hackernews · bjin · Aug 13, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49285244)

**Background**: AI agent frameworks provide developers with abstractions and runtimes for building autonomous systems that call tools, manage context, and coordinate subagents; examples include LangChain, Microsoft Agent Framework, and AutoGen. DeepSeek Harness is an 'agent harness' — the runtime layer that orchestrates an agent's loop, plugins, and session state. Its architecture follows the 'everything is a plugin' model, and it leverages Cordis v4, a plugin system that can hot-load and unload components while rolling back side effects. The early preview is MIT-licensed and explicitly not production-ready.

<details><summary>References</summary>
<ul>
<li><a href="https://deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://deepseek-code.com/">DeepSeek Harness: Open-Source AI Agent Framework</a></li>
<li><a href="https://www.langchain.com/resources/ai-agent-frameworks">The best AI agent frameworks in 2026</a></li>

</ul>
</details>

**Discussion**: Community reaction is largely positive but measured. Commenters praised the append-only, replayable session logs as a 'killer feature' and appreciated that US models' encrypted traces can't match it; one author clarified it's an early rough preview. Skeptics noted it may be only moderately useful and raised concerns about plugin fatigue, while others highlighted the significance of Cordis v4's hot-reload and side-effect rollback.

**Tags**: `#AI agents`, `#open-source`, `#developer tools`, `#DeepSeek`, `#agent framework`

---

<a id="item-6"></a>
## [Pixel Metrics Fail to Rank World Models; New Tool 'worldproof' Diagnoses Why](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 8.0/10

The author released worldproof, an open-source diagnostic tool for world models, and found that pixel metrics like SSIM and PSNR cannot rank world models on real robot video because a trivial last-frame baseline already scores near-perfectly (0.983 SSIM, 53.9 dB PSNR on a SO-101 arm recording). The error does not grow with horizon, so all models tie and the evaluation has no discriminative power. This is a critical evaluation pitfall for the world-model community: benchmarks that rely on pixel metrics may give false confidence or fail to rank models at all on real-world data. The open-source diagnostic tool also provides practical value for researchers to measure the usable evaluation horizon on their own data. Using 64 rollouts per configuration and interquartile mean with stratified bootstrap confidence intervals, the author measured a last-frame baseline on DROID (15fps) and found three regimes: near-perfect ties at steps 1–3, a steep monotonic decline with separable models at steps 4–24, and a floor around 0.20 SSIM beyond step 28 where predictions are decorrelated. Caveats include that LPIPS does not separate the two datasets and points the opposite way on masked variants, and that including step 0 inflates summary scalars because a copy baseline gets a nearly free first step at high frame rates.

reddit · r/MachineLearning · /u/georgia_bucea · Aug 13, 19:58

**Background**: World models are neural networks that learn the dynamics of an environment from data, often by predicting future frames given actions; they are used in robotics and planning to enable agents to 'imagine' outcomes. SSIM (structural similarity) and PSNR (peak signal-to-noise ratio) are common pixel-level image quality metrics that compare predicted frames to ground truth, but they do not necessarily reflect semantic or task-relevant accuracy. The last-frame baseline—simply predicting that nothing changes—represents a trivial lower bound that can already score highly on slow-moving or high-frame-rate video, exposing when an evaluation setup has no discriminative power.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Structural_similarity">Structural similarity index measure - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio">Peak signal-to-noise ratio - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#world-models`, `#evaluation-metrics`, `#robotics`, `#machine-learning`, `#diagnostics`

---

<a id="item-7"></a>
## [DeepMind's SL2T Brings Sign Language-to-Text AI to Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

DeepMind released SL2T, a large multilingual sign language-to-text model, first deployed in Pixel 11's Gboard and Live Transcribe, supporting American Sign Language to English with zero-shot 70 BLEURT on FLEURS-ASL. This is a significant step for accessibility, as sign language AI moves from research to consumer products. It also demonstrates the potential of privacy-preserving multimodal models by using only pose keypoints instead of raw video. The model was trained on over 100,000 hours of data covering 50+ sign languages. It only processes hand and body pose keypoints, preserving privacy, and will expand to more devices and languages beyond ASL-to-English.

telegram · zaihuapd · Aug 13, 08:55

**Background**: FLEURS-ASL is an extension of the FLORES/FLEURS benchmarks to American Sign Language, enabling evaluation of sign language translation. BLEURT is a learned evaluation metric based on BERT that measures fluency and meaning preservation. DeepMind's SL2T shows that sign language translation can work directly from body coordinates, a departure from video-based approaches.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/">Putting sign language AI into users’ hands — Google DeepMind</a></li>
<li><a href="https://arxiv.org/html/2408.13585">FLEURS - ASL : Including American Sign Language in Massively...</a></li>
<li><a href="https://arxiv.org/abs/2004.04696">[2004.04696] BLEURT: Learning Robust Metrics for Text Generation</a></li>

</ul>
</details>

**Tags**: `#AI`, `#accessibility`, `#DeepMind`, `#sign language`, `#multimodal model`

---

<a id="item-8"></a>
## [Google Launches Gemini 3.6 Flash, Reveals Gemini 4 Pretraining](https://t.me/zaihuapd/43177) ⭐️ 8.0/10

Google has unveiled Gemini 3.6 Flash, claiming it cuts output tokens by 17% compared to Gemini 3.5 Flash and completes multi-step tasks with fewer reasoning steps and tool calls. The company also announced that training has begun on the next-generation Gemini 4 model. This release shows Google rapidly iterating on its Gemini line with visible efficiency gains and a more aggressive pricing strategy, which could reshape developer choices in the LLM API market. The confirmation of Gemini 4 pretraining signals the direction of the next frontier-model generation. Gemini 3.6 Flash features improved code generation, knowledge work, and computer operation, with a knowledge cutoff updated to March 2026. Its API pricing is $1.5 per million input tokens and $7.5 per million output tokens; Google also introduced Gemini 3.5 Flash for high-throughput, low-latency scenarios.

telegram · zaihuapd · Aug 13, 17:32

**Background**: LLM inference transforms text prompts into responses through tokenization, transformer layers with self-attention, and autoregressive token generation. Tool calling allows a language model to invoke external functions or APIs instead of answering directly, while computer-operation capabilities let AI agents navigate software interfaces like a human user. These concepts underpin the efficiency and capability changes Google describes in Gemini 3.6 Flash.

<details><summary>References</summary>
<ul>
<li><a href="https://arpitbhayani.me/blogs/how-llm-inference-works/">How LLM Inference Works</a></li>
<li><a href="https://blog.solega.co/how-to-implement-tool-calling-with-gemma-4-and-python/">How to Implement Tool Calling with Gemma 4 and Python - Solega Blog</a></li>
<li><a href="https://openai.com/index/computer-using-agent/">Computer-Using Agent | OpenAI</a></li>

</ul>
</details>

**Tags**: `#Gemini`, `#Google`, `#AI模型`, `#大语言模型`, `#技术发布`

---