![CircleCI](https://img.shields.io/circleci/build/gh/aberdean/project-ml-microservice-kubernetes)

## Project Overview

This project containerizes a machine learning Python flask app using Docker and deploys it on a Kubernetes cluster.
The app predicts housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. The data was initially taken from [Kaggle](https://www.kaggle.com/c/boston-housing).

---

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Making predictions
In a separate terminal, run: `./make_prediction.sh`

---

### Project Structure
The project includes 4 directories:
- model_data containing the machine learning models
- output_txt_files containing the output of running a prediction on Docker and on Kubernetes
- .circleci containing the configuration file to implement CI/CD through CircleCI
- .git containing the git files
It also includes the following files:
- app.py the main Python flask app
- Dockerfile to define a Docker container
- LICENSE containing info on the license
- Makefile to build the project
- make_prediction.sh to run predictions
- README.md this file
- requirements.txt containing the dependencies that are installed through the Makefile
- run_docker.sh to launch a Docker container
- run_kubernetes.sh to deploy containers on a Kubernetes cluster
- upload_docker.sh to upload a Docker image to Docker Hub
- .gitignore to list files that Git should ignore

---

## Authors
 - Antonella Bernobich Dean - [aberdean](https://github.com/aberdean)

## License
This project is licensed under the MIT License - see the [LICENSE](https://github.com/aberdean/static/blob/master/LICENSE) file for details.

