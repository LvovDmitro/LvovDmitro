# Figure sources

The profile uses two original figures by Dmitry Lvov and Ilya Pershin. They were extracted from the authors' papers at the user's request. Neither image has been redrawn, relabelled, enhanced or generated. Extraction changes the page framing and raster resolution only.

## LogitGaze-Med

- **Files:** `logitgaze-med-figure3.png`, 1176 × 828 pixels; `logitgaze-med-figure3-mobile.png`, 588 × 828 pixels.
- **Article:** *From Human Attention to Diagnosis: Semantic Patch-Level Integration of Vision-Language Models in Medical Imaging*, Dmitry Lvov and Ilya Pershin, NeurIPS 2025.
- **Source:** [official proceedings](https://proceedings.nips.cc/paper_files/paper/2025/hash/be7bc8aa38696723cebe296b6122d7e3-Abstract-Conference.html), [official PDF](https://proceedings.neurips.cc/paper_files/paper/2025/file/be7bc8aa38696723cebe296b6122d7e3-Paper-Conference.pdf).
- **Location:** Figure 3, page 7. Rows are human scanpaths (top), LogitGaze-Med predictions (middle), and GazeSearch predictions (bottom). The four columns show Normal, Cardiomegaly, Consolidation and Pneumonia cases. These are target-present search tasks.
- **Extraction:** the full grid uses PDF clip rectangle `(110, 193, 502, 469)` in PDF points, rendered at 216 DPI. The narrow-screen version is a contiguous crop `(110, 193, 306, 469)` at the same resolution: the first two case columns, with all three method rows. All original case labels and annotations remain intact. The adjacent table and original caption are outside the crops; the row-order context is stated in the profile caption.
- **Source PDF SHA-256:** `73f9457299197975cd522a98f29b8b41e74ada30108e1dc3ab35514ef6b092a7`.
- **Full image SHA-256:** `d15e7109d53c2742e7d8149f3d6df3214363a38d6dd93cc55fa44c6bcc5dea2c`.
- **Narrow-screen image SHA-256:** `aa975aaacbaacd751b01037857618af6cdf974417e7e7c9ed809860c4692f66c`.

The profile's numerical comparison comes from Table 1, page 6: the CheXNet variant of LogitGaze-Med scores 0.419 on ScanMatch without fixation duration, versus 0.332 for the GazeSearch baseline, in target-present search on GazeSearch. Both methods are conditioned on the first fixation and were trained from scratch. The paper reports 0.419 ± 0.016 and 0.332 ± 0.019; the profile quotes their central values. It does not infer an unspecified train/test split or claim superiority across all metrics. These are reported paper results, not a new evaluation run for the profile.

## SCFR

- **File:** `scfr-paper-figure2.png`, 1131 × 615 pixels.
- **Article:** *Source-Causal Control of Historical Context in Longitudinal Radiology Report Generation*, Dmitry Lvov and Ilya Pershin, accepted at NeurIPS 2026.
- **Public references:** [paper](https://openreview.net/forum?id=GHvYdC6tmg), [conference page](https://neurips.cc/virtual/2026/poster/154092), [code](https://github.com/LvovDmitro/SCFR).
- **Figure source:** author manuscript created on 19 October 2026, Figure 2, page 5. This is identified as an author-manuscript figure rather than a claim that it is the exact final published proceedings version.
- **Meaning:** the executable SCFR pipeline constructs proposals from three source-valid report generations and selects among five candidates. References supply fitting targets and offline evaluation metrics; reference reports and matched wrong-history interventions do not enter deployment-time routing. The figure contains no patient records or new empirical results.
- **Extraction:** PDF clip rectangle `(116, 70, 493, 275)` in PDF points, rendered at 216 DPI. The original caption is outside the image; its essential context is recorded above.
- **Source PDF SHA-256:** `68533de9a0162f429f7df89e5e2babf520e979d5e328c6647fc5b4042b4f40b3`.
- **Image SHA-256:** `84c8bfe88effcbc22b33aebfc9dcd68002dd836de41cc514d937bbf145b97151`.

## Attribution and rights

Reproduced from papers by Dmitry Lvov and Ilya Pershin at the author's request. [NeurIPS copyright guidance](https://nips.cc/FAQ/Copyright) states that authors retain copyright and grant NeurIPS a non-exclusive publication license. No new license is assigned to the original papers, figures or underlying data by this README. The source papers and their separate terms remain authoritative.
