I'm a researcher at [Med AI Lab, Innopolis University](https://ilya-pershin.com/lab/). I develop models for medical imaging and human attention, and study how data and evaluation choices change clinical predictions. I also help students design experiments and check their code and results.

[![Email](https://img.shields.io/badge/Email-d.lvov%40innopolis.ru-0F766E?style=flat-square)](mailto:d.lvov@innopolis.ru)

## Research & code

### SCFR: using patient history in radiology reports

*First-author paper · NeurIPS 2026 main track, accepted poster*

A report generator can carry an old finding into a new report. SCFR controls how prior images and reports affect the description of the current examination, then chooses among reports built from valid sources. The release includes a CPU demo and separate fitting, inference and evaluation commands.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/SCFR) [![Paper](https://img.shields.io/badge/Paper-0F766E?style=flat-square)](https://openreview.net/forum?id=GHvYdC6tmg)

### LogitGaze: predicting where people look

*NeurIPS 2025 main track (LogitGaze-Med, first author) · ICLR 2025 workshop (LogitGaze)*

What people look at depends on what they are searching for. LogitGaze uses semantic features from vision-language models to predict sequences of eye fixations. LogitGaze-Med extends this approach to radiologists' attention on chest X-rays.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/LogitGaze) [![LogitGaze paper](https://img.shields.io/badge/Paper-LogitGaze-0F766E?style=flat-square)](https://openreview.net/forum?id=Om4j6IVb42) [![LogitGaze-Med paper](https://img.shields.io/badge/Paper-LogitGaze--Med-0F766E?style=flat-square)](https://proceedings.nips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html)

### Document segmentation for technical question answering

*First-author paper · IEEE Access, 2026*

Splitting a technical PDF into plain text can separate a figure from its caption. Our pipeline detects document elements and keeps those pairs together, adding descriptions from a vision-language model so that diagrams and other visual elements can be used for question answering.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/mindlab-itmo/layout-aware-doc-segmentation) [![Paper](https://img.shields.io/badge/Paper-0F766E?style=flat-square)](https://doi.org/10.1109/ACCESS.2026.3655813)

### Similar scores, different high-risk episodes

*Coauthored paper · TAE 2026 workshop*

A different representation of the same patient history produced different high-risk episode lists, while differences in aggregate predictive performance remained uncertain. In each primary top-decile selection, 15.5% of readmission episodes and 25.0% of ICU-transfer episodes were absent from the other representation's set.

<picture>
  <source media="(max-width: 600px)" srcset="assets/ehr-selection-mobile.svg">
  <img src="assets/ehr-selection.svg" width="760" alt="Representation-specific share of each primary top-decile episode set: 34 of 219 for readmission (15.5%) and 51 of 204 for ICU transfer (25.0%).">
</picture>

<sub>Raw history versus Era+backfill on EHRSHOT. Figure from the public aggregates of Korobeinikova, Lvov and Pershin. [Source and definitions](assets/README.md).</sub>

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/LvovDmitro/ehrshot-state-or-space) [![Paper](https://img.shields.io/badge/Paper-0F766E?style=flat-square)](https://openreview.net/forum?id=RffArnWpec)

### Same top fraction, different workload

*Coauthored paper · TAE 2026 workshop*

Selecting the top 10% of a restricted cohort can create a different referral workload from selecting the top 10% of the full population. Our CDC Natality audit keeps risk scores fixed and separates the effect of who is eligible from the effect of how many people can be selected.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/vache4ogan/prenatal-risk-scoreability) [![Paper](https://img.shields.io/badge/Paper-0F766E?style=flat-square)](https://openreview.net/forum?id=puYbvC47rw)

### AI Dungeon Master: eight agents, one game

*Team project · LangGraph and LangChain*

Storytelling, combat rules and world state have to agree during a Dungeons & Dragons session. I contributed to a team prototype in which eight agents share game state and divide those responsibilities.

[![Code](https://img.shields.io/badge/Code-334155?style=flat-square&logo=github&logoColor=white)](https://github.com/ITMO-Agentic-AI/ai-dungeon-master)

## Tools

![Python](https://img.shields.io/badge/Python-334155?style=flat-square&logo=python&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-334155?style=flat-square&logo=pytorch&logoColor=white) ![Transformers](https://img.shields.io/badge/Transformers-334155?style=flat-square&logo=huggingface&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-334155?style=flat-square&logo=scikitlearn&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-334155?style=flat-square&logo=numpy&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-334155?style=flat-square&logo=pandas&logoColor=white) ![LangGraph](https://img.shields.io/badge/LangGraph-334155?style=flat-square&logo=langgraph&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-334155?style=flat-square&logo=docker&logoColor=white) ![ClearML](https://img.shields.io/badge/ClearML-334155?style=flat-square) ![Git](https://img.shields.io/badge/Git-334155?style=flat-square&logo=git&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-334155?style=flat-square&logo=linux&logoColor=white)

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
