# Systematic Literature Review Protocol

## Cancer Survival Prediction Using Machine Learning and Deep Learning

| Protocol item | Details |
|---|---|
| **Protocol version** | 1.1 |
| **Protocol date** | 14 October 2026 |
| **Review type** | Systematic literature review (SLR), including a comparative analysis of baseline survival models |
| **Publication window** | January 2023–September 2026, inclusive |
| **Registration** | OSF/Zenodo Registries — identifier to be added after registration |
| **Status** | Protocol prepared; search and review stages should be documented as they are completed |

## 1. Background and rationale

Cancer survival prediction is an important area of clinical research. Reliable estimates of survival-related outcomes can support risk stratification, prognosis, treatment planning, and patient management.

Machine learning (ML) and deep learning (DL) methods have been applied to cancer survival prediction using patient-level clinical, demographic, molecular, genomic, imaging, pathological, and other data. Studies differ in their cancer populations, datasets, model families, outcome definitions, validation designs, and evaluation metrics. These differences make it difficult to compare results across papers or to identify which modelling approaches are most consistently evaluated.

This review will systematically identify and synthesize primary research on cancer survival prediction, describe the ML/DL and computational survival-modelling approaches used, identify limitations and evidence gaps, and compare baseline models when the studies provide sufficiently consistent within-study evaluations.

## 2. Aim and objectives

The overall aim is to review research published from January 2023 through September 2026 on computational approaches to cancer survival prediction.

The objectives are to:

1. Identify the ML, DL, and computational/statistical survival-analysis models used in eligible studies.
2. Describe the cancer types, patient populations, datasets, and data sources studied.
3. Summarize survival outcomes and evaluation metrics reported.
4. Identify methodological limitations and research gaps.
5. Compare baseline survival models only where results are reported under consistent within-study validation settings and evaluation metrics.

## 3. Research questions

| ID | Research question | Planned synthesis |
|---|---|---|
| **RQ1** | What machine learning and deep learning techniques have been used for cancer survival prediction? | Classify model families, architectures, hybrid approaches, and modelling pipelines. |
| **RQ2** | What cancer types, patient populations, and datasets have been investigated for cancer survival prediction? | Summarize cancer sites/subtypes, cohorts, sample sizes, datasets, and data sources. |
| **RQ3** | What survival outcomes and evaluation metrics have been used to evaluate cancer survival prediction models? | Tabulate endpoints, prediction formulations, metric names/variants, and reported values. |
| **RQ4** | What limitations and research gaps are evident in existing cancer survival prediction studies? | Synthesize author-reported limitations and review-identified methodological or evidence gaps. |
| **RQ5** | How do baseline survival models perform relative to one another under consistent validation settings and evaluation metrics? | Compare eligible within-study baseline comparisons; do not compare unadjusted values across unrelated studies. |

## 4. Review scope

The review focuses on primary research that predicts cancer survival or prognosis using patient-level cancer data. Eligible studies may concern any cancer type or subtype and may use clinical, demographic, genomic, molecular, imaging, radiomic, pathological, or multimodal features.

The review will record the outcome definition and modelling formulation used in each study. Survival-related outcomes may include overall survival, disease-free survival, progression-free survival, recurrence-free survival, cancer-specific survival, disease-specific survival, mortality, time to recurrence, time to progression, or another clearly defined cancer-related survival endpoint.

Studies that focus only on diagnosis, detection, classification, segmentation, staging, or treatment response without evaluating survival outcomes are outside the review scope.

### 4.1 Modelling approaches

The workbook permits ML, DL, and computational/statistical survival-analysis models. The review will therefore record the actual modelling approach reported by each eligible study rather than restricting extraction to a predetermined list of algorithms. Models may include, where encountered:

- Tree-based and ensemble methods, including Random Forest and boosting methods.
- Kernel and margin-based methods, including Support Vector Machines.
- Neural networks and deep-learning architectures.
- Deep survival models and hybrid ML/DL pipelines.
- Computational or statistical survival-analysis models used as predictive methods or comparators.

Traditional statistical models will not automatically be treated as ML/DL models. Their role in each paper (primary predictive method, feature-processing component, or comparator) will be recorded separately.

### 4.2 Interpretation of the survival-classification/ordinary-regression exclusion

