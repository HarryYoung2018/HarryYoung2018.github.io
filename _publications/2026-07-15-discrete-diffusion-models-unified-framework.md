---
title: "Discrete Diffusion Models: A Unified Framework from Tokenization to Generation"
collection: publications
category: manuscripts
permalink: /publication/2026-discrete-diffusion-survey
excerpt: 'A survey arguing that in discrete diffusion, tokenization is not preprocessing but the primary design axis: it fixes the geometry of corruption, the difficulty of denoising, controllability, and cost. Transition-matrix, masked/absorbing-state, and score/ratio-based models all emerge as instances of one four-component framework.'
date: 2026-07-15
venue: 'arXiv preprint · under review at TMLR'
paperurl: 'https://arxiv.org/abs/2607.13431'
citation: 'Ye Yuan, Weien Li, Rui Song, et al. (including Yonghan Yang), Dawn Song, Philip S. Yu, and Xue Liu. (2026). &quot;Discrete Diffusion Models: A Unified Framework from Tokenization to Generation.&quot; <i>arXiv:2607.13431</i>. Under review at TMLR.'
---

**Status:** preprint on arXiv, under review at **TMLR** · **My role:** contributing author (13th of 23).

<p>
  <a href="https://arxiv.org/abs/2607.13431" class="btn btn--info">Paper (arXiv)</a>
  <a href="https://github.com/AAAAA-Academia-Attractions/Discrete-Diffusion" class="btn btn--info">Curated paper list</a>
</p>

## Summary

In continuous diffusion, Gaussian noise gives a natural geometry. In discrete domains — text, code,
proteins, molecules, action sequences — there is no obvious notion of a "small perturbation". The
survey's central thesis is that **tokenization is the primary design axis**: how the discrete state
space is built determines the topology of corruption, how hard denoising is, and downstream
controllability, validity, and cost.

- A **tokenization-centric lens** over three token families: semantic (subwords), quantized
  (VQ codebooks), and natural alphabets (amino acids, nucleotides, atom types).
- A **four-component framework** — corruption operator, denoiser parameterization, training
  objective, sampler — under which D3PM, masked diffusion, SEDD, and discrete flow matching emerge as
  special cases, often differing in a single component.
- A **cross-domain map** spanning text and code, multimodal generation, proteins, genomics,
  molecules and graphs, planning and agents, and tabular data.

Led by Ye Yuan in [Prof. Steve Liu's Cyber-Physical Intelligence Lab](https://cpil-lab.github.io/),
with collaborators across nine institutions and guidance from Prof. Dawn Song and Prof. Philip Yu.
