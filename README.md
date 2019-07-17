# My Docker :whale:


## Everything related to Docker, containers, images, etc here :rocket:


#### Workspace


Name | Description | Command
:---: | :---: | :---:
[Portainer](https://www.portainer.io) | :whale: Awesome Docker management | ```docker volume create portainer_data```<br>:point_down:<br>```docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer```<br>:point_down:<br>http://localhost:9000
[Tensorflow GPU](https://www.tensorflow.org/install/docker#gpu_support) | :zap: Container with Tensorflow-GPU latest version (nightly 2.0) and Jupyter Notebook | ```docker run --runtime=nvidia --rm nvidia/cuda nvidia-smi```<br>:point_down:<br>```docker run --runtime=nvidia -it --rm tensorflow/tensorflow:latest-gpu-jupyter```
[ML Workspace](https://github.com/ml-tooling/ml-workspace) | :fire: Amazing all-in-one web-based IDE specialized for machine learning and data science | ```docker run -d -p 8091:8091 -v "${PWD}:/workspace" --restart always mltooling/ml-workspace:latest```<br>:point_down:<br>http://localhost:8091
[VSCode Server](https://github.com/cdr/code-server) | :pencil: Run VS Code on a remote server | ```docker run -it -p 127.0.0.1:8443:8443 -v "${PWD}:/home/coder/project" codercom/code-server --allow-http --no-auth```<br>:point_down:<br>http://localhost:8443


#### To-do


* [fast.ai](https://github.com/fastai/) | :rocket: Container with all fast.ai dependencies and Jupyter Notebook
* Dockerize some GUI applications
* ...