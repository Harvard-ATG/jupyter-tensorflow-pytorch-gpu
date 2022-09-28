# jupyter-tensorflow-pytorch-gpu

Jupyter docker image built for data science courses that comes with Cuda drivers, TensorFlow and Pytorch with GPU support.

To use:

```
$ docker pull harvardat/jupyter-tensorflow-pytorch-gpu:latest
$ docker run --rm -p 8888:8888 jupyter-tensorflow-pytorch-gpu:latest
```

Note that the `Dockerfile` is adapted from the official [Tensorflow GPU docker image](https://hub.docker.com/r/tensorflow/tensorflow) as well as [Jupyter Docker Stacks](https://github.com/jupyter/docker-stacks). The base image `harvardat/tensorflow-gpu-base` (https://github.com/Harvard-ATG/jupyterhub-dockerfiles) includes the CUDA drivers, and this image installs additional dependencies/packages and configures the environment.
