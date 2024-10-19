# aws-etl-with-airflow documentation!

## Description

An end-to-end ETL project with AWS using Airflow in a  EC2 instance for data pipeline orchestration, S3 for storage and Amazon Redshipt for data warehouse

## Commands

The Makefile contains the central entry points for common tasks related to this project.

### Syncing data to cloud storage

* `make sync_data_up` will use `aws s3 sync` to recursively sync files in `data/` up to `s3://raw-data/data/`.
* `make sync_data_down` will use `aws s3 sync` to recursively sync files from `s3://raw-data/data/` to `data/`.


