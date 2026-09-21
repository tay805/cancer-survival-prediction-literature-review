Systematic Literature Review Protocol

Cancer Survival Prediction Using Machine Learning and Deep Learning

Protocol Version: 1.0
Protocol Date: 21 September 2026
Review Type: Systematic Literature Review (SLR) with a comparative analysis of baseline survival models
Registration: OSF Registries (identifier to be added upon registration)

1. Review Background

Cancer survival prediction is an important area of clinical research because accurate estimation of survival-related outcomes can support risk stratification, treatment planning, clinical decision-making, and patient management.

The increasing availability of clinical, genomic, molecular, imaging, radiomic, pathological, and multi-omics data has created opportunities for machine learning and deep learning approaches to model complex relationships associated with cancer survival.

Machine learning and deep learning methods have been applied across different cancer types, datasets, data modalities, and survival outcomes. However, the literature varies substantially in terms of modelling approaches, input data, validation strategies, evaluation metrics, and reporting practices.

Newly proposed methods are commonly benchmarked against established baseline survival models. The relative performance of these baselines is difficult to assess from individual studies, because comparisons are made on different cohorts, under different validation protocols, and against different comparators.

This systematic literature review examines the existing research on machine learning and deep learning approaches for cancer survival prediction, synthesizes the methodological characteristics, evidence, limitations, and research gaps across the field, and analyses how established baseline models perform relative to one another under controlled conditions.

2. Review Objective

The objective of this systematic literature review is to systematically identify, classify, evaluate, and synthesize research on cancer survival prediction using machine learning and deep learning approaches, with particular emphasis on cancer types, patient populations, datasets, data modalities, prediction outcomes, modelling techniques, validation strategies, evaluation metrics, explainability, limitations, and research gaps.

In addition, the review conducts a comparative analysis of predefined comparator survival models, using within-study comparisons reported in the included studies, to determine how these models perform relative to one another when the dataset, validation protocol, and evaluation metric are held constant. A separate comparative analysis examines within-study performance comparisons among predefined survival-model comparators.

3. Research Questions

RQ1

What machine learning and deep learning techniques have been used for cancer survival prediction?

RQ2

What cancer types, patient populations, and datasets have been investigated for cancer survival prediction?

RQ3

What types of data and features have been used for cancer survival prediction?

RQ4

What survival outcomes and evaluation metrics, including measures of discrimination and calibration, have been used to assess cancer survival prediction models?

RQ5

What validation strategies, including internal and external validation, have been used to evaluate cancer survival prediction models?

RQ6

What explainability and interpretability methods have been applied to cancer survival prediction models, and how have they been evaluated?

RQ7

What methodological limitations and research gaps are evident in existing cancer survival prediction studies?

RQ8

How do established baseline survival models perform relative to one another when they are compared within the same study, on the same cohort, under the same validation protocol and evaluation metric?

4. Review Scope

The review focuses specifically on machine learning and deep learning approaches used for cancer survival prediction.

The review considers studies involving human cancer populations or datasets derived from human cancer patients.

The review covers different cancer types and cancer subtypes rather than restricting the analysis to a particular cancer.

The review considers clinical, demographic, genomic, molecular, imaging, radiomic, pathological, multi-omics, and multimodal data.

The review considers survival and related time-to-event outcomes, including overall survival, disease-free survival, progression-free survival, recurrence-free survival, cancer-specific survival, disease-specific survival, mortality, and other clearly defined cancer-related time-to-event outcomes.

The review also examines predefined comparator survival models as they are compared within the included studies (Section 19).

5. Machine Learning and Deep Learning Scope

The review includes studies that use machine learning or deep learning as a component of cancer survival prediction.

Machine learning approaches may include, but are not limited to:

Random Forest

Random Survival Forest

Support Vector Machine

Gradient Boosting

XGBoost

LightGBM

Decision Tree

k-Nearest Neighbours

Other supervised machine learning approaches

Deep learning approaches may include, but are not limited to:

Artificial Neural Networks

Deep Neural Networks

Convolutional Neural Networks

Recurrent Neural Networks

Long Short-Term Memory networks

Gated Recurrent Units

Autoencoders

Transformers

DeepSurv

DeepHit

Other neural survival models

Hybrid and multimodal approaches involving machine learning or deep learning are also considered.

Traditional statistical survival models without a machine learning or deep learning component are outside the primary scope of the review.

Traditional statistical methods may be reported as comparator or baseline methods within an eligible machine learning or deep learning study.

5.1 Operational Definition of Machine Learning and Deep Learning

A study falls within the machine learning and deep learning scope when at least one model whose survival predictions are evaluated in the study meets one of the following conditions:

