---
title: "BioXArena: Benchmarking LLM Agents on Multi-Modal Biomedical Machine Learning Tasks"
collection: publications
category: manuscripts
permalink: /publication/2026-bioxarena-biomedical-ml-agent-benchmark
excerpt: 'A biomedical ML coding benchmark testing whether agents can write task-specific model-building code for heterogeneous, often multi-modal biomedical data. 76 end-to-end tasks across 9 domains, each with hidden labels, held-out graders, and biology-aware metrics on a common 0–1 scale — agents must write runnable code, train models, and submit predictions on private test samples.'
date: 2026-05-15
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2605.15766'
citation: 'Loka Li, Duzhen Zhang, Xingbo Du, et al. (including Yonghan Yang), Bin Zhang, and Le Song. (2026). &quot;BioXArena: Benchmarking LLM Agents on Multi-Modal Biomedical Machine Learning Tasks.&quot; <i>arXiv:2605.15766</i>.'
---

**Status:** preprint on arXiv · **My role:** key contributions to the formulation of the paper —
shaping how the benchmark was framed, which task families it should cover, and how agent
performance is argued for and presented.

<p>
  <a href="https://arxiv.org/abs/2605.15766" class="btn btn--info">Paper (arXiv)</a>
</p>

## Summary

**BioXArena** asks a harder question than most agent benchmarks: not whether an agent can *answer*
a biomedical question, but whether it can **build a working model** for one. Agents must write
runnable code, train a model on a real dataset, and submit predictions for held-out private test
samples.

- **76 end-to-end tasks** across **9 domains**: sequence, single-cell, structure, network biology,
  chemical biology, perturbation dynamics, phenotype–disease, imaging, and text-integrated tasks.
- Each task is curated from primary sources into a **unified public capsule** with **hidden labels**
  and **held-out graders**.
- **Biology-aware metrics** are normalized onto a common 0–1 scale, so scores are comparable across
  very different data modalities.

Work with the [GenBio AI](https://genbio.ai/) group under [Prof. Le Song](https://dasongle.github.io/).
