---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<p>
  <a href="/files/Yonghan-Yang-CV.pdf" class="btn btn--info">Full CV (PDF)</a>
  <a href="/files/Yonghan-Yang-Resume.pdf" class="btn btn--info">One-page résumé (PDF)</a>
</p>

Education
======
* **B.Sc. in Artificial Intelligence**, [MBZUAI](https://mbzuai.ac.ae/), Abu Dhabi — *Aug 2025 – May 2029 (expected)*. GPA 3.8/4.0.
  * Honors: Dean's List (inaugural cohort, Fall 2025, top 10%); *Sheikh Tahnoon bin Zayed Scholarship in AI Excellence*; Pioneer Scholarship.
  * Courses: Applied Machine Learning (ML7501, M.S. course), Algorithms & Data Structures, Probability & Statistics, Calculus & Linear Algebra, Introduction to AI, Python Programming, Software, Web & Mobile Engineering, Physics & Life Science in the Age of AI.
* **High school**, [Beijing National Day School](https://www.bnds.cn/), Beijing — *Sep 2019 – Jul 2025*. GPA 4.2/4.3 (unweighted).
  * Advanced Placement program jointly with [Wasatch Academy](https://wasatch.academy/).
  * Courses: Calculus III, Differential Equations, Linear Algebra, Probability Theory, Mathematical Modeling, Sociology, Marine Biology.
  * SAT 1550 (Math 800, English 750); TOEFL 111/120; CEFR C1 (191/200); 11 AP exams with eight 5s (Calculus BC, Physics C: Mechanics, Physics 1, Chemistry, Biology, Computer Science A, Statistics, Psychology).

Experience
======
* **[Cyber-Physical Intelligence Lab](https://cpil-lab.github.io/) & [AAAAA Community](https://github.com/AAAAA-Academia-Attractions)**, *Researcher* — *Oct 2025 – present*
  * Supervised by [Prof. Steve Liu](https://cs.mcgill.ca/~xueliu/site/intro.html) and mentored by [Ye Yuan](https://stevenyuan666.github.io/). CPIL studies trustworthy, efficient, and agentic AI across MBZUAI, McGill University, and Mila; AAAAA Community is a research collective spanning universities, labs, and industry.
  * **[Diffusion Surrogate for Offline Optimization](/publication/2026-spade-offline-black-box-optimization)** (*co-first author*, Oct 2025 – Jan 2026): conditional diffusion models as calibrated surrogates for offline optimization, with a kNN support-proximity prior that keeps the optimizer out of unsupported regions. **Accepted at ICML 2026** (poster presented in Seoul) and the ICLR 2026 DeLTa workshop.
  * **Surrogate-Guided Memory Retrieval for Agents** (*co-first author*, Apr 2026 – present): surrogate-guided offline training of what an autonomous agent recalls, scoring each memory by how much it helps downstream tasks.
  * **[Grounded Multimodal Social Deduction Agents](/publication/2026-quack-multimodal-social-deduction-agents)** (*contributing author*, Feb 2026 – present): QUACK audits whether agents' claims in social deduction games are grounded in what they saw and did. **Accepted at EMNLP 2026.**
  * **[Discrete Diffusion Survey](/publication/2026-discrete-diffusion-survey)** (*contributing author*, Mar 2026 – present): discrete diffusion unified in one design space from tokenization to generation. Under review at TMLR.
  * **[Agentic Benchmark for Financial Intelligence](/publication/2026-herculean-agentic-benchmark-financial-intelligence)** (*contributing author*, Mar – May 2026): evaluated agents on trading, hedging, market-insight, and auditing workflows, and ran key experiments. Under review at ACL ARR.
* **[GenBio AI](https://genbio.ai/)**, *Research Engineer Intern* (remote, since May 2026) — *Oct 2025 – present*
  * **[Multi-Modal Biomedical ML Agent Benchmark](/publication/2026-bioxarena-biomedical-ml-agent-benchmark)** (*contributing author*, Oct 2025 – May 2026): designed the agent framework and curated a 76-task benchmark of agents' code generation for biological research; key contributions to the paper's formulation. **Accepted at NeurIPS 2026.** Supervised by [Prof. Le Song](https://dasongle.github.io/).
* **Shanghai Academy of AI for Science**, *Researcher* (remote) — *May 2026 – present*
* **[Harvard Medical School](https://hms.harvard.edu/)**, *Research Collaborator* (remote) — *Mar – May 2026*
  * **Semi-supervised High-order Relation Learning** (*contributing author*): prediction and analysis on a drug combination–disease relationship dataset. Supervised by [Prof. Jun Wen](https://jungel2star.github.io/).
* **Paper Reviewer**, ICLR — *Feb 2026 – present*
  * ICLR 2027 main conference; [ICLR 2026 Workshop FM4Science](https://fm-science.github.io/).

Publications
======
<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

Awards and honors
======
* MBZUAI *Dean's List*, inaugural cohort (Fall 2025, top 10%) · *Sheikh Tahnoon bin Zayed Scholarship in AI Excellence* & *Pioneer Scholarship* (2025)
* 2026 COMAP MCM, Problem A — *Honorable Mention*
* 2025 IMMC — *Outstanding* (top 1%, Greater China round) & *Meritorious* (top 10%, International round)
* iGEM high-school section — *Gold Medal* & *Top 10* for three years (2023–2025); 2025 *Best Measurement* & *Best Part Collection* as instructor; 2024 *Best Wiki* nominee as student leader
* 2024 John Locke Institute Global Essay Prize — *Finalist* & *Merit* (Economics)
* 2024 Goi Peace Foundation International Essay Contest for Young People — *Finalist* (top 100 of 10,233)
* 2024 ARML — *National Silver* · 2024 Purple Comet! Math Meet — China *2nd*, global 16th · 2024 Johns Hopkins Math Tournament — Team *Silver*, Power & Relay Round *Bronze*
* 2023 British Biology Olympiad — *Global Gold* · 2022 UKBC Intermediate Biology Olympiad — *Bronze*
* 2023 COMAP HiMCM — *Honorable Mention* · 2022 Junior Canadian Chemistry Olympiad — China *Gold*, global *Bronze* · 2022 Berkeley Math Tournament — *Honorable Mention*
* 2022 China Thinks Big — research paper accepted to the Digital Library collection
* AP Scholar (2023) & AP Scholar with Distinction (2024, 2025) · 2019 FIRST Tech Challenge — Beijing regional *first prize*

Activities
======
* **Mathematical Modeling Challenge** (COMAP, MAA & AMS), *team leader* — *Jan 2025 – present*
  * 2026 MCM Honorable Mention; 2025 IMMC Outstanding (Greater China) and Meritorious (International). Built MILP scheduling models with `PuLP` and typeset both papers in LaTeX.
* **Synthetic Biology, [iGEM](https://igem.org/)** — BNDS-China, *student leader* (2024) and *instructor* (2025–2026) — *Oct 2022 – present*
  * Gold medal and top 10 in 2023–2025. Developed a programmable probiotic platform against gut dysbiosis (2024) and one for feline gut health (2025); built the dry-lab modeling. See the [project page](/portfolio/2-igem-bnds-china/).
* **Rhino-Bird Science Talent Advancement Program** (BNRist, Tsinghua & Tencent) — *Apr – Aug 2024*
  * 30-hour research training; implemented the attention mechanism in PyTorch; researched dynamic game theory in college admissions.
* **Jingwan Applied Math Summer Camp** (Beijing Normal University), *team leader* — *Jul – Aug 2023*
  * Modeled honeybee colony collapse disorder from hive data, leading a team of three.
* **School clubs**, Beijing National Day School — *Sep 2022 – Jul 2025*
  * President of biology club *BioCamp*; co-founder of math club *MathCorner*; vice president of the origami club; school badminton team.
* **Volunteering** — *Sep 2023 – present*
  * MBZUAI HCI Symposium 2025 (event operations); IUCN World Conservation Congress 2025 at ADNEC, Abu Dhabi; Beijing environmental-protection volunteer (2024); co-founder of a dyslexia support group.

Skills and interests
======
* **Coding:** Python, Rust, TypeScript; deep learning with PyTorch. **Writing:** Markdown, Typst, LaTeX. **Visuals:** Manim, PowerPoint, Photoshop.
* **AI tooling:** Anthropic certificates (Jan 2026) in Building with the Claude API, Claude Code in Action, Model Context Protocol, and AI Fluency; AWS AI Practitioner Learning Plan (Apr 2026).
* **Lab:** SnapGene, Benchling, AlphaFold, AutoDock Vina, PyMOL.
* **Languages:** Mandarin (native), English (fluent); learning French and Japanese.
* Sketching, tennis, running (70 km+ a month), fencing, badminton, origami, and oil painting.
