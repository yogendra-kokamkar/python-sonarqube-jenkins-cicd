# Jenkins CI Pipeline for Python Project and SonarQube

![python-unittest-sonarqube-jenkins](https://github.com/yogendra-kokamkar/python-sonarqube-jenkins-cicd/assets/55878086/09319bd0-0f45-48b5-b52b-7c1e296e973f)

This repository contains the configuration for a Jenkins CI pipeline that performs the following tasks:
1. Checks in Python code.
2. Performs unit tests.
3. Generates a code coverage report.
4. Integrates the unit tests and code coverage with SonarQube.
5. Sends an email notification in case of pass or fail.

## Prerequisites

Ensure you have the following set up before running the pipeline:
- A Jenkins server with the following plugins installed:
  - Pipeline
  - Git
  - SonarQube Scanner
  - JUnit
  - Email Extension
- A SonarQube server configured and accessible.
- Python installed on the Jenkins agent with `pip` and the required dependencies (`pytest`, `pytest-cov`).

## Repository Structure

```plaintext
.
├── Jenkinsfile
├── src/
│   └── your_code.py
├── tests/
│   └── test_your_code.py
├── sonar-project.properties
└── requirements.txt
