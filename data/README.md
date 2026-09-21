# Data

This directory contains the datasets developed for the cancer survival prediction literature review.

## Directory Structure

### `raw/`

This directory contains the master bibliographic database and source-level literature records.

The master database contains information such as:

* Study ID
* Authors
* Publication year
* Title
* Journal or conference
* Publication type
* DOI
* Database or source
* Other bibliographic information

### `screening/`

This directory contains records associated with the screening and eligibility assessment of the identified publications.

The screening records document:

* Title and abstract screening
* Full-text screening
* Inclusion and exclusion decisions
* Reasons for exclusion
* Reviewer decisions, where applicable

### `extraction/`

This directory contains the structured information extracted from studies included in the review.

The extraction data include information related to:

* Cancer type
* Cancer subtype
* Dataset
* Data source
* Sample size
* Data modality
* Clinical features
* Genomic features
* Imaging and radiomic features
* Prediction target
* Survival endpoint
* Machine learning methods
* Deep learning architectures
* Preprocessing methods
* Feature selection
* Validation strategy
* Evaluation metrics
* External validation
* Explainability methods
* Reported limitations

## Data Management

The datasets are maintained under Git version control.

Changes to the datasets are recorded through GitHub commits, allowing the development and modification of the literature database and extracted evidence to be tracked over time.

## Data Privacy and Copyright

The repository contains bibliographic information and research data extracted from published literature.

Copyrighted full-text articles are not redistributed through this repository.

No patient-level personal or sensitive data are stored in this repository.

## Reproducibility

The datasets provide the structured evidence base for the analysis presented in the associated literature-review manuscript.
