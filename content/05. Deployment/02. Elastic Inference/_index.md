+++
title = "Elastic Inference Lab"
menuTitle = "Elastic Inference"
weight = 20
+++

Elastic Inference allows you to fine-tune the GPU resources according to your needs. Deep learning typically requires much more computational power during training than during inference. At the same time, inference workloads run for much longer (usually 24x7), rapidly accumulating costs. With Elastic Inference, you can deploy your model with a much finer-grained control over how much GPU it will actually have - and a cost that can be up to 75% cheaper. Elastic Inference is straightforward to use and supports:

- TensorFlow
- Pytorch through TorchScript (see [post on how-to](https://aws.amazon.com/blogs/machine-learning/reduce-ml-inference-costs-on-amazon-sagemaker-for-pytorch-models-using-amazon-elastic-inference/))
- MXNet

In this example we'll see how simple it is to deploy a model using elastic inference instead of a GPU-enabled instance.

To start the lab: on your notebook instance, click on the SageMaker icon on the left bar to open the list of examples. 
![SageMaker Examples](/images/other_topics/sagemaker_examples.png)

Then scroll down to the ***SageMaker Python SDK > tensorflow_serving_pretrained_model_elastic_inference.ipynb*** and click on it. It's close to the bottom of the sidebar.
![Managed Spot TensorFlow](/images/deployment/ei_example.png)

SageMaker will open a preview of the example on a new tab. Click on the **Create a Copy** button to get a complete working copy of the example.
![Create a Copy](/images/other_topics/example_create_copy.png) 

Confirm the prompt to create the folder with the notebook and any additional files.
![Confirm create copy](/images/other_topics/confirm_example_copy.png).

{{% notice note %}}
The example still uses the 1st generation of Elastic Inference (_EIA1_). Where available, EIA2 is the second generation of Elastic Inference accelerators. It offers improved performance and increased memory for a [lower price](https://aws.amazon.com/machine-learning/elastic-inference/pricing/).
{{% /notice %}}