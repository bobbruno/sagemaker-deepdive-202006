+++
title = "SageMaker Experiments lab"
menuTitle = "Experiments"
weight = 30
+++

This demo shows how you can use [SageMaker Experiments](https://github.com/aws/sagemaker-experiments#sagemaker-experiments-python-sdk) to organize, track, compare, and evaluate your machine learning (ML) model training experiments. You can read more about it [on the SageMaker documentation](https://docs.aws.amazon.com/sagemaker/latest/dg/experiments.html).

We'll use an [Amazon SageMaker example](https://github.com/awslabs/amazon-sagemaker-examples/) to learn about SageMaker Experiments.

On your notebook instance, click on the SageMaker icon on the left bar to open the list of examples. 
![SageMaker Examples](/images/other_topics/sagemaker_examples.png)

Then scroll down to the ***SageMaker Experiments > mnist-handwritten-digits-classification-experiment.ipynb*** and click on it. 
![SM Experiments](/images/other_topics/experiments_example.png)

SageMaker will open a preview of the example on a new tab. Click on the **Create a Copy** button to get a complete working copy of the example.
![Create a Copy](/images/other_topics/example_create_copy.png) 

Confirm the prompt to create the folder with the notebook and any additional files.
![Confirm create copy](/images/other_topics/confirm_example_copy.png).

[This notebook](https://github.com/awslabs/amazon-sagemaker-examples/blob/master/sagemaker-experiments/mnist-handwritten-digits-classification-experiment.ipynb) shows how to use SageMaker Experiments to track and analyze several trials to find the impact of different modeling approaches. The [SageMaker Experiments SDK](https://sagemaker-experiments.readthedocs.io/en/latest/index.html) documentation shows how it can be used to track all components of each experiment trial.

{{% notice note %}}
SageMaker Experiments is also integrated into the SageMaker Studio interface. If you want to explore Studio, there are also [examples](https://github.com/awslabs/amazon-sagemaker-examples/tree/master/aws_sagemaker_studio) you can try on your own.
{{% /notice %}}