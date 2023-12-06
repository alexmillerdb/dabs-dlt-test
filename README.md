# DABs, DLT, and GitHub Actions demo
_Intent of the demo is to showcase how customers can use DABs with DLT and automate CICD with GitHub Actions_

# DABs resources/files:
* [databricks.yml](https://github.com/alexmillerdb/dabs-dlt-test/blob/main/databricks.yml): Defines the bundle name, resources to include (DLT pipeline configuration), and `targets` to deploy (Databricks environments) 
* [resources/dlt_pipeline.yml](https://github.com/alexmillerdb/dabs-dlt-test/blob/main/resources/dlt_pipeline.yml): DLT pipeline configuration file to validate, deploy, and run across `targets` 

# GitHub Actions files:
* [dlt-job-actions-ci.yaml](https://github.com/alexmillerdb/dabs-dlt-test/blob/main/.github/workflows/dlt-job-actions-ci.yaml): GitHub Actions CI pipeline using self-hosted runner; triggers on Pull Request to main
* [dlt-job-actions-cd.yaml](https://github.com/alexmillerdb/dabs-dlt-test/blob/main/.github/workflows/dlt-job-actions-cd.yaml): GitHub Actions CD pipeline using self-hosted runner; triggers on push to main

# Additional links to help:
* [Adding self-hosted runners to repository, organization, enterprise](https://docs.github.com/en/enterprise-server@3.7/actions/hosting-your-own-runners/managing-self-hosted-runners/adding-self-hosted-runners)
* [About self-hosted runners](https://docs.github.com/en/enterprise-server@3.7/actions/hosting-your-own-runners/managing-self-hosted-runners/about-self-hosted-runners)
* [What are DABs](https://docs.databricks.com/en/dev-tools/bundles/index.html)
* [Databricks Asset Bundles DLT example](https://docs.databricks.com/en/delta-live-tables/tutorial-bundles.html)
* [MLOps Stacks Example](https://docs.databricks.com/en/dev-tools/bundles/mlops-stacks.html)