The model is a tree-based or ensemble method, a kernel method, an instance-based method, a Bayesian or probabilistic graphical model, or a neural network of any architecture.

The model uses features learned by a deep learning model, including pretrained or foundation-model embeddings, even when the final survival component is a Cox model.

The following are classified as statistical models and do not by themselves bring a study into scope: Cox proportional hazards models (including stratified, time-varying, and spline-based variants), penalised Cox regression (LASSO, ridge, elastic net), parametric and accelerated failure time models, logistic regression, and nomograms derived from these models.

Machine learning used only for feature selection or preprocessing does not bring a study into scope when the evaluated predictive model is a statistical model.

Statistical models remain eligible as comparators within an in-scope study and as predefined comparators in the comparative analysis (Section 19.2).

6. Population and Data

The review considers studies involving human cancer populations or datasets derived from human cancer patients.

Eligible data sources may include:

Clinical databases

Electronic health records

Cancer registries

Public cancer datasets

Genomic databases

Molecular datasets

Medical imaging datasets

Radiomics datasets

Digital pathology datasets

Multi-omics datasets

Institutional patient cohorts

Multi-centre patient cohorts

Synthetic datasets that do not represent an appropriate human cancer population are outside the primary scope of the review.

7. Survival Outcomes

Eligible studies address at least one cancer-related survival or time-to-event outcome.

These include:

Overall survival (OS)

Disease-free survival (DFS)

Progression-free survival (PFS)

Recurrence-free survival (RFS)

Cancer-specific survival (CSS)

Disease-specific survival (DSS)

Mortality

Time to recurrence

Time to progression

Other clearly defined cancer-related time-to-event outcomes

Studies focused exclusively on cancer diagnosis, detection, classification, segmentation, staging, or treatment response without a relevant survival outcome are outside the primary scope.

Studies that model survival as a binary or categorical outcome at a fixed time horizon are eligible. They are identified during data extraction and analysed separately from studies that model time-to-event outcomes with censoring.

8. Eligibility Criteria

A study is eligible for inclusion when it satisfies the following criteria:

The study concerns cancer, malignant neoplasms, or a defined cancer type or subtype.

The study involves a human cancer population or a dataset derived from human cancer patients.

The study addresses cancer survival or a clearly defined cancer-related time-to-event outcome.

The study develops, evaluates, compares, or applies a machine learning or deep learning approach that meets the operational definition in Section 5.1.

The study provides sufficient methodological information to identify the data, modelling approach, and relevant outcomes.

The study is published as a peer-reviewed journal article or peer-reviewed full conference paper. Preprints are not eligible.

The study is written in English.

The study is published between 1 January 2015 and the final database search date in 2026.

9. Exclusion Criteria

A study is excluded when one or more of the following conditions apply:

The study does not concern cancer.

The study does not involve a human cancer population or a dataset derived from human cancer patients.

The study does not address cancer survival or a relevant time-to-event outcome.

The study focuses exclusively on cancer diagnosis, detection, classification, segmentation, staging, or treatment response without a relevant survival outcome.

No model whose survival predictions are evaluated in the study meets the operational definition of machine learning or deep learning in Section 5.1. This includes studies that rely exclusively on conventional statistical survival modelling.

The publication is a review article, systematic review, meta-analysis, editorial, commentary, letter, opinion article, or other secondary or non-primary publication.

The publication is a conference abstract without sufficient methodological information.

The publication is a book chapter, thesis, dissertation, or other non-eligible publication type.

The publication is a preprint that has not undergone peer review.

The publication is not written in English.

The publication falls outside the defined publication period.

The record is a duplicate of another identified publication.

The publication does not contain sufficient information for the planned data extraction.

10. Publication Period

The review considers publications dated from 1 January 2015 through the final database search date in 2026.

The start date captures the emergence of deep learning approaches to survival analysis and the rapid growth of machine learning applications in cancer survival prediction. Studies published before this date are outside the scope of the review.

The exact final search date is recorded when the database searches are conducted.

11. Information Sources

The literature search uses the following scholarly databases:

Scopus

Web of Science

PubMed/MEDLINE

IEEE Xplore

ScienceDirect

Peer-reviewed conference proceedings are identified through Scopus, Web of Science, and IEEE Xplore. Proceedings that are not indexed in these sources are not searched.

No other information sources are searched, apart from the supplementary search methods specified in Section 12.3.

12. Search Strategy

12.1 Search Concepts

The search strategy is developed around three concepts, combined with the Boolean operator AND:

Cancer

Survival prediction or survival analysis

Machine learning and deep learning

12.2 Draft Search String

