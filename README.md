# Data  Synthsis for LLMs, World Models & Long-Horizon Agents

This repository tracks and organizes the latest, most relevant work in synthetic data for LLMs, world models, and long-horizon agentic data synthesis—aggregating papers, tools, datasets, blogs, and other practical resources into a single, searchable hub.

## **Surveys**

| Date | Paper | Link | Desc | Venue |
| --- | --- | --- | --- | --- |
| 2026.05 | [Synthetic Data for LLM Training: Decision Guide 2026](https://www.digitalapplied.com/blog/synthetic-data-generation-llm-training-decision-guide-2026) | [](https://www.digitalapplied.com/blog/synthetic-data-generation-llm-training-decision-guide-2026) | address the provable phenomenon of "model collapse"; prove that the fix is accumulating real data alongside synthetic data, where retaining even a 10% original real-data seed dramatically limits performance degradation.

 | *Digital Applied* |

---

## **General tasks**

### Method

| Date | Paper | Link | Desc | Venue |
| --- | --- | --- | --- | --- |
| 2022.12 | [Self-Instruct: Aligning Language Models with Self-Generated Instructions](https://arxiv.org/abs/2212.10560) | [](https://www.google.com/search?q=%5Bhttps%3A%2F%2Fgithub.com%2Fyizhongw%2Fself-instruct%5D%28https%3A%2F%2Fgithub.com%2Fyizhongw%2Fself-instruct%29) | establish paradigm for generating a large number of instructions from a small number of seeds.

 | *ACL 2023* |
| 2023.04 | [WizardLM: Empowering Large Language Models to Follow Complex Instructions](https://www.google.com/search?q=https://arxiv.org/abs/2304.12244) | [](https://www.google.com/search?q=%5Bhttps%3A%2F%2Fgithub.com%2Fnlpxucan%2FWizardLM%5D%28https%3A%2F%2Fgithub.com%2Fnlpxucan%2FWizardLM%29) | propose Evol-Instruct to automatically evolve simple instructions into complex ones for enhancing LLM instruction-following.
 | *ICLR 2024* |
| 2023.06 | [Textbooks Are All You Need](https://www.google.com/search?q=https://arxiv.org/abs/2306.11644) | [](https://www.google.com/search?q=%5Bhttps%3A%2F%2Fhuggingface.co%2Fmicrosoft%2Fphi-1%5D%28https%3A%2F%2Fhuggingface.co%2Fmicrosoft%2Fphi-1%29) | demonstrate that highly curated, "textbook-quality" synthetic data enables smaller language models to achieve performance rivaling much larger counterparts.
 | *arXiv* |

---
## **Multi-Agents & World Models**

| Date | Paper | Link | Desc | Venue |
| --- | --- | --- | --- | --- |
| 2026.02 | [Agent World Model: Infinity Synthetic Environments for Agentic Reinforcement Learning](https://arxiv.org/abs/2602.10090) | [](https://www.google.com/search?q=%5Bhttps%3A%2F%2Fgithub.com%2FSnowflake-Labs%2Fagent-world-model%5D%28https%3A%2F%2Fgithub.com%2FSnowflake-Labs%2Fagent-world-model%29) | propose generating executable worlds rather than samples by synthesizing 1,000 code-driven, database-backed environments to scale agentic RL and improve out-of-distribution generalization.
 | *ICML 2026* |
| 2026.04 | [Agent-World: Scaling Real-World Environment Synthesis for Evolving General Agent Intelligence](https://arxiv.org/abs/2604.18292) | [](https://www.google.com/search?q=%5Bhttps%3A%2F%2Fagent-tars-world.github.io%2F-%2F%5D%28https%3A%2F%2Fagent-tars-world.github.io%2F-%2F%29) | discover executable environments and synthesize verifiable tasks to train agents, dynamically generating new tasks based on capability gaps for agent-environment co-evolution.
 | *arXiv* |
| 2026.06 | [Autodata: An agentic data scientist to create high quality synthetic data](https://arxiv.org/abs/2606.25996) | [](https://www.google.com/search?q=%5Bhttps%3A%2F%2Ffacebookresearch.github.io%2FRAM%2Fblogs%2Fautodata%2F%5D%28https%3A%2F%2Ffacebookresearch.github.io%2FRAM%2Fblogs%2Fautodata%2F%29) | treat the data-generation agent as an autonomous data scientist via Agentic Self-Instruct, meta-optimizing it to maximize the downstream value of the entire generated dataset rather than just individual examples.
 | *arXiv* |
| 2026.07 | [LeAct: Learning to Reason from Expert Actions](https://arxiv.org/abs/2607.21856) |  | propose treating expert systems as reasoning teachers through backward generation, $\Delta$-scoring, and expert-policy forcing.
 | *arXiv* |
| 2026.07 | [Environment-free Synthetic Data Generation for API-Calling Agents](https://www.google.com/search?q=%23) |  | introduce the ESAT pipeline that uses an LLM as an on-the-fly digital world model by ingesting API specifications to simulate stateful environments and generate multi-turn trajectories without computationally expensive executable sandboxes.

 | *arXiv* |

---