The workbook lists “cancer survival classification or ordinary regression” as an exclusion criterion. For consistent screening, this protocol interprets that criterion as excluding studies that use only generic classification or ordinary regression without a defined cancer survival/prognostic endpoint or an appropriate survival-analysis formulation. A study that predicts a clearly defined survival endpoint at a fixed time horizon should be assessed against the full eligibility criteria and the protocol interpretation should be applied consistently. This rule should be confirmed by the review team before screening begins and any decision documented as a protocol clarification.

## 5. Eligibility criteria

### 5.1 Inclusion criteria

A study will be included when it meets **all** applicable criteria below.

| ID | Inclusion criterion | Screening guidance |
|---|---|---|
| **I1** | Focuses on cancer survival or prognostic prediction. | A survival-related outcome must be evaluated. |
| **I2** | Uses machine learning, deep learning, or a computational/statistical survival-analysis model. | Record the role and type of each model; do not infer an algorithm that the paper does not report. |
| **I3** | Uses patient-level cancer data. | Data may come from an institutional cohort, registry, public cancer dataset, or another patient-derived source. |
| **I4** | Reports survival-related outcomes and/or evaluation metrics. | Extract the outcome definition and the metrics actually reported. |
| **I5** | Provides sufficient methodological information. | There must be enough information to identify the population/data, modelling approach, and survival outcome or evaluation. |
| **I6** | Is a peer-reviewed research article. | Primary research only; apply the exclusion rules to reviews and other non-primary publication types. |
| **I7** | Falls within the predefined publication window. | January 2023 through September 2026, inclusive. |
| **I8** | Is published in English. | Apply this rule consistently at screening. |

### 5.2 Exclusion criteria

Apply the exclusion criteria in the order shown. At full-text screening, record one **primary** exclusion reason using the first applicable criterion.

| Order | ID | Exclusion criterion | Operational rule |
|---:|---|---|---|
| 1 | **E1** | Outside the publication window | Published before January 2023 or after September 2026. |
| 2 | **E2** | Ineligible publication type | Review, systematic review, survey, editorial, letter, book chapter, or other non-primary research publication. |
| 3 | **E3** | Not focused on cancer | The study does not concern cancer or a defined cancer population. |
| 4 | **E4** | No survival outcome evaluated | Focuses only on diagnosis, detection, classification, segmentation, staging, or treatment response without evaluating survival outcomes. |
| 5 | **E5** | Survival classification or ordinary regression only | Applies the protocol interpretation in Section 4.2: generic classification or ordinary regression without a defined cancer survival/prognostic endpoint or appropriate survival-analysis formulation. |
| 6 | **E6** | Insufficient methodological information | The population/data, modelling approach, or relevant outcome cannot be established sufficiently for extraction. |
| 7 | **E7** | Duplicate record | The record duplicates another identified publication; retain the preferred record and link duplicates where useful. |

If a record fails more than one criterion, assign the first applicable reason in this table. Records that cannot be confidently classified from title and abstract should proceed to full-text assessment.

## 6. Publication period and language

The review covers publications dated **1 January 2023 to 30 September 2026, inclusive**, and written in English. The exact date on which each database is searched must be recorded. If the search is run after September 2026, publication eligibility remains bounded by the stated window unless a formal protocol amendment changes it.

## 7. Information sources

The workbook identifies the following six sources. The searcher should record the platform/interface used, date searched, query as executed, filters, and number of records returned for each source.

| No. | Database or source | Search approach |
|---:|---|---|
| 1 | IEEE Xplore | Search the supplied Boolean query using the source's available search fields and syntax. |
| 2 | Lens.org | Search title and abstract fields with cancer, survival/prognosis, and ML/DL terms; apply the specified review-publication exclusion if supported by the interface. |
| 3 | ACM Digital Library | Search for survival prediction/prognosis terms combined with cancer and ML/DL terms. |
| 4 | Springer Nature Link | Search for survival prediction/prognosis terms combined with cancer and ML/DL terms. |
| 5 | Frontiers | Search for survival prediction/overall survival, cancer, and ML/DL terms. |
| 6 | PubMed | Search title/abstract terms and relevant MeSH headings as shown below. |

No additional database should be represented as searched unless it is actually searched and documented. Any supplementary search (for example, reference-list checking) should be recorded separately, including its method and yield.

## 8. Search strategy

### 8.1 Search concepts

The general search structure combines four concepts:

| Concept | Purpose | Example terms from the search plan |
|---|---|---|
| Cancer | Identify the disease population | `cancer`, `neoplasm`, `carcinoma`, `tumor`, `tumour` |
| Survival/prognosis | Identify the target outcome | `survival prediction`, `overall survival`, `survival prognosis`, `cancer prognosis` |
| Prediction/modelling | Capture predictive work | `prediction`, `prognostic prediction`, `predicting survival`, `modelling` where supported |
| ML/DL/AI | Identify computational methods | `machine learning`, `deep learning`, `neural network`, `random forest`, `support vector machine`, `gradient boosting`, `XGBoost`, `transformer` |

The exact Boolean structure varies by source because search fields and query syntax differ. The database-specific strings below are taken from the workbook and should be retained in the search log exactly as executed. Any syntax changes required by a platform must be documented.

### 8.2 Database-specific search strings

| Source | Search string |
|---|---|
| **IEEE Xplore** | `("cancer survival" OR "survival prediction" OR "survival prognosis" OR "cancer prognosis") AND ("machine learning" OR "deep learning" OR "neural network" OR "random forest" OR "support vector machine" OR "deep neural network")` |
| **Lens.org** | `(title:("survival prediction" OR "prognostic prediction" OR "predicting survival" OR "survival prognosis") OR abstract:("survival prediction" OR "prognostic prediction" OR "predicting survival" OR "survival prognosis")) AND (title:(cancer OR neoplasm OR carcinoma OR tumor OR tumour) OR abstract:(cancer OR neoplasm OR carcinoma OR tumor OR tumour)) AND (title:("machine learning" OR "deep learning" OR "neural network" OR "random forest" OR "support vector machine" OR "gradient boosting" OR XGBoost OR transformer) OR abstract:("machine learning" OR "deep learning" OR "neural network" OR "random forest" OR "support vector machine" OR "gradient boosting" OR XGBoost OR transformer)) NOT publication_supplementary_type:review` |
| **ACM Digital Library** | `("survival prediction" OR "overall survival" OR "survival prognosis") AND (cancer OR carcinoma OR tumor OR tumour OR neoplasm) AND ("machine learning" OR "deep learning" OR "neural network")` |
| **Springer Nature Link** | `("survival prediction" OR "cancer survival" OR "overall survival" OR "survival prognosis") AND (cancer OR carcinoma OR tumor OR tumour) AND ("machine learning" OR "deep learning" OR "neural network")` |
| **Frontiers** | `("survival prediction" OR "overall survival") AND cancer AND ("machine learning" OR "deep learning")` |
| **PubMed** | `("survival prediction"[Title/Abstract] OR "overall survival"[Title/Abstract] OR "survival prognosis"[Title/Abstract]) AND (Neoplasms[Mesh] OR cancer*[Title/Abstract] OR carcinoma*[Title/Abstract] OR tumor*[Title/Abstract] OR tumour*[Title/Abstract]) AND (Machine Learning[Mesh] OR "Artificial Intelligence"[Mesh] OR "machine learning"[Title/Abstract] OR "deep learning"[Title/Abstract] OR "neural network*"[Title/Abstract])` |


### 8.3 Search documentation

For every source, retain the following information in the `search/` directory or equivalent project location:

- Source/database and platform.
- Date searched.
- Full query exactly as executed.
- Filters and limits applied.
- Number of records retrieved.
- Export format and export filename.
- Any syntax adaptation, access limitation, or search error.

## 9. Study identification and record management

Export records from each source in a format that preserves available bibliographic metadata, including title, authors, year, abstract, DOI, source, and URL where available. Keep the original exports unchanged in a raw-data location and work from copies for cleaning and screening.

Assign each record a unique identifier. Maintain a record of the source or sources in which each record was found so that the study-selection flow can be reported transparently.

## 10. Duplicate management

Identify duplicates using DOI, title, author names, publication year, and other available metadata. Manually inspect uncertain matches. Retain one preferred record for screening while preserving the link to duplicate records and their sources.

