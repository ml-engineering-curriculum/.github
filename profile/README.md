# ML Engineering Curriculum

## ⚠️ AI-Generated Content Disclaimer

> The content in these repositories is generated with AI assistance and undergoes ongoing human review. It may contain errors or outdated information. Treat it as a learning resource: cross-reference official docs, test code in a safe environment, and report issues via GitHub Issues or Discussions.

---

> A hands-on, role-based curriculum for engineers who build and train machine-learning models — from your first production model to principal-level ML strategy.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](https://github.com/orgs/ml-engineering-curriculum/discussions)
[![Repositories: 18](https://img.shields.io/badge/repositories-18-blue.svg)](https://github.com/orgs/ml-engineering-curriculum/repositories)

🌐 **Website:** [ml-engineering-curriculum.github.io](https://ml-engineering-curriculum.github.io/) · part of the [AI Career Curriculum](https://ai-curriculum-project.github.io/)

## 🎯 Overview

This org covers **ML engineering** — *building and training* the models: data pipelines, classical and deep learning, fine-tuning and alignment, evaluation, distributed training, and the senior-to-principal work of setting ML architecture and strategy. Every role track has a paired **learning** repository (modules, lecture chapters, exercises) and a **solutions** repository with reference walkthroughs.

**At a glance:**

- 🏢 **18 curriculum repositories** (9 learning + 9 solutions)
- 📚 **9 role tracks**
- 🧭 Ladder runs from **ML Engineer (L20)** to **Principal ML Engineer (L48)**, with four specialist tracks in between

## 🔗 Curriculum Family

One of 6 sibling orgs in the **AI Career Curriculum ecosystem**, organized by what you *do* relative to a model:

- **[AI Infrastructure Curriculum](https://github.com/ai-infra-curriculum)** — *run* the platforms (Kubernetes, GPUs, training infra, serving, MLOps, IaC, SRE). ([site](https://ai-infra-curriculum.github.io/))
- **ML Engineering Curriculum** *(you are here)* — *build & train* the models (data, fine-tuning, pretraining, RLHF, evals).
- **[AI Engineering Curriculum](https://github.com/ai-engineering-curriculum)** — *build with* the models (agentic apps, RAG, multi-agent systems). ([site](https://ai-engineering-curriculum.github.io/))
- **[AI Governance Curriculum](https://github.com/ai-governance-curriculum)** — *govern & assure* AI (security, compliance, evaluation, safety). ([site](https://ai-governance-curriculum.github.io/))
- **[AI Startup Curriculum](https://github.com/ai-startup-curriculum)** — *turn it into a company* — the startup operating school for technical founders (functional curricula × role pathways × stages). ([site](https://ai-startup-curriculum.github.io/))
- **[AI Workforce Curriculum](https://github.com/ai-workforce-curriculum)** — *work alongside* the models (AI-assisted engineering, analysis, product, and team leadership). ([site](https://ai-workforce-curriculum.github.io/))

---

## 📚 Learning Tracks

### 🟢 Foundation (L20)

| Role | Focus | Repositories |
|------|-------|--------------|
| **Machine Learning Engineer** | ML foundations, data for ML, classical & deep learning, experiment tracking, deployment, drift monitoring | [📘 Learning](https://github.com/ml-engineering-curriculum/ml-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/ml-engineer-solutions) |

### 🔵 Specialist & Senior (L30–L35)

| Role | Focus | Repositories |
|------|-------|--------------|
| **AI Data Engineer** | Data sourcing & licensing, curation & dedup, labeling ops, synthetic data, contamination checks, dataset versioning | [📘 Learning](https://github.com/ml-engineering-curriculum/ai-data-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/ai-data-engineer-solutions) |
| **Fine-Tuning Engineer** | SFT data, PEFT (LoRA/QLoRA), preference optimization, safety tuning, distributed fine-tuning, quantization | [📘 Learning](https://github.com/ml-engineering-curriculum/fine-tuning-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/fine-tuning-engineer-solutions) |
| **Model Evaluation Engineer** | Benchmarks, LLM eval harnesses, LLM-as-judge, human eval, agent & safety evals, production eval | [📘 Learning](https://github.com/ml-engineering-curriculum/model-evaluation-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/model-evaluation-engineer-solutions) |
| **NLP Engineer** | Tokenization, classical NLP, classification, extraction, QA, summarization, machine translation | [📘 Learning](https://github.com/ml-engineering-curriculum/nlp-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/nlp-engineer-solutions) |
| **Senior Machine Learning Engineer** | ML systems architecture, production LLM integration, experimentation at scale, ML SLOs, technical leadership | [📘 Learning](https://github.com/ml-engineering-curriculum/senior-ml-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/senior-ml-engineer-solutions) |
| **Training Pipeline Engineer** | Distributed training, data pipelines at scale, cluster orchestration, checkpointing, elastic training, throughput | [📘 Learning](https://github.com/ml-engineering-curriculum/training-pipeline-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/training-pipeline-engineer-solutions) |

### ⭐ Staff & Principal (L40+)

| Role | Focus | Repositories |
|------|-------|--------------|
| **Staff Machine Learning Engineer** | Multi-team ML architecture, foundation-model training programs, ML platform strategy, capacity & TCO | [📘 Learning](https://github.com/ml-engineering-curriculum/staff-ml-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/staff-ml-engineer-solutions) |
| **Principal Machine Learning Engineer** | Org & industry ML strategy, north-star ML architecture, influence without authority, the technical bar | [📘 Learning](https://github.com/ml-engineering-curriculum/principal-ml-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/principal-ml-engineer-solutions) |

> Specialist tracks (fine-tuning, evaluation, NLP, training pipelines) branch from ML Engineer and can be taken in any order.

---

## 🚀 Quick Start

1. **Choose a track** from the table above, based on your experience and direction.
2. **Clone its repository:**

   ```bash
   git clone https://github.com/ml-engineering-curriculum/ml-engineer-learning.git
   cd ml-engineer-learning
   ```

3. **Start with the first module** and read its `README.md`.
4. **Work through the exercises** in each module.
5. **Check the paired solutions repository** for reference walkthroughs.

---

## 🛠️ Technologies Covered

- **Languages & frameworks:** Python, PyTorch, JAX
- **Distributed training:** FSDP, DeepSpeed, Megatron, NCCL, CUDA, Triton
- **Fine-tuning & alignment:** SFT, PEFT (LoRA/QLoRA), preference optimization, quantization
- **Orchestration:** Ray, Kubernetes, Slurm
- **Experiment tracking:** MLflow, Weights & Biases
- **Evaluation:** Benchmark harnesses, LLM-as-judge, human evaluation, red-team evals

---

## 📈 Career Progression

See the **[Career Progression Guide](https://github.com/ml-engineering-curriculum/.github/blob/main/CAREER_PROGRESSION.md)** for level descriptions, a skills matrix, promotion criteria, and specialist tracks.

---

## 🤝 Contributing

Contributions are welcome across the organization:

- Fix broken links, stale references, or inaccurate explanations
- Add depth to modules, exercises, or projects
- Improve validation for runnable exercises
- Report issues or ideas via [GitHub Discussions](https://github.com/orgs/ml-engineering-curriculum/discussions)
- Follow the `CONTRIBUTING.md` in the specific repository you want to improve

---

## 📜 License

Curriculum repositories are MIT-licensed unless noted otherwise. See the target repository's `LICENSE` file for authoritative terms.

---

## 📞 Support

- **Issues:** use the relevant repository's GitHub Issues
- **Discussions:** [organization discussions](https://github.com/orgs/ml-engineering-curriculum/discussions)
- **Docs:** [Career Progression](https://github.com/ml-engineering-curriculum/.github/blob/main/CAREER_PROGRESSION.md)

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
