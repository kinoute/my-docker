# My Docker :whale:


## Everything related to Docker, containers, images, etc here :rocket:


#### Workspace


Name | Description | Command
:---: | :---: | :---:
[Tensorflow GPU](https://www.tensorflow.org/install/docker#gpu_support) | :zap: Container with Tensorflow-GPU latest version (nightly 2.0) and Jupyter Notebook | ```docker run --runtime=nvidia -it --rm tensorflow/tensorflow:latest-gpu-jupyter```
[ML Workspace](https://github.com/ml-tooling/ml-workspace) | :fire: Amazing all-in-one web-based IDE specialized for machine learning and data science | ```docker run -d -p 8091:8091 -v "${PWD}:/workspace" --restart always mltooling/ml-workspace:latest```


#### To-do


* [fast.ai](https://github.com/fastai/) | :rocket: Container with all fast.ai dependencies and Jupyter Notebook
* [VSCodium](https://github.com/VSCodium/vscodium) | :pencil: Containerized version of VSCodium
* ...
