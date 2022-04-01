# docker-teradatasqlalchemy

A Docker image that extends the official Python image and adds `teradatasqlalchemy`.
## Building

The dockerfile is parametrized. You need to specify PYTHON_VERSION and TERADATASQLALCHEMY_VERSION to build the image:

```
docker build --build-arg PYTHON_VERSION=3.9 --build-arg TERADATASQLALCHEMY_VERSION=17.10.0.9 -t teradata/teradatasqlalchemy:latest .
podman build --build-arg PYTHON_VERSION=3.9 --build-arg TERADATASQLALCHEMY_VERSION=17.10.0.9 -t teradata/teradatasqlalchemy:latest .
```