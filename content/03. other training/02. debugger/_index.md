+++
title = "SageMaker Debugger lab"
menuTitle = "Debugger"
weight = 20
+++

[Amazon SageMaker Debugger](https://github.com/awslabs/sagemaker-debugger) is a new feature which offers the capability to debug machine learning models during training by identifying and detecting problems with the models in real-time.

We'll use an [Amazon SageMaker example](https://github.com/awslabs/amazon-sagemaker-examples/) to learn about SageMaker Debugger.

On your notebook instance, click on the SageMaker icon on the left bar to open the list of examples. 
![SageMaker Examples](/images/other_topics/sagemaker_examples.png)

Then scroll down to the *** SageMaker Debugger > tf2-keras-default-container.ipynb *** and click on it. It's close to the bottom of the sidebar.
![SM Debugger](/images/other_topics/debugger_example.png)

SageMaker will open a preview of the example on a new tab. Click on the **Create a Copy** button to get a complete working copy of the example.
![Create a Copy](/images/other_topics/example_create_copy.png) 

Confirm the prompt to create the folder with the notebook and any additional files.
![Confirm create copy](/images/other_topics/confirm_example_copy.png).

[This notebook](https://github.com/awslabs/amazon-sagemaker-examples/blob/master/sagemaker-debugger/tensorflow2/tensorflow2_zero_code_change/tf2-keras-default-container.ipynb) shows how to use the SageMaker Debugger without making any changes to the training script and using a built-in rule to monitor your training job using a tf.keras (TF 2.1.0) ResNet example.

{{% notice note %}}
SageMaker Debugger has several other examples. If you want to explore more, you can find them [here](https://github.com/awslabs/amazon-sagemaker-examples/tree/master/sagemaker-debugger).
{{% /notice %}}