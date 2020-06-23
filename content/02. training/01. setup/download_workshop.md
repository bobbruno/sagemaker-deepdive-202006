---
title: "Download the workshop content"
date: 2019-10-28T00:14:06-07:00
weight: 20
---
### Launch JupyterLab client and clone the workshop repository
* Your notebook instance should now be ready. Click *JupyterLab* to launch your client.
![launch jupyter](/images/setup/launch_jupyter.png)

* Click *File > New >  Terminal* to launch terminal in your JupyterLab instance.
![Launch terminal](/images/setup/launch_terminal.png)

{{% attachments %}}

* Download the workshop code and notebooks. Change directory to ~/SageMaker, download and unzip the labs file. If the `wget` command doesn't work, try copying the link above and using it as the `wget` parameter.
```bash
cd ~/SageMaker
wget https://master.dmbqjbidi9r7o.amplifyapp.com/02.%20training/01.%20setup/download_workshop.files/distributed_labs.zip
unzip distributed_labs.zip
```
* Confirm that you're able to see the contents. Should see 3 parts
```
ls distributed_labs
```
