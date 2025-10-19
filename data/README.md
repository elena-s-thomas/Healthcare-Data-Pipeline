# Data Directory Structure

## Local Development Storage
This directory is used for **local development and testing only**. 
**Primary storage is in Google Cloud Storage (GCS).**

## Raw Data (`data/raw/`)
Contains **small samples** of original data for local development and testing.

### CMS Synthetic Data (`data/raw/cms-synpuf/`)
- `sample_1/` - First sample of CMS DE-SynPUF data (for local development)
  - `beneficiary/` - Patient demographic and enrollment files (3 files per year)
  - `inpatient/` - Hospital admission claims data
  - `outpatient/` - Outpatient visit claims data  
  - `carrier/` - Physician services and procedures (2 files: A and B)
  - `pde/` - Prescription drug events (optional)

## Processed Data (`data/processed/`)
Contains **locally processed** data for testing before GCS upload.

### CMS Synthetic Data (`data/processed/cms-synpuf/`)
- Cleaned and transformed versions of raw data
- Files ready for GCS upload and BigQuery ingestion

## Cloud Storage Structure
- **GCS Raw**: `gs://<bucket>/raw/cms-synpuf/sample_1/`
- **GCS Processed**: `gs://<bucket>/processed/cms-synpuf/`

## File Naming Convention
- Raw files: Keep original CMS naming
- Processed files: Use descriptive names (e.g., `beneficiary_cleaned_2008.csv`)
