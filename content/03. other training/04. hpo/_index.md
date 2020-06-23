+++
title = "Automatic Model Tuning"
menuTitle = "HPO/Model Tuning"
weight = 40
+++

This demo shows how you can use [SageMaker Automatic Model Tuning](https://docs.aws.amazon.com/sagemaker/latest/dg/automatic-model-tuning.html) to find the best version of a model by running many training jobs on your dataset using the algorithm and ranges of hyperparameters that you specify. It can do that through either of random or bayesian search. If you have information from past tuning jobs, they can also be leveraged by Bayesian Search as a stronger prior.

We'll use an [Amazon SageMaker example](https://github.com/awslabs/amazon-sagemaker-examples/) to learn about SageMaker Experiments.

On your notebook instance, click on the SageMaker icon on the left bar to open the list of examples. 
![SageMaker Examples](/images/other_topics/sagemaker_examples.png)

Then scroll down to the ***SageMaker Python SDK > tf-eager-sm-scriptmode.ipynb*** and click on it. It's the last one.
![SM Model Tuning](/images/other_topics/hpo_example.png)

SageMaker will open a preview of the example on a new tab. Click on the **Create a Copy** button to get a complete working copy of the example.
![Create a Copy](/images/other_topics/example_create_copy.png) 

Confirm the prompt to create the folder with the notebook and any additional files.
![Confirm create copy](/images/other_topics/confirm_example_copy.png).

[This notebook](https://github.com/awslabs/amazon-sagemaker-examples/blob/master/sagemaker-python-sdk/tensorflow-eager-script-mode/tf-eager-sm-scriptmode.ipynb) will use a TensorFlow training script for a relatively complete workflow. The workflow includes local training and hosted training in SageMaker, as well as local inference and SageMaker hosted inference with a real time endpoint. Additionally, **Automatic Model Tuning** in SageMaker will be used to tune the model's hyperparameters. 

{{% notice note %}}
There are several other [Automatic Model Tuning examples](https://github.com/awslabs/amazon-sagemaker-examples/tree/master/hyperparameter_tuning) you can explore to learn more about this feature.
{{% /notice %}}