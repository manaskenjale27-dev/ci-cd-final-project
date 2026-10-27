# CI/CD Tools and Practices Final Project

This repository contains the template to be used for the Final Project for the Coursera course **CI/CD Tools and Practices**.

Repository name: `ci-cd-final-project`

## Setup

After entering the lab environment, run the setup script in the `./bin` folder to install the prerequisite software:

```bash
bash bin/setup.sh
```

Then exit the shell and start a new one for the Python virtual environment to be activated.

## Continuous integration

The GitHub Actions workflow is located at `.github/workflows/workflow.yml`. It installs dependencies, runs flake8 lint checks, and runs unit tests with nose.

## OpenShift Pipelines

The Tekton task definitions are located at `.tekton/tasks.yml`. They include a cleanup task and a nose unit-test task.

## License

Licensed under the Apache License. See [LICENSE](LICENSE).

## Author

Skills Network
