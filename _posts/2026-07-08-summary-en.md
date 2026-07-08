---
layout: default
title: "Horizon Summary: 2026-07-08 (EN)"
date: 2026-07-08
lang: en
---

> From 41 items, 14 important content pieces were selected

---

1. [China Plans $295B National Computing Network Over 5 Years](#item-1) ⭐️ 9.0/10
2. [16-Year-Old KVM Flaw Allows VM Escape on Intel and AMD](#item-2) ⭐️ 9.0/10
3. [China plans to restrict top AI model exports](#item-3) ⭐️ 9.0/10
4. [Kokoro: High-Quality TTS That Runs on CPU](#item-4) ⭐️ 8.0/10
5. [EU Chat Control Proposal: Mass Surveillance of Encrypted Messages](#item-5) ⭐️ 8.0/10
6. [EU mandates driver monitoring cameras in new cars](#item-6) ⭐️ 8.0/10
7. [Why skilled workers leave Germany despite high demand](#item-7) ⭐️ 8.0/10
8. [Microsoft lays off idTech team at id Software](#item-8) ⭐️ 8.0/10
9. [sqlite-utils 4.0 Introduces Schema Migrations and More](#item-9) ⭐️ 8.0/10
10. [MIRA: 5B Parameter Multiplayer World Model for Rocket League](#item-10) ⭐️ 8.0/10
11. [Constraining Fine-Tuning to Trusted LoRA Subspace Prevents Poisoning](#item-11) ⭐️ 8.0/10
12. [Anthropic Releases Claude Sonnet 5 with Strong Agentic Abilities](#item-12) ⭐️ 8.0/10
13. [Nvidia Blackwell dies US-made, but packaged in Taiwan](#item-13) ⭐️ 8.0/10
14. [DeepSeek develops its own AI inference chip](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [China Plans $295B National Computing Network Over 5 Years](https://t.me/zaihuapd/42399) ⭐️ 9.0/10

China announced a plan to invest approximately 2 trillion yuan ($295 billion) over five years to build a nationwide interconnected data center network, prioritizing domestic AI chips from suppliers like Huawei with a target of at least 80% adoption, reducing reliance on US companies such as Nvidia and AMD. This represents one of the largest computing infrastructure investments globally, which could reshape AI hardware supply chains, accelerate China's technological self-sufficiency, and significantly impact the global chip market. The network is a key component of China's 'six networks' infrastructure plan and will be operated by state-owned telecom enterprises. China Telecom and China Unicom have already launched 'token packages' that sell computing power like mobile data.

telegram · zaihuapd · Jul 7, 04:45

**Background**: Under its 15th Five-Year Plan, China introduced the 'six networks' infrastructure initiative, which includes computing power networks, satellite internet, and 5G-Advanced/6G. The computing power network aims to integrate scattered computing resources, making high-performance computing accessible to enterprises and public sectors. Additionally, China has developed 'computing power tokens' that standardize green energy-powered computing capacity, reducing costs for AI applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.digitimes.com/news/a20260616VL212/infrastructure-technology-industrial-communications-water.html">China's six-network plan signals a long-term infrastructure and technology self-reliance push</a></li>
<li><a href="https://www.scmp.com/tech/big-tech/article/3353891/china-ramps-building-national-computing-power-network-ai-token-demand-surges">China ramps up building a national computing power network as AI token demand surges | South China Morning Post</a></li>
<li><a href="https://english.news.cn/20260522/74806708cbd64cd5adfaa1a8527f5ec7/c.html">China races to industrialize computing power with token factory, consumer token plans -Xinhua</a></li>

</ul>
</details>

**Tags**: `#computing infrastructure`, `#AI chips`, `#China tech policy`, `#Huawei`, `#semiconductor`

---

<a id="item-2"></a>
## [16-Year-Old KVM Flaw Allows VM Escape on Intel and AMD](https://github.com/V4bel/Januscape) ⭐️ 9.0/10

Security researchers disclosed Januscape (CVE-2026-53359), a 16-year-old KVM/x86 vulnerability that enables virtual machine escape on both Intel and AMD platforms. A proof-of-concept (PoC) exploit has been released, and the flaw was previously used as a 0-day in Google's kvmCTF competition. This is the first known KVM VM escape affecting both Intel and AMD systems, posing a severe threat to multi-tenant cloud environments. The vulnerability breaks the isolation boundary between guest VMs and the host, potentially allowing attackers to compromise the entire host and other VMs. The vulnerability is a use-after-free flaw in the shadow MMU emulation, where a guest can corrupt the host kernel's shadow page tables through internal operations. In RHEL and other distributions, local unprivileged users can also exploit the bug to escalate privileges to root.

telegram · zaihuapd · Jul 7, 10:14

**Background**: KVM (Kernel-based Virtual Machine) is a Linux kernel module that allows the host to run multiple virtual machines. The shadow MMU is responsible for managing page tables for guest VMs when hardware virtualization support (like Intel EPT or AMD NPT) is not used or available. A use-after-free vulnerability occurs when a program continues to use a memory object after it has been freed, potentially leading to memory corruption and arbitrary code execution.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html">16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host on Intel and AMD x86 Systems</a></li>
<li><a href="https://securityaffairs.com/194868/security/januscape-16-year-old-linux-kvm-bug-enables-cloud-vm-escape-attacks.html">Januscape: 16-Year-Old Linux KVM Bug Enables Cloud VM Escape Attacks</a></li>
<li><a href="https://gbhackers.com/16-year-old-januscape-kvm-escape-vulnerability/">16-Year-Old Januscape KVM Escape Vulnerability Lets Attackers Compromise Linux Hosts</a></li>

</ul>
</details>

**Tags**: `#security`, `#virtualization`, `#KVM`, `#vulnerability`, `#cloud`

---

<a id="item-3"></a>
## [China plans to restrict top AI model exports](https://www.reuters.com/world/beijing-is-looking-curbing-overseas-access-chinas-top-ai-models-sources-say-2026-07-07/) ⭐️ 9.0/10

China's Ministry of Commerce has held meetings with Alibaba, ByteDance, and startup Zhipu to discuss restricting access to the country's most advanced AI models, including future releases, and potentially criminalizing technology leaks. This represents a major potential shift in global AI policy, affecting major Chinese AI companies and the international availability of leading AI models, with significant implications for the AI industry and geopolitics. The restrictions may only apply to future model releases and are still under discussion, with no final decision yet. The talks also considered restricting foreign investment in domestic AI startups.

telegram · zaihuapd · Jul 7, 11:42

**Background**: Export controls on AI models are part of broader national security measures. China has been developing advanced AI models like those from Alibaba (Qwen) and ByteDance (Doubao), and the government is increasingly concerned about technology leakage and geopolitical competition.

**Tags**: `#AI policy`, `#national security`, `#China`, `#export controls`, `#AI models`

---

<a id="item-4"></a>
## [Kokoro: High-Quality TTS That Runs on CPU](https://ariya.io/2026/03/local-cpu-friendly-high-quality-tts-text-to-speech-with-kokoro/) ⭐️ 8.0/10

Kokoro, an open-source TTS model with 82 million parameters, delivers high-quality speech synthesis that runs efficiently on CPU without requiring a GPU. This is significant for users without dedicated GPUs, enabling high-quality local TTS for accessibility tools, podcast generation, and more, democratizing speech synthesis. Kokoro supports IPA pronunciation guides for correcting homographs, and has been integrated into a Chrome extension for reading web pages aloud with highlighting.

hackernews · speckx · Jul 7, 18:24 · [Discussion](https://news.ycombinator.com/item?id=48821576)

**Background**: Text-to-speech (TTS) converts written text into spoken audio. Many high-quality TTS models require powerful GPUs, limiting their accessibility. Kokoro is a lightweight model (82M parameters) optimized for CPU inference, making it suitable for everyday hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://kokorottsai.com/">Kokoro TTS: Advanced AI Text-to-Speech Model with 82M parameters</a></li>
<li><a href="https://grokipedia.com/page/Kokoro_TTS">Kokoro TTS</a></li>

</ul>
</details>

**Discussion**: Community feedback is highly positive, with users praising Kokoro for its CPU-friendliness and accessibility use cases. Some note limitations with single-word pronunciation and suggest improvements like better homograph handling. A Chrome extension was shared to streamline usage on web pages.

**Tags**: `#text-to-speech`, `#machine learning`, `#accessibility`, `#CPU`, `#open source`

---

<a id="item-5"></a>
## [EU Chat Control Proposal: Mass Surveillance of Encrypted Messages](https://fightchatcontrol.eu/chat-control-overview) ⭐️ 8.0/10

The European Union's Chat Control proposals (1.0 and 2.0) would require tech companies to scan all private messages on users' devices for child sexual abuse material (CSAM), effectively breaking end-to-end encryption. The plan has drawn widespread criticism from privacy advocates and technical experts for enabling mass surveillance. If enacted, Chat Control would mandate client-side scanning, undermining the security and privacy of all encrypted communications in the European Union. This sets a dangerous precedent for mass surveillance and could severely impact trust in digital communications and software engineering practices. Chat Control 1.0 provided a temporary derogation from the ePrivacy Directive allowing voluntary scanning but expired in 2024; however, companies like Meta, Google, and Microsoft announced they would continue scanning. Chat Control 2.0 proposes mandatory scanning of all messages, including encrypted ones, without a warrant or suspicion.

hackernews · gasull · Jul 7, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48818311)

**Background**: End-to-end encryption (E2EE) ensures that only the sender and recipient can read message contents. Client-side scanning (CSS) works by scanning a message on the user's device before encryption (or after decryption) to check against a database of known CSAM hashes without revealing content to the service provider — but in practice, it can be bypassed or expanded to scan for other content, posing privacy risks. The EU's Chat Control proposal aims to combat child sexual abuse online but has been widely criticized by technologists and human rights groups as a form of mass surveillance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Regulation_to_Prevent_and_Combat_Child_Sexual_Abuse">Chat Control - Wikipedia</a></li>
<li><a href="https://www.eff.org/deeplinks/2026/04/eu-parliament-blocks-mass-scanning-our-chats-whats-next">EU Parliament Blocks Mass-Scanning of Our Chats—What's Next? | Electronic Frontier Foundation</a></li>
<li><a href="https://www.patrick-breyer.de/en/posts/chat-control/">Chat Control: The EU's CSAM scanner proposal</a></li>

</ul>
</details>

**Discussion**: Commenters overwhelmingly oppose the proposal, viewing it as a broad surveillance tool disguised as child protection. One user notes that while everyone wants to stop child abuse, the law is overly broad and would affect all users. Another points out the irony of the EU claiming to protect privacy while pushing this surveillance, and a third mentions that the European Parliament even blocked a party that opposed chat control.

**Tags**: `#privacy`, `#encryption`, `#surveillance`, `#EU legislation`, `#CSAM`

---

<a id="item-6"></a>
## [EU mandates driver monitoring cameras in new cars](https://allaboutcookies.org/eu-mandatory-distracted-driver-system) ⭐️ 8.0/10

The European Union has mandated that every new car sold must include a driver monitoring camera system to detect and deter distracted driving. This regulation affects all new cars in the EU, potentially reducing accidents caused by distraction, but it also raises significant privacy and user experience concerns among drivers. The system typically uses an infrared camera on the steering column to track the driver's face and eye movements at high frequency, and it can integrate with other safety features like lane keep assist.

hackernews · nickslaughter02 · Jul 7, 20:50 · [Discussion](https://news.ycombinator.com/item?id=48823557)

**Background**: Driver monitoring systems (DMS) are a type of advanced driver-assistance system (ADAS) that use cameras and sensors to monitor driver alertness. They detect signs of fatigue, distraction, or impairment. The EU's mandate aligns with a global trend toward requiring DMS in new vehicles, similar to regulations in other regions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Driver_monitoring_system">Driver monitoring system - Wikipedia</a></li>
<li><a href="https://www.edmunds.com/car-technology/driver-monitoring-system.html">Driver Monitoring Systems | Edmunds</a></li>

</ul>
</details>

**Discussion**: Community comments reveal a mix of support and criticism. Some users praise the accuracy of systems like Ford's Blue Cruise for catching distractions, while others complain about annoying beeps, intrusive UX (e.g., Volvo's lane assist), and privacy concerns akin to Boeing's alarm issues.

**Tags**: `#EU regulation`, `#driver monitoring`, `#privacy`, `#automotive`, `#safety`

---

<a id="item-7"></a>
## [Why skilled workers leave Germany despite high demand](https://www.dw.com/en/germany-migrants-skilled-workers-integration-labor-market-bureaucracy-language-housing/a-77853162) ⭐️ 8.0/10

An article and a Hacker News discussion highlight the reasons skilled workers leave Germany, focusing on bureaucracy, cultural integration barriers, and limited career advancement opportunities. This matters because Germany faces a skilled labor shortage, and losing foreign talent undermines its economic competitiveness and integration efforts. Community comments point to specific issues: slow bureaucracy, poor infrastructure, cultural exclusivity, and lack of upward mobility, especially for those not in international companies.

hackernews · theanonymousone · Jul 7, 10:42 · [Discussion](https://news.ycombinator.com/item?id=48815982)

**Background**: Germany has actively recruited skilled workers from abroad to address demographic and labor shortages. However, retention has been challenging due to complex visa processes, language barriers, and a reserved social culture. The discussion reflects broader debates about integration and career mobility for expatriates.

**Discussion**: Commenters share personal experiences of feeling unwelcome and facing limited career growth. Some cite systemic issues like declining infrastructure and bureaucracy, while others highlight success stories but note that integration takes a long time.

**Tags**: `#immigration`, `#skilled workers`, `#Germany`, `#career mobility`, `#culture`

---

<a id="item-8"></a>
## [Microsoft lays off idTech team at id Software](https://gamefromscratch.com/microsoft-fire-idtech-team-at-id-software/) ⭐️ 8.0/10

Microsoft has laid off the entire idTech engine development team at id Software, effectively ending internal development of the proprietary game engine. This move may force future id Software titles to rely on third-party engines like Unreal Engine, reducing engine diversity and potentially diminishing the unique technical identity of id games. The layoffs are part of broader cuts within Microsoft Gaming, though no official confirmation from Microsoft or id Software has been provided. The idTech engine has powered iconic franchises such as Doom and Quake.

hackernews · bauc · Jul 7, 15:33 · [Discussion](https://news.ycombinator.com/item?id=48819244)

**Background**: idTech is a proprietary game engine developed by id Software, known for pioneering advanced graphics techniques like real-time ray casting and megatextures. Microsoft acquired id Software in 2021 as part of its ZeniMax Media purchase. Game engines are foundational tools for game development, and maintaining a proprietary engine requires specialized internal expertise.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech">id Tech - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech_5">id Tech 5 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Id_Tech_6">id Tech 6 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments reflect a mix of criticism and skepticism. Some argue Microsoft is sacrificing technical uniqueness for cost efficiency, potentially strengthening Epic Games' engine monopoly. Others question whether the idTech team was actually let go, noting the article lacks direct evidence.

**Tags**: `#Microsoft`, `#id Software`, `#game engines`, `#layoffs`, `#game development`

---

<a id="item-9"></a>
## [sqlite-utils 4.0 Introduces Schema Migrations and More](https://simonwillison.net/2026/Jul/7/sqlite-utils-4/#atom-everything) ⭐️ 8.0/10

sqlite-utils 4.0 has been released, adding database schema migrations, nested transactions via a new `db.atomic()` method, and support for compound foreign keys. This is the first major version bump since 3.0 in November 2020. This update addresses long-standing developer requests for schema migration support in a widely-used Python library for SQLite, making it easier to manage database changes in projects. The addition of nested transactions and compound foreign keys further enhances the library's utility for complex database operations. Migrations are defined in Python files using the `Migrations` class and the `table.transform()` method, which implements the SQLite-recommended pattern of recreating tables to allow advanced schema changes. The library's `migrate` command applies pending migrations and tracks them in a dedicated table.

rss · Simon Willison · Jul 7, 19:32

**Background**: sqlite-utils is a Python library and command-line tool for manipulating SQLite databases, created by Simon Willison. Schema migrations are a way to version-control and apply incremental changes to a database schema, which is important for evolving applications. Prior to 4.0, users had to manually handle schema changes, often using raw SQL or external migration tools.

**Tags**: `#sqlite-utils`, `#SQLite`, `#Python`, `#schema migrations`, `#database`

---

<a id="item-10"></a>
## [MIRA: 5B Parameter Multiplayer World Model for Rocket League](https://www.reddit.com/r/MachineLearning/comments/1upofuw/mira_multiplayer_interactive_world_models_trained/) ⭐️ 8.0/10

Researchers from General Intuition, Kyutai, and Epic Games released MIRA, a 5-billion-parameter multiplayer world model trained on 10,000 hours of synthetic Rocket League gameplay, capable of running 4 players at 20 fps on a single NVIDIA B200 GPU, along with a playable demo, technical paper, and a 1,000-hour dataset. MIRA represents a significant step toward large-scale, interactive world models for multi-agent environments, enabling real-time simulation and planning in a complex game. Its open-source release (code, demo, dataset) accelerates research in world models, reinforcement learning, and game AI, with potential applications beyond gaming. The model has 5 billion parameters and achieves 20 frames per second for four players on an NVIDIA B200 GPU. It was trained on synthetic data generated from Rocket League replays, and the released dataset includes 1,000 hours of 4-player gameplay.

reddit · r/MachineLearning · /u/MasterScrat · Jul 7, 07:59

**Background**: A world model is a machine learning system that learns an internal representation of an environment and predicts how it evolves in response to actions, enabling agents to plan and reason without constant real-world interaction. Rocket League, a high-speed multiplayer game with physics-based interactions, serves as a challenging testbed for multi-agent world models. MIRA builds on prior work in interactive video generation and world models, but tackles the additional complexity of multiple interacting agents.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence)</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/world-models/">What Is a World Model? | NVIDIA Glossary</a></li>
<li><a href="https://www.notboring.co/p/world-models">World Models: Computing the Uncomputable</a></li>

</ul>
</details>

**Tags**: `#world models`, `#multi-agent`, `#reinforcement learning`, `#game AI`, `#Rocket League`

---

<a id="item-11"></a>
## [Constraining Fine-Tuning to Trusted LoRA Subspace Prevents Poisoning](https://www.reddit.com/r/MachineLearning/comments/1uq68li/what_if_a_model_could_only_learn_what_trusted/) ⭐️ 8.0/10

A new paper proposes restricting fine-tuning to a subspace learned from trusted LoRA adapters, making certain malicious updates geometrically unreachable. This defense addresses the growing threat of poisoning in fine-tuning by fundamentally limiting what the model can learn, rather than detecting attacks. It could protect applications like personalized assistants and user-adapted models from hidden backdoors. The approach was tested on 196 public LoRA adapters, including adaptive attacks designed to bypass the defense, and showed sharp drops in attack success while preserving useful adaptation on covered tasks.

reddit · r/MachineLearning · /u/Bright_Warning_8406 · Jul 7, 20:00

**Background**: LoRA (Low-Rank Adaptation) is a technique for fine-tuning large models by adding lightweight low-rank matrices to existing weights, avoiding full retraining. The paper proposes constraining fine-tuning updates to lie within a subspace spanned by a pool of trusted LoRA adapters, so that new adaptations must be combinations of previously verified behaviors.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LoRA_(machine_learning)">LoRA (machine learning) - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/lora">What is LoRA (Low-Rank Adaption)? | IBM</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#AI safety`, `#fine-tuning`, `#LoRA`, `#adversarial defense`

---

<a id="item-12"></a>
## [Anthropic Releases Claude Sonnet 5 with Strong Agentic Abilities](https://t.me/zaihuapd/42404) ⭐️ 8.0/10

Anthropic has released Claude Sonnet 5, a new model that boasts the strongest agentic abilities among Sonnet models, capable of planning, using browsers and terminal tools, and running autonomously. It outperforms Sonnet 4.6 in reasoning, tool use, coding, and knowledge work, and approaches the performance of Opus 4.8 at a lower cost. This release makes advanced agentic AI capabilities more accessible and affordable, potentially accelerating adoption in automation, software development, and research. It also intensifies competition in the AI model market, particularly against models like GPT-4 and Gemini. Claude Sonnet 5 is immediately available across all plans and becomes the default model for Free and Pro tiers. Pricing is set at $2 per million input tokens until August 31, 2026, making it cost-effective for heavy usage.

telegram · zaihuapd · Jul 7, 09:02

**Background**: Anthropic's Claude model family includes Sonnet (mid-size, balanced) and Opus (large, high-performance). Agentic capabilities refer to the model's ability to autonomously plan and execute tasks using external tools like browsers and code terminals, mimicking human-like interaction with digital environments.

**Tags**: `#AI`, `#Claude`, `#Anthropic`, `#model release`, `#agent`

---

<a id="item-13"></a>
## [Nvidia Blackwell dies US-made, but packaged in Taiwan](https://www.tomshardware.com/tech-industry/nvidia-and-intel-tout-chips-built-in-america-but-every-arizona-made-blackwell-die-is-still-packaged-in-taiwan) ⭐️ 8.0/10

Nvidia's Blackwell wafers are now being mass-produced at TSMC's Fab 21 in Arizona using a custom 4NP process, but the finished dies must be shipped over 7,000 miles to Taiwan for advanced CoWoS-L packaging. This highlights the persistent dependency of US chip manufacturing on Taiwanese advanced packaging, underscoring the gap in domestic packaging infrastructure and its strategic implications for supply chain resilience. The wafers use TSMC's 4NP node custom for Nvidia, and the packaging step involves dicing, stacking, and CoWoS-L integration. No US facility currently mass-produces or packages HBM, and complete domestic supply chain is not expected before 2028–2029.

telegram · zaihuapd · Jul 7, 09:47

**Background**: Advanced packaging, such as TSMC's CoWoS-L, is crucial for high-performance AI chips like Blackwell because it allows multiple dies (e.g., GPU and HBM memory) to be integrated into a single package with high interconnect density. The US has focused on advancing logic fabrication but lags in packaging capacity, leading to a reliance on Asian supply chains. Several companies like Amkor, TSMC, and SK Hynix are building packaging plants in the US, but these are not yet operational.

**Tags**: `#semiconductor`, `#nvidia`, `#supply chain`, `#geopolitics`

---

<a id="item-14"></a>
## [DeepSeek develops its own AI inference chip](https://www.reuters.com/world/china/chinas-deepseek-developing-its-own-ai-chip-sources-say-2026-07-07/) ⭐️ 8.0/10

DeepSeek, a Chinese AI company, is developing its own AI inference chip to reduce dependence on Nvidia and Huawei chips, according to three sources. The project began about a year ago and is still in early stages. This move is significant as it could reduce DeepSeek's vulnerability to US export restrictions and reshape the AI hardware landscape in China. If successful, it may inspire other Chinese AI firms to pursue chip independence. The chip focuses on inference, not training, meaning it is designed to run trained models for user queries. DeepSeek has started contacting chip design, foundry, and memory companies, and has been hiring chip design engineers privately in recent months.

telegram · zaihuapd · Jul 7, 11:08

**Background**: DeepSeek previously relied on Nvidia H800 and Huawei Ascend chips for its models. US export controls have restricted China's access to advanced AI chips, prompting domestic companies to develop alternatives. Founder Liang Wenfeng acknowledged in a rare 2024 interview that chip restrictions pose a challenge.

**Tags**: `#AI chips`, `#DeepSeek`, `#China`, `#semiconductor`, `#inference`

---