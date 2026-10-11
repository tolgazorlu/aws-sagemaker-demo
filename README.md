# AWS SageMaker Demo

A single-script walkthrough of training and deploying an XGBoost binary classifier on Amazon SageMaker.

## About
Demonstrates the end-to-end SageMaker workflow: provisioning an S3 bucket, loading the UCI bank marketing dataset, splitting train/test data, and training an XGBoost estimator. Built June 2022 as a learning exercise with the AWS SageMaker tutorial dataset.

## Features
- Creates an S3 bucket for training artifacts
- Downloads and prepares the bank marketing dataset
- Trains an XGBoost classifier via `sagemaker.estimator.Estimator`
- Region-aware selection of the XGBoost container image

## Tech stack
- Python
- boto3, sagemaker SDK
- pandas, numpy, matplotlib

## Getting started
Requires an AWS account with SageMaker and S3 access, run from a SageMaker notebook instance or an environment with the SageMaker SDK and AWS credentials configured.

```bash
pip install boto3 sagemaker pandas numpy matplotlib
python sagemaker-demo.py
```

Edit `bucket_name` in `sagemaker-demo.py` to a globally unique S3 bucket name before running.

## Status
Learning project, course work from the AWS SageMaker tutorial. Not maintained.
