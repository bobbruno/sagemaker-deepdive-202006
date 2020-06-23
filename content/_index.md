---
title: "SageMaker Deep Dive for Adidas"
chapter: true
weight: 1
---

## Welcome to the SageMake Deep Dive workshop.

This workshop has the following agenda:

### 1. Training

- Develop your training script using the **Notebook->Local->Training job** pattern.
- Leverage **Horovod** in your training script to run **distributed parallel** training across many instances
- Leverage **Spot Training** and **Checkpoints** to reduce costs and save your training Progress
- Select and use **GPU** instances to train deep learning models faster
- Use **Amazon SageMaker Debugger** on your training jobs to identify deviations, inspect the model's internals and solve problems faster
- Use **Amazon SageMaker Experiments** to track, compare and manage model training trials
- Use **Amazon SageMaker Automatic Model Tuning** to find optimized hyperparameters for your model.


### 2. Pipelines, Orchestration and Deployment

- Create **Inference Pipelines** with several models chained as one ML Product
- Learn how to use **Batch Transform** to do bulk inference on offline files
- Create **Amazon SageMaker Processing Jobs** to prepare your data for training and/or inference:
  - Using **SparkML**
  - Using **Dask**
- Use **Step Functions** to orchestrate the automation of complex ML Pipelines.