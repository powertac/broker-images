# PowerTAC Broker Images

This repository contains Dockerfiles for building Docker images for use with the
[PowerTAC Experiment Scheduler](https://github.com/powertac/powertac-experiment-scheduler).

## Requirements

The Docker command line interface is required to build the broker images. Please refer to the Docker documentation for
installation details: [Install Docker Engine - Docker Documentation](https://docs.docker.com/engine/install/).

## Building an image

Use the `docker build` command to build an image:

```bash
$ docker build -t IMAGE_NAME:IMAGE_TAG BROKER_IMAGE_PATH
```

- `IMAGE_NAME`: name of the created image (lowercase)
- `IMAGE_TAG`: tag of the created image (lowercase); can be omitted and defaults to `latest`
- `BROKER_IMAGE_PATH`: path to the directory containing the Dockerfile

To build AgentUDE17's image you can use this command, for example:

```bash
$ docker build -t agentude:2017 ./agentude17
```

## Adding an images

Please create a pull request if you want to add an image to this repository.