The draft search string for Scopus is given below. It is tested in the pilot search (Section 12.4) and finalised before the formal searches are conducted.

TITLE-ABS-KEY ( cancer* OR tumor* OR tumour* OR neoplas* OR carcinoma*
    OR malignan* OR oncolog* )
AND TITLE-ABS-KEY ( "survival prediction" OR "survival analysis"
    OR "survival model*" OR "prognostic model*" OR "prognosis prediction"
    OR "time-to-event" OR "overall survival" OR "disease-free survival"
    OR "progression-free survival" OR "recurrence-free survival"
    OR "cancer-specific survival" OR "disease-specific survival"
    OR mortality OR death )
AND TITLE-ABS-KEY ( "machine learning" OR "deep learning"
    OR "neural network*" OR "random survival forest*" OR "random forest*"
    OR "gradient boost*" OR xgboost OR lightgbm OR "support vector"
    OR transformer* OR convolutional OR autoencoder* OR deepsurv
    OR deephit )
AND PUBYEAR > 2014
AND LANGUAGE ( english )
AND DOCTYPE ( ar OR cp )


The string is translated into the syntax of each other database. Each translation preserves the three concepts and the limits on publication year, language, and document type.

12.3 Supplementary Search Methods

The following supplementary methods are used:

Backward citation searching of the reference lists of all studies included in the systematic review.

Forward citation searching of all studies included in the systematic review, using the citation index of Scopus.

Screening of the reference lists of review articles identified during screening. Review articles are not themselves included.

Records identified through supplementary methods are screened against the same eligibility criteria and reported as a separate stream in the PRISMA flow diagram.

12.4 Pilot Search

A pilot search is run in Scopus before the formal searches are conducted. The number of records retrieved is recorded.

The pilot search evaluates whether the draft search strategy retrieves known relevant studies identified during the preliminary, non-systematic reading of the literature and whether the search concepts retrieve relevant terminology used in the field.

Any change to the search strategy or review scope resulting from the pilot search is documented as a protocol amendment before the formal searches begin.

12.5 Search Documentation

For each information source, the following are recorded in the search/ directory:

Database name and search platform

Date on which the search was run

Complete search string exactly as executed

Limits and filters applied

Number of records retrieved

13. Study Identification

Records retrieved from the selected information sources are collected and retained as the initial literature set.

The original database exports are preserved in the data/raw/ directory where technically and legally appropriate.

Each study is assigned a unique study identifier for use throughout the screening, extraction, and analysis processes.

14. Duplicate Management

Duplicate records identified across databases are documented and removed from the screening set.

Duplicate identification uses bibliographic information such as DOI, database identifiers, title, authors, publication year, and other available metadata.

When a conference paper and an extended journal version of the same study are both identified, the more complete version is retained and the records are linked.

When a preprint and its peer-reviewed version are both identified, the peer-reviewed version is retained and the preprint is treated as a duplicate.

The relationship between duplicate records and the retained study record is preserved where appropriate.

15. Screening Process

15.1 Screening Tool

Screening is conducted using [screening tool to be confirmed]. Screening records are maintained in the data/screening/ directory.

15.2 Calibration

Before screening begins, all screening reviewers independently screen a calibration set of 50 randomly selected records against the eligibility criteria. Agreement is measured with Cohen's kappa.

When kappa is below 0.61, the eligibility criteria and their interpretation are clarified, and the calibration exercise is repeated with a new set of records before screening continues.

15.3 Title and Abstract Screening

Two reviewers independently screen the title and abstract of every record against the eligibility criteria.

Records included by at least one reviewer proceed to full-text screening. Records that cannot be confidently excluded based on title and abstract are retained for full-text assessment.

15.4 Full-Text Screening

Two reviewers independently assess the full text of every potentially eligible study against the eligibility criteria.

Disagreements are resolved by discussion. Disagreements that remain unresolved are decided by a third reviewer.

Each excluded study is assigned the first applicable reason from the following hierarchy:

Not cancer

Not a human cancer population

No relevant survival outcome

Statistical model only (Section 5.1)

Ineligible publication type, including preprints

Insufficient information

Outside the publication period

Not in English

15.5 Decision Rule for the Machine Learning Criterion

Screeners apply the following sequence:

Identify the model or models whose survival predictions the study evaluates.

If any is a tree-based, ensemble, kernel, instance-based, Bayesian, or neural model, the study meets the machine learning criterion.

Otherwise, if any uses features learned by a deep learning model, the study meets the criterion.

Otherwise, the study is excluded with the reason "statistical model only".

Records that cannot be classified from the title and abstract are retained for full-text screening.

15.6 Reporting of Agreement

