# AI researcher & ML engineer

I work at [Med AI Lab, Innopolis University](https://ilya-pershin.com/lab/), building models for medical imaging and human attention. I also study how patient-history representations and evaluation choices affect clinical risk assessment.

**First-author papers:** [NeurIPS 2025](https://proceedings.nips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html) · [NeurIPS 2026 — accepted](https://openreview.net/forum?id=GHvYdC6tmg) · [IEEE Access 2025](https://doi.org/10.1109/ACCESS.2025.3566772) / [2026](https://doi.org/10.1109/ACCESS.2026.3655813)

**Workshop papers:** [ICLR 2025](#user-content-iclr-2025-workshop) · [NeurIPS 2026](#user-content-neurips-2026-workshop)

[![Email](https://img.shields.io/badge/Email-d.lvov%40innopolis.ru-0969DA?style=flat-square)](mailto:d.lvov@innopolis.ru)

## Conference papers

### SCFR: longitudinal radiology reports

**NeurIPS 2026 · accepted** · First author, with Ilya Pershin

SCFR controls how a patient's prior images and reports influence a new radiology report. It selects among current-only and history-conditioned proposals without access to a reference report at inference. The release includes a CPU demo and separate fitting, inference and evaluation commands.

The stress audit found lower reference-based false-positive counts than the wrong-history baseline, with a false-negative trade-off. [Audit results](https://github.com/LvovDmitro/SCFR/blob/main/evidence/confirmatory_gate_5000.md).

[![Paper](https://img.shields.io/badge/Paper-0969DA?style=flat-square)](https://openreview.net/forum?id=GHvYdC6tmg) [![Code](https://img.shields.io/badge/Code-30363D?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/SCFR) [![CPU demo](https://img.shields.io/badge/CPU_demo-30363D?style=flat-square)](https://github.com/LvovDmitro/SCFR#install-and-run)

### LogitGaze-Med: predicting radiologists' attention

**NeurIPS 2025** · First author, with Ilya Pershin

We combine visual features, diagnostic text and semantic priors from a medical vision-language model to predict fixation locations and dwell times on chest X-rays. The paper also tests predicted gaze as additional supervision for pathology classification.

On GazeSearch target-present trials, the CheXNet variant scored **0.419 ScanMatch**, against **0.332 for the GazeSearch baseline**, without fixation-duration information (Table 1).

[![Paper](https://img.shields.io/badge/Paper-0969DA?style=flat-square)](https://proceedings.nips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html) [![Code](https://img.shields.io/badge/Code-30363D?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/LogitGaze)

## Journal papers

### Multimodal document segmentation for technical QA

**IEEE Access 2026** · First author

Our pipeline detects document elements with YOLOv10, keeps figures linked to their captions and adds descriptions from a vision-language model. Those fragments let a question-answering system use the diagrams and other visual content of a technical document.

[![Paper](https://img.shields.io/badge/Paper-0969DA?style=flat-square)](https://doi.org/10.1109/ACCESS.2026.3655813) [![Code](https://img.shields.io/badge/Code-30363D?style=flat-square&logo=github&logoColor=white)](https://github.com/mindlab-itmo/layout-aware-doc-segmentation)

### Uncertainty in cardiac landmark detection

**IEEE Access 2025** · First author

Uncertainty estimation for cardiac landmarks and disease classification from chest X-rays, using multiple radiologist annotations to account for label noise.

[![Paper](https://img.shields.io/badge/Paper-0969DA?style=flat-square)](https://doi.org/10.1109/ACCESS.2025.3566772)

## Workshop papers

### ICLR 2025 workshop

[Reasoning and Planning for Large Language Models](https://workshop-llm-reasoning-planning.github.io/) · Coauthor

**LogitGaze: Predicting Human Attention Using Semantic Information from Vision-Language Models**

Our earlier scanpath-prediction work uses word-level semantics extracted from a vision-language model through the logit lens. It studies visual search in natural images; LogitGaze-Med develops the medical-imaging direction.

[![Paper](https://img.shields.io/badge/Paper-0969DA?style=flat-square)](https://openreview.net/forum?id=Om4j6IVb42) [![Code](https://img.shields.io/badge/Code-30363D?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/LogitGaze)

### NeurIPS 2026 workshop

[Can We Trust AI Evaluation? (TAE / Trust-AI-Eval)](https://tai-eval.github.io/) · Two accepted papers, coauthor

**Similar Scores, Different High-Risk Episodes: Auditing Model Selection in Longitudinal EHRs**

Comparing raw and Era+backfill histories on EHRSHOT, 15.5% of readmission episodes and 25.0% of ICU-transfer episodes in each primary top-decile selection were unique to the representation. Differences in aggregate predictive performance remained uncertain.

[![Paper](https://img.shields.io/badge/Paper-0969DA?style=flat-square)](https://openreview.net/forum?id=RffArnWpec) [![Code](https://img.shields.io/badge/Code-30363D?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/ehrshot-state-or-space)

**Same Top Fraction, Different Workload: Auditing Eligibility and Capacity in Clinical Risk Evaluation**

With the same risk scores, changing who is eligible can also change how many people are selected. We separate these effects in a CDC Natality audit of referral workload.

[![Paper](https://img.shields.io/badge/Paper-0969DA?style=flat-square)](https://openreview.net/forum?id=puYbvC47rw) [![Code](https://img.shields.io/badge/Code-30363D?style=flat-square&logo=github&logoColor=white)](https://github.com/vache4ogan/prenatal-risk-scoreability)

## Engineering

### AI Dungeon Master

**Team prototype · LangGraph and LangChain**

Eight agents coordinate storytelling, rules and world state for Dungeons & Dragons. I added action/question routing and refactored the LangGraph orchestrator, including hooks for world and player-state updates.

[![Code](https://img.shields.io/badge/Code-30363D?style=flat-square&logo=github&logoColor=white)](https://github.com/ITMO-Agentic-AI/ai-dungeon-master) [![Contribution](https://img.shields.io/badge/Contribution-0969DA?style=flat-square)](https://github.com/ITMO-Agentic-AI/ai-dungeon-master/commit/a6ff27bfbd4385df9d1357b17397e855c8025903)

## Tools

![Python](https://img.shields.io/badge/Python-30363D?style=flat-square&logo=python&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-30363D?style=flat-square&logo=pytorch&logoColor=white) ![Transformers](https://img.shields.io/badge/Transformers-30363D?style=flat-square&logo=huggingface&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-30363D?style=flat-square&logo=scikitlearn&logoColor=white) ![LangGraph](https://img.shields.io/badge/LangGraph-30363D?style=flat-square&logo=langgraph&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-30363D?style=flat-square&logo=docker&logoColor=white) ![ClearML](https://img.shields.io/badge/ClearML-30363D?style=flat-square) ![Linux](https://img.shields.io/badge/Linux-30363D?style=flat-square&logo=linux&logoColor=white)

I also help students design experiments and review their code and results.

<details>
<summary>Full publication titles</summary>

- **Source-Causal Control of Historical Context in Longitudinal Radiology Report Generation** — NeurIPS 2026, accepted. [Paper](https://openreview.net/forum?id=GHvYdC6tmg)
- **From Human Attention to Diagnosis: Semantic Patch-Level Integration of Vision-Language Models in Medical Imaging** — NeurIPS 2025. [Proceedings](https://proceedings.nips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html)
- **Enhancing Technical Question Answering Quality Through Multimodal Document Segmentation** — IEEE Access, 2026. [DOI](https://doi.org/10.1109/ACCESS.2026.3655813)
- **Uncertainty Estimation in Cardio Landmark Detection and Heart Disease Diagnosis on Chest X-Ray Images** — IEEE Access, 2025. [DOI](https://doi.org/10.1109/ACCESS.2025.3566772)
- **LogitGaze: Predicting Human Attention Using Semantic Information from Vision-Language Models** — ICLR 2025, Workshop on Reasoning and Planning for Large Language Models. [Paper](https://openreview.net/forum?id=Om4j6IVb42)
- **Similar Scores, Different High-Risk Episodes: Auditing Model Selection in Longitudinal EHRs** — NeurIPS 2026, Can We Trust AI Evaluation? workshop. [Paper](https://openreview.net/forum?id=RffArnWpec)
- **Same Top Fraction, Different Workload: Auditing Eligibility and Capacity in Clinical Risk Evaluation** — NeurIPS 2026, Can We Trust AI Evaluation? workshop. [Paper](https://openreview.net/forum?id=puYbvC47rw)

</details>
