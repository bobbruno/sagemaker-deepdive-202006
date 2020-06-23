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

* Download the workshop code and notebooks. Enter bash (optional), change directory to ~/SageMaker, clone the repository
```bash
cd ~/SageMaker
wget distributed_labs.zip
unzip distributed_labs.zip
```
* Confirm that you're able to see the contents. Should see 3 parts
```
ls distributed_labs
```