Cohen's kappa and percentage agreement are reported for the calibration exercise, title and abstract screening, and full-text screening.

16. Data Extraction

16.1 Extraction Procedure

Structured data are extracted from studies that satisfy the final eligibility criteria, using an extraction form that is piloted on five included studies before full extraction begins.

One reviewer extracts data from all included studies. A second reviewer independently extracts data from a random 20% sample of included studies. Agreement is reported, and discrepancies are resolved by discussion.

All numeric performance values are verified against the source publication. Values that appear only in figures are flagged.

The structured extraction data are maintained in the data/extraction/ directory.

16.2 Extraction Variables

The extraction process records bibliographic, methodological, computational, dataset, outcome, validation, and performance characteristics.

The extraction variables include, where applicable:

Study identification

Authors

Publication year

Publication type

Country

Cancer type

Cancer subtype

Study population

Dataset

Data source

Sample size

Data modality

Clinical features

Genomic features

Molecular features

Imaging features

Radiomic features

Pathological features

Multi-omics features

Prediction target

Survival endpoint

Survival modelling formulation (time-to-event with censoring, or fixed-horizon classification)

Handling of censoring

Machine learning method

Deep learning architecture

Hybrid modelling approach

Preprocessing

Feature selection

Model development

Validation strategy

External validation

Evaluation metrics

Discrimination metric variant (Harrell, Uno, time-dependent)

Calibration measures

Reported performance

Baseline and comparator models

Performance of each model in each comparison instance

Cohort and feature set per comparison instance

Validation protocol per comparison instance

Tuning procedure for baseline models

Source of baseline results (produced by the authors or copied from previous work)

Location of reported values (table, text, or figure)

Explainability method

Evaluation of explainability

Code and data availability

Reported limitations

Research gaps

16.3 Counting Rule for Evaluation Metrics

A metric is recorded as reported when the study gives a numeric value of that metric for at least one of its own models. A metric that is named, defined, or discussed without a numeric value for the study's own models is not recorded as reported.

17. Quality Assessment

Risk of bias and applicability are assessed using PROBAST+AI.

One reviewer assesses all included studies. A second reviewer independently assesses a random 20% sample of included studies and all studies included in the comparative analysis (Section 19). Disagreements are resolved by discussion, and unresolved disagreements are decided by a third reviewer.

TRIPOD+AI is used as the reference standard when extracting the reporting of discrimination, calibration, and validation.

The assessment criteria and results are documented in the repository.

18. Evidence Synthesis

The included studies are synthesized using descriptive analysis and the comparative analysis specified in Section 19.

The synthesis considers:

Publication trends

Cancer types

Datasets

Sample sizes

Data modalities

Machine learning methods

Deep learning architectures

Survival outcomes

Evaluation metrics

Validation strategies

External validation

Explainability

Methodological limitations

Research gaps

Quantitative summaries are used where the extracted data support meaningful aggregation. Every proportion is reported with its denominator.

Studies that model survival as fixed-horizon classification are summarised separately from studies that model time-to-event outcomes with censoring.

Performance values are not pooled across studies, and no meta-analysis is planned, because the included studies are expected to differ substantially in cohorts, cancer types, validation protocols, and metric variants. Synthesis follows the Synthesis Without Meta-analysis (SWiM) reporting guideline.

Qualitative synthesis is used to compare methodological approaches, findings, limitations, and research trends.

Risk of bias results are presented descriptively and are used in the sensitivity analyses of the comparative analysis.

19. Comparative Analysis of Baseline Models

19.1 Rationale

Performance values reported in different studies are not directly comparable, because they depend on the cohort, cancer type, censoring rate, validation protocol, and variant of the evaluation metric. The comparative analysis therefore uses only within-study comparisons, in which these factors are held constant by the original authors. Performance values are not pooled across studies.

19.2 Predefined Comparator Models

Predefined comparator models are defined in advance as the following models, grouped into two families.

Statistical, machine learning, and neural survival models:

Cox proportional hazards

Penalised Cox regression (LASSO, ridge, elastic net)

Random Survival Forest

Gradient-boosted survival models

Survival Support Vector Machine

DeepSurv

Cox-nnet

DeepHit

Whole-slide image and multimodal survival models:

ABMIL

TransMIL

DeepAttnMISL

PORPOISE

MCAT

MOTCat

SurvPath

This list is fixed at the protocol date. Any change is recorded as a protocol amendment.

Cox proportional hazards is a statistical model rather than a machine learning method. It is included here as a predefined comparator, consistent with Section 5.

19.3 Eligibility for the Comparative Analysis

An included study contributes to the comparative analysis when it satisfies all of the following:

