+++
title = "Spot training lab"
menuTitle = "Spot training"
weight = 10
+++

We'll use an [Amazon SageMaker example](https://github.com/awslabs/amazon-sagemaker-examples/) to learn how to use spot instances for training jobs. Managed Spot Training uses Amazon EC2 Spot instance to run training jobs instead of on-demand instances. You can specify which training jobs use spot instances and a stopping condition that specifies how long Amazon SageMaker waits for a job to run using Amazon EC2 Spot instances. These result in savings of up to 90%.

![Spot Instances](/images/intro/spot_instances.png)

Spot instances can be interrupted with a 2-minute warning, and the training script has to be able to save and restore its state to resume training. You can configure your managed spot training job to use checkpoints for that. Amazon SageMaker copies checkpoint data from a local path to Amazon S3. When the job is restarted, Amazon SageMaker copies the data from Amazon S3 back into the local path. Let's see how spot training works.

On your notebook instance, click on the SageMaker icon on the left bar to open the list of examples. 
![SageMaker Examples](/images/other_topics/sagemaker_examples.png)

Then scroll down to the *** SageMaker Python SDK > managed_spot_training_tensorflow_estimator.ipynb *** and click on it. It's close to the bottom of the sidebar.
![Managed Spot TensorFlow](/images/other_topics/managed_spot_tf.png)

SageMaker will open a preview of the example on a new tab. Click on the **Create a Copy** button to get a complete working copy of the example.
![Create a Copy](/images/other_topics/example_create_copy.png) 

Confirm the prompt to create the folder with the notebook and any additional files.
![Confirm create copy](/images/other_topics/confirm_example_copy.png).

The example is based on another that's been deprecated, but it illustrates the concept of spot training well. The original example can still be found on [another branch](https://github.com/awslabs/amazon-sagemaker-examples/blob/workshop/sagemaker-python-sdk/tensorflow_iris_dnn_classifier_using_estimators/tensorflow_iris_dnn_classifier_using_estimators.ipynb) of the repository.