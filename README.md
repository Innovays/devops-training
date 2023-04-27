[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Innovays/devops-training/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Innovays/devops-training/tree/main)

# Introduction:
In this project, I utilized the skills learned in a course to operationalize a Machine Learning Microservice API. The project involved using a pre-trained, sklearn model to predict housing prices in Boston based on several features such as average rooms in a home, data about highway access, teacher-to-pupil ratios, and more. This project tested my ability to operationalize a Python Flask app (in a provided file, app.py) that serves out predictions about housing prices through API calls. This project could be extended to any pre-trained machine learning model such as image recognition and data labeling.

# Project Motivation:
The motivation behind this project was to practically apply all the techniques and methods taught in the "Microservices at Scale using AWS & Kubernetes" module.

# Project Goal:
The goal of this project was to operationalize a working, machine learning microservice using Kubernetes, which is an open-source system for automating the management of containerized applications.

# Tech Stack:

- Python
- Flask
- Kubernetes
- Docker
- Linux
- Bash
- Pylint
- Hadolint
- CircleCI

# Tasks:
In this project, I completed the following tasks:

* (+) Tested the project code using linting
* (+) Completed a Dockerfile to containerize the application
* (+) Deployed the containerized application using Docker and made a prediction
* (+) Improved the log statements in the source code for this application
* (+) Configured Kubernetes and created a Kubernetes cluster
* (+) Deployed a container using Kubernetes and made a prediction
* (+) Uploaded a complete Github repo with CircleCI to indicate that the code has been tested

# How to Setup the Environment:

* Create a virtualenv with Python 3.7 and activate it.
      $  python3 -m venv ~/.vdevops-training
      $  source ~/.vdevops-training/bin/activate
* Install necessary dependencies (Basically on Linux: Docker & Python) .
      $  python3 -m pip install --upgrade
      $  python3 -m pip install --no-cache-dir -r requirements.txt 
* Run "make lint" to check for linting errors.

# Set the Environment-Variables
* Adjust the ".env"-file 


# Running in Docker:

* Run "./run_docker.sh" to start the docker container and create the Flask app within the container.
* Run "./make_prediction.sh" to make predictions.

# Running in Kubernetes Cluster:

Install Minikube and Virtualbox.
* Run "minikube start" to start a local cluster.
* Run "./run_kubernetes.sh" to start the Kubernetes pod and create the Flask app in the container.
* Run "./make_prediction.sh" to make predictions.
