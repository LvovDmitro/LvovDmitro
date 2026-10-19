# AI researcher & ML engineer

I build models for medical imaging and human attention at [Med AI Lab, Innopolis University](https://ilya-pershin.com/lab/). I also study how data representation and evaluation choices affect clinical risk assessment.

**First-author papers:** [NeurIPS 2025](https://proceedings.nips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html) · [NeurIPS 2026](https://openreview.net/forum?id=GHvYdC6tmg) (accepted poster) · [IEEE Access 2026](https://doi.org/10.1109/ACCESS.2026.3655813)

[![Email](https://img.shields.io/badge/Email-d.lvov%40innopolis.ru-0F766E?style=flat-square)](mailto:d.lvov@innopolis.ru)

## Research & code

### SCFR: using patient history in radiology reports

*First-author paper · NeurIPS 2026 main track, accepted poster*

<picture>
  <source media="(max-width: 600px)" srcset="assets/scfr-mobile.svg">
  <img src="assets/scfr.svg" width="760" alt="Concept: the current examination and prior context enter source control before a current report is selected.">
</picture>

A report generator can carry an old finding into a new report. SCFR controls how prior images and reports influence the current description, then selects among reports built from valid sources. Includes a CPU demo and fitting, inference and evaluation commands.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/SCFR) [![Paper](https://img.shields.io/badge/Paper-0F766E?style=flat-square)](https://openreview.net/forum?id=GHvYdC6tmg)

### LogitGaze: predicting where people look

*NeurIPS 2025 main track (LogitGaze-Med, first author) · ICLR 2025 workshop (LogitGaze)*

<picture>
  <source media="(max-width: 600px)" srcset="assets/logitgaze-mobile.svg">
  <img src="assets/logitgaze.svg" width="760" alt="Concept: image and search task provide vision-language semantics for predicting an eye-fixation sequence. The scanpath icon is illustrative.">
</picture>

What people look at depends on what they are searching for. LogitGaze uses semantic features from vision-language models to predict sequences of eye fixations. LogitGaze-Med extends this approach to radiologists' attention on chest X-rays.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/LogitGaze) [![LogitGaze paper](https://img.shields.io/badge/Paper-LogitGaze-0F766E?style=flat-square)](https://openreview.net/forum?id=Om4j6IVb42) [![LogitGaze-Med paper](https://img.shields.io/badge/Paper-LogitGaze--Med-0F766E?style=flat-square)](https://proceedings.nips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html)

### Document segmentation for technical question answering

*First-author paper · IEEE Access, 2026*

<picture>
  <source media="(max-width: 600px)" srcset="assets/document-qa-mobile.svg">
  <img src="assets/document-qa.svg" width="760" alt="Concept: detect document layout, keep figures paired with captions, and add visual descriptions for technical question answering.">
</picture>

Splitting a technical PDF into plain text can separate a figure from its caption. Our pipeline detects document elements, keeps those pairs together and adds descriptions from a vision-language model, making diagrams and other visual elements available for question answering.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/mindlab-itmo/layout-aware-doc-segmentation) [![Paper](https://img.shields.io/badge/Paper-4F46E5?style=flat-square)](https://doi.org/10.1109/ACCESS.2026.3655813)

### Similar scores, different high-risk episodes

*Coauthored paper · TAE 2026 workshop*

<picture>
  <source media="(max-width: 600px)" srcset="assets/ehr-selection-mobile.svg">
  <img src="assets/ehr-selection.svg" width="760" alt="Representation-specific share of each primary top-decile episode set: 34 of 219 for readmission (15.5%) and 51 of 204 for ICU transfer (25.0%).">
</picture>

A different representation of the same patient history produced different high-risk episode lists, while differences in aggregate predictive performance remained uncertain. We audit which episodes enter the top decile, going beyond a comparison of overall scores.

<sub>Raw history versus Era+backfill on EHRSHOT. Public aggregates: Korobeinikova, Lvov and Pershin. [Figure source and definitions](assets/README.md#ehr-selection-data-figure).</sub>

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/ehrshot-state-or-space) [![Paper](https://img.shields.io/badge/Paper-1D4ED8?style=flat-square)](https://openreview.net/forum?id=RffArnWpec)

### Same top fraction, different workload

*Coauthored paper · TAE 2026 workshop*

<picture>
  <source media="(max-width: 600px)" srcset="assets/prenatal-mobile.svg">
  <img src="assets/prenatal.svg" width="760" alt="Concept: with risk scores fixed, selecting ten percent of the full cohort or ten percent of an eligible cohort can imply different absolute workloads.">
</picture>

Selecting the top 10% of a restricted cohort can create a different referral workload from selecting the top 10% of the full population. Our CDC Natality audit holds risk scores fixed and separates eligibility from absolute selection capacity.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/vache4ogan/prenatal-risk-scoreability) [![Paper](https://img.shields.io/badge/Paper-1D4ED8?style=flat-square)](https://openreview.net/forum?id=puYbvC47rw)

### AI Dungeon Master: eight agents, one game

*Team project · LangGraph and LangChain*

<picture>
  <source media="(max-width: 600px)" srcset="assets/dungeon-mobile.svg">
  <img src="assets/dungeon.svg" width="760" alt="Concept: eight agent nodes connect to a shared game state, coordinating story, rules and the game world.">
</picture>

Storytelling, combat rules and world state have to agree during a Dungeons & Dragons session. I contributed to a team prototype in which eight agents share game state and divide those responsibilities.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/ITMO-Agentic-AI/ai-dungeon-master)

## Tools

![Python](https://img.shields.io/badge/Python-334155?style=flat-square&logo=python&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-334155?style=flat-square&logo=pytorch&logoColor=white) ![Transformers](https://img.shields.io/badge/Transformers-334155?style=flat-square&logo=huggingface&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-334155?style=flat-square&logo=scikitlearn&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-334155?style=flat-square&logo=numpy&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-334155?style=flat-square&logo=pandas&logoColor=white) ![LangGraph](https://img.shields.io/badge/LangGraph-334155?style=flat-square&logo=langgraph&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-334155?style=flat-square&logo=docker&logoColor=white) ![ClearML](https://img.shields.io/badge/ClearML-334155?style=flat-square) ![Git](https://img.shields.io/badge/Git-334155?style=flat-square&logo=git&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-334155?style=flat-square&logo=linux&logoColor=white)

I also help students design experiments and review their code and results.

<details>
<summary>Publication details</summary>

- **Source-Causal Control of Historical Context in Longitudinal Radiology Report Generation** (NeurIPS 2026, main track, accepted poster). [Paper](https://openreview.net/forum?id=GHvYdC6tmg)
- **From Human Attention to Diagnosis: Semantic Patch-Level Integration of Vision-Language Models in Medical Imaging** (NeurIPS 2025, main track). [Proceedings](https://proceedings.nips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html)
- **Enhancing Technical Question Answering Quality Through Multimodal Document Segmentation** (IEEE Access, 2026). [DOI](https://doi.org/10.1109/ACCESS.2026.3655813)
- **Uncertainty Estimation in Cardio Landmark Detection and Heart Disease Diagnosis on Chest X-Ray Images** (IEEE Access, 2025). [DOI](https://doi.org/10.1109/ACCESS.2025.3566772)
- **LogitGaze: Predicting Human Attention Using Semantic Information from Vision-Language Models** (ICLR 2025, Workshop on Reasoning and Planning for Large Language Models). [Paper](https://openreview.net/forum?id=Om4j6IVb42)
- **Similar Scores, Different High-Risk Episodes: Auditing Model Selection in Longitudinal EHRs** (TAE workshop, NeurIPS 2026). [Paper](https://openreview.net/forum?id=RffArnWpec)
- **Same Top Fraction, Different Workload: Auditing Eligibility and Capacity in Clinical Risk Evaluation** (TAE 2026 workshop). [Paper](https://openreview.net/forum?id=puYbvC47rw)

</details>
