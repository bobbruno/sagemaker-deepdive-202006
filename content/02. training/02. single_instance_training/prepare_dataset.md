+++
title = "Prepare training dataset"
weight = 20
+++
### Download the CIFAR10 dataset and upload it to Amazon S3

On a terminal window in JupyterLab client, navigate to the notebook directory

```
cd ~/SageMaker/sagemaker-workshop-202006/notebooks/
```
Activate the TensorFlow conda environment
```
source activate tensorflow_p36
```
{{% notice info %}}
Before running the command above, you may have to run "`. /home/ec2-user/anaconda3/etc/profile.d/conda.sh`".
{{% /notice %}}

Download CIFAR10 dataset and convert it to TFRecords format
```
python generate_cifar10_tfrecords.py --data-dir dataset
```
Confirm that the dataset was downloaded successfully. Run:
```
sudo yum install tree -y
tree dataset
```
You should see the following output
```
dataset
├── eval
│   └── eval.tfrecords
├── train
│   └── train.tfrecords
└── validation
    └── validation.tfrecords
```

Create a new S3 bucket starting with _sagemaker-_ and upload the dataset to it. Be sure to add a unique identifier, such as your account id.
```
aws s3 mb s3://<your_bucket>
```
{{% notice warning %}}
**Note:** Bucket names should be unique globally. If a bucket with the same name already exists, add another unique identifier such as today's date or your last name.
{{% /notice %}}
{{% notice info %}}
Make a note of the name of the bucket you created. We'll need it when we prepare SageMaker for training.
{{% /notice %}}

Proceed only if you don't see an error. Now, upload the dataset to S3
```
aws s3 sync dataset/ s3://<your_bucket>/cifar10-dataset/
```
