# Data Synthesis for LLMs, World Models & Long-Horizon Agents

A curated collection of recent and influential work on **synthetic data for large language models, world models, and long-horizon agents**.

This repository tracks papers, open-source projects, datasets, benchmarks, and practical resources related to:

- Synthetic instruction and reasoning data
- Agent trajectory synthesis
- Executable environment generation
- World models for agent training
- Expert-to-model knowledge distillation
- Self-improving and self-evolving data-generation pipelines
- Synthetic data for long-horizon planning and tool-use agents

---

## Surveys & Guides

| Date | Resource | Project / Source | Description | Venue |
| --- | --- | --- | --- | --- |
| 2026.05 | [Synthetic Data for LLM Training: Decision Guide 2026](https://www.digitalapplied.com/blog/synthetic-data-generation-llm-training-decision-guide-2026) | [Website](https://www.digitalapplied.com/blog/synthetic-data-generation-llm-training-decision-guide-2026) | Provides a practical decision framework for synthetic-data generation and discusses model-collapse risks, emphasizing the importance of retaining and accumulating real data alongside synthetic data. | *Digital Applied* |

---

## General-Purpose Synthetic Data


### Methods

| Date | Paper | Project / Code | Description | Venue |
| --- | --- | --- | --- | --- |
| 2022.12 | [Self-Instruct: Aligning Language Models with Self-Generated Instructions](https://arxiv.org/abs/2212.10560) | [GitHub](https://github.com/yizhongw/self-instruct) | Establishes the **Self-Instruct** paradigm: bootstrap a large instruction-tuning dataset from a small set of seed tasks using the language model itself, followed by filtering and refinement. | *ACL 2023* |
| 2023.04 | [WizardLM: Empowering Large Language Models to Follow Complex Instructions](https://arxiv.org/abs/2304.12244) | [GitHub](https://github.com/nlpxucan/WizardLM) | Introduces **Evol-Instruct**, which automatically evolves simple instructions into increasingly complex ones to improve instruction-following capabilities. | *ICLR 2024* |
| 2023.06 | [Textbooks Are All You Need](https://arxiv.org/abs/2306.11644) | [Phi-1](https://huggingface.co/microsoft/phi-1) | Demonstrates that carefully curated, textbook-quality synthetic data can enable relatively small language models to achieve strong coding and reasoning performance. | *arXiv* |
| 2026.03 | [Reasoning-Driven Synthetic Data Generation and Evaluation](https://arxiv.org/abs/2603.29791) | [Google Research](https://research.google/pubs/reasoning-driven-synthetic-data-generation-and-evaluation/) | Introduces **Simula**, a seedless and reasoning-driven framework that reframes synthetic-data generation as **dataset-level mechanism design**. Instead of optimizing individual samples in isolation, Simula explicitly controls dataset-wide **coverage, local diversity, complexity, and quality** through hierarchical taxonomy construction, diversification, complexification, and critic-based quality control, enabling synthetic datasets to be designed around downstream model and domain requirements. | *TMLR 2026* |


---


## Agents, World Models & Long-Horizon Data

| Date | Paper | Project / Code | Description | Venue |
| --- | --- | --- | --- | --- |
| 2025.10 | [AgentFrontier: Expanding the Capability Frontier of LLM Agents with ZPD-Guided Data Synthesis](https://arxiv.org/abs/2510.24695) | [DeepResearch](https://github.com/Alibaba-NLP/DeepResearch) | Introduces **ZPD-guided data synthesis**, reframing difficulty calibration as the primary mechanism for selecting high-value agent training data. The AgentFrontier Engine uses an adversarial **Less Knowledgeable Peer (LKP) vs. More Knowledgeable Other (MKO)** calibration: tasks that a base model cannot solve independently but a stronger tool-augmented agent can solve are retained as lying within the model's **Zone of Proximal Development (ZPD)**. Combined with iterative agentic refinement and automated verification, this targets the model's evolving capability frontier rather than average task difficulty. AgentFrontier-30B-A3B achieves **28.6% on Humanity's Last Exam**, **93.4% on ZPD Exam-v1**, and state-of-the-art results on R-Bench-T and xBench-ScienceQA. | *ICLR 2026* |
| 2026.01 | [From Self-Evolving Synthetic Data to Verifiable-Reward RL: Post-Training Multi-turn Interactive Tool-Using Agents](https://arxiv.org/abs/2601.22607) | [GitHub](https://github.com/inclusionAI/AReaL) | Unifies **self-evolving synthetic data generation with verifier-based RL** for multi-turn interactive tool-using agents. Its EigenData/AReaL-SEA pipeline synthesizes tool-grounded dialogues together with executable per-instance verifiers, then applies SFT followed by GRPO-style RL with trajectory-level rewards and dynamic filtering. | *arXiv / Submitted to ICML 2026* |
| 2026.02 | [Agent World Model: Infinity Synthetic Environments for Agentic Reinforcement Learning](https://arxiv.org/abs/2602.10090) | [GitHub](https://github.com/Snowflake-Labs/agent-world-model) | Introduces **Agent World Model (AWM)**, a fully synthetic environment-generation pipeline that scales to 1,000 executable, database-backed environments for multi-turn tool-use and agentic reinforcement learning. | *ICML 2026* |
| 2026.04 | [Agent-World: Scaling Real-World Environment Synthesis for Evolving General Agent Intelligence](https://arxiv.org/abs/2604.18292) | [Project](https://agent-tars-world.github.io/-/) | Builds a self-evolving training arena that discovers real-world tool ecosystems, synthesizes verifiable tasks, identifies agent capability gaps, and continuously generates new training environments and tasks. | *arXiv* |
| 2026.06 | [Autodata: An Agentic Data Scientist to Create High Quality Synthetic Data](https://arxiv.org/abs/2606.25996) | [Project](https://facebookresearch.github.io/RAM/blogs/autodata/) | Treats synthetic-data generation as an autonomous data-science process. Its **Agentic Self-Instruct** formulation iteratively creates, evaluates, analyzes, and improves datasets, while also meta-optimizing the data-generation agent itself. | *arXiv* |
| 2026.07 | [LeAct: Learning to Reason from Expert Actions](https://arxiv.org/abs/2607.21856) | — | Treats expert systems such as game solvers, planners, and other algorithmic experts as reasoning teachers, enabling latent reasoning supervision to be recovered from expert actions. | *arXiv* |
| 2026.07 | [Environment-free Synthetic Data Generation for API-Calling Agents](https://arxiv.org/abs/2607.16900) | [Apple Research](https://machinelearning.apple.com/research/environment-free) | Generates multi-turn API-agent trajectories without constructing executable environments. An LLM acts as an on-the-fly stateful world model for synthetic trajectory generation. | *arXiv* |


