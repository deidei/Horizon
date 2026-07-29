---
layout: default
title: "Horizon Summary: 2026-07-29 (EN)"
date: 2026-07-29
lang: en
---

> From 42 items, 11 important content pieces were selected

---

1. [Claude Shared Links Indexed by Search Engines Leak User Data](#item-1) ⭐️ 9.0/10
2. [Open-source engine runs Gemma 4 26B in 2GB RAM on M-series Mac](#item-2) ⭐️ 8.0/10
3. [Mitchell Hashimoto Launches Superlogical, Built on libghostty](#item-3) ⭐️ 8.0/10
4. [Kimi Launches K3-256k: Half-Price Long-Context AI Model](#item-4) ⭐️ 8.0/10
5. [LLMs Fail to Reliably Follow Long Policy Documents](#item-5) ⭐️ 8.0/10
6. [AI Worms Exploit Microsoft Copilot for Word Self-Propagation](#item-6) ⭐️ 8.0/10
7. [NVIDIA Notifies AIC Partners of GPU Price Hike, Shipments Halted](#item-7) ⭐️ 8.0/10
8. [Russian FSB Charges Telegram Founder Durov with Aiding Terrorism](#item-8) ⭐️ 8.0/10
9. [Hugging Face Abused for Deepfake Nude Images](#item-9) ⭐️ 8.0/10
10. [Moonshot AI seeks $2B at $30B valuation, plans HK IPO](#item-10) ⭐️ 8.0/10
11. [China Drafts Anti-Cyber Violence Law Targeting AI Abuse](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Claude Shared Links Indexed by Search Engines Leak User Data](https://t.me/zaihuapd/42830) ⭐️ 9.0/10

A privacy vulnerability in Anthropic's Claude AI has caused thousands of shared conversation links to be indexed by Google and other search engines, exposing sensitive user data such as API keys, cryptocurrency wallets, and personal information. This incident exposes sensitive data that could lead to identity theft, financial loss, or corporate espionage, and highlights a recurring security gap in AI chat services that competitors like ChatGPT have already addressed. The vulnerability stems from missing 'noindex' meta tags on shared chat pages, allowing search engines to crawl and index them. Similar vulnerabilities in ChatGPT were fixed within about a year of discovery, but Anthropic has not yet resolved this issue.

telegram · zaihuapd · Jul 29, 02:40

**Background**: Claude's 'Share Chat' feature lets users create public links to conversations, intended for sharing with specific people. When a page lacks a 'noindex' tag, search engines like Google may index it, making the content publicly searchable. This is a common oversight in web privacy, and proper use of robots.txt or noindex tags can prevent indexing.

<details><summary>References</summary>
<ul>
<li><a href="https://overcentral.com/en/claude-ai-shared-chats-leak/">Claude AI Privacy Leak: Shared Conversations Indexed by Google</a></li>
<li><a href="https://news.aibase.com/news/29922">Anthropic Claude's Shared Chat Function Exposes Privacy Risks...</a></li>
<li><a href="https://www.zdnet.com/article/claude-ai-shared-chats-indexed-by-google/">Claude AI shared chats indexed by Google - see if your... | ZDNET</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#Claude`, `#AI`, `#vulnerability`

---

<a id="item-2"></a>
## [Open-source engine runs Gemma 4 26B in 2GB RAM on M-series Mac](https://github.com/drumih/turbo-fieldfare) ⭐️ 8.0/10

TurboFieldfare, a new open-source inference engine written in Swift and Metal, enables running the 4-bit quantized Gemma 4 26B-A4B-IT model on any M-series Mac with as little as 2GB RAM by streaming routed experts from SSD. This breakthrough dramatically lowers the hardware barrier for running large language models locally, making powerful on-device AI accessible to users with memory-constrained Macs. It demonstrates a practical approach for running models that exceed available RAM by offloading experts to SSD, which could influence future inference engine designs. The model's 4-bit quantized weights are about 14GB, but the engine uses only ~2GB RAM by keeping the shared layers and KV cache in memory while streaming routed experts from SSD with a small cache and bounded parallel pread. It achieves 5-6 tok/s on an 8GB M2 MacBook Air and 31-35 tok/s on an M5 MacBook Pro, and includes an experimental OpenAI-compatible server with streaming and tool calls.

hackernews · gitpusher42 · Jul 29, 15:05 · [Discussion](https://news.ycombinator.com/item?id=49098510)

**Background**: Large language models (LLMs) like Gemma 4 26B are often too large to fit entirely in consumer device memory. Mixture-of-Experts (MoE) architectures have many specialized 'expert' subnetworks but only activate a few per token, allowing conditional computation. 4-bit quantization reduces weight precision to save space, and KV caching stores previous token states to speed up generation. This engine cleverly exploits MoE sparsity to only load the needed experts from SSD.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/mixture-of-experts-moe-layers">Mixture of Experts ( MoE ) Layers</a></li>
<li><a href="https://medium.com/@minh.hoque/understanding-kv-caching-in-transformers-729271c9b74a">Understanding KV Caching in Transformers - Medium</a></li>
<li><a href="https://arxiv.org/abs/1810.05723">[1810.05723] Post-training 4-bit quantization of convolution ... True 4-Bit Quantized Convolutional Neural Network Training on ... 4-Bit Model Quantization - emergentmind.com Post training 4-bit quantization of convolutional networks ... Post training 4-bit quantization of convolutional networks ... Post training 4-bit quantization of convolutional networks ... 4-bit CNN Quantization Method With Compact LUT-Based ... Images</a></li>

</ul>
</details>

**Discussion**: Community comments are generally positive and engaged. Some users question how this compares to mmap in llama.cpp, and the author notes that the key difference is synchronizing SSD reads with inference. A few users offer compilation tips for older macOS versions and suggest collaboration on related projects like DiffusionGemma.

**Tags**: `#inference engine`, `#on-device AI`, `#LLM`, `#Mac`, `#Metal`

---

<a id="item-3"></a>
## [Mitchell Hashimoto Launches Superlogical, Built on libghostty](https://www.superlogical.com/) ⭐️ 8.0/10

Mitchell Hashimoto announced Superlogical, a new company that will build commercial products on top of the open-source libghostty terminal library. He also plans to transfer ownership of the Ghostty terminal emulator to a non-profit organization. This represents a novel open-source business model where a core project is given to a non-profit, while a company builds on its library as a public dependency. It could inspire other developers to separate library and product ownership, fostering sustainable ecosystems. Superlogical will use libghostty exactly as designed, consuming the same MIT-licensed components available to all, and plans to upstream shared terminal improvements. Ghostty is a fast, GPU-accelerated cross-platform terminal emulator with a C-compatible library (libghostty).

hackernews · yan · Jul 29, 15:41 · [Discussion](https://news.ycombinator.com/item?id=49098965)

**Background**: Ghostty is a terminal emulator that uses platform-native UI and GPU acceleration, and its library libghostty allows embedding the terminal in third-party projects. Mitchell Hashimoto is the creator of Ghostty and previously founded HashiCorp. The announcement details the transfer of Ghostty ownership to a non-profit to ensure its independence.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.</a></li>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>
<li><a href="https://ghostty.org/">Ghostty</a></li>

</ul>
</details>

**Discussion**: Commenters praised the ownership transfer model as a smart way to separate the core open-source project from the commercial entity. Some drew parallels to legacy technologies like OLE/COM, while one user criticized the enigmatic title, preferring more informative headlines. Overall sentiment was positive, with high engagement.

**Tags**: `#open-source`, `#terminal`, `#business model`, `#software engineering`

---

<a id="item-4"></a>
## [Kimi Launches K3-256k: Half-Price Long-Context AI Model](https://www.kimi.com/code/docs/en/kimi-code/models) ⭐️ 8.0/10

Kimi (Moonshot AI) has released the K3-256k model, offering a 256k-token context window at half the price of the existing 1M-token K3 model. This pricing makes long-context AI more accessible for developers and users who typically use under 256k context, potentially accelerating adoption of large-context models in coding and knowledge work. According to a community comment from wxw, within the 256k context, K3-256k delivers the same results as the 1M version, but uses about half the quota. The model is available via Kimi's API and platform.

hackernews · monneyboi · Jul 29, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49101852)

**Background**: Kimi is a Chinese AI chatbot and LLM series developed by Moonshot AI, known for its long-context capabilities. The original K3 model supports a 1M-token context window, which is among the largest available. The new K3-256k variant reduces cost while maintaining performance for most use cases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_(chatbot)">Kimi (AI) - Wikipedia</a></li>
<li><a href="https://platform.kimi.ai/docs/models">Model List - Kimi API Platform</a></li>
<li><a href="https://codingscape.com/blog/llms-with-largest-context-windows">LLMs with largest context windows</a></li>

</ul>
</details>

**Discussion**: Community reaction is generally positive. Users like timcobb note that 256k is sufficient for most tasks and 1M is often excessive. madihaa appreciates the lower cost as they typically stay under 200k context. xyzsparetimexyz calls the price reduction 'massive'. MangoCoffee comments that LLMs are quickly becoming commodities, and US AI labs may lose their moat.

**Tags**: `#LLM`, `#AI`, `#pricing`, `#context-length`, `#Kimi`

---

<a id="item-5"></a>
## [LLMs Fail to Reliably Follow Long Policy Documents](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

A new paper titled 'Handbook.md' demonstrates that large language models fail to reliably follow long policy documents, revealing fundamental limitations in context windows and attention mechanisms. This finding challenges the assumption that LLMs can govern AI agents via lengthy instructions, highlighting a critical safety risk for deploying agents in real-world tasks. The paper shows that even models with claimed 1M token context windows degrade significantly when processing long policies, with performance dropping as document length increases.

hackernews · spIrr · Jul 29, 13:01 · [Discussion](https://news.ycombinator.com/item?id=49096969)

**Background**: Large language models (LLMs) process text using a transformer architecture with an attention mechanism that assigns relevance to different parts of the input. The context window limits how much text the model can consider at once. While recent models boast million-token windows, practical effectiveness is hindered by memory and attention constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.plainenglish.io/context-window-in-llms-198e8079d3c8">Context Window in LLMs. In this article, I will try to simplify</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transformer_(deep_learning)">Transformer (deep learning) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters agree with the findings, noting that even with CLAUDE.md files, models like Claude ignore early instructions after about 10 minutes. Some argue that 'agentic AI' is a synthetically trained capability that fails without post-training on specific handbooks.

**Tags**: `#LLM`, `#AI safety`, `#long-context`, `#agents`, `#benchmark`

---

<a id="item-6"></a>
## [AI Worms Exploit Microsoft Copilot for Word Self-Propagation](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 8.0/10

Researchers have demonstrated a new class of AI worms that can self-propagate through Microsoft Copilot for Word by embedding malicious prompt injection instructions in documents, causing Copilot to automatically modify and forward the infection to new documents without user intervention. This vulnerability highlights a fundamental security flaw in AI agents that cannot distinguish between user commands and data content, posing a serious risk to enterprise environments where AI tools have broad access to documents and email. The worm leverages indirect prompt injection, where adversarial prompts hidden in document text (e.g., using white text) trick Copilot into executing commands like forwarding the infected document to new contacts. No robust mitigation exists yet.

hackernews · Canopy9560 · Jul 29, 11:44 · [Discussion](https://news.ycombinator.com/item?id=49096188)

**Background**: Prompt injection attacks allow attackers to embed hidden instructions in text that large language models may interpret as legitimate commands. Microsoft Copilot for Word integrates LLM capabilities directly into the document editing experience, giving the AI access to read and modify document content. When a user opens a crafted document, Copilot may be tricked into performing actions like sending emails or modifying other documents, enabling the worm to spread.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**Discussion**: Community reactions express concern that this vulnerability class is fundamentally unfixable as long as AI conflates instructions with data. Some users have already uninstalled Copilot, while others highlight existing techniques like white text still working to inject prompts.

**Tags**: `#AI security`, `#prompt injection`, `#Copilot`, `#LLM vulnerabilities`, `#cybersecurity`

---

<a id="item-7"></a>
## [NVIDIA Notifies AIC Partners of GPU Price Hike, Shipments Halted](https://t.me/zaihuapd/42834) ⭐️ 8.0/10

NVIDIA has notified all AIC (Add-in Card) partners of a GPU price increase affecting both Blackwell flagship products with GDDR7 memory and GeForce consumer products with GDDR6 memory. In response, major GPU manufacturers have closed warehouses and paused shipments, tightening supply from late July. This price increase signals higher costs for consumers and could impact the entire GPU market, as NVIDIA passes on rising memory costs. It may also prompt adjustments in product pricing and availability across the board. The price increase covers both GDDR7-based Blackwell flagship line and GDDR6-based GeForce consumer line. Supply chain sources indicate that memory costs for 8GB, 12GB, and 16GB GPUs will increase by approximately $76, $114, and $152 respectively. The RTX 50 SUPER series is also affected.

telegram · zaihuapd · Jul 29, 03:54

**Background**: NVIDIA's AIC (Add-in Card) partners are manufacturers like ASUS, MSI, and Gigabyte that buy GPU chips from NVIDIA and build finished graphics cards. The Blackwell architecture is NVIDIA's latest GPU microarchitecture succeeding Hopper and Ada Lovelace, designed for both datacenter and gaming. GDDR7 is the latest generation of graphics memory offering higher bandwidth than GDDR6. The price increase is driven by rising costs of GDDR7 memory, which NVIDIA previously absorbed but now passes on to partners.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techpowerup.com/news-tags/AIC">News Posts matching 'AIC' | TechPowerUp</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#GPU`, `#price increase`, `#hardware`, `#supply chain`

---

<a id="item-8"></a>
## [Russian FSB Charges Telegram Founder Durov with Aiding Terrorism](https://www.interfax.ru/russia/1106228) ⭐️ 8.0/10

The Russian Federal Security Service (FSB) announced criminal charges against Telegram founder Pavel Durov under Article 205.1.1.1 of the Criminal Code (aiding terrorism) and placed him on an international wanted list. This escalates tensions between Russia and a major encrypted messaging platform, raising concerns about privacy, encryption, and platform liability. It could set a precedent for how governments hold tech leaders accountable for user content. The FSB alleges Telegram management refused to delete channels and bots used by Ukrainian intelligence and terrorist groups for planning attacks, causing deaths of women and children and billions of rubles in damages.

telegram · zaihuapd · Jul 29, 05:56

**Background**: Telegram is an encrypted messaging app founded by Pavel Durov. It has been a subject of controversy for hosting content related to terrorism and extremism. Russia had previously attempted to block Telegram in 2018 but later lifted the ban.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nodeseek.com/post-846558-1">快讯•俄罗斯通缉TG创始人杜罗夫</a></li>
<li><a href="https://www.guancha.cn/internation/2026_07_29_825460.shtml">俄国家安全局：通缉“电报”创始人杜罗夫</a></li>

</ul>
</details>

**Tags**: `#Telegram`, `#privacy`, `#regulation`, `#national security`, `#surveillance`

---

<a id="item-9"></a>
## [Hugging Face Abused for Deepfake Nude Images](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

AI Forensics reported on July 28 that Hugging Face is widely used to generate non-consensual deepfake pornographic content, including images of children, despite the platform's policies against such material. This report highlights a critical AI safety and ethics issue, exposing the gap between platform policies and actual enforcement. It has significant implications for AI governance, platform responsibility, and the protection of vulnerable individuals, especially women and children. In a test, seven out of the top nine image-editing models on Hugging Face could easily "undress" women with simple prompts. A honeypot set up by the researchers received over 1,000 requests in seven days, of which 73% were sexually explicit and nearly 7% targeted children.

telegram · zaihuapd · Jul 29, 08:20

**Background**: Hugging Face is a company and open-source platform where the machine learning community collaborates on models, datasets, and applications. Deepfake technology uses AI, such as generative adversarial networks (GANs), to create highly realistic fake images or videos. The report claims Hugging Face has almost no platform-level safeguards to prevent its tools from generating harmful content.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.ibm.com/think/topics/hugging-face">What is Hugging Face? | IBM</a></li>
<li><a href="https://baike.baidu.com/item/深度伪造/56522542">深度伪造_百度百科</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#deepfakes`, `#Hugging Face`, `#ethics`, `#non-consensual content`

---

<a id="item-10"></a>
## [Moonshot AI seeks $2B at $30B valuation, plans HK IPO](https://t.me/zaihuapd/42845) ⭐️ 8.0/10

Moonshot AI is raising up to $2 billion in a new funding round at a $30 billion valuation, its third round in six months, and is preparing for a Hong Kong IPO. This rapid valuation growth from $4 billion to $30 billion reflects the surging demand for Kimi's chatbot and large language model, signaling high market confidence in Chinese AI startups. The company's annual recurring revenue exceeded $200 million in April, driven by Kimi chatbot and large model demand, and it has launched Kimi Work, a desktop AI agent for autonomous workflows.

telegram · zaihuapd · Jul 29, 10:12

**Background**: Moonshot AI (also known as 月之暗面) is a Chinese AI startup behind the Kimi chatbot. The company has been rapidly scaling, with previous funding rounds led by Meituan. AI agents like Kimi Work are software programs powered by large language models that can autonomously execute tasks, use tools, and interact with systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/products/kimi-work">Kimi Work: Next-Gen Desktop AI Agent for Knowledge Workers</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>

</ul>
</details>

**Tags**: `#AI`, `#funding`, `#Moonshot AI`, `#startup`, `#valuation`

---

<a id="item-11"></a>
## [China Drafts Anti-Cyber Violence Law Targeting AI Abuse](https://mp.weixin.qq.com/s/PrzKFhbwjgFEGBPADvFD6Q) ⭐️ 8.0/10

On July 29, 2026, China's Cyberspace Administration published a draft anti-cyber violence law that for the first time includes specific provisions regulating AI-generated cyber violence and imposes enhanced monitoring and protection duties on platforms. This draft law marks a significant step in Chinese online governance by directly addressing AI-generated harms, which could set a precedent for how other countries regulate AI misuse in cyber violence. The 60-article draft defines cyber violence broadly, requires platforms to build detection mechanisms, and introduces personality rights injunctions and mental damage compensation for victims.

telegram · zaihuapd · Jul 29, 10:59

**Background**: AI-generated cyber violence refers to harmful content such as deepfake abuse, automated harassment, or AI-driven disinformation that targets individuals. China's Civil Code already includes personality rights protections, but this law specifically targets online contexts and AI tools.

<details><summary>References</summary>
<ul>
<li><a href="https://en.bitig.info/blog/ai-generated-cyber-attacks-weapon/">How AI - Generated Cyber Attacks Became a Weapon | Bitig</a></li>
<li><a href="https://natlawreview.com/article/china-s-new-civil-law-adds-right-publicity">China’s New Civil Law Adds Right of Publicity</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#cyber law`, `#platform liability`, `#China`, `#tech policy`

---