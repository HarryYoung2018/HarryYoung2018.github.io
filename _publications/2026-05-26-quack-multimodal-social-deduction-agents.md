---
title: "QUACK: Questioning, Understanding, and Auditing Communicated Knowledge in Multimodal Social Deduction Agents"
collection: publications
category: manuscripts
permalink: /publication/2026-quack-multimodal-social-deduction-agents
excerpt: 'Social deduction games are a popular testbed for reasoning and deception in LLM agents, but scoring only win rates cannot tell whether an agent’s words are grounded in what it actually saw and did. QUACK audits agents at three levels — outcomes, trajectories, and utterance-level consistency — and finds even the strongest VLM hallucinates 15.1% of its verifiable spatial claims.'
date: 2026-05-26
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2605.27068'
citation: 'Ye Yuan, Rui Song, Weien Li, et al. (including Yonghan Yang), and Xue Liu. (2026). &quot;QUACK: Questioning, Understanding, and Auditing Communicated Knowledge in Multimodal Social Deduction Agents.&quot; <i>arXiv:2605.27068</i>.'
---

**Status:** preprint on arXiv · **My role:** contributing author.

<p>
  <a href="https://arxiv.org/abs/2605.27068" class="btn btn--info">Paper (arXiv)</a>
  <a href="https://github.com/AAAAA-Academia-Attractions/QUACK" class="btn btn--info">Code</a>
</p>

## Summary

Social deduction games are a popular way to probe reasoning, deception, coordination, and belief
modeling in LLM agents — but most environments score only **game outcomes** such as win rate, and
most are **text-only**. That makes it impossible to tell whether an agent's language is actually
*grounded* in what it perceived and did.

**QUACK** is an open-source environment and evaluation framework that audits grounding directly.
Agents navigate configurable **graph-based maps under partial observability**, see rendered global
and local views, complete location-bound tasks, discuss freely, and vote under hidden-role
adversarial incentives.

The core **Statement Verification Pipeline** reconstructs each agent's ground-truth trajectory from
engine logs and checks *every* discussion claim against it, automatically flagging:

- **spatial hallucination** — claims about places the agent never observed
- **unsupported accusation** — accusations with no grounded evidence
- **deception collapse** and **language–action inconsistency**

**Finding:** across three frontier VLMs in both homogeneous and cross-model adversarial settings,
even the strongest agent **hallucinates 15.1% of its verifiable spatial claims** and makes **over
half of its accusations without grounded evidence.**

Work with the [Mila](https://mila.quebec/en) group led by [Ye Yuan](https://stevenyuan666.github.io/)
and [Prof. Xue (Steve) Liu](https://cs.mcgill.ca/~xueliu/site/intro.html).
