# Career Progression Guide — ML Engineering

A career-ladder guide for the discipline of **building and training models** — data curation, training pipelines, supervised fine-tuning, preference optimization (RLHF/DPO), evaluation, experiment discipline, and pretraining at scale. This is one of five sibling curricula in the **AI Career Curriculum ecosystem**.

> **Status:** all eight roles — the four-rung core ladder and four specialist tracks — have authored learning content and reference solutions. Content is under ongoing human review.

## Career Ladder Overview

```
   ┌──────────────────────────────────────────────────────────┐
   │  L48  Principal Machine Learning Engineer   (15+ yrs)     │  ← frontier-scale programs
   ├──────────────────────────────────────────────────────────┤
   │  L40  Staff Machine Learning Engineer       (10–15 yrs)   │  ← pretraining & scaling
   ├──────────────────────────────────────────────────────────┤
   │  L30  Senior Machine Learning Engineer      (5–9 yrs)     │  ← advanced fine-tuning & eval
   ├──────────────────────────────────────────────────────────┤
   │  L20  Machine Learning Engineer             (0–4 yrs)     │  ← training pipelines & SFT
   └──────────────────────────────────────────────────────────┘
            (bottom = entry, top = most senior)
```

**Specialist tracks** branch off the core ladder: **Fine-Tuning Engineer**, **Model Evaluation Engineer**, and **NLP Engineer** (L30), and **Training Pipeline Engineer** (L35). See [Specialist Roles](#specialist-roles) below.

Years-of-experience bands are approximate signals, not hard gates. Demonstrated scope, ownership, and technical judgment matter more than tenure — strong practitioners move faster, and switching domains (e.g., infra → ML) can reset effective experience at a given rung.

## Level Descriptions

### L20 — Machine Learning Engineer

The entry rung. You own the mechanics of turning data into a trained, reproducible model.

- **Responsibilities:** Build and run training pipelines for well-scoped models; execute supervised fine-tuning (SFT) jobs; keep experiments reproducible and tracked; ship trained artifacts that meet a defined eval bar.
- **Representative work:** Fine-tune an open base model on a curated dataset; stand up a data-loading + tokenization pipeline; instrument runs with experiment tracking; reproduce a published result and document the delta.
- **Technical depth expected:** Training loops and optimizers; data curation and cleaning; SFT mechanics; reproducibility (seeds, environment pinning, deterministic data order); experiment tracking (e.g., Weights & Biases / MLflow); basic single-/multi-GPU training; reading and acting on training curves.

### L30 — Senior Machine Learning Engineer

You own model quality end-to-end and make the dataset and evaluation decisions that determine whether a model is actually good.

- **Responsibilities:** Drive advanced fine-tuning programs; design evaluation harnesses that catch real regressions; engineer datasets (sourcing, deduplication, mixing, quality filtering); mentor L20s on experiment discipline.
- **Representative work:** Run a DPO / preference-optimization pass and prove it improved the target behavior without regressions; build a multi-metric eval harness with held-out and adversarial sets; design a data-mixing strategy and ablate its components.
- **Technical depth expected:** Advanced fine-tuning (LoRA/QLoRA, full fine-tuning trade-offs); preference optimization (DPO, RLHF fundamentals, reward modeling); eval-harness design and metric selection; dataset engineering at scale; debugging silent quality regressions; cost/quality trade-off reasoning.

### L40 — Staff Machine Learning Engineer

You set training strategy across teams and operate at the scale where systems behavior dominates results.

- **Responsibilities:** Own pretraining and large-scale training strategy; design distributed-training architecture; run principled ablation programs; make scaling-law-informed bets on compute, data, and model size; resolve cross-team training-platform bottlenecks.
- **Representative work:** Plan a pretraining run with a data/compute budget justified by scaling laws; architect distributed training (data/tensor/pipeline/FSDP parallelism); design an ablation matrix that isolates which interventions actually move loss; lead incident response on a stalled large run.
- **Technical depth expected:** Pretraining strategy; distributed training (FSDP, tensor/pipeline/sequence parallelism, communication overlap); scaling laws and compute-optimal allocation; rigorous ablation methodology; numerical stability and large-run debugging; checkpoint/restart and fault tolerance.

### L48 — Principal Machine Learning Engineer

You define the model-building program for an organization and are accountable for frontier-scale outcomes.

- **Responsibilities:** Set multi-quarter frontier-scale training programs; own alignment and preference pipelines at production scale; define applied-ML architecture and standards across the org; make the highest-leverage compute and research-direction calls.
- **Representative work:** Charter a frontier-scale training program with risk-managed milestones; design end-to-end alignment pipelines (SFT → reward modeling → RLHF/DPO → evaluation → release gating); establish org-wide standards for reproducibility, eval, and safe model release; represent the model-building org in cross-functional bets.
- **Technical depth expected:** Frontier-scale program design; full alignment-pipeline architecture; applied-ML system architecture; research-to-production translation; deep judgment on compute economics, data strategy, and risk; technical leadership and standard-setting.

## Specialist Roles

### L30 — Fine-Tuning Engineer

- **Focus:** post-training foundations, SFT dataset engineering, supervised fine-tuning, PEFT (LoRA/QLoRA), preference optimization, safety and alignment tuning, distributed fine-tuning, evaluating fine-tuned models, and quantization, export, and serving.

### L30 — Model Evaluation Engineer

- **Focus:** evaluation foundations, benchmark engineering, classical ML evaluation in depth, LLM benchmark harnesses, LLM-as-judge platforms, human evaluation, generative and multimodal evaluation, agent and tool evaluation, safety and red-team evaluation, and production evaluation.

### L30 — NLP Engineer

- **Focus:** tokenization and text foundations, classical NLP, text classification, sequence labelling and information extraction, question answering and machine reading, summarization and controlled generation, and machine translation and multilingual NLP.

### L35 — Training Pipeline Engineer

- **Focus:** distributed training foundations, training frameworks in depth, training-scale data pipelines, cluster orchestration for training, networking and storage for training, checkpointing, fault tolerance and elastic training, and throughput and MFU.

## Skills Matrix by Level

| Skill Area | L20 — ML Engineer | L30 — Senior | L40 — Staff | L48 — Principal |
|---|---|---|---|---|
| **Data** | Curate & clean datasets | Engineer datasets, mixing & filtering | Design pretraining data strategy | Set org-wide data strategy & sourcing economics |
| **Training** | Run SFT & training pipelines | Advanced fine-tuning (LoRA/full) | Pretraining & large-run strategy | Frontier-scale training programs |
| **Fine-tuning / Alignment** | Basic SFT | DPO, reward modeling, RLHF basics | Alignment ablations at scale | End-to-end alignment pipeline architecture |
| **Evaluation** | Run defined eval suites | Design eval harnesses & metrics | Eval strategy & ablation rigor | Org eval standards & release gating |
| **Distributed Systems** | Single/multi-GPU jobs | Multi-node training | FSDP, tensor/pipeline parallelism | Frontier cluster-scale program design |
| **Experiment Discipline** | Reproducible, tracked runs | Mentor on rigor; ablation basics | Principled ablation programs | Define reproducibility/research standards |
| **Leadership** | Owns own work | Mentors juniors | Cross-team technical direction | Org-wide standards & strategy |

## Compensation Ranges (United States, 2026)

Total compensation (base + bonus + equity). ML roles skew high relative to general software engineering, and the top of each band is set by frontier labs.

| Level | Role | Typical Total Comp (USD) |
|---|---|---|
| L20 | Machine Learning Engineer | $150k – $220k |
| L30 | Senior Machine Learning Engineer | $230k – $400k |
| L40 | Staff Machine Learning Engineer | $400k – $650k |
| L48 | Principal Machine Learning Engineer | $600k – $1M+ |

**Variance is large.** Geography (SF Bay Area / NYC pay a premium over most other US metros), company type (frontier labs and top-tier AI companies sit at the high end; enterprises and non-tech industries at the low end), and equity composition (illiquid startup equity vs. liquid public stock vs. frontier-lab cash-heavy packages) can swing these numbers substantially. Treat the bands as directional, not contractual.

## Promotion Criteria

**L20 → L30.** Move from executing well-scoped training jobs to owning model quality. You consistently ship reproducible results without supervision, can run and defend a fine-tuning program (including preference optimization), design evaluations that catch real regressions, and have started making dataset decisions that measurably improve outcomes.

**L30 → L40.** Move from single-model quality to training strategy at scale. You operate distributed training competently, reason about scaling laws when allocating compute and data, run ablation programs that produce trustworthy conclusions, and influence the direction of training work beyond your immediate team.

**L40 → L48.** Move from leading large runs to defining the program. You set multi-quarter frontier-scale strategy, own alignment/eval pipelines at production scale, establish standards other teams adopt, and are trusted with the organization's highest-leverage compute and research bets.

At every transition the bar is **demonstrated scope at the next level**, not potential — you should already be operating there before the title follows.

## Learning Paths

Each role maps to a paired `-learning` (curriculum, exercises, projects) and `-solutions` (reference implementations) repository. The core progression:

1. **Start at L20** — `ml-engineer-learning`. Build fluency in training pipelines, SFT, reproducibility, and experiment tracking. Check work against `ml-engineer-solutions`.
2. **Advance to L30** — `senior-ml-engineer-learning`. Layer on advanced fine-tuning, DPO/RLHF, eval-harness design, and dataset engineering.
3. **Advance to L40** — `staff-ml-engineer-learning`. Take on pretraining strategy, distributed training, scaling laws, and ablation methodology.
4. **Advance to L48** — `principal-ml-engineer-learning`. Work through frontier-scale program design, alignment-pipeline architecture, and applied-ML systems.

Use the `-solutions` repos to self-check, not to shortcut: the discipline being trained is experiment rigor, and copying a result defeats the exercise.


## Specialist Tracks

Specialist tracks branch off the core ladder for depth in one area.

- **Fine-Tuning Engineer** *(available, L30)* — SFT, LoRA/QLoRA, and preference optimization in depth.
- **Model Evaluation Engineer** *(available, L30)* — eval-harness design, benchmark construction, and regression detection.
- **NLP Engineer** *(available, L30)* — domain-specialized language modeling, from classical NLP to multilingual generation.
- **Training Pipeline Engineer** *(available, L35)* — high-throughput, fault-tolerant distributed training systems.
- **ML Research Engineer** *(planned)* — translating research ideas into rigorous, reproducible experiments.
- **Applied ML Engineer** *(planned)* — taking trained models into production product contexts.
- **CV / Recommendation Engineer** *(planned)* — further domain-specialized model building.

## Repository Map

All repositories live under the [`ml-engineering-curriculum`](https://github.com/ml-engineering-curriculum) GitHub organization. Every role has a paired `-learning` repo (modules, lecture chapters, exercises) and a `-solutions` repo (reference walkthroughs).

| Level | Role | Modules | Learning | Solutions | Status |
|---|---|---|---|---|---|
| L20 | Machine Learning Engineer | 10 | [ml-engineer-learning](https://github.com/ml-engineering-curriculum/ml-engineer-learning) | [ml-engineer-solutions](https://github.com/ml-engineering-curriculum/ml-engineer-solutions) | Complete |
| L30 | Fine-Tuning Engineer | 11 | [fine-tuning-engineer-learning](https://github.com/ml-engineering-curriculum/fine-tuning-engineer-learning) | [fine-tuning-engineer-solutions](https://github.com/ml-engineering-curriculum/fine-tuning-engineer-solutions) | Complete |
| L30 | Model Evaluation Engineer | 12 | [model-evaluation-engineer-learning](https://github.com/ml-engineering-curriculum/model-evaluation-engineer-learning) | [model-evaluation-engineer-solutions](https://github.com/ml-engineering-curriculum/model-evaluation-engineer-solutions) | Complete |
| L30 | NLP Engineer | 13 | [nlp-engineer-learning](https://github.com/ml-engineering-curriculum/nlp-engineer-learning) | [nlp-engineer-solutions](https://github.com/ml-engineering-curriculum/nlp-engineer-solutions) | Complete |
| L30 | Senior Machine Learning Engineer | 10 | [senior-ml-engineer-learning](https://github.com/ml-engineering-curriculum/senior-ml-engineer-learning) | [senior-ml-engineer-solutions](https://github.com/ml-engineering-curriculum/senior-ml-engineer-solutions) | Complete |
| L35 | Training Pipeline Engineer | 10 | [training-pipeline-engineer-learning](https://github.com/ml-engineering-curriculum/training-pipeline-engineer-learning) | [training-pipeline-engineer-solutions](https://github.com/ml-engineering-curriculum/training-pipeline-engineer-solutions) | Complete |
| L40 | Staff Machine Learning Engineer | 10 | [staff-ml-engineer-learning](https://github.com/ml-engineering-curriculum/staff-ml-engineer-learning) | [staff-ml-engineer-solutions](https://github.com/ml-engineering-curriculum/staff-ml-engineer-solutions) | Complete |
| L48 | Principal Machine Learning Engineer | 6 | [principal-ml-engineer-learning](https://github.com/ml-engineering-curriculum/principal-ml-engineer-learning) | [principal-ml-engineer-solutions](https://github.com/ml-engineering-curriculum/principal-ml-engineer-solutions) | Complete |

## The AI Career Curriculum Ecosystem

ML Engineering is one of five sibling curricula. Each owns a distinct layer of the AI stack:

- **[ML Engineering](https://github.com/ml-engineering-curriculum)** *(this org)* — **builds and trains the models.** Data curation, training pipelines, fine-tuning, preference optimization, evaluation, and pretraining at scale.
- **[AI Infrastructure](https://github.com/ai-infra-curriculum)** — **runs the platforms.** The substrate beneath model-building: GPU clusters, training-infra operation, scheduling, networking, and reliability.
- **[AI Engineering](https://github.com/ai-engineering-curriculum)** — **builds WITH models.** Applied LLM and agent products: orchestration, retrieval, tool use, and shipping AI-powered applications.
- **[AI Governance](https://github.com/ai-governance-curriculum)** — **governs and assures.** Policy, risk, assurance, and compliance for AI systems.
- **[AI Startup](https://github.com/ai-startup-curriculum)** — **turns it into a company.** The startup operating school for technical founders.

**Boundary, made explicit:** ML Engineering owns *model-building* (turning data + compute into trained models). AI Infrastructure owns the *substrate* that model-building runs on (the GPU clusters and training infrastructure, operated as a platform). AI Engineering owns *applied LLM/agent products* built on top of finished models. The same training run touches all three disciplines — ML Engineering authors it, AI Infrastructure keeps the cluster healthy, and AI Engineering consumes the resulting model in a product.

<!-- aicg:maintained-by -->
Maintained by [VeriSwarm.ai](https://veriswarm.ai)
