+++
title = "Introduction to Distributed Training"
menuTitle = "Distributed Training Intro"
weight = 10
chapter = false
+++

In a typical machine learning development workflow, there are two main stages where you can get benefit from scaling out.

![parallel distributed](/images/intro/parallel_distributed.png)

1. Running large-scale parallel experiments: In this scenario our goal is to find the best model/hyperparameters/network architecture by exploring a space of possibilities. From the user perspective, this is just starting new jobs without having to wait for the previous ones to finish.
2. Running distributed training of a single model: In this scenario our goal is to train a single model faster, by distributing its computation across nodes in a cluster. This requires at least small adaptations to the training code to handle parallelism and synchronization between compute nodes.

This workshop will cover both types of parallelism. We'll practice how to leverage Horovod for parallel distributed training of a single large model; then we'll see how we can leverage the power of SageMaker-managed infrastructure to run experiments and hyperparameter optimization in parallel.
