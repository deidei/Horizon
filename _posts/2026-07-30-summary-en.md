---
layout: default
title: "Horizon Summary: 2026-07-30 (EN)"
date: 2026-07-30
lang: en
---

> From 38 items, 16 important content pieces were selected

---

1. [GitHub Launches Stacked PRs in Public Preview](#item-1) ⭐️ 9.0/10
2. [Gemini Robotics 2: Whole-Body Intelligence for Robots](#item-2) ⭐️ 9.0/10
3. [OpenAI Cuts GPT-5.6 Luna Cost by 80%](#item-3) ⭐️ 9.0/10
4. [Kimi K3 Achieves Frontier Performance with Novel Engineering](#item-4) ⭐️ 9.0/10
5. [Anthropic's AI Finds Severe Weakness in NIST Post-Quantum Candidate HAWK](#item-5) ⭐️ 9.0/10
6. [Warning: Cheap streaming sticks pose security risks](#item-6) ⭐️ 8.0/10
7. [UEFA and 55 National Associations Refuse FIFA Competitions](#item-7) ⭐️ 8.0/10
8. [Google expands age verification on Android globally via new API](#item-8) ⭐️ 8.0/10
9. [Economic Benefits of Refactoring with AI Oversight](#item-9) ⭐️ 8.0/10
10. [GCC steering committee adopts AI-generated contribution policy](#item-10) ⭐️ 8.0/10
11. [Schneier: AI Writing Tools Erode Critical Thinking](#item-11) ⭐️ 8.0/10
12. [Assistant Professor Loses PhD Candidates Due to Conference Review Process](#item-12) ⭐️ 8.0/10
13. [MLVC: Learned Video Codec for Cross-Platform Deployment](#item-13) ⭐️ 8.0/10
14. [Russia charges Telegram founder Durov with terrorism facilitation](#item-14) ⭐️ 8.0/10
15. [Google DeepMind disbands AlphaFold team, key members join Anthropic](#item-15) ⭐️ 8.0/10
16. [欧盟启动 AI 超级工厂招标 拟撬动约 300 亿欧元投资](#item-16) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GitHub Launches Stacked PRs in Public Preview](https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/) ⭐️ 9.0/10

GitHub announced the public preview of Stacked PRs, a workflow that allows developers to manage multiple interdependent pull requests as an ordered stack. This feature aims to break large changes into smaller, reviewable PRs. This is a major workflow change that could improve code review efficiency and enable more granular collaboration on large features. It may become a standard practice, especially for teams using trunk-based development. The feature is in public preview with known issues; for example, merging an entire stack is broken in many cases, and squash-and-merge requires re-approval for each PR in the stack. A CLI tool (gh-stack) is also available.

hackernews · tomzorz · Jul 30, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49112232)

**Background**: Stacked PRs break a large change into a series of smaller, logically ordered pull requests, each building on the previous one. This is different from a single large PR with many commits. The workflow is inspired by practices used in large open-source projects like the Linux kernel, where patches are sent as a series. GitHub's implementation includes a CLI and UI integration.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-07-30-stacked-pull-requests-are-now-in-public-preview/">Stacked pull requests are now in public preview - GitHub Changelog</a></li>
<li><a href="https://github.github.com/gh-stack/">GitHub Stacked PRs | GitHub Stacked PRs</a></li>

</ul>
</details>

**Discussion**: Community reaction is mixed: developer Steve Klabnik praised it as a huge change, while matharmin reported significant bugs and frustration with the preview's instability. Sameenkarim from the GitHub team asked for feedback and noted it's one of GitHub's largest launches. Overall, excitement about the concept but concern over execution.

**Tags**: `#GitHub`, `#stacked PRs`, `#development workflow`, `#pull requests`, `#version control`

---

<a id="item-2"></a>
## [Gemini Robotics 2: Whole-Body Intelligence for Robots](https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/) ⭐️ 9.0/10

Google DeepMind announced Gemini Robotics 2, a new model family that provides robots with whole-body intelligence, enabling coordinated control from feet to fingertips, advanced dexterity, and multi-robot collaboration. This represents a significant leap in robotics AI, potentially enabling robots to operate more naturally and adaptively in real-world environments, which could accelerate automation in industries and homes. Gemini Robotics 2 is based on the Gemini 2.0 large language model and is a vision-language-action model. It is currently restricted to trusted testers including Agile Robots, Agility Robotics, Boston Dynamics, and Enchanted Tools.

hackernews · ai2027 · Jul 30, 15:15 · [Discussion](https://news.ycombinator.com/item?id=49111237)

**Background**: Robots have traditionally been controlled by separate modules for perception, planning, and control. Gemini Robotics 2 integrates these into a single AI model that can understand natural language, perceive the environment, and generate whole-body actions. This approach aims to make robots more capable of handling complex, unstructured tasks without task-specific programming.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/gemini-robotics-2-brings-whole-body-intelligence-to-robots/">Gemini Robotics 2 brings whole body intelligence to robots</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gemini_Robotics">Gemini Robotics</a></li>
<li><a href="https://deepmind.google/models/gemini-robotics/vla/">Gemini Robotics 2 — Google DeepMind</a></li>

</ul>
</details>

**Discussion**: Community comments show a mix of excitement and skepticism. A DeepMind researcher praised the lab's breadth of work. Some users compared Google's efforts favorably to Anthropic and OpenAI, while others doubted the practicality of humanoid robots due to actuator limitations. Overall sentiment is cautiously optimistic.

**Tags**: `#robotics`, `#deepmind`, `#AI`, `#gemini`, `#whole-body intelligence`

---

<a id="item-3"></a>
## [OpenAI Cuts GPT-5.6 Luna Cost by 80%](https://openai.com/index/advancing-the-price-performance-frontier-with-gpt-5-6/) ⭐️ 9.0/10

OpenAI has announced GPT-5.6 Luna, its fastest and most affordable model, with an 80% reduction in cost and significant improvements in token-generation efficiency. This massive price-performance improvement makes high-quality AI inference far more accessible, potentially reshaping the competitive landscape and enabling new applications that were previously cost-prohibitive. The 80% cost reduction is attributed to kernel-level optimizations (20% reduction in serving cost) and experiments that increased token-generation efficiency by over 15%, according to the community discussion.

hackernews · tedsanders · Jul 30, 17:15 · [Discussion](https://news.ycombinator.com/item?id=49112867)

**Background**: GPT-5.6 is a family of models from OpenAI, released in July 2026, including Sol (flagship), Terra (balanced), and Luna (cost-efficient). Luna was already cheap and capable, but this update makes it five times cheaper. The model is available via the OpenAI API with various rate limits.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/models/gpt-5.6-luna">GPT-5.6 Luna Model | OpenAI API</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>
<li><a href="https://techjournal.org/openai-gpt-5-6-sol-terra-luna">GPT-5.6 Explained: Sol, Terra & Luna (July 2026)</a></li>

</ul>
</details>

**Discussion**: Community members expressed surprise at the magnitude of the price drop, with some comparing it to the dial-up to broadband transition. Users noted that separating trivial from non-trivial tasks for model selection remains a hard problem, and that the cost savings could enable running many more parallel agents.

**Tags**: `#AI`, `#GPT`, `#cost reduction`, `#performance`, `#OpenAI`

---

<a id="item-4"></a>
## [Kimi K3 Achieves Frontier Performance with Novel Engineering](https://www.reddit.com/r/MachineLearning/comments/1vaysjf/how_kimi_k3_engineered_its_way_to_the_frontier_r/) ⭐️ 9.0/10

Moonshot AI released Kimi K3, an open-weight model that ranks 4th out of 580 models on Artificial Analysis, behind only Claude Opus 5, Fable 5, and GPT-5.6 Sol. It introduces Kimi Delta Attention, Quantile Balancing, and AgentENV for significant efficiency gains. Kimi K3 demonstrates that open-weight models can rival proprietary frontier models through novel engineering, potentially democratizing access to top-tier AI. Its innovations in attention, load balancing, and training infrastructure could influence future LLM design. Kimi Delta Attention replaces the KV cache in 69 of 93 layers with a 128x128 matrix per head, reducing memory for a 1M-token context from 104.6 GiB to 27.2 GiB. Quantile Balancing uses router score margins from a single batch to keep 896 experts per layer evenly loaded, replacing fixed-step bias nudging.

reddit · r/MachineLearning · /u/noninertialframe96 · Jul 30, 16:37

**Background**: Large language models often use attention mechanisms that require caching key-value pairs, which becomes memory-intensive for long contexts. Mixture-of-Experts (MoE) models route tokens to different experts, but load imbalance can hurt efficiency. Reinforcement learning from human feedback (RLHF) commonly relies on sandboxed environments for safe training.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>
<li><a href="https://openathena.ai/blog/quantile-balancing/">Mixture of Experts Quantile Balancing: Validated at 32B-A5B (1e22 FLOPs) Scale | Open Athena</a></li>
<li><a href="https://github.com/kvcache-ai/AgentENV">GitHub - kvcache-ai/AgentENV: AgentENV (AENV) is a ...</a></li>

</ul>
</details>

**Tags**: `#model architecture`, `#attention mechanism`, `#open-weight`, `#LLM`, `#training infrastructure`

---

<a id="item-5"></a>
## [Anthropic's AI Finds Severe Weakness in NIST Post-Quantum Candidate HAWK](https://startupfortune.com/claude-mythos-broke-hawk-and-the-nist-post-quantum-timeline-may-not-survive-it/) ⭐️ 9.0/10

Anthropic's Claude Mythos Preview model discovered a severe weakness in the NIST post-quantum candidate HAWK-256, reducing its security margin from 2^64 to 2^38 in about 60 hours at a cost of $100,000 in API fees. This demonstration of AI-driven cryptanalysis shows that large language models can uncover subtle cryptographic flaws that human experts missed for years, potentially accelerating the post-quantum cryptography transition and emphasizing the need for cryptographic agility. The attack is not polynomial-time, so larger key sizes remain secure, and HAWK has not been withdrawn from the NIST process. The research also includes an improved attack on 7-round AES-128, but full 10-round AES-128 remains unaffected.

telegram · zaihuapd · Jul 30, 05:47

**Background**: NIST is standardizing post-quantum cryptographic algorithms to resist attacks from future quantum computers. HAWK is a candidate in the third round of NIST's post-quantum digital signature selection process. The security margin indicates the computational effort required to break an algorithm; a reduction from 2^64 to 2^38 means the algorithm is significantly weaker than previously believed.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/security/2026/07/mythos-uncovers-crypto-weaknesses-that-went-unknown-for-years/">Mythos attack on 3rd-round PQC algorithm candidate puts it ...</a></li>
<li><a href="https://www.nist.gov/pqc">Post-quantum cryptography | NIST</a></li>
<li><a href="https://csrc.nist.gov/csrc/media/Projects/pqc-dig-sig/documents/round-1/spec-files/hawk-spec-web.pdf">HAWK Specification Document - NIST Computer Security Resource ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cryptanalysis`, `#post-quantum cryptography`, `#NIST`, `#Anthropic`

---

<a id="item-6"></a>
## [Warning: Cheap streaming sticks pose security risks](https://krebsonsecurity.com/2026/07/read-this-before-you-buy-that-tv-streaming-stick/) ⭐️ 8.0/10

Krebs on Security published an advisory warning that many cheap TV streaming sticks are pre-loaded with malware and adware used for residential proxy fraud and ad fraud. This exposes consumers to privacy violations and turns their home internet into a tool for cybercrime, while major retailers continue to sell these risky devices. The devices often run outdated Android versions with no security patches and may be intentionally configured for malicious proxy services, making them vulnerable to remote exploitation.

hackernews · speckx · Jul 30, 17:04 · [Discussion](https://news.ycombinator.com/item?id=49112744)

**Background**: Residential proxy fraud involves routing internet traffic through legitimate home IP addresses to hide criminal activity. Cheap streaming sticks and TV boxes are often infected with malware that uses the owner's internet connection as a proxy, enabling ad fraud or other scams. These devices are sold on major e-commerce platforms despite repeated warnings.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fraudlogix.com/glossary/what-is-a-residential-proxy/">Residential Proxy: Detection Evasion & Fraud Prevention | Fraudlogix</a></li>
<li><a href="https://www.trendmicro.com/vinfo/us/security/news/cybercrime-and-digital-threats/the-rise-of-residential-proxies-and-its-impact-on-cyber-risk-exposure-management">The Rise of Residential Proxies as a Cybercrime Enabler | Trend Micro (US)</a></li>
<li><a href="https://spur.us/platform/residential-proxy-detection">Residential Proxy Detection – Expose Automation & Abuse | Spur</a></li>

</ul>
</details>

**Discussion**: Commenters debate retailer accountability, with some arguing Amazon and Best Buy should share responsibility. Users share real experiences of adware on cheap devices, and many note that the low price should have been a red flag. Some express concern about their connection being used for proxy services.

**Tags**: `#security`, `#privacy`, `#streaming devices`, `#malware`, `#consumer alerts`

---

<a id="item-7"></a>
## [UEFA and 55 National Associations Refuse FIFA Competitions](https://www.uefa.com/news-media/news/02a7-213a92896eb0-54dfbf454e3b-1000--statement-on-behalf-of-uefa-and-its-55-national-associations/) ⭐️ 8.0/10

UEFA and its 55 national associations have jointly declared that they will not participate in FIFA competitions, citing concerns over corruption, financial motives, and the increasing commercialization of football. This unprecedented boycott could reshape global football governance, potentially leading to competing tournaments and challenging FIFA's monopoly as the sport's governing body. The decision is in response to FIFA's proposed expansion of the World Cup to 64 teams and alleged corruption under President Gianni Infantino's leadership.

hackernews · dickfickling · Jul 30, 18:40 · [Discussion](https://news.ycombinator.com/item?id=49113929)

**Background**: FIFA is the international governing body of football, organizing major tournaments like the World Cup. UEFA is the European football governing body, overseeing clubs and national teams in Europe. Tensions have been high due to FIFA's commercial practices and governance controversies.

**Discussion**: Commenters largely support UEFA's stance, criticizing FIFA's corruption and commercialization. Some suggest UEFA should organize its own World Cup, while others worry about the impact on players and fans. The discussion highlights a deep rift in football governance.

**Tags**: `#football`, `#FIFA`, `#UEFA`, `#sports governance`, `#corruption`

---

<a id="item-8"></a>
## [Google expands age verification on Android globally via new API](https://android-developers.googleblog.com/2026/07/google-play-age-signals-api-safer-experiences.html) ⭐️ 8.0/10

Google announced the global expansion of age checks on Android by the end of 2026 through the Play Age Signals API, allowing apps to request a user's age range with parental consent via Family Link. This move has significant implications for privacy, regulation, and developers, as it enables age-appropriate content without requiring full identity verification, potentially setting a new standard for platform-wide age gating. The Age Signals API is currently in beta, returning age ranges (e.g., 0-12, 13-15, 16-17, 18+) and requires Android 6.0 or higher; testing is underway in Brazil before full global rollout.

hackernews · dmantis · Jul 30, 10:13 · [Discussion](https://news.ycombinator.com/item?id=49107950)

**Background**: Age verification has been a contentious topic, often requiring accounts or ID uploads. Google's approach tries to balance privacy and safety by using parental controls through Family Link, letting parents share a child's age range without revealing exact birth dates.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.android.com/google/play/age-signals/overview">Play Age Signals overview | Android Developers</a></li>
<li><a href="https://developer.android.com/google/play/age-signals/use-age-signals-api">Use Play Age Signals API (beta) - Android Developers</a></li>
<li><a href="https://cybernews.com/tech/android-developers-age-verification-tool-google/">What is Google’s Android Age Signals API tool? | Cybernews</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed feelings: some oppose mandatory account creation and monopolistic effects, while others worry about complexity and partial solutions, with a user sarcastically suggesting age-gating for the elderly to protect against scams.

**Tags**: `#android`, `#age verification`, `#privacy`, `#regulation`, `#google play`

---

<a id="item-9"></a>
## [Economic Benefits of Refactoring with AI Oversight](https://martinfowler.com/articles/exploring-gen-ai/refactoring-economic-benefit.html) ⭐️ 8.0/10

Martin Fowler's article presents a quantitative analysis of refactoring's economic benefits, specifically examining how AI tools can assist but require human oversight to maintain code quality and safety. This matters because it provides a grounded, evidence-based perspective on AI-assisted refactoring, helping developers and managers make informed decisions about investing in such practices. The article uses empirical measurements to show that while AI can reduce token consumption by making code more compact, human oversight is crucial to prevent introducing errors or losing conceptual integrity.

hackernews · javaeeeee · Jul 30, 15:10 · [Discussion](https://news.ycombinator.com/item?id=49111176)

**Background**: Refactoring is the process of restructuring existing code without changing its external behavior to improve non-functional attributes. AI tools like large language models can suggest refactorings but lack understanding of broader project context, making human review essential for safety.

**Discussion**: Commenters praise the article for being specific and quantitative, with 'whats_a_quasar' noting it's how AI commentary should be written. Some debate the role of AI versus human practices, and 'firasd' emphasizes the indispensable human-in-the-loop for understanding project-wide context.

**Tags**: `#refactoring`, `#AI`, `#software engineering`, `#economics`, `#best practices`

---

<a id="item-10"></a>
## [GCC steering committee adopts AI-generated contribution policy](https://lwn.net/Articles/1086041/) ⭐️ 8.0/10

The GCC steering committee has announced a new policy addressing AI-generated contributions, requiring contributors to certify that they have reviewed and taken responsibility for any code produced with the assistance of generative AI. This policy sets an important precedent for large open source projects managing the influx of AI-generated submissions, aiming to maintain code quality and community trust while avoiding alienating contributors. The policy mandates disclosure of AI use and a human review certification; it also explicitly welcomes contributors who have not yet followed the policy, guiding them toward compliance.

hackernews · arto · Jul 30, 11:45 · [Discussion](https://news.ycombinator.com/item?id=49108685)

**Background**: GCC (GNU Compiler Collection) is a cornerstone open source compiler suite. As generative AI tools like GitHub Copilot become prevalent, maintainers face challenges distinguishing genuine human contributions from automated low-quality or spam submissions, prompting the need for clear policies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/niccrane_maintaining-open-source-in-the-age-of-generative-activity-7437947698504249346-CHV8">AI - generated contributions in open source : Challenges... | LinkedIn</a></li>
<li><a href="https://groundy.com/articles/are-ai-generated-prs-killing-open-source/">Are AI - Generated PRs Killing Open Source ? | Groundy</a></li>
<li><a href="https://ai.plainenglish.io/building-community-contributing-to-open-source-projects-with-ai-4e9597afcf50">Building Community: Contributing to Open - Source Projects with AI</a></li>

</ul>
</details>

**Discussion**: Community comments reveal a wide spectrum of opinions: some praise the policy's welcoming tone, others criticize its enforceability, and one memorable quote highlights the economic asymmetry AI creates. Overall sentiment is engaged but divided.

**Tags**: `#GCC`, `#AI policy`, `#open source`, `#software engineering`, `#community discussion`

---

<a id="item-11"></a>
## [Schneier: AI Writing Tools Erode Critical Thinking](https://simonwillison.net/2026/Jul/30/bruce-schneier/#atom-everything) ⭐️ 8.0/10

Bruce Schneier argues that using AI for writing assignments like policy memos harms the development of critical thinking skills, as these tasks are designed as 'gym tasks' for mental exercise. This argument is significant as it questions the widespread adoption of AI in education and professional training, highlighting potential long-term cognitive consequences for students and employees. Schneier distinguishes between 'gym tasks' (for skill development) and 'work tasks' (for output), and notes that employers are already noticing a decline in critical thinking among graduates.

rss · Simon Willison · Jul 30, 18:25

**Background**: Bruce Schneier is a renowned security technologist and author who frequently writes about technology's societal impacts. He uses the 'gym task' metaphor to describe assignments whose primary purpose is mental exercise, not output, emphasizing that the process of writing itself develops critical thinking skills.

**Tags**: `#AI`, `#education`, `#critical thinking`, `#Bruce Schneier`, `#writing`

---

<a id="item-12"></a>
## [Assistant Professor Loses PhD Candidates Due to Conference Review Process](https://www.reddit.com/r/MachineLearning/comments/1vawwb8/i_have_lost_three_and_a_half_potential_phd/) ⭐️ 8.0/10

An assistant professor reports losing three and a half potential PhD students because the students were discouraged by the negative experiences of submitting papers to top machine learning conferences, despite the papers receiving positive reviews. This highlights a systemic problem in ML academia where the peer review process—characterized by high randomness and repeated resubmissions—alienates talented undergraduates, potentially deterring the next generation of researchers. The professor noted that papers with no obvious flaws attracted increasingly random reviewer criticisms after each resubmission, and even a paper with four unanimous weak accepts was eventually rejected.

reddit · r/MachineLearning · /u/AffectionateLife5693 · Jul 30, 15:30

**Background**: Top machine learning conferences like NeurIPS, ICML, and ICLR (often called the 'big three') use a peer review process where papers are submitted and reviewed by volunteers. The process has been criticized for its high variance and sometimes arbitrary decisions, leading to the term 'lottery ticket submissions' for papers submitted with minimal effort in hope of acceptance. This post illustrates how the process can frustrate even strong papers and discourage young researchers.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.roboflow.com/ai-computer-vision-conferences/">Top AI & Computer Vision Conferences in 2026</a></li>
<li><a href="https://research.com/conference-rankings/computer-science/machine-learning">World's Best Computer Science - Machine Learning & Artificial intelligence Conferences: H-Index Computer Science - Machine Learning & Artificial intelligence Conferences Ranking 2026 | Research.com</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#academia`, `#peer review`, `#PhD`, `#conference review`

---

<a id="item-13"></a>
## [MLVC: Learned Video Codec for Cross-Platform Deployment](https://www.reddit.com/r/MachineLearning/comments/1vb3xwd/mlvc_multiplatform_learned_video_codec_for/) ⭐️ 8.0/10

Researchers introduced MLVC, a multi-platform learned video codec that overcomes cross-platform numerical inconsistency by transmitting entropy model scale parameters through the hyperprior, enabling reliable decoding across different NPUs. This work addresses a critical barrier to real-world deployment of neural video codecs: the lack of bit-exact computation across heterogeneous hardware. By enabling cross-NPU compatibility at 100 FPS, MLVC brings learned codecs closer to practical use in video streaming and communication. MLVC achieves ~100 FPS encoding/decoding for 360p/540p video on consumer NPUs. It avoids requiring bit-exact neural network execution by explicitly sending entropy-model scale parameters through the hyperprior, ensuring consistent entropy decoding across platforms.

reddit · r/MachineLearning · /u/tanelai · Jul 30, 19:40

**Background**: Neural video codecs use deep learning to compress video, potentially outperforming traditional hand-crafted codecs like H.264/H.265. However, deployment is hindered by high power consumption and cross-platform numerical inconsistency, where slight differences in arithmetic between NPUs (e.g., Apple vs. Intel) can break entropy decoding. A neural processing unit (NPU) is a specialized accelerator for AI inference, but current NPU toolchains lack standardized fixed-point arithmetic, leading to non-bit-exact results.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neural_processing_unit">Neural processing unit - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/neural-processing-unit">What is a neural processing unit (NPU)? - IBM</a></li>

</ul>
</details>

**Tags**: `#video codec`, `#machine learning`, `#neural networks`, `#NPU`, `#cross-platform`

---

<a id="item-14"></a>
## [Russia charges Telegram founder Durov with terrorism facilitation](https://t.me/zaihuapd/42859) ⭐️ 8.0/10

On July 29, the Russian Federal Security Service (FSB) charged Telegram founder Pavel Durov under Article 205.1, Part 1.1 of the Criminal Code for facilitating terrorism, and placed him on an international wanted list. This marks a significant escalation in Russia's crackdown on tech platforms, setting a precedent for holding tech leaders personally liable for content moderation failures, and could further strain international relations regarding digital governance. The FSB alleges that Telegram's management refused to delete channels, groups, and bots used by Ukrainian intelligence and terrorist groups to coordinate sabotage, attacks, and fraud, causing numerous casualties and billions of rubles in damage.

telegram · zaihuapd · Jul 30, 03:45

**Background**: The FSB is Russia's primary security agency, responsible for counterintelligence and counterterrorism. Telegram is a widely used messaging app known for its encryption and minimal content moderation. Russian authorities have previously fined Telegram for non-compliance with data laws, but this criminal charge is unprecedented.

**Tags**: `#Telegram`, `#Pavel Durov`, `#FSB`, `#cybercrime`, `#geopolitics`

---

<a id="item-15"></a>
## [Google DeepMind disbands AlphaFold team, key members join Anthropic](https://www.ft.com/content/61b2953d-ee0d-45de-af6e-a9c1cf524b33?syn-25a6b1a6=1) ⭐️ 8.0/10

Google DeepMind has disbanded the Nobel Prize-winning AlphaFold team, reassigning most members to other projects, while three core researchers—John Jumper, Jonas Adler, and Alexander Pritzel—have left to join rival AI company Anthropic. This move signals a strategic shift at DeepMind away from foundational biology research toward large language models and other AI applications, and it represents a significant talent acquisition for Anthropic, which is competing directly with OpenAI and Google in the AI race. Nearly a quarter of the original AlphaFold paper authors have left the company entirely, while others have been internally transferred to projects like Gemini, enzyme design, nuclear fusion, and genomics, as well as to Alphabet's drug discovery subsidiary Isomorphic Labs.

telegram · zaihuapd · Jul 30, 07:45

**Background**: AlphaFold is an AI system developed by DeepMind that predicts the three-dimensional structure of proteins from their amino acid sequences, achieving breakthrough accuracy in the CASP14 competition in 2020. In 2024, Demis Hassabis and John Jumper were awarded half of the Nobel Prize in Chemistry for their work on AlphaFold. The team's dissolution reflects DeepMind's pivot toward more commercially focused AI projects like Gemini.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AlphaFold">AlphaFold</a></li>
<li><a href="https://alphafold.com/">AlphaFold Protein Structure Database</a></li>

</ul>
</details>

**Tags**: `#DeepMind`, `#AlphaFold`, `#Anthropic`, `#AI research`, `#protein folding`

---

<a id="item-16"></a>
## [欧盟启动 AI 超级工厂招标 拟撬动约 300 亿欧元投资](https://www.wsj.com/world/europe/eu-opens-call-for-creation-of-local-ai-gigafactories-c286213d) ⭐️ 8.0/10

EU launches tender for AI super factories aiming to mobilize about 30 billion euros to boost local AI capabilities.

telegram · zaihuapd · Jul 30, 11:50

**Tags**: `#AI infrastructure`, `#European Union`, `#investment`, `#policy`

---