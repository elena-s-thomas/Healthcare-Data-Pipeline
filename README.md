# Healthcare Data Pipeline

### Steps
1. Initialize a Git repo with project scaffold based on the above YAML.
2. Start with Step 1: Write Jupyter notebooks for cleaning one of the selected datasets (e.g., CMS Synthetic).
3. Configure Google Cloud Storage buckets and prepare for data upload.
4. Set up Mage pipelines to orchestrate the ETL process end-to-end.
5. Validate transformations with SQL in BigQuery.
6. Deploy Looker Studio dashboard for minimal but useful insights


### Dataset: 
[CMS Medicare Claims Synthetic Data (DE-SynPUF)](https://www.cms.gov/data-research/statistics-trends-and-reports/medicare-claims-synthetic-public-use-files)

### GCP Project:
[healthcare-data-pipeline-raw](https://console.cloud.google.com/storage/browser/healthcare-data-pipeline-raw;tab=objects?forceOnBucketsSortingFiltering=true&project=shaped-totem-475620-f0&prefix=&forceOnObjectsSortingFiltering=false)