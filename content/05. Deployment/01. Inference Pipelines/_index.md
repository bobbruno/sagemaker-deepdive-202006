+++
title = "Inference Pipelines and Batch Transformations lab"
menuTitle = "Inference Pipelines"
weight = 10
+++

An [*inference pipeline*](https://docs.aws.amazon.com/sagemaker/latest/dg/inference-pipelines.html) is an Amazon SageMaker model that is composed of a linear sequence of two to five containers that process requests for inferences on data. You use an inference pipeline to define and deploy any combination of pretrained Amazon SageMaker built-in algorithms and your own custom algorithms packaged in Docker containers.

In this example we'll see how to chain a Spark ML feature engineering set of transformations to an XGBoost model to create an ML Product. We'll also see how AWS Glue can be used to run managed Spark without having to start and stop a cluster manually. This example sends a pySpark script (`abalone_processing.py`) to AWS Glue for processing. Once it is run (it will take some time to start the Spark engine to process the script), you can proceed with training the XGBoost model on the transformed data.

To start the lab: on your notebook instance, click on the SageMaker icon on the left bar to open the list of examples. 
![SageMaker Examples](/images/other_topics/sagemaker_examples.png)

Then scroll down to the ***Advanced Functionality > inference_pipeline_sparkml_xgboost_abalone.ipynb*** and click on it. It's close to the bottom of the sidebar.
![Managed Spot TensorFlow](/images/deployment/inference_pipeline_example.png)

SageMaker will open a preview of the example on a new tab. Click on the **Create a Copy** button to get a complete working copy of the example.
![Create a Copy](/images/other_topics/example_create_copy.png) 

Confirm the prompt to create the folder with the notebook and any additional files.
![Confirm create copy](/images/other_topics/confirm_example_copy.png).