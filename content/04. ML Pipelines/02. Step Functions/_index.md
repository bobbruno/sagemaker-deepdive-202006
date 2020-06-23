+++
title = "Step Funcions and the DS SDK"
menuTitle = "Step Functions"
weight = 20
+++

This lab describes how to use the AWS Step Functions Data Science SDK to create a machine learning model retraining workflow. The Step Functions SDK is an open source library that allows data scientists to easily create and execute machine learning workflows using AWS Step Functions and Amazon SageMaker. 

A Step Function is an implementation of a state machine as an executable orchestration, and can be represented as a directed graph, as below:
![Step Function](/images/ml_pipelines/step_function.gif). Step Functions can execute the following logics:

- Execute a [Task](https://docs.aws.amazon.com/step-functions/latest/dg/amazon-states-language-task-state.html) (including integrations with SageMaker, Lambda, AWS Glue and [several other AWS Services](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-service-integrations.html))
- Make a [Choice](https://docs.aws.amazon.com/step-functions/latest/dg/amazon-states-language-choice-state.html) on which step to continue execution
- Signal a [Failure](https://docs.aws.amazon.com/step-functions/latest/dg/amazon-states-language-fail-state.html) or a [Successful](https://docs.aws.amazon.com/step-functions/latest/dg/amazon-states-language-succeed-state.html) execution
- [Wait](https://docs.aws.amazon.com/step-functions/latest/dg/amazon-states-language-wait-state.html) for an event
- Execute several tasks in [Parallel](https://docs.aws.amazon.com/step-functions/latest/dg/amazon-states-language-parallel-state.html)
- Dynamically iterate through [Mapping](https://docs.aws.amazon.com/step-functions/latest/dg/amazon-states-language-map-state.html)

They also keep a full log of each execution and can be monitored online. For more information, please see the following resources:

- [AWS Step Functions](https://aws.amazon.com/step-functions/)
- [AWS Step Functions Developer Guide](https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html)
- [AWS Step Functions Data Science SDK](https://aws-step-functions-data-science-sdk.readthedocs.io)

In this notebook, we will use the DS SDK to create steps that capture and transform data using [AWS Glue](https://aws.amazon.com/glue/), incorporate this data into the training of a machine learning model, deploy the model to a SageMaker endpoint, link these steps together to create a workflow, and then execute the workflow in AWS Step Functions.

To start the lab: on your notebook instance, click on the SageMaker icon on the left bar to open the list of examples. 
![SageMaker Examples](/images/other_topics/sagemaker_examples.png)

Then scroll down to the ***Step Functions Data Science SDK > automate_model_retraining_workflow.ipynb*** and click on it. It's close to the bottom of the sidebar.
![Step Functions](/images/ml_pipelines/step_functions_example.png)

SageMaker will open a preview of the example on a new tab. Click on the **Create a Copy** button to get a complete working copy of the example.
![Create a Copy](/images/other_topics/example_create_copy.png) 

Confirm the prompt to create the folder with the notebook and any additional files.
![Confirm create copy](/images/other_topics/confirm_example_copy.png).

{{% notice warning %}}
Due to changes in the Jupyter Lab interface handling, it's not possible to see the Step Function diagrams directly in the notebook. The code works with no problems in Jupyter Lab, but if you want to see the diagrams, that functionality works using the Jupyter classic interface. You may want to open the Jupyter classic interface after copying the example. <br>
That can be done through the menu, at ***Help > Launch Classic Notebook***.
{{% /notice%}}

