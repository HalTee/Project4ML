[![CircleCI](https://dl.circleci.com/status-badge/img/gh/HalTee/Project4ML/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/HalTee/Project4ML/tree/main)


## Project Overview

This project  operationalizes a Machine Learning Microservice API.

A `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project operationalizes a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

## How to run the Python scripts and web apps
For example running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

## Files and their functions

1.kubernetes_out.txt - This is the ouput of a prediction made after running the ./make_prediction.sh script while the kubernetes pod is running.

2.docker_out.txt - This contains log info after the containerized application was run and a prediction was made 

3.run_kubernetes.sh -This script is used to  deploy the application using kubectl on kubernetes.

4.run_docker.sh - This script is used to run and build a docker image locally that is later uploaded to docker hub.
