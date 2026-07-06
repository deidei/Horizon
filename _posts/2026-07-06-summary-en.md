---
layout: default
title: "Horizon Summary: 2026-07-06 (EN)"
date: 2026-07-06
lang: en
---

> From 27 items, 6 important content pieces were selected

---

1. [Digital games ownership debate: It's about property rights, not format](#item-1) ⭐️ 8.0/10
2. [Starring the Computer: A unique catalog of movie computers](#item-2) ⭐️ 8.0/10
3. [Free Online Book on Compilers and Language Design](#item-3) ⭐️ 8.0/10
4. [Competence Gate: Using Internal Confidence for Tool-Use Gating](#item-4) ⭐️ 8.0/10
5. [Fudan Course Lets Students Create Questions That Fail AI Models](#item-5) ⭐️ 8.0/10
6. [SpaceX Shows Investors a Thinner-than-iPhone Prototype](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Digital games ownership debate: It's about property rights, not format](https://popcar.bearblog.dev/its-about-ownership/) ⭐️ 8.0/10

A blog post argues that the real issue with digital games is lack of ownership, not the physical vs digital debate, and calls for government regulation to protect consumer property rights. This debate affects millions of gamers who spend money on digital games but may lose access due to DRM or platform shutdowns. Regulation could fundamentally change how digital goods are sold and owned. The post emphasizes that platforms like Steam allow offline play if DRM is bypassed, but many modern games require online checks. The author advocates for laws ensuring digital purchases are truly owned, not just licensed.

hackernews · popcar2 · Jul 5, 14:56 · [Discussion](https://news.ycombinator.com/item?id=48794750)

**Background**: Digital rights management (DRM) restricts how consumers use digital products they 'buy'. In video games, DRM often ties a game to a specific platform or requires online authentication, meaning consumers only own a license, not the game itself. This has led to concerns about ownership, as games can become unplayable if DRM servers shut down.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_rights_management">Digital rights management - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Always-on_DRM">Always-on DRM - Wikipedia</a></li>
<li><a href="https://www.digitaltrends.com/gaming/what-is-drm-in-video-games/">What is DRM in video games and how does it work? - Digital Trends</a></li>

</ul>
</details>

**Discussion**: Commenters widely agree with the article, with many supporting regulation to ensure true ownership. Some highlight that DRM and subscription models have eroded traditional property rights, and others note that cracks and piracy offer more security than legitimate purchases.

**Tags**: `#ownership`, `#digital rights`, `#DRM`, `#gaming`, `#regulation`

---

<a id="item-2"></a>
## [Starring the Computer: A unique catalog of movie computers](https://www.starringthecomputer.com/computers.html) ⭐️ 8.0/10

The website 'Starring the Computer' provides a comprehensive, crowd-sourced catalog of computers that have appeared in movies and television shows, with detailed listings and community discussions. This resource is significant for retro computing enthusiasts, film buffs, and pop culture historians, as it documents the intersection of technology and media, preserving the memory of iconic hardware and its cultural impact. The site has earned a score of 8.0/10 on the platform, with 177 points and 43 comments, indicating strong community validation. Notable insights from comments include the frequent reuse of IBM AN-FSQ-7 panels from 1950s SAGE in movies and a discussion about 6502 assembly code in the original Westworld.

hackernews · gitowiec · Jul 5, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48796093)

**Background**: The website catalogs computers appearing in films and TV, similar to the Internet Movie Car Database for vehicles. Retro computing fans often enjoy spotting vintage hardware in media, and this site serves as a definitive reference. The community contributes corrections and trivia, such as identifying that the slanted panels in many movies are actually modems from the SAGE system.

**Discussion**: Commenters express appreciation for the site's depth, with technical insights such as the widespread reuse of SAGE panels and a correction about 6502 code in Westworld (the code predates the CPU). There is also nostalgia for 80s hardware design and a suggestion to compare with IMCDB. One user notes that in the TV show 'King of Queens', fake computers were often just CRT TVs with paper printouts taped over the screen.

**Tags**: `#retro computing`, `#movies`, `#pop culture`, `#hardware`, `#trivia`

---

<a id="item-3"></a>
## [Free Online Book on Compilers and Language Design](https://dthain.github.io/books/compiler/) ⭐️ 8.0/10

A comprehensive free online textbook titled 'Introduction to Compilers and Language Design' has gained significant attention, with over 282 upvotes and 47 comments on Hacker News. This resource provides an accessible, high-quality learning tool for a notoriously difficult subject, benefiting both students and self-taught programmers interested in compilers and language design. The book covers topics such as error handling, constant folding, and optimization via tree rewriting and instruction count reduction, and includes a sample project for building a C-style compiler step by step.

hackernews · AlexeyBrin · Jul 5, 11:54 · [Discussion](https://news.ycombinator.com/item?id=48793454)

**Background**: Compilers are programs that translate source code written in a high-level programming language into machine code. This field is foundational to computer science but often considered challenging. The book breaks down complex concepts into practical lessons, making it suitable for both beginners and experienced developers.

**Discussion**: Commenters praised the book for its clear explanations and practical project, with one noting it gave useful insights into error handling and constant folding for a 3D printing DSL compiler. Another compared it favorably to the tiny self-compiling C compiler C4, and some noted its focus on C and its idiosyncrasies.

**Tags**: `#compilers`, `#language design`, `#free textbook`, `#education`

---

<a id="item-4"></a>
## [Competence Gate: Using Internal Confidence for Tool-Use Gating](https://www.reddit.com/r/MachineLearning/comments/1unw5un/competence_gate_gating_tooluse_on_a_small_models/) ⭐️ 8.0/10

A new LoRA adapter called Competence Gate for Qwen3.5-4B reads internal confidence signals from the model’s activations to decide whether to answer directly, search the web, or retrieve from local documents, reducing hallucinations and improving error detection with a d' improvement of 0.46. This approach addresses a critical limitation of small language models: poor verbalized confidence calibration. By gating tool use on internal signals rather than stated confidence, it improves reliability for local deployment and reduces leakage of private queries to public search. The adapter is a 10MB LoRA plus a small orchestration layer, runs locally on Apple Silicon/MLX and via GGUF for llama.cpp/Ollama. It also includes a two-signal version that routes personal information questions to local retrieval, cutting private query leakage from 22% to 10%. However, the gate failed to improve grounded document QA on SQuAD 2.0, indicating that parametric competence and evidential grounding are distinct capabilities.

reddit · r/MachineLearning · /u/Synthium- · Jul 5, 07:49

**Background**: Small language models often struggle to accurately express their confidence levels, tending to be overconfident in verbalized outputs. Researchers have found that internal activations can contain more reliable confidence signals than the model's generated text. This technique, known as probing or reading internal states, has been explored in prior work. The d-prime (d') metric measures discrimination ability between signal and noise, commonly used in signal detection theory.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2604.22271">[2604.22271] How LLMs Detect and Correct Their Own Errors: The Role of Internal Confidence Signals</a></li>
<li><a href="https://medium.com/@georgekar91/measuring-confidence-in-llm-responses-e7df525c283f">Measuring Confidence in LLM responses | by George Karapetyan | Medium</a></li>
<li><a href="https://stats.stackexchange.com/questions/492673/understanding-and-implementing-the-dprime-measure-in-python">machine learning - Understanding and implementing the dprime...</a></li>

</ul>
</details>

**Discussion**: The Reddit post includes an update that the gate did not improve grounded document QA on SQuAD 2.0 and actually increased fabrication. The author acknowledges this limitation and discusses construct specificity, noting that 'knowing when to defer' involves at least two distinct signals: parametric competence and evidential grounding.

**Tags**: `#machine learning`, `#small language models`, `#tool use`, `#confidence calibration`, `#open weights`

---

<a id="item-5"></a>
## [Fudan Course Lets Students Create Questions That Fail AI Models](https://mp.weixin.qq.com/s/d53O-6mVFZqMa_Sti1yEPw) ⭐️ 8.0/10

In a Fudan University 'Data Mining Techniques' course, the final exam was redesigned as 'human tests AI', where 51 students each created 10 computational problems with unique answers to challenge three AI models. The AI models scored higher when they answered more incorrectly, rewarding the students' ability to expose AI weaknesses. This innovative assessment paradigm shifts focus from rote memorization to evaluating students' creativity and critical thinking in an AI-augmented world. It highlights the importance of teaching students how to command and judge AI outputs, rather than how to perform tasks manually. 50 out of 51 students managed to make at least one AI model fail, but only 4 students succeeded in making a model score zero on the entire exam. The strongest model, Claude, was never completely defeated, and the average score across all AI models was 85.7 points.

telegram · zaihuapd · Jul 5, 08:40

**Background**: Traditional exams focusing on algorithmic recall and memory are considered obsolete in the AI era, as large language models can easily perform such tasks. The instructor, Xiao Yanghua, emphasized that future assessments will prioritize evaluation, judgment, and creative thinking, aligning with the shift in classrooms from training students 'how to do' to training them 'how to command AI and judge its results'.

**Tags**: `#AI evaluation`, `#education`, `#LLMs`, `#pedagogy`, `#creative assessment`

---

<a id="item-6"></a>
## [SpaceX Shows Investors a Thinner-than-iPhone Prototype](https://www.wsj.com/tech/spacexs-telecom-dreams-d461e568) ⭐️ 8.0/10

SpaceX has reportedly shown investors a prototype handheld device that is thinner than an iPhone, runs its own operating system, and integrates Starlink satellite connectivity, with potential plans to enter the mobile phone market. If confirmed, this could disrupt the smartphone industry by combining SpaceX's Starlink satellite network with a dedicated device, offering global connectivity beyond traditional cellular networks and challenging current mobile operators and device makers. The device reportedly uses a Qualcomm Snapdragon chip and integrates AI technology from Elon Musk's xAI, though Musk has publicly denied the reports. The product is still in early stages and may involve building ground networks or partnering with cellular carriers.

telegram · zaihuapd · Jul 5, 14:10

**Background**: SpaceX currently operates the Starlink satellite internet constellation, which provides broadband to remote areas and has a 'Direct to Cell' capability for standard smartphones. This prototype suggests SpaceX may develop its own hardware to fully leverage satellite connectivity, moving beyond just providing service to existing phones.

<details><summary>References</summary>
<ul>
<li><a href="https://www.msn.cn/zh-cn/技术/人工智能/spacex新人工智能设备将使用高通芯片-马斯克否认/ar-AA270Ujt">SpaceX新人工智能设备将使用高通芯片?马斯克否认 - MSN</a></li>
<li><a href="https://zglg.work/ai/news/zh/2026-07-01-spacex-reportedly-showed-investors-a-sleeker-than-iphone-ai-device-prototype">SpaceX被曝研发AI设备原型：比iPhone更薄，计划搭载xAI技术</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Starlink`, `#mobile phone`, `#satellite communication`, `#telecommunications`

---