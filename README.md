# Dmitry Lvov

I build and evaluate models for medical imaging at Innopolis University’s [AI in Medicine Lab](https://ilya-pershin.com/lab/). I’m also a part-time engineer at ITMO University’s Mind Lab.

[Website](https://lvovdmitro.github.io/) · [CV](https://lvovdmitro.github.io/Dmitry_Lvov_Research_CV.pdf) · [ORCID](https://orcid.org/0009-0008-3211-5853)

## Main-track conference papers

### SCFR and prior exams in radiology reports

NeurIPS 2026 · [Paper](https://neurips.cc/virtual/2026/loc/sydney/poster/154092) · [Code](https://github.com/LvovDmitro/SCFR)

I led an audit that varied the available history while keeping each current chest X-ray fixed. SCFR uses a report generated from the current image alone to choose among candidate reports.

### LogitGaze-Med and radiologists’ gaze

NeurIPS 2025 · [Paper](https://proceedings.neurips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html) · [Recorded talk](https://slideslive.com/39050986/from-human-attention-to-diagnosis-semantic-patchlevel-integration-of-visionlanguage-models-in-medical-imaging)

I used patch-level features from a medical vision-language model to predict where radiologists look. I tested whether the predicted fixations helped train a chest X-ray classifier.

## Journal articles

### Compact visual evidence for whole-slide pathology

Journal of Pathology Informatics, 2026 · [Article 100763](https://doi.org/10.1016/j.jpi.2026.100763) · [Code](https://github.com/LvovDmitro/compact-visual-evidence)

I measured how a whole-slide model’s confidence changed when selected patches were kept or removed, using equally sized random sets from the same slide as controls.

- [Multimodal document segmentation for technical question answering](https://doi.org/10.1109/ACCESS.2026.3655813), IEEE Access 2026. [Code](https://github.com/mindlab-itmo/layout-aware-doc-segmentation)
- [Uncertainty in cardiac landmark detection and disease diagnosis on chest X-rays](https://doi.org/10.1109/ACCESS.2025.3566772), IEEE Access 2025.
- [Automatic calculation of cardiometric coefficients on chest X-rays](https://doi.org/10.1109/ACCESS.2024.3524116), IEEE Access 2025.

## Workshop papers

- [Similar Scores, Different High-Risk Episodes](https://neurips.cc/virtual/2026/loc/sydney/178289), NeurIPS 2026 workshop, Can We Trust AI Evaluation? [Code](https://github.com/LvovDmitro/ehrshot-state-or-space)
- [Same Top Fraction, Different Workload](https://neurips.cc/virtual/2026/loc/sydney/178202), NeurIPS 2026 workshop, Can We Trust AI Evaluation? [Code](https://github.com/vache4ogan/prenatal-risk-scoreability)
- [LogitGaze: Predicting Human Attention Using Semantic Information from Vision-Language Models](https://openreview.net/forum?id=Om4j6IVb42), Reasoning and Planning for Large Language Models, ICLR 2025. [Code for natural-image experiments](https://github.com/LvovDmitro/LogitGaze)

## Engineering

I added action and question routing and refactored the LangGraph orchestration in the [AI Dungeon Master](https://github.com/ITMO-Agentic-AI/ai-dungeon-master) prototype.

If you work on related research, you can reach me at [d.lvov@innopolis.ru](mailto:d.lvov@innopolis.ru).
