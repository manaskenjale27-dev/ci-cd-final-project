# CI/CD Final Project

Project name: **CI/CD Tools and Practices Final Project**

This repository contains the sample application and CI/CD configuration for the Coursera CI/CD Tools and Practices final project.

## Continuous integration

GitHub Actions is configured in `.github/workflows/workflow.yml` to install dependencies, lint the Python service with flake8, and run unit tests with nose.

## OpenShift Pipelines

Tekton task definitions are in `.tekton/tasks.yml`. They include a cleanup task and a nose unit-test task. The OpenShift pipeline uses cleanup, git-clone, flake8, nose, buildah, and deploy steps.

## Application

The application is packaged with the repository's Dockerfile and is configured to listen on port 8000 in the container.

## Setup

Run the setup script in the lab environment:

```bash
bash bin/setup.sh
```

Then start a new shell so the virtual environment can be activated.

## License

Licensed under the Apache License 2.0. See [LICENSE](LICENSE).
