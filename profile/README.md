# ML Engineering Curriculum

> A hands-on curriculum for **building the models themselves** — data curation, training pipelines, fine-tuning, preference optimization (RLHF/DPO), pretraining at scale, and the evaluation that proves a model got better.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](https://github.com/orgs/ml-engineering-curriculum/discussions)

## ⚠️ AI-Generated Content Disclaimer

> The content in these repositories is generated with AI assistance and undergoes ongoing human review. It may contain errors or outdated information. Treat it as a learning resource: cross-reference official docs, test code in a safe environment, and report issues via GitHub Issues or Discussions.

## 🎯 Overview

This org is the **ML engineering** vertical of a four-part curriculum family: it teaches how to *build and train models* — going from your first reproducible fine-tuning run to leading a frontier-scale pretraining program. It sits one direction over from [AI Engineering](https://github.com/ai-engineering-curriculum) (which builds *with* models): here you produce the models others consume. Every role has a paired **learning** repository (modules, lecture chapters, exercises, quizzes) and a **solutions** repository with reference walkthroughs.

## 📚 Role Ladder

| Role | Level | Focus | Repositories |
|------|-------|-------|--------------|
| **Machine Learning Engineer** | Entry (L20) | Data prep & curation, training pipelines, supervised fine-tuning, reproducibility, experiment tracking | [📘 Learning](https://github.com/ml-engineering-curriculum/ml-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/ml-engineer-solutions) |
| **Applied ML Engineer** | Build (L30) | Fine-tuning (LoRA/QLoRA/full), eval-harness design, preference optimization (DPO), dataset engineering | [📘 Learning](https://github.com/ml-engineering-curriculum/applied-ml-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/applied-ml-engineer-solutions) |
| **ML Research Engineer** | Staff/Lead (L40) | Pretraining at scale, distributed-training strategy, scaling laws, architecture & data ablations, RLHF systems | [📘 Learning](https://github.com/ml-engineering-curriculum/ml-research-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/ml-research-engineer-solutions) |
| **Foundation Model Engineer** | Frontier (L48) | End-to-end model programs, frontier-scale pretraining, alignment pipelines, model release & evaluation | [📘 Learning](https://github.com/ml-engineering-curriculum/foundation-model-engineer-learning) · [✅ Solutions](https://github.com/ml-engineering-curriculum/foundation-model-engineer-solutions) |

> The distributed-training **infrastructure** (GPU clusters, NCCL, schedulers, checkpointing) lives in the [AI Infrastructure Curriculum](https://github.com/ai-infra-curriculum). This org owns the *modeling* question — "did the training run produce a better model?" — not the cluster operations. The two cross-reference: infra's distributed-training modules are the recommended on-ramp into the L40 research track.

## 🔗 Curriculum Family

This is one of four sibling orgs covering the full landscape of AI work — organized by what you *do* relative to a model:

- **[AI Infrastructure Curriculum](https://github.com/ai-infra-curriculum)** — *run* the platforms (Kubernetes, GPUs, training infra, serving, MLOps, IaC, SRE).
- **ML Engineering Curriculum** *(you are here)* — *build & train* the models (data, fine-tuning, pretraining, RLHF, evals).
- **[AI Engineering Curriculum](https://github.com/ai-engineering-curriculum)** — *build with* the models (agentic apps, RAG, multi-agent systems).
- **[AI Governance Curriculum](https://github.com/ai-governance-curriculum)** — *govern & assure* AI (security, compliance, evaluation, safety).

## 🤝 Contributing

Contributions welcome — fix broken links or stale references, add depth, improve exercise validation, or open a [Discussion](https://github.com/orgs/ml-engineering-curriculum/discussions).

---

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