If a conference paper and an expanded journal article describe the same study, assess whether they are duplicate or companion reports. Retain the report that provides the most complete eligible information and record the relationship. Do not remove distinct studies merely because they use the same dataset.

## 11. Screening procedure

### 11.1 Screening stages

Screen records in two stages:

1. **Title and abstract screening:** assess relevance against the review questions and eligibility criteria.
2. **Full-text screening:** assess potentially eligible papers against all inclusion and exclusion criteria.

Records that cannot confidently be excluded from the title and abstract should proceed to full-text screening.

### 11.2 Reviewer decisions and disagreements

Where two reviewers are available, both should independently screen records at each stage. Resolve disagreements through discussion; refer unresolved disagreements to a third reviewer where available. If only one reviewer is available, state this in the final review and acknowledge it as a limitation rather than reporting independent screening.

Before full screening, pilot the criteria on a small sample of records and clarify ambiguous rules. Record the calibration sample, reviewer decisions, and any resulting clarifications. Do not claim inter-rater agreement statistics unless they are actually calculated.

### 11.3 Full-text exclusion reasons

Use the ordered exclusion reasons in Section 5.2. Record one primary reason for each full-text exclusion and retain a list of excluded full-text reports with reasons for PRISMA reporting.

## 12. Data extraction

### 12.1 Extraction process

Use a structured extraction form and pilot it on a small number of eligible studies before extracting all records. Revise the form only when necessary and document substantive changes. Verify extracted numerical results against the publication. If a value is available only in a figure, mark it as figure-derived and record the extraction method.

### 12.2 Extraction variables

Extract the following fields where reported and applicable.

| Category | Variables |
|---|---|
| Bibliographic details | Study ID, title, authors, year, publication type, DOI/URL, country or study setting |
| Population and cancer | Cancer type/subtype, inclusion population, cohort characteristics, sample size, number of events where reported |
| Data and features | Dataset/source, clinical and demographic variables, genomic/molecular data, imaging/radiomics, pathology, multi-omics, multimodal inputs |
| Outcome | Survival/prognostic endpoint, endpoint definition, time horizon, time-to-event or fixed-horizon formulation, censoring information |
| Models | ML/DL/statistical survival models, architecture, comparator models, hybrid approach, baseline/proposed-model distinction |
| Methodology | Preprocessing, missing-data handling, feature selection, class balancing if relevant, train/validation/test split, cross-validation, hyperparameter tuning |
| Validation | Internal validation, external validation, temporal/geographical validation, independent test cohort, validation dataset and protocol |
| Metrics and results | Metric names and variants, reported values, uncertainty intervals where available, calibration and discrimination measures, comparator results |
| Baseline comparison | Cohort and feature set, split/protocol, tuning procedure, source of baseline values, exact values and location in paper |
| Interpretability | Explainability/interpretability method and any evaluation of explanations |
| Transparency | Code availability, data availability, reproducibility information |
| Critical appraisal | Author-reported limitations, review-identified concerns, research gaps |

### 12.3 Rules for extracting metrics

Record a metric as reported only when the study provides a numeric result for at least one evaluated model. A metric that is merely named or discussed without a numeric result should not be coded as a reported result. Preserve metric variants and evaluation settings; do not treat different variants as interchangeable.

## 13. Quality and methodological appraisal

Assess the methodological quality and risk of bias using a suitable prediction-model appraisal framework. The original protocol specified PROBAST+AI; use it only after confirming that the version and guidance are appropriate for the included study designs and available information. Apply the selected tool consistently and document adaptations or items that cannot be assessed.

Where feasible, one reviewer may assess all studies and a second reviewer independently assess a sample, with all comparative-analysis studies double-assessed. Report the actual procedure used. Use TRIPOD+AI as a reporting reference when examining reporting of model development, validation, discrimination, and calibration; reporting completeness should be distinguished from risk of bias.

## 14. Evidence synthesis

Synthesize findings descriptively and thematically, organized around the five research questions. Planned summaries include:

- Publication year and study characteristics.
- Cancer types, populations, datasets, and sample sizes.
- Modelling techniques and architectures.
- Survival endpoints and prediction formulations.
- Evaluation metrics and reported performance.
- Validation strategies, including external validation.
- Baseline models and within-study comparisons.
- Limitations, reproducibility concerns, and research gaps.

