---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 29 items, 10 important content pieces were selected

---

1. [vLLM v0.25.0: Major Overhaul with Model Runner V2 Default](#item-1) ⭐️ 9.0/10
2. [Humanoid Robot Performs World-First Surgery on Live Pigs](#item-2) ⭐️ 9.0/10
3. [OpenAI Releases GPT-5.6 Series with Flagship Sol Model](#item-3) ⭐️ 9.0/10
4. [SGLang v0.5.15: Major Performance Boost with GLM-5.2 and Spec V2](#item-4) ⭐️ 8.0/10
5. [ClickHouse team boosts PgBouncer throughput 4x](#item-5) ⭐️ 8.0/10
6. [VultronRetriever Models Top MTEB Leaderboard](#item-6) ⭐️ 8.0/10
7. [Apple Sues OpenAI for Systematic Trade Secret Theft](#item-7) ⭐️ 8.0/10
8. [Six U-Boot FIT Vulnerabilities Allow Code Execution Before Boot](#item-8) ⭐️ 8.0/10
9. [Zhipu AI Founder Launches 'Touch High Plan' for AGI](#item-9) ⭐️ 8.0/10
10. [Shanghai aims for high-quality brain control by 2027 with BCI breakthroughs](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0: Major Overhaul with Model Runner V2 Default](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0, released with 558 commits from 232 contributors, makes Model Runner V2 the default execution path for all dense models, removes legacy PagedAttention, and achieves Transformers backend parity with native vLLM speed. This release marks a significant architectural shift for vLLM, simplifying the codebase by removing legacy components and improving performance across modeling backends, which directly benefits users deploying large language models for inference. Model Runner V2 now supports EVS (Efficient Video Sampling), realtime embeddings, and dynamic speculative decoding with full CUDA graphs, while the new Streaming Parser Engine unifies tool-call/reasoning parsing.

github · khluu · Jul 11, 20:06

**Background**: vLLM is an open-source high-throughput LLM inference engine developed by UC Berkeley and others. It originally used PagedAttention to manage memory efficiently. Model Runner V2 is a newer, more flexible execution framework that replaces legacy components, improving performance and maintainability.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm -project/ vllm</a></li>
<li><a href="https://docs.vllm.ai/en/stable/features/speculative_decoding/dynamic_speculative_decoding/">Dynamic Speculative Decoding - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2025-10-31-run-multimodal-reasoning-agents-nvidia-nemotron">Run Multimodal Reasoning Agents with NVIDIA Nemotron on vLLM | vLLM Blog</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#release`, `#model serving`, `#performance`

---

<a id="item-2"></a>
## [Humanoid Robot Performs World-First Surgery on Live Pigs](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

Surgeons remotely controlled a Unitree G1 humanoid robot to successfully perform two minimally invasive gallbladder removal surgeries on live pigs, marking the world's first use of a general-purpose humanoid robot for live surgery. The results were published in the journal Nature. This breakthrough demonstrates that low-cost general-purpose humanoid robots could potentially replace expensive dedicated surgical systems like the da Vinci, making advanced surgery accessible in resource-limited settings such as rural areas, battlefields, or space. The cost is roughly one-tenth that of traditional surgical robots. The Unitree G1 base model costs about $13,500, and roughly $67,000 with dexterous hands; it stands 1.5 meters tall and weighs 27 kg. The study was led by researchers at the University of California San Diego.

telegram · zaihuapd · Jul 11, 02:29

**Background**: Traditional surgical robots like the da Vinci system cost $500,000 to several million dollars and are bulky. General-purpose humanoid robots were originally designed for general tasks but can perform delicate surgical operations via remote control and dexterous hands. Dexterous hand technology has advanced rapidly in recent years, with AI large models improving precision.

<details><summary>References</summary>
<ul>
<li><a href="https://m.dzplus.dzng.com/share/general/0/NEWS2139618WUMBNTSKAWAFL">半岛聚焦丨65...</a></li>
<li><a href="https://www.jinantimes.com.cn/news-243-5048472.html">jinantimes.com.cn/news-243-5048472.html</a></li>
<li><a href="http://www.news.cn/tech/20240827/d8f188d8e0b9486aadc1ce2ae72efd15/c.html">灵巧手引领人形机器人“心灵手巧”-新华网</a></li>

</ul>
</details>

**Tags**: `#人形机器人`, `#手术`, `#医疗机器人`, `#远程手术`, `#低成本`

---

<a id="item-3"></a>
## [OpenAI Releases GPT-5.6 Series with Flagship Sol Model](https://t.me/zaihuapd/42497) ⭐️ 9.0/10

OpenAI has officially released the GPT-5.6 series, introducing three models: Sol (flagship), Terra (balanced), and Luna (low-cost, high-concurrency). The series significantly improves capabilities in code, knowledge work, design, research, and cybersecurity, and introduces max/ultra reasoning modes, multi-agent collaboration, and Programmatic Tool Calling. This release marks a major step in OpenAI's tiered model strategy, offering tailored performance-cost trade-offs for different use cases. The new reasoning modes and tool-calling capabilities enable more efficient and complex task automation, potentially lowering costs and expanding the applicability of large language models in enterprise and research settings. GPT-5.6 Sol is the most capable model for cybersecurity and long-horizon reasoning tasks, while Terra balances performance and cost, and Luna targets high-throughput, low-cost scenarios. The max reasoning mode gives Sol extended thinking time, and the ultra mode allows spawning sub-agents for parallel decomposition. Programmatic Tool Calling enables models to orchestrate tools through code rather than individual API round-trips.

telegram · zaihuapd · Jul 11, 13:34

**Background**: The GPT-5.6 series comes just two months after GPT-5.5, reflecting OpenAI's rapid iteration pace. Tiered model families (like Sol, Terra, Luna) allow users to choose the best fit for their budget and performance needs. Max/ultra reasoning modes extend the concept of chain-of-thought by allowing deeper deliberation or parallel sub-agent execution. Programmatic Tool Calling, originally pioneered by Anthropic's Claude, enables more efficient tool use by reducing latency and improving reliability.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT - 5 . 6 Sol : a next-generation model | OpenAI</a></li>
<li><a href="https://www.freepixel.com/blog/openai-gpt-5-6-sol/">OpenAI GPT - 5 . 6 Sol : Ultimate Features, Availability Guide</a></li>
<li><a href="https://medium.com/mlworks/whats-new-with-openai-s-gpt5-6-551b3d8cc6b6">What’s New With OpenAI’s GPT 5 . 6 ? | by Mayur Jain | Medium</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-5.6`, `#AI models`, `#large language models`, `#multi-agent`

---

<a id="item-4"></a>
## [SGLang v0.5.15: Major Performance Boost with GLM-5.2 and Spec V2](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

SGLang v0.5.15 introduces production-tuned GLM-5.2 NVFP4 on Blackwell, makes Spec V2 default for up to 11% TPS improvement, and adds IndexShare MTP to reduce draft-step costs by up to 1.9x. These optimizations significantly enhance inference throughput and cost-efficiency for serving large language models, benefiting developers and enterprises deploying LLMs at scale. IndexShare MTP reuses the indexer top-k across draft steps, and Spec V2 uses CUDA-graphable DSA draft-extend to eliminate unnecessary syncs. FlashInfer autotune now covers draft-model graphs.

github · Fridge003 · Jul 10, 22:58

**Background**: SGLang is an open-source LLM inference engine known for high performance. NVFP4 is NVIDIA's 4-bit floating-point format for efficient inference on Blackwell GPUs. Speculative decoding accelerates generation by using a smaller draft model.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>
<li><a href="https://huggingface.co/blog/zai-org/glm-52-blog">GLM-5.2: Built for Long-Horizon Tasks</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#performance optimization`, `#speculative decoding`, `#GPU serving`, `#sglang`

---

<a id="item-5"></a>
## [ClickHouse team boosts PgBouncer throughput 4x](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse Managed Postgres team scaled PgBouncer throughput by 4x using SO_REUSEPORT for socket reuse and a peering mechanism for efficient cancel forwarding. This improvement enables PgBouncer to utilize multiple CPU cores, overcoming its single-threaded bottleneck. It benefits PostgreSQL deployments with high connection turnover and query cancellation loads. The setup requires setting so_reuseport=1 in pgbouncer.ini and configuring peer_id with a [peers] section to forward cancel requests to the correct owning process.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a single-threaded PostgreSQL connection pooler, limiting it to one CPU core. Running multiple processes with SO_REUSEPORT lets the OS distribute connections, but cancel requests must reach the exact process that owns the session. Peering solves this by encoding a peer_id in cancel keys and forwarding misrouted cancellations.

<details><summary>References</summary>
<ul>
<li><a href="https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres">How we scale PgBouncer in ClickHouse Managed Postgres</a></li>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>
<li><a href="https://deepwiki.com/pgbouncer/pgbouncer/7.3-peer-forwarding-and-cancel-requests">Peer Forwarding and Cancel Requests | DeepWiki</a></li>

</ul>
</details>

**Discussion**: Commenters expressed interest in the peering setup and noted alternatives like Odyssey and pgdog. Others shared experiences running multiple PgBouncer processes on Kubernetes. The discussion was constructive, with questions about so_reuseport and peering configuration.

**Tags**: `#PostgreSQL`, `#PgBouncer`, `#performance`, `#connection pooling`, `#scalability`

---

<a id="item-6"></a>
## [VultronRetriever Models Top MTEB Leaderboard](https://www.reddit.com/r/MachineLearning/comments/1utmxq8/vultronretriever_family_of_models_released_on/) ⭐️ 8.0/10

The VultronRetriever family of models (Prime-8B, Core-4.5B, Flash-0.8B) were released on HuggingFace, achieving #1 in their respective classes on the MTEB Leaderboard, with Prime-8B as global #1 and claiming up to 16x smaller index storage and 12x higher throughput. This release significantly advances retrieval efficiency, enabling large-scale embedding and retrieval tasks with drastically reduced storage and latency, and brings state-of-the-art retrieval to edge devices like iPhone for fully offline use. The models utilize Hydra Architecture for late interaction retrieval, offering high precision and up to half the memory of comparable models. They were trained on datasets with 0% cross-dataset duplication and 0% eval contamination.

reddit · r/MachineLearning · /u/madkimchi · Jul 11, 15:22

**Background**: MTEB (Massive Text Embedding Benchmark) is a standard public leaderboard for evaluating embedding models across retrieval, classification, clustering, and other tasks. Late interaction retrieval, as used in ColBERT, processes queries and documents separately until final stages for efficient and precise retrieval. The Hydra Architecture unifies retrieval and generation in a single vision-language model.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/spaces/mteb/leaderboard">MTEB Leaderboard - a Hugging Face Space by mteb</a></li>
<li><a href="https://arxiv.org/html/2603.28554">Hydra: Unifying Document Retrieval and Generation in a Single Vision-Language Model</a></li>
<li><a href="https://embeddings-benchmark.github.io/mteb/get_started/usage/leaderboard/">Run the Leaderboard - Massive Text Embedding Benchmark</a></li>

</ul>
</details>

**Tags**: `#retrieval`, `#MTEB`, `#NLP`, `#AI`, `#model release`

---

<a id="item-7"></a>
## [Apple Sues OpenAI for Systematic Trade Secret Theft](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 8.0/10

Apple filed a lawsuit on July 10 in the U.S. District Court for the Northern District of California against OpenAI, two former employees, and io Products, accusing them of systematically stealing trade secrets related to product design, manufacturing processes, and supply chain to accelerate OpenAI's consumer hardware development. This lawsuit between two tech giants highlights escalating tensions over intellectual property and talent poaching, potentially reshaping how companies protect trade secrets in the AI and hardware sectors. Apple alleges that former employee Chang Liu accessed internal networks after leaving and downloaded dozens of hardware files, while OpenAI's hardware chief Tang Yew Tan reportedly sent supplier documents to his personal email before resigning and asked job applicants to bring Apple parts to interviews. Apple also claims over 400 former employees now work at OpenAI.

telegram · zaihuapd · Jul 11, 03:14

**Background**: Apple is known for its tight secrecy around product development and hardware design. OpenAI, initially a non-profit AI research lab, has increasingly shifted toward building consumer hardware, including a rumored AI device. Trade secret lawsuits often arise when employees move between competitors, but this case is notable for its scale and the allegation of systematic theft.

**Tags**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#hardware`

---

<a id="item-8"></a>
## [Six U-Boot FIT Vulnerabilities Allow Code Execution Before Boot](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

Security firm Binarly disclosed six vulnerabilities in U-Boot's FIT signature verification code, with two enabling arbitrary code execution and four causing device crashes, affecting versions since 2013.07. These flaws allow attackers to execute malicious code before the operating system and security software load, potentially disabling firmware defenses and installing persistent firmware malware. For devices with remote firmware update capabilities like BMCs, exploitation can occur without physical access. The vulnerabilities (BRLY-2026-037 through BRLY-2026-042) are in the FIT signature verification logic. Binarly submitted patches that were accepted, but deployment requires hardware vendors to integrate fixes into firmware updates, leaving unsupported legacy devices vulnerable.

telegram · zaihuapd · Jul 11, 08:32

**Background**: U-Boot is a widely used open-source bootloader for embedded devices. FIT (Flattened Image Tree) is a format for packaging kernel, device tree, and other images with cryptographic signatures. The signature verification process ensures only trusted firmware is loaded. Baseboard Management Controllers (BMCs) are specialized microcontrollers that manage system monitoring and remote firmware updates, making them particularly exposed to remote firmware attacks.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/u-boot-fit-signature-verification/">Six U - Boot FIT Signature Verification Flaws Enable Code Execution...</a></li>
<li><a href="https://docs.u-boot-project.org/en/latest/usage/fit/signature.html">U - Boot FIT Signature Verification — Das U - Boot unknown version...</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#bootloader`, `#U-Boot`, `#firmware`

---

<a id="item-9"></a>
## [Zhipu AI Founder Launches 'Touch High Plan' for AGI](https://mp.weixin.qq.com/s/3CQSkf_kBnXiCDgS4L-Cgg) ⭐️ 8.0/10

Zhipu AI founder Tang Jie announced the 'Touch High Plan' in an internal letter, committing to AGI research over short-term commercialization. The plan identifies four key challenges: long-term tasks, autonomous agents, self-training, and safety governance. This signals a strategic shift towards long-term AGI research in China, with significant resources allocated to safety and interpretability, which could influence global AI development. Zhipu's open-source approach and competitive models may accelerate progress in transparent AI. Zhipu plans to invest billions in mechanistic interpretability to make black-box models transparent. Its GLM-5.2 model is already competitive with leading overseas models and is popular in open-source communities.

telegram · zaihuapd · Jul 11, 13:59

**Background**: Mechanistic interpretability is a subfield of explainable AI that aims to understand neural networks by analyzing their internal mechanisms. Zhipu AI is a Chinese AI company known for its GLM series of models, which are open-source and widely used in research and applications. The 'Touch High Plan' outlines a multi-year roadmap for achieving AGI through these four pillars.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability - Wikipedia</a></li>
<li><a href="https://www.scmp.com/tech/tech-trends/article/3359170/zhipu-ai-releases-harness-glm-52-model-chinese-firm-takes-aim-anthropic">Zhipu AI releases harness for GLM-5.2 model as Chinese firm takes aim at Anthropic | South China Morning Post</a></li>

</ul>
</details>

**Tags**: `#AGI`, `#AI safety`, `#interpretability`, `#Zhipu AI`, `#GLM`

---

<a id="item-10"></a>
## [Shanghai aims for high-quality brain control by 2027 with BCI breakthroughs](https://t.me/zaihuapd/42501) ⭐️ 8.0/10

Shanghai's Science and Technology Commission issued the 'Shanghai Brain-Computer Interface Future Industry Cultivation Action Plan (2025-2030)', aiming to achieve high-quality brain control and first clinical applications of semi-invasive BCI products in China by 2027. This marks a significant government push for BCI technology in China, potentially accelerating clinical adoption and establishing Shanghai as a hub for neurotechnology innovation. The plan also targets five or more invasive and semi-invasive BCI products to complete medical device type testing and clinical trials, aiming to restore partial language and motor functions for patients with aphasia and paralysis.

telegram · zaihuapd · Jul 11, 15:49

**Background**: Brain-computer interfaces (BCIs) enable direct communication between the brain and external devices. They are categorized as non-invasive (scalp electrodes), semi-invasive (electrodes placed under the skull but outside the brain), or invasive (implanted directly into brain tissue). Semi-invasive BCIs like ECoG offer a balance between signal quality and surgical risk.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Brain–computer_interface">Brain–computer interface - Wikipedia</a></li>
<li><a href="http://learn.neurotechedu.com/introtobci/">Intro to Brain Computer Interface - NeurotechEDU</a></li>
<li><a href="https://flcube.com/?p=26674">Shanghai's Ambitious Plan to Revolutionize Brain -Computer Interfaces</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#neurotechnology`, `#policy`, `#medical technology`, `#Shanghai`

---