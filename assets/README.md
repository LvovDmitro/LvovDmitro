# EHR selection figure

`ehr-selection.svg` and `ehr-selection-mobile.svg` are desktop and mobile views of the same public aggregate results from **Similar Scores, Different High-Risk Episodes: Auditing Model Selection in Longitudinal EHRs**, by Polina Korobeinikova, Dmitry Lvov and Ilya Pershin.

[Study](https://openreview.net/forum?id=RffArnWpec) · [Repository](https://github.com/LvovDmitro/ehrshot-state-or-space) · [Exact source CSV](https://github.com/LvovDmitro/ehrshot-state-or-space/blob/4a8dfe18a048a3baa6fc21a8f727bc40d3ca4959/paper/aggregate_outputs/ensemble_top10_cross_representation.csv)

The primary comparison uses raw histories and Era+backfill histories on EHRSHOT. Each representation selects its own top-decile set of episodes.

| Task | Episodes per set | Shared episodes | Episodes unique to each representation | Representation-specific share |
| --- | ---: | ---: | ---: | ---: |
| 30-day readmission | 219 | 185 | 34 | 15.5% |
| ICU transfer | 204 | 153 | 51 | 25.0% |

The percentages are 34/219 and 51/204, rounded to one decimal place. The remaining 84.5% and 75.0% are shared between the two sets. The denominator is each primary top-decile episode set, not all patients, all positive outcomes or the union of the sets.

These are selected-set overlap results. They are not classification error rates, performance gains or measures of clinical benefit. In the study's ten primary task-metric comparisons, all paired patient-cluster 95% intervals for performance differences include zero. The figure should be read with that uncertainty and the full paper's protocol.

The graphics were plotted with Matplotlib from these published counts. They contain no images, records, identifiers or predictions for individual patients. Text remains editable in the SVGs; there are no embedded bitmap assets. The mobile version changes the layout only and shows the same values.

This figure credits the study's authors and links to its public evidence. It does not assign a new license to the original repository, article or data.