At least two established baselines are evaluated in the same comparison.

The compared models are evaluated on the same cohort and feature set, under the same data split or cross-validation protocol.

The baseline results are produced by the study's authors on that split, rather than copied from a previous publication, unless the study states that the split is identical.

A numeric discrimination value is reported for each compared model.

The discrimination metric is Harrell's C-index, Uno's C-index, time-dependent C-index, or time-dependent AUC, and the variant is recorded.

The performance of each study's own proposed model is extracted for context. It is excluded from the predefined comparator comparisons.

19.4 Unit of Analysis

A comparison instance is a set of models evaluated on one cohort and feature set under one protocol within one study. A study may contribute more than one instance. Instances from the same study are not treated as independent.

19.5 Synthesis Method

The comparative analysis follows the SWiM reporting guideline and uses vote counting based on direction of effect.

The primary analysis is conducted at the study level. For each pair of baselines, a study is classified as favouring one model when that model achieves the higher discrimination value in the majority of the study's instances in which both models appear. Otherwise the study is recorded as a tie.

Within an instance, identical values at the reported precision are recorded as ties.

Instance-level tallies are reported as a secondary analysis and are explicitly labelled as non-independent.

The magnitude of each difference is reported as the difference in the discrimination metric, summarised by median and range for each pair of baselines.

Formal statistical testing is not planned, because instances are clustered within studies and the number of eligible studies per pair is expected to be small. Where at least ten studies inform a given pair, a sign test on study-level outcomes may be reported as exploratory.

19.6 Calibration

Where a study reports a calibration measure, such as the Brier score or integrated Brier score, for two or more established baselines, the same procedure is applied to that measure separately. Pairs for which the discrimination and calibration results favour different models are reported.

19.7 Sensitivity Analyses

The primary analysis is repeated under the following restrictions:

Instances using Harrell's C-index only.

Excluding values read from figures rather than tables or text.

Excluding studies that do not describe how the baselines were tuned.

Excluding studies at high overall risk of bias under PROBAST+AI.

19.8 Comparison-Specific Risk of Bias

For each instance, the review records whether the baselines were tuned and how, whether baseline results were produced by the authors or copied from previous work, and where each value appears in the publication. These variables are used to interpret the results and to define the sensitivity analyses.

20. Analysis and Visualization

The analysis uses structured data maintained in the repository.

Where applicable, computational scripts are used to generate analytical tables and figures.

Figures and tables remain traceable to their underlying datasets and analysis procedures.

Analysis resources are maintained in the analysis/ directory, while generated figures and tables are maintained in the figures/ and tables/ directories.

21. Reporting

The review is reported in accordance with PRISMA 2020, including the PRISMA 2020 for Abstracts checklist.

The literature search is reported in accordance with PRISMA-S.

The synthesis, including the comparative analysis, is reported in accordance with SWiM.

The study-selection process is documented using a PRISMA 2020 flow diagram. The diagram reports records identified from databases and from supplementary methods as separate streams, and reports the reasons for exclusion at full-text screening.

The final manuscript reports the search methodology, study-selection process, characteristics of included studies, evidence synthesis, comparative analysis, limitations, and research gaps.

22. Data and Research Materials

Bibliographic records, screening data, extracted study characteristics, analytical resources, figures, tables, and other research materials that can legally and ethically be shared are maintained in this repository.

Copyrighted full-text publications are not redistributed through the repository.

No patient-level personal or sensitive data are included in the repository.

23. Version Control

The review materials are maintained using Git and GitHub.

Changes to the protocol, literature database, screening records, extraction data, analysis, figures, tables, and manuscript are tracked through version control.

Major stable versions of the review materials are preserved through GitHub Releases and archived through Zenodo.

24. Protocol Registration

The protocol is registered on OSF Registries before the formal database searches are conducted. The registration identifier is added to this document upon registration.

25. Protocol Amendments

Any substantive methodological change made after the protocol is registered is documented in the repository.

Protocol amendments include the date, affected methodological component, reason for the change, and description of the modification.

The repository history provides an additional record of changes to the review methodology.

26. Review Status

The protocol has been finalised. The pilot search, formal database searches, screening, data extraction, analysis, and synthesis have not yet been conducted. These activities are conducted according to the methodology documented in this protocol.

Development of this protocol was informed by a preliminary, non-systematic reading of the literature by the authors. Studies known from that reading are included only when they are identified through the database searches or the supplementary search methods specified in this protocol.

27. Authors

Tawseef Ahmed Teli
ORCID: https://orcid.org/0000-0001-8784-0923

Aanisa Ali

Hilal Ahmad Khanday