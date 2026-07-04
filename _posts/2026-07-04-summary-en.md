---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 47 items, 8 important content pieces were selected

---

1. [EU Parliament Spyware Investigator Hacked with Pegasus](#item-1) ⭐️ 9.0/10
2. [PostgreSQL and the OOM killer: Why strict memory overcommit matters](#item-2) ⭐️ 8.0/10
3. [CDD Recovers Verbatim Finetuning Data from LLM Logits Alone](#item-3) ⭐️ 8.0/10
4. [Anthropic accuses Alibaba of massive distillation attack on Claude](#item-4) ⭐️ 8.0/10
5. [Huawei Launches Atlas 350 AI Accelerator with Ascend 950PR](#item-5) ⭐️ 8.0/10
6. [Alibaba Orders All Employees to Uninstall Claude Products](#item-6) ⭐️ 8.0/10
7. [NASA Launches Rescue Satellite for Failing Swift Telescope](#item-7) ⭐️ 8.0/10
8. [Tencent Xuanwu's Atuin AI beats Mythos on CyberGym benchmark](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [EU Parliament Spyware Investigator Hacked with Pegasus](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 9.0/10

Citizen Lab found that a member of the European Parliament committee investigating spyware was infected with Pegasus on his iPhone in October 2022 and again in March 2023. This breach demonstrates that spyware is being used against those who investigate it, implying authorization across multiple EU countries and compromising sensitive information. It raises urgent questions about surveillance sovereignty and device security policies within the European Parliament. The first infection overlapped with a Pegasus campaign targeting Russian and Belarusian-exiled journalists, suggesting a customer with multi-country authorization. The compromised phone contained both personal medical information and confidential government documents, highlighting the lack of separation between work and personal devices.

hackernews · ledoge · Jul 3, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48779683)

**Background**: Pegasus is a commercial spyware developed by Israeli firm NSO Group, used by governments to covertly surveil targets including journalists and activists. Citizen Lab is a cybersecurity watchdog that has exposed numerous Pegasus infections. The European Parliament has a committee investigating spyware abuses across member states.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://therecord.media/international-spyware-agreement-new-members">Finland, Germany, Ireland, Japan, Poland, South Korea added to US-led spyware agreement | The Record from Recorded Future News</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted ongoing spyware scandals in Greece, Poland, and Italy, with some arguing the hack was a domestic Greek operation rather than an attack on the EU Parliament. Others pointed out that multiple EU countries have used Pegasus, and questioned the Parliament's device separation policies.

**Tags**: `#Pegasus`, `#spyware`, `#cybersecurity`, `#European Parliament`, `#espionage`

---

<a id="item-2"></a>
## [PostgreSQL and the OOM killer: Why strict memory overcommit matters](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud published a blog post explaining their decision to use strict memory overcommit (vm.overcommit_memory=2) for PostgreSQL to avoid OOM killer issues and improve database reliability at scale. This is significant because many PostgreSQL operators face instability from the OOM killer under default heuristic overcommit, and strict overcommit offers a proven alternative for production environments. Strict overcommit (mode 2) denies memory allocations that would exceed available memory, which can prevent OOM killer incidents but may cause fork failures if not carefully tuned; the article advises thorough testing before deployment.

hackernews · furkansahin · Jul 3, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48774509)

**Background**: Linux memory overcommit has three modes: heuristic (0), always (1), and strict (2). The default heuristic mode allows processes to overcommit memory based on internal heuristics, but under memory pressure the OOM killer may kill processes, including PostgreSQL, causing reliability issues.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@amerather_9719/how-linux-kernel-manages-application-memory-27c23ac94177">How Linux Kernel Manages Application Memory | by Amer... | Medium</a></li>
<li><a href="https://kernel-internals.org/mm/overcommit/">Memory Overcommit - Linux Kernel Internals</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-03-02-optimize-memory-vm-swappiness-overcommit-ubuntu/view">How to Optimize Memory (vm.swappiness, overcommit ) on Ubuntu</a></li>

</ul>
</details>

**Discussion**: Comments caution that while strict overcommit avoids OOM killer, it can prevent fork() calls and requires careful testing, especially when adjusting overcommit ratios. One commenter shared issues with Go applications allocating virtual memory alongside PostgreSQL.

**Tags**: `#PostgreSQL`, `#Linux memory management`, `#OOM killer`, `#database reliability`, `#sysadmin`

---

<a id="item-3"></a>
## [CDD Recovers Verbatim Finetuning Data from LLM Logits Alone](https://www.reddit.com/r/MachineLearning/comments/1umn2dk/contrastive_decoding_diffing_cdd_recovering/) ⭐️ 8.0/10

Contrastive Decoding Diffing (CDD) recovers verbatim content from narrowly finetuned LLMs using only grey-box logit access, without requiring model weights or activations. It achieves a verbatim recovery score of 4+/5 on 19/20 organism x model pairs across four model families. This method significantly advances model diffing and security, as it can extract exact finetuning data from LLMs without whitebox access. It also revealed an unexpected data contamination issue: a fictional scientist persona from synthetic data generation consistently appeared across unrelated finetuning domains. CDD contrasts the base and finetuned model's logits directly, using a single default configuration with no per-organism calibration or layer selection. The prior whitebox method, Activation Difference Lens (ADL), never exceeded a 3/5 recovery score on the same benchmark despite requiring full weight access.

reddit · r/MachineLearning · /u/CebulkaZapiekana · Jul 3, 19:01

**Background**: Model diffing aims to surface systematic behavioral differences between LLM versions or finetuned models. Recent work showed that finetuning leaves detectable traces in activation differences between base and finetuned models, but that method required full weight access. Contrastive decoding is a technique that selects tokens by contrasting outputs from different models, and CDD applies this idea to recover training data.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2602.10371">Simple LLM Baselines are Competitive for Model Diffing</a></li>
<li><a href="https://aiwiki.ai/wiki/contrastive_decoding">Contrastive decoding | AI Wiki</a></li>
<li><a href="https://www.geeksforgeeks.org/nlp/contrastive-decoding-in-natural-language-processing/">Contrastive Decoding in Natural Language... - GeeksforGeeks</a></li>

</ul>
</details>

**Tags**: `#LLM security`, `#model diffing`, `#contrastive decoding`, `#machine learning`, `#finetuning`

---

<a id="item-4"></a>
## [Anthropic accuses Alibaba of massive distillation attack on Claude](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic sent a letter to the US Senate Banking Committee accusing Alibaba of orchestrating the largest known 'distillation attack' against its Claude AI model, using nearly 25,000 fraudulent accounts to perform over 28.8 million interactions between April 22 and June 5, 2026. This incident underscores the growing threat of model theft through distillation attacks, which can undermine the intellectual property and competitive advantage of AI companies, potentially spurring stricter regulations and defensive measures across the industry. Anthropic stated that the attack involved Alibaba's AI lab Qwen and is the largest such attack targeting the company, with detection efforts revealing the fraudulent accounts and massive interaction volume. The distillation technique allows a weaker model to mimic a stronger one by learning from its outputs.

telegram · zaihuapd · Jul 3, 06:21

**Background**: Model distillation is a technique where a smaller, less capable model learns to replicate the behavior of a larger, more powerful model by training on its outputs. Distillation attacks occur when adversaries abuse public APIs to gather this training data without authorization. Anthropic has developed methods to detect and prevent such attacks, but emphasizes that industry-wide cooperation is needed to address the issue at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#model distillation`, `#intellectual property`, `#Anthropic`, `#Alibaba`

---

<a id="item-5"></a>
## [Huawei Launches Atlas 350 AI Accelerator with Ascend 950PR](https://t.me/zaihuapd/42329) ⭐️ 8.0/10

At Huawei China Partner Conference 2026, Huawei announced and launched the Atlas 350 AI inference accelerator card powered by the new Ascend 950PR processor, claiming 2.87x the compute performance of Nvidia's H20 and being the first domestic card to support FP4 low-precision inference. This announcement strengthens Huawei's position in the AI accelerator market, especially for inference workloads, and provides an alternative to Nvidia's offerings in China amid ongoing trade restrictions. The FP4 support could significantly reduce model size and latency for large language models. The Atlas 350 features 112 GB of HBM memory using Huawei's self-developed high-bandwidth memory, supports single-card loading of 70B-parameter models, and delivers 2 PFLOPS for MXFP4 precision. It also includes improved vector compute and 2.5x interconnect bandwidth over previous generations.

telegram · zaihuapd · Jul 3, 08:35

**Background**: FP4 is a 4-bit floating-point precision format used to accelerate AI inference by reducing memory footprint and computation while maintaining acceptable accuracy. The Ascend 950PR is Huawei's latest AI processor optimized for inference and recommendation tasks, and its CANN framework now achieves over 95% CUDA code compatibility, easing migration from Nvidia platforms. H20 is a lower-end Nvidia GPU designed for the Chinese market to comply with US export controls.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eetrend.com/content/2025/100594934.html">华 为 昇 腾 950 /960/970炸裂发布！ 还首发了自研HBM内存！ 昇 腾 950 ...</a></li>
<li><a href="https://www.omniyq.com/sys-nd/500.html">昇 腾 950 ：国产算力的一个里程碑 - 云擎天下-超高性价比AI算力服务平台</a></li>
<li><a href="https://www.cfi.cn/p20260421002039.html">DeepSeek启动首轮外部融资 有望助推国产算力生态全面铺开- CFi.CN...</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#AI accelerator`, `#hardware`, `#deep learning`, `#inference`

---

<a id="item-6"></a>
## [Alibaba Orders All Employees to Uninstall Claude Products](https://t.me/zaihuapd/42334) ⭐️ 8.0/10

Alibaba has internally ordered all employees to immediately uninstall Anthropic's Claude products, including models Sonnet, Opus, Fable, and the Claude Code agent tool, effective July 10. This follows Anthropic's accusation that Alibaba used approximately 25,000 fake accounts to interact with Claude over 28 million times between April 22 and June 5. This incident highlights growing tensions between major Chinese tech firms and Western AI providers over usage policies and security. It could lead to stricter AI governance within enterprises and affect how Chinese companies access advanced AI models. Alibaba had previously reimbursed employees for using external models like Claude, GPT, and Gemini. The ban covers not only chat models but also agentic products like Claude Code, which is a terminal-based AI coding assistant.

telegram · zaihuapd · Jul 3, 13:00

**Background**: Claude is a series of large language models developed by Anthropic, a US-based AI company. The models range from Haiku to Fable, with increasing capability and cost. Alibaba's alleged abuse of fake accounts to bypass usage limits prompted Anthropic to tighten its risk control policies, leading to this internal ban.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://claude.com/resources/tutorials/choosing-the-right-claude-model">Choosing the right Claude model : Haiku, Sonnet , Opus , or Fable</a></li>
<li><a href="https://docs.anthropic.com/en/docs/claude-code/overview">Claude Code overview - Anthropic</a></li>

</ul>
</details>

**Tags**: `#Alibaba`, `#Claude`, `#Anthropic`, `#enterprise AI`, `#security`

---

<a id="item-7"></a>
## [NASA Launches Rescue Satellite for Failing Swift Telescope](https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a) ⭐️ 8.0/10

On July 3, NASA launched the LINK spacecraft, built by Katalyst Space Technologies, on a mission to capture and boost the aging Swift space telescope to a higher orbit, marking the first private attempt to retrieve a US government satellite. This mission demonstrates commercial satellite servicing capabilities that could extend the life of expensive space assets and mitigate space debris, potentially revolutionizing how aging satellites are managed. The LINK spacecraft will use a robotic arm to grab Swift and then fire thrusters to lift it by about 240 kilometers (150 miles), potentially allowing Swift to resume observations by September and extending its operational life beyond 2026.

telegram · zaihuapd · Jul 3, 15:43

**Background**: Orbital decay occurs when a satellite's orbit gradually lowers due to atmospheric drag, especially during periods of high solar activity. The Swift observatory, launched in 2004, studies gamma-ray bursts and has been losing altitude; without intervention, it could burn up in Earth's atmosphere as soon as October 2025. Satellite servicing using robotic arms is a growing field, with DARPA and commercial companies developing technologies to repair, refuel, and reposition spacecraft in orbit.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a">Rescue mission is launched to save an aging NASA telescope ...</a></li>
<li><a href="https://www.reuters.com/business/aerospace-defense/space-startup-katalyst-launches-orbital-rescue-mission-aging-nasa-observatory-2026-07-03/">Space startup Katalyst launches orbital rescue mission for ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Swift_rescue_mission">Swift Boost Mission - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#space`, `#NASA`, `#satellite rescue`, `#astronomy`

---

<a id="item-8"></a>
## [Tencent Xuanwu's Atuin AI beats Mythos on CyberGym benchmark](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 8.0/10

Tencent Xuanwu Lab announced that its Atuin AI scored 84.0% on the UC Berkeley-led CyberGym cybersecurity benchmark, surpassing Anthropic's Claude Mythos Preview. Atuin AI is built on the open-source model GLM-5.1 and cost less than 0.1% of Mythos's budget. This achievement demonstrates that a low-cost, open-source AI model can outperform a powerful proprietary model in real-world vulnerability discovery, potentially democratizing advanced cybersecurity capabilities. It also highlights significant progress in applying AI to automated vulnerability analysis. Atuin AI discovered multiple previously undetected high-severity logical vulnerabilities in projects such as curl, gnark, OpenSSL, Python cryptography, and Java bc-java, with the highest score reaching 9.3. On the Berkeley BVI real-world vulnerability leaderboard, Atuin AI ranked first in severity and fifth in total number of severe vulnerabilities.

telegram · zaihuapd · Jul 3, 16:12

**Background**: CyberGym is a large-scale cybersecurity benchmark for evaluating AI agents on real-world vulnerability analysis tasks, containing 1,507 historical vulnerabilities from 188 open-source projects. Claude Mythos is Anthropic's advanced but unreleased AI model known for its vulnerability-finding abilities; a public version called Claude Fable 5 was later released. GLM-5.1 is an open-weight language model from Z.AI, released under the MIT License, designed for long-horizon autonomous tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cybergym.io/cybergym/">CyberGym: Evaluating AI Agents' Real-World Cybersecurity ...</a></li>
<li><a href="https://arxiv.org/abs/2506.02548">[2506.02548] CyberGym: Evaluating AI Agents' Real-World ... CyberGym Leaderboard - llm-stats.com CyberGym Benchmark 2026: 9 model averages | BenchLM.ai Defense at AI speed: Microsoft’s new multi-model agentic ... CyberGym-E2E: Scalable Real-World Benchmark for AI Agents ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>

</ul>
</details>

**Tags**: `#网络安全`, `#AI`, `#漏洞挖掘`, `#基准测试`

---