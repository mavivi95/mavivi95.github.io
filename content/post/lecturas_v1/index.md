---
title: "📚 Recommended Readings on Cooperative AI (Vol. 1)"

subtitle: "Five papers on cooperation, social intelligence, preference learning, and multi-agent evaluation"

summary: "A selection of foundational and recent papers that have shaped how I think about cooperation, mixed-motive environments, reward learning, LLM-based agents, and resilience in multi-agent systems."

date: 2025-10-22
lastmod: 2026-09-18

tags:
  - Cooperative AI
  - Multi-Agent Systems
  - Large Language Models
  - Preference Learning
  - Social Dilemmas
  - Research Reflections

featured: true

image:
  filename: lecturas.png
  focal_point: center
  preview_only: true

authors:
  - admin
---

Cooperative AI is not only a technical challenge. It also raises a broader question: how can we design artificial agents that pursue their objectives while supporting cooperation and collective welfare?

This question becomes especially important in mixed-motive systems, where individual and collective interests are neither fully aligned nor entirely opposed. In these environments, agents must learn how to coordinate, communicate, adapt to different partners, and respond when cooperation is threatened.

In this first volume, I share five papers that have influenced how I think about cooperative AI, social dilemmas, preference learning, LLM-based agents, and cooperative resilience. Together, they provide a useful path from the general research agenda to concrete methods and experimental environments.

#### 1. 🧭 [Open Problems in Cooperative AI](https://arxiv.org/abs/2012.08630) — Dafoe et al., 2021

This paper presents a broad research agenda for Cooperative AI. It argues that artificial intelligence should explicitly study problems in which agents can improve their outcomes through cooperation.

The authors organize the field around several major challenges, including cooperative capabilities, communication, commitment, institutional design, human–AI interaction, and cooperation among artificial agents. The paper also connects ideas from multi-agent systems, game theory, social choice, behavioral science, and AI alignment.

💡 **Why read it:** It is one of the best starting points for understanding Cooperative AI as a research field. Rather than proposing a single algorithm, it maps the central questions and explains why cooperation should be treated as a distinct scientific problem.

📌 **What to focus on:** The distinction between building agents that can cooperate and designing mechanisms or institutions that make cooperation more likely.

---

#### 2. 🤖 [Evaluating Generalization Capabilities of LLM-Based Agents in Mixed-Motive Scenarios Using Concordia](https://proceedings.neurips.cc/paper_files/paper/2025/hash/d0251bbbc0288f241b878775ba1735dc-Abstract-Datasets_and_Benchmarks_Track.html) — Smith et al. and Concordia Contest Participants, 2025

LLM-based agents can communicate fluently and appear socially capable, but this does not necessarily mean that they can cooperate reliably across new partners and situations.

This NeurIPS 2025 paper introduces a methodology for evaluating LLM-based agents in zero-shot, mixed-motive environments using Concordia, a natural-language multi-agent simulation framework. The agents are evaluated across diverse scenarios involving negotiation, coordination, collective action, persuasion, and norm enforcement.

The results reveal important gaps between fluent social interaction and robust cooperative generalization. In particular, current agents can struggle in situations that require persuasion, adaptation to unfamiliar partners, or the enforcement of social norms.

This work is especially meaningful to me because I participated in the Concordia Contest and contributed to the collective evaluation effort behind the paper.

💡 **Why read it:** It demonstrates why evaluating an agent in a single environment is insufficient. Cooperative intelligence requires generalization across different social situations, objectives, and interaction partners.

📌 **What to focus on:** The experimental definition of general cooperative intelligence and the distinction between performing well in one scenario and generalizing across multiple mixed-motive contexts.

---

#### 3. 🎯 [Extrapolating Beyond Suboptimal Demonstrations via Inverse Reinforcement Learning from Observations](https://proceedings.mlr.press/v97/brown19a.html) — Brown et al., 2019

This paper introduces **Trajectory-ranked Reward EXtrapolation (T-REX)**, a method for learning reward functions from approximately ranked demonstrations.

Traditional imitation learning often assumes that demonstrations are close to optimal. T-REX takes a different perspective: even when demonstrations are imperfect, their relative quality can provide useful information about the underlying objective.

Instead of directly reproducing demonstrated behavior, the method learns a reward function from preferences over trajectories. Once the reward has been inferred, a reinforcement learning agent can potentially discover a policy that performs better than the original demonstrations.

This paper has been particularly relevant to my research on preference-based reward learning and cooperative resilience. It provides an important methodological foundation for using ranked trajectories to infer which behaviors should be encouraged in multi-agent environments.

💡 **Why read it:** It offers a clear example of how preferences and rankings can provide supervision when an explicit reward function is difficult to specify.

📌 **What to focus on:** How trajectory rankings are transformed into a learned reward function, and why reward inference can allow an agent to outperform imperfect demonstrations.

---

#### 4. 🏘️ [Generative Agents: Interactive Simulacra of Human Behavior](https://dl.acm.org/doi/10.1145/3586183.3606763) — Park et al., 2023

This paper introduces generative agents: LLM-based computational agents designed to produce believable individual and social behavior.

The proposed architecture combines three central processes:

- **Memory**, which stores the agent’s experiences.

- **Reflection**, which transforms individual observations into higher-level conclusions.

- **Planning**, which uses memories and reflections to guide future behavior.

The authors evaluate the architecture in a sandbox environment populated by 25 agents. From relatively simple initial conditions, the agents produce emergent social behaviors such as forming relationships, sharing information, coordinating activities, and organizing a social event.

💡 **Why read it:** It provides an influential architecture for building LLM-based agents with memory, reflection, and planning. It also illustrates how individual cognitive mechanisms can produce collective patterns.

📌 **What to focus on:** The interaction between memory retrieval, reflection, and planning, as well as the evaluation of whether the resulting behavior is genuinely coherent and socially meaningful.

⚠️ **A useful critical question:** Believable behavior is not necessarily cooperative, robust, or human-equivalent behavior. This distinction is essential when using generative agents to study social systems.

---

#### 5. 🍎 [Scalable Evaluation of Multi-Agent Reinforcement Learning with Melting Pot](https://proceedings.mlr.press/v139/leibo21a.html) — Leibo et al., 2021

Melting Pot is an evaluation suite designed to study generalization in multi-agent reinforcement learning. It contains sequential social dilemmas in which agents must interact over time while facing tensions between individual incentives and collective outcomes.

The suite evaluates more than task performance. It examines whether agents can generalize to new social partners and unfamiliar configurations after training. Its environments represent challenges such as resource sharing, coordination, reciprocity, competition, and collective action.

One of its best-known environments is **Commons Harvest**, which models a tragedy-of-the-commons problem. Agents collect apples from a renewable shared resource, but excessive consumption can prevent regeneration and lead to collective collapse.

Melting Pot has been central to my own research because it provides environments in which cooperative resilience can be studied under disruptions. It allows us to evaluate not only whether agents cooperate under stable conditions, but also whether they can preserve collective welfare when environmental or behavioral conditions change.

💡 **Why read it:** It connects theoretical questions about cooperation with concrete and reproducible multi-agent environments.

📌 **What to focus on:** The evaluation protocol for social generalization and the difference between learning a successful policy and learning a policy that remains effective with unfamiliar partners.

---

#### 🔗 How these papers connect

These five papers address different layers of Cooperative AI:

1. **Open Problems in Cooperative AI** defines the broader research agenda.

2. **The Concordia evaluation** asks whether LLM-based agents can generalize across mixed-motive social situations.

3. **T-REX** shows how preferences over trajectories can be used to infer reward functions.

4. **Generative Agents** proposes an architecture for socially situated LLM-based agents.

5. **Melting Pot** provides controlled environments for evaluating cooperation and social generalization.

Together, they also reveal an important distinction: an agent can communicate fluently, imitate believable behavior, or perform well in a particular task without necessarily being robustly cooperative.

For me, this distinction motivates the study of **cooperative resilience**: the capacity of a multi-agent system to preserve collective welfare before, during, and after disruptions.

#### 📖 Suggested reading order

If you are new to the field, I recommend starting with:
  1. **Open Problems in Cooperative AI**, to understand the overall research landscape.
  
  2. **Melting Pot**, to see how cooperation can be evaluated experimentally.
  
  3. **The Concordia paper**, to understand the challenges of evaluating LLM-based social agents.
  
  4. **Generative Agents**, to explore memory, reflection, and planning in LLM agents.
  
  5. **T-REX**, if you are interested in reward inference and preference-based learning.

#### 🌱 Closing thoughts

Cooperative AI brings together technical and social questions. It requires us to think not only about what an individual agent can achieve, but also about how multiple agents interact, how collective outcomes emerge, and how cooperation can be sustained when conditions change.

These papers have helped me connect ideas from multi-agent reinforcement learning, large language models, preference learning, social dilemmas, and resilience. They also show how much remains open: defining meaningful evaluation criteria, understanding generalization, learning appropriate incentives, and designing agents that support collective welfare in uncertain environments.

This is only the first volume. Future editions will include additional work on cooperative resilience, human–AI interaction, multi-agent safety, incentive design, and collective intelligence.