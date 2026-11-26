<h1>Dmitry Lvov</h1>

<p>I build and test models that read medical images. I’m interested in what changes a prediction, whether it’s an earlier chest X-ray or a few patches from a pathology slide.</p>

<p><a href="https://lvovdmitro.github.io/"><strong>Website</strong></a> · <a href="https://lvovdmitro.github.io/Dmitry_Lvov_Research_CV.pdf"><strong>CV</strong></a> · <a href="mailto:d.lvov@innopolis.ru"><strong>Email</strong></a></p>

<h2>Selected research</h2>

<h3>SCFR · When should an earlier scan change a report?</h3>
<p><strong>NeurIPS 2026</strong> · Main track</p>
<p>
  <img align="right" width="44%" src="https://lvovdmitro.github.io/cover-scfr.webp" alt="Illustration of two overlapping chest X-rays with a report beside them">
  I led the experiments for a method that chooses among reports generated with different sources of patient history. It uses a report from the current X-ray alone as its reference for that choice.
</p>
<p><a href="https://neurips.cc/virtual/2026/loc/sydney/poster/154092"><strong>Paper</strong></a> · <a href="https://github.com/LvovDmitro/SCFR"><strong>Code</strong></a></p>
<details>
<summary>What happened with the wrong history?</summary>
<p>The stress test held the current chest X-ray fixed and supplied another patient’s history matched on reported findings and prior-report length. SCFR reduced reference-based false positives compared with the wrong-history baseline. False negatives increased in that comparison.</p>
</details>
<br clear="right">

<h3>LogitGaze-Med · Where will a radiologist look next?</h3>
<p><strong>NeurIPS 2025</strong> · Main track</p>
<p>
  <img align="right" width="44%" src="https://lvovdmitro.github.io/cover-logitgaze-med.webp" alt="Illustration of a blue optical lens and fixation points on a grid">
  I extracted patch-level features from a medical vision-language model to predict where radiologists look and how long they look there. I also tested predicted gaze as supervision for a chest X-ray classifier.
</p>
<p><a href="https://proceedings.neurips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html"><strong>Paper</strong></a> · <a href="https://slideslive.com/39050986/from-human-attention-to-diagnosis-semantic-patchlevel-integration-of-visionlanguage-models-in-medical-imaging"><strong>Watch the talk</strong></a></p>
<details>
<summary>How closely did the model match the recorded gaze?</summary>
<p>Table 1 compares scanpaths on GazeSearch target-present trials. Higher ScanMatch scores mean a closer match to the recorded gaze.</p>
<table>
<thead><tr><th scope="col">Model</th><th scope="col">ScanMatch</th></tr></thead>
<tbody>
<tr><td>LogitGaze-Med (CheXNet)</td><td><strong>0.419</strong></td></tr>
<tr><td>GazeSearch baseline</td><td>0.332</td></tr>
</tbody>
</table>
<p>Both methods received the first fixation. This comparison excludes fixation duration.</p>
</details>
<br clear="right">

<h3>Compact visual evidence · Which patches drive a slide prediction?</h3>
<p><strong>Journal of Pathology Informatics</strong> · 2026</p>
<p>
  <img align="right" width="44%" src="https://lvovdmitro.github.io/cover-pathology.webp" alt="Illustration of a pathology slide and four magnified tissue patches">
  I measured how a whole-slide model’s confidence changed when its highest-attention patches were kept or removed. I used equally sized random sets from the same slide as controls.
</p>
<p><a href="https://doi.org/10.1016/j.jpi.2026.100763"><strong>Paper</strong></a> · <a href="https://github.com/LvovDmitro/compact-visual-evidence"><strong>Code</strong></a></p>
<details>
<summary>Were the most-attended patches inside the annotated tumour?</summary>
<p>On <strong>48 of 49</strong> tumour-positive CAMELYON16 slides, at least one of the three highest-attention patch centres fell inside an annotated tumour contour. This was an exploratory spatial check.</p>
</details>
<br clear="right">

<h2>Other papers</h2>

<h3>IEEE Access</h3>
<ul>
<li><strong><a href="https://doi.org/10.1109/ACCESS.2026.3655813">Multimodal document segmentation for technical question answering</a></strong> · 2026 · <a href="https://github.com/mindlab-itmo/layout-aware-doc-segmentation">Code</a><br>
I kept figures tied to their captions and brought that visual context into the question-answering pipeline.</li>
<li><strong><a href="https://doi.org/10.1109/ACCESS.2025.3566772">Uncertainty in cardiac landmark detection and disease diagnosis on chest X-rays</a></strong> · 2025<br>
I used annotations from multiple radiologists to estimate uncertainty in landmark detection and disease classification.</li>
<li><strong><a href="https://doi.org/10.1109/ACCESS.2024.3524116">Automatic calculation of cardiometric coefficients on chest X-rays</a></strong> · 2025<br>
I worked on using detected landmarks to derive measurements from chest X-rays.</li>
</ul>

<h3>Workshops</h3>
<ul>
<li><strong><a href="https://neurips.cc/virtual/2026/loc/sydney/178289">Similar Scores, Different High-Risk Episodes</a></strong> · NeurIPS 2026 TAE workshop · <a href="https://github.com/LvovDmitro/ehrshot-state-or-space">Code</a><br>
I helped design and rerun the comparison of two patient-history representations to see who entered a high-risk group.</li>
<li><strong><a href="https://neurips.cc/virtual/2026/loc/sydney/178202">Same Top Fraction, Different Workload</a></strong> · NeurIPS 2026 TAE workshop · <a href="https://github.com/vache4ogan/prenatal-risk-scoreability">Code</a><br>
I designed the workload comparison and checked how eligibility rules change who is reviewed and how many referrals they generate.</li>
<li><strong><a href="https://openreview.net/forum?id=Om4j6IVb42">LogitGaze: Predicting Human Attention Using Semantic Information from Vision-Language Models</a></strong> · ICLR 2025 Reasoning and Planning workshop · <a href="https://github.com/LvovDmitro/LogitGaze">Natural-image code</a><br>
I used features from LLaVA’s logit lens to predict scanpaths during visual search in natural images.</li>
</ul>

<h2>Experience</h2>
<ul>
<li><strong>Researcher at Innopolis University’s AI in Medicine Lab.</strong> I design chest X-ray experiments and discuss the results with radiologists. I mentor students on clinical ML projects and review their code and manuscripts.</li>
<li><strong>Part-time engineer at ITMO University’s Mind Lab.</strong> I build tools that help question-answering models read technical documents, including their figures and diagrams.</li>
<li><strong>Engineering project.</strong> I added question and action routing and refactored the LangGraph orchestration in the <a href="https://github.com/ITMO-Agentic-AI/ai-dungeon-master">AI Dungeon Master prototype</a>.</li>
</ul>
<p>I’d like to hear from researchers working on longitudinal imaging or ways to test what a clinical model learns from an image.</p>
