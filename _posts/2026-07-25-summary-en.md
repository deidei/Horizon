---
layout: default
title: "Horizon Summary: 2026-07-25 (EN)"
date: 2026-07-25
lang: en
---

> From 26 items, 9 important content pieces were selected

---

1. [vLLM v0.26.0: Inkling, DeepSeek-V4, fp32 lm_head](#item-1) ⭐️ 9.0/10
2. [SGLang v0.5.16: DSpark Decoding & Inkling Support](#item-2) ⭐️ 9.0/10
3. [Open-Weight AI Reaches Its Kubernetes Moment](#item-3) ⭐️ 8.0/10
4. [Ruff v0.16.0: Default rules jump from 59 to 413](#item-4) ⭐️ 8.0/10
5. [Claude Opus 5 Resists Prompt Injection Best Yet](#item-5) ⭐️ 8.0/10
6. [Can AMD Break NVIDIA's CUDA Moat?](#item-6) ⭐️ 8.0/10
7. [Ctrip Fined 10M Yuan for Data Export Violations in China](#item-7) ⭐️ 8.0/10
8. [China Fines Ctrip $730M for Monopoly Abuse](#item-8) ⭐️ 8.0/10
9. [Microsoft to Block Pirated Windows Activation via TPM](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0: Inkling, DeepSeek-V4, fp32 lm_head](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 9.0/10

vLLM v0.26.0 introduces support for the Inkling model family (1T-parameter multimodal MoE), DeepSeek-V4 inference optimizations (specialized routing kernel, fused_topk_bias), fp32 lm_head via head_dtype, and flexible attention backends per KV-cache group. These enhancements significantly improve inference performance and accuracy for state-of-the-art large language models, making vLLM a more versatile and production-ready inference engine for the AI community. Inkling support includes base modeling, CUDA graphs, Hopper FA4 attention, MTP=1 speculative decoding, LoRA, and NVFP4 quantization. DeepSeek-V4 gains a 2.94% E2E TPOT improvement from a specialized routing kernel, plus ROCm and XPU optimizations for sparse decode/prefill.

github · khluu · Jul 25, 10:38

**Background**: vLLM is an open-source high-throughput LLM inference engine. The Inkling model from Thinking Machines Lab is a 975B-parameter MoE transformer with 1M context length, requiring advanced optimization for efficient inference. NVFP4 is a 4-bit floating point quantization format from NVIDIA ModelOpt, enabling reduced memory usage with minimal accuracy loss.

<details><summary>References</summary>
<ul>
<li><a href="https://vllm.ai/blog/2026-07-15-inkling">TML Inkling on vLLM: Day-0 Support with Optimized Performance | vLLM Blog</a></li>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM Documentation</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#performance`, `#release`, `#deep learning`

---

<a id="item-2"></a>
## [SGLang v0.5.16: DSpark Decoding & Inkling Support](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 9.0/10

SGLang v0.5.16 introduces DSpark, a confidence-driven speculative decoding algorithm achieving 383.7 tok/s on DeepSeek-V4-Pro, and adds support for the 975B-parameter Inkling multimodal MoE model with up to 71.7k tok/s input and 171.0 tok/s per-user decode on Blackwell hardware. This release significantly boosts inference throughput for large language models via DSpark's adaptive verification, and enables serving of one of the largest open-weight multimodal models (Inkling), potentially lowering cost and latency for complex AI applications. DSpark drafts semi-autoregressively in blocks and sizes verify windows based on its own confidence, enabled via `--speculative-algorithm DSPARK`. Inkling is a 975B-parameter multimodal MoE with 1M-token context, mixing sliding-window, full and Mamba2 attention, with native MTP and NVFP4 support.

github · Qiaolin-Yu · Jul 25, 00:13

**Background**: Speculative decoding accelerates LLM inference by generating multiple tokens from a draft model and verifying them with the target model. SGLang is an open-source serving framework for large models. DSpark improves upon fixed-length drafting by dynamically adjusting the verify window based on confidence. Inkling is a large multimodal MoE model from Thinking Machines Lab with open weights.

<details><summary>References</summary>
<ul>
<li><a href="https://hyper.ai/en/papers/DSpark">DSpark : Confidence-Scheduled Speculative Decoding with... | HyperAI</a></li>
<li><a href="https://thinkingmachines.ai/inkling/">Inkling - Thinking Machines Lab</a></li>

</ul>
</details>

**Tags**: `#speculative decoding`, `#LLM serving`, `#SGLang`, `#multimodal MoE`, `#performance`

---

<a id="item-3"></a>
## [Open-Weight AI Reaches Its Kubernetes Moment](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

An article by Tobi Knaup argues that open-weight AI models are following the same trajectory as Kubernetes, becoming foundational infrastructure that provides a cost baseline and fosters decentralized innovation. This paradigm shift could democratize AI development, reduce dependency on proprietary models, and influence geopolitical dynamics by enabling decentralized innovation and setting inference cost baselines. The article highlights that open-weight models provide a baseline for inference costs, and discusses challenges such as model origin verification and the need for collaborative development akin to open-source software like Linux.

hackernews · tknaup · Jul 25, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49048034)

**Background**: Kubernetes is an open-source platform for managing containerized workloads, widely adopted as standard infrastructure. Open-weight AI models release trained parameters but not necessarily training data, allowing others to run inference. The article draws a parallel suggesting open-weight models could become the Kubernetes of AI, enabling decentralized innovation.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/open-models/">Open models by OpenAI</a></li>
<li><a href="https://openai.com/global-affairs/open-weights-and-ai-for-all/">Open weights and AI for all | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tokenomics">Tokenomics</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism about the feasibility of banning models by origin, criticize the opacity of tokenomics pricing, and call for more collaborative open-weight development similar to Linux. Some note that OpenAI has released useful open-weight models but wish for more frequent updates.

**Tags**: `#open-weight AI`, `#open-source models`, `#AI infrastructure`, `#geopolitics`, `#tokenomics`

---

<a id="item-4"></a>
## [Ruff v0.16.0: Default rules jump from 59 to 413](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0, released on July 23, 2026, increases the number of default lint rules from 59 to 413, adding many new checks that can detect syntax errors and runtime errors. This significant expansion of default rules will cause many existing Python projects and CI pipelines to fail with new warnings, forcing developers to update their codebases or adjust configurations. It demonstrates Ruff's growing maturity and the trend toward stricter default linting in the Python ecosystem. The update affects tools like Datasette, sqlite-utils, and LLM, where hundreds of warnings were found and fixed using `ruff check --fix --unsafe-fixes`. Examples of new defaults include checks for naive datetime usage (DTZ005), blind exception catching (BLE001), and useless attribute access (B018).

rss · Simon Willison · Jul 25, 22:44

**Background**: Ruff is an extremely fast Python linter and code formatter written in Rust, developed by Astral. It serves as a drop-in replacement for tools like Flake8, isort, and pyupgrade. The default rule set had not been updated since Ruff v0.1.0, and the total available rules have grown from 708 to 968.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/linter/">The Ruff Linter | Ruff - Astral</a></li>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ruff: An extremely fast Python linter and code ...</a></li>
<li><a href="https://astral.sh/">Astral: High-performance Python tooling</a></li>

</ul>
</details>

**Tags**: `#ruff`, `#python`, `#linting`, `#astral`, `#tooling`

---

<a id="item-5"></a>
## [Claude Opus 5 Resists Prompt Injection Best Yet](https://simonwillison.net/2026/Jul/25/boris-cherny/#atom-everything) ⭐️ 8.0/10

Boris Cherny highlighted that Claude Opus 5 is the least prompt-injectable model based on evaluation results from Anthropic's system card. This marks a significant security improvement for large language models. Prompt injection is a critical vulnerability in LLMs, so improved resistance directly enhances AI safety and deployment trust. This could encourage wider adoption of LLMs in sensitive applications. The system card reveals that Opus 5 performed well across prompt injection evaluations and red teaming, making it very hard to attack successfully. The model is priced the same as Opus 4.8 and offers a fast mode at double cost.

rss · Simon Willison · Jul 25, 00:42

**Background**: Prompt injection is a cybersecurity exploit where crafted inputs cause unintended behavior in LLMs by overriding system instructions. System cards are documents published by AI developers that detail model capabilities, safety evaluations, and guardrails. This news demonstrates ongoing efforts to address a key vulnerability in LLM deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>
<li><a href="https://openai.com/index/gpt-5-5-system-card/">GPT‑5.5 System Card - OpenAI</a></li>

</ul>
</details>

**Tags**: `#prompt-injection`, `#anthropic`, `#claude`, `#generative-ai`, `#ai`

---

<a id="item-6"></a>
## [Can AMD Break NVIDIA's CUDA Moat?](https://newsletter.semianalysis.com/p/can-amd-break-the-cuda-moat-amd-advancing) ⭐️ 8.0/10

A detailed analysis of AMD's challenges and strategies to compete with NVIDIA's CUDA ecosystem, covering agentic kernel generation, software quality improvements, and Helios MI455X production issues. AMD's ability to break the CUDA moat is crucial for reducing NVIDIA's dominance in AI hardware, potentially lowering costs and fostering innovation in the GPU market. The article mentions agentic kernel generation using LLM agents for automated optimization, unstable internal development clusters at AMD, and production ramp challenges for the Helios MI455X rack, along with up to 105% discounts from finance engineering.

rss · Semianalysis · Jul 25, 00:33

**Background**: CUDA is NVIDIA's proprietary parallel computing platform introduced in 2007, creating a software ecosystem that locks developers into NVIDIA hardware. This 'CUDA moat' makes it difficult for competitors like AMD to gain traction despite offering competitive hardware. AMD is attempting to overcome this through initiatives like ROCm and new approaches such as agentic kernel generation, which uses LLMs to automatically generate and optimize GPU kernels.

<details><summary>References</summary>
<ul>
<li><a href="https://priyanka-dalmia.medium.com/the-cuda-trap-why-nvidias-real-moat-is-software-not-chips-6f97b25b02bc">The “ CUDA Trap”: Why Nvidia’s Real Moat is Software, Not... | Medium</a></li>
<li><a href="https://www.theregister.com/on-prem/2024/12/17/nvidias-cuda-moat-may-not-be-as-impenetrable-as-you-think/1487298">Nvidia's CUDA moat may not be as impenetrable as you think</a></li>
<li><a href="https://introl.com/blog/amd-helios-mi455x-nvidia-competition-ces-2026">AMD Helios Challenges NVIDIA: The MI 455 X and the... | Introl Blog</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#CUDA`, `#AI Hardware`, `#Software Ecosystem`, `#GPU Competition`

---

<a id="item-7"></a>
## [Ctrip Fined 10M Yuan for Data Export Violations in China](https://t.me/zaihuapd/42758) ⭐️ 8.0/10

Shanghai Ctrip Business Co., Ltd. was fined 10 million yuan by the Shanghai Cyberspace Administration on June 13, 2023, for failing to comply with data export security assessment requirements and illegally transferring personal data abroad. This fine signals intensified regulatory enforcement in China's data privacy landscape, particularly for companies involved in cross-border data transfers. It serves as a warning for other internet firms to comply with China's data export security assessment requirements. The penalty includes both a 10 million yuan fine and a deadline for corrective actions. The company has since cooperated with rectification efforts. The Shanghai Cyberspace Administration noted that some internet enterprises in public service sectors continue to illegally export personal data.

telegram · zaihuapd · Jul 25, 02:24

**Background**: China's Data Export Security Assessment Measures, effective from September 1, 2022, require data processors to undergo a security assessment before transferring certain data abroad. This regulation aims to protect personal information and national security. The measures are part of a broader framework including the Cybersecurity Law, Data Security Law, and Personal Information Protection Law.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gov.cn/zhengce/zhengceku/2022-07/08/content_5699851.htm">数据出境安全评估办法_国务院部门文件_中国政府网</a></li>

</ul>
</details>

**Tags**: `#data privacy`, `#regulation`, `#cross-border data`, `#China`

---

<a id="item-8"></a>
## [China Fines Ctrip $730M for Monopoly Abuse](https://t.me/zaihuapd/42767) ⭐️ 8.0/10

On July 25, 2023, China's State Administration for Market Regulation fined Ctrip 5.179 billion yuan for abusing its market dominance, and ordered it to refund 122 million yuan in forced deposits and carry out comprehensive rectification. This is one of the largest antitrust fines in China's tech sector, signaling strong regulatory enforcement against monopolistic practices in online travel. It impacts Ctrip's dominant position and sets a precedent for other platforms. The fine includes confiscation of illegal gains of 1.658 billion yuan and a penalty of 3.521 billion yuan. Ctrip was also required to refund 122 million yuan in 'order deposits' forcibly deducted from hotel operators.

telegram · zaihuapd · Jul 25, 11:56

**Background**: Abuse of market dominance refers to conduct where a dominant firm uses its power to restrict competition, such as imposing unfair trading conditions. 'Order deposits' are sums held by Ctrip from hotel operators as a form of guarantee, which the regulator found to be an abuse. The Chinese Anti-Monopoly Law prohibits such behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://www.boss-young.com/newsDetail?id=52ddd620-e6d1-45fd-9b5e-08dc0b651319">邦信阳律师事务所</a></li>
<li><a href="https://k.sina.com.cn/article_7879996025_1d5af327906803iaki.html?from=tech">k.sina.com.cn/article_7879996025_1d5af327906803iaki.html?from=tech</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#China`, `#regulation`, `#online travel`, `#monopoly`

---

<a id="item-9"></a>
## [Microsoft to Block Pirated Windows Activation via TPM](https://www.techspot.com/news/113232-microsoft-using-tpm-chips-crack-down-pirated-windows.html) ⭐️ 8.0/10

Microsoft announced that it will require TPM 2.0 attestation for KMS (Key Management Service) servers, meaning a server must cryptographically prove its hardware identity to Microsoft before it can process volume activation requests. This enforcement starts with the next Windows Server release, with preparatory warnings coming to Windows Server 2025 in August 2026. This move directly targets the widely used KMS-based piracy methods, where attackers run fake KMS servers to activate unauthorized copies of Windows. By tying activation to trusted hardware, Microsoft makes it significantly harder for unauthorized activations to succeed, which could impact millions of pirated installations and force the piracy community to develop new workarounds. The TPM attestation feature will be mandatory only for volume activation; consumer Windows editions are not affected. The upcoming Windows Server version will be the first to require TPM proof, and Windows Server 2025 will receive a preparatory notification in August 2026. The blog also notes that Microsoft already blocked the KMS38 loophole in 2025, but a new tool called TSforge from the Massgrave group claims to bypass the entire Windows DRM architecture.

telegram · zaihuapd · Jul 25, 15:55

**Background**: KMS (Key Management Service) is a Microsoft volume activation method used by organizations to activate multiple Windows and Office installations locally. Pirates have long exploited this by setting up fake KMS servers on the internet or locally to activate unauthorized copies. TPM (Trusted Platform Module) 2.0 is a hardware security chip that provides cryptographic attestation, ensuring that only genuine, unmodified KMS servers can process activations. This is part of a broader trend of hardware-based security enforcement in Windows.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/manage/component-updates/tpm-key-attestation">TPM Key Attestation | Microsoft Learn</a></li>
<li><a href="https://massgrave.dev/kms38">KMS38 Documentation | MAS</a></li>
<li><a href="https://github.com/massgravel/TSforge">GitHub - massgravel/TSforge: A collection of activation/evaluation extension methods for Windows Vista through 11. · GitHub</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#Windows`, `#TPM`, `#DRM`, `#Piracy`

---