Use tables and figures where they make the evidence easier to compare. Report each percentage with its numerator and denominator. Separate time-to-event analyses that account for censoring from fixed-horizon prediction approaches when their formulations or metrics are not comparable.

Do not pool performance values across unrelated studies simply because they use the same metric name. Differences in cohorts, outcome definitions, censoring, validation design, and metric variants may make such pooling misleading. Any quantitative synthesis must be justified by the extracted data and described transparently; otherwise, use structured narrative synthesis.

## 15. Comparative analysis of baseline models

### 15.1 Rationale

Reported performance from different studies is not directly comparable when populations, datasets, endpoints, validation designs, or metric variants differ. The baseline comparison will therefore prioritize **within-study comparisons** conducted under consistent conditions.

### 15.2 Eligibility for a baseline comparison

A comparison may be included when:

1. At least two baseline survival models are evaluated in the same study.
2. The models are evaluated on the same cohort and, where applicable, the same feature set.
3. The data split or validation protocol is the same for the models being compared.
4. A numeric result is reported for each model using the same metric and metric variant.
5. The compared outcome and evaluation setting are sufficiently described to interpret the comparison.

Record comparisons that do not meet these conditions in the descriptive synthesis, but do not treat them as like-for-like evidence in the primary baseline comparison.

### 15.3 Comparison extraction and synthesis

For every eligible comparison, extract model names, cohort, feature set, validation protocol, metric and variant, numeric values, tuning information, and whether the values were generated by the study authors or taken from previous work.

Summarize which baseline performs better within each eligible comparison and report the difference in the metric when it can be calculated from the reported values. Treat comparisons from the same study as potentially dependent. Avoid claiming that one model is universally superior based on a small or heterogeneous set of comparisons. If evidence is too sparse or inconsistent, provide a descriptive table rather than a pooled estimate.

## 16. Analysis and visualization

Maintain analysis scripts, extracted data, and generated figures/tables in traceable project directories, for example:

```text
search/
  database_search_log.csv
  search_strings.md
data/
  raw/
  screening/
  extraction/
analysis/
figures/
tables/
```

The directory structure is a suggested organization, not evidence that these files already exist. Tables and figures should be traceable to the underlying extraction data. Any scripts used for counts, descriptive statistics, or plots should be retained with sufficient notes to reproduce the outputs.

## 17. Reporting standards

Report the review using PRISMA 2020 and the PRISMA 2020 for Abstracts checklist as appropriate. Document database searching in a transparent, reproducible manner consistent with PRISMA-S principles. Use a PRISMA flow diagram to show records identified, duplicates removed, records screened, full texts assessed, and studies included. Report database records and any supplementary-search records separately when applicable.

Report the actual methods used, including deviations from this protocol, rather than describing planned procedures as completed procedures.

## 18. Data availability and research materials

Where permitted by copyright, licensing, and ethical requirements, retain the search log, bibliographic metadata, screening decisions, extraction tables, analysis scripts, figures, and tables in the project repository. Do not redistribute copyrighted full-text articles or patient-level personal or sensitive data. Clearly document any material that cannot be shared and the reason for the restriction.

## 19. Version control and protocol amendments

Use version control to track changes to the protocol, search strings, screening decisions, extraction form, analysis, and manuscript. Any substantive change after registration or the start of formal searching should be documented with:

- Date of amendment.
- Section or procedure changed.
- Previous and revised approach.
- Reason for the change.
- Whether the change was made before or after screening/results were known.

Do not silently change eligibility criteria or search limits after observing the results.

## 20. Protocol registration

Register the protocol on OSF Registries if that remains the selected registration route. Add the registration identifier and link to this document once registration is complete. Do not describe the protocol as registered before the registration has been completed.

## 21. Review status

At the time this protocol is prepared, the accompanying workbook specifies the search sources, draft queries, five research questions, and eligibility criteria. Final executed searches, screening, extraction, appraisal, and synthesis should be marked complete only after each activity has actually been performed. Update this section as the review progresses.

## 22. Authors

- **Tawseef Ahmed Teli** — ORCID: [0000-0001-8784-0923](https://orcid.org/0000-0001-8784-0923)
- **Aanisa Ali**
- **Hilal Ahmad Khanday**
