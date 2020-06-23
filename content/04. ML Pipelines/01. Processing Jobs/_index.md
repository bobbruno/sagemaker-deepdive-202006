+++
title = "Processing Jobs"
menuTitle = "Processing Jobs"
weight = 10
+++

With [SageMaker Processing Jobs](https://docs.aws.amazon.com/sagemaker/latest/dg/processing-job.html), you can use a simplified, managed experience on Amazon SageMaker to run your data processing workloads, such as feature engineering, data validation, model evaluation, and model interpretation. You can also use the Amazon SageMaker Processing APIs during the experimentation phase and after the code is deployed in production to evaluate performance.

![Processing Jobs](/images/ml_pipelines/processing_job.png)

In the diagram above you can see that a processing job is just an orchestration of containers managed by SageMaker, with defined input and output points. If your transformations are based on [scikit-learn](https:scikit-learn.org), you can just provide a transformation script (as shown in [the documentation](https://docs.aws.amazon.com/sagemaker/latest/dg/use-scikit-learn-processing-container.html)).

But you can also [create your own transformations](https://docs.aws.amazon.com/sagemaker/latest/dg/use-your-own-processing-code.html), and we'll see two examples of that, which you can reuse for your own pipelines.

- Processing data using Spark
- Processing data using Dask