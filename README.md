# Jenkins CI Pipeline for Python Project and SonarQube

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