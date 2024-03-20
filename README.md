
# Predicting Data Exfiltration via DNS

## Overview
This repository consists of development of machine learning models capable of predicting data exfiltration attempts via DNS queries. 

It includes the following model types:
- Standard Static ML model
- ML model that adapts to patterns in real-time

## Set Up
- [Install `Docker` and `Docker-compose` on your system](https://docs.docker.com/get-docker/)
- Run docker script on your system, once docker is installed.
    - [docker_script.bat](docker_script.bat) for windows
    - [docker_script.sh](docker_script.sh) for Linux/MacOS
    
## Contents
- `Static Model .ipynb`: Implementation for static model including data preprocessing, feature engineering, and model training processes.
- `Dynamic Model .ipynb`: Implementation for dynamic model which includes real-time data processing and adaptive learning mechanisms.
- `Kafka_dataset.csv`: Dataset for the dynamic model training that simulates **real-time DNS query data through Kafka streams**.
- `Static_dataset.csv`: Dataset for the static model training to analyze historical DNS query data.
- `docker-compose.yml`: Docker Compose configuration file for setting up the Kafka streaming environment required for the dynamic model's data processing.
- `docker_script.bat`, `docker_script.sh`: Scripts to help set up the Docker environment on Windows and Unix-based systems, respectively.
- `requirements.txt`: Specifies the Python package dependencies necessary to run the project.

### Prerequisites
- Docker installed on your machine.
- Python 3.x along with Jupyter or any compatible IDE for running the notebooks.

### Setup
1. **Environment Preparation**: Begin by setting up the Kafka environment using Docker. Utilize the provided `docker_script.bat` for Windows or `docker_script.sh` for Unix/Linux systems to automate the setup.
2. **Install Dependencies**: Install the Python dependencies specified in `requirements.txt` by running the following command:
   ```
   pip install -r requirements.txt
   ```
3. **Run the Notebooks**: Navigate to the `.ipynb` notebooks in Jupyter or your preferred IDE. Ensure the Kafka environment is up and running before executing the dynamic model notebook.

## Highlights
- Implemented classifier for predicting DNS-based data exfiltration, achieving an impressive accuracy rate of over 90% through meticulous data analysis and feature engineering.
- Demonstrated expertise in dynamic model creation by implementing a cutting-edge solution capable of adapting in real-time, showcasing a remarkable improvement of 15% in detection accuracy compared to static models.
- Leveraged ML techniques to uncover nuanced patterns in streaming data, resulting in a dynamic model with a 20% increase in sensitivity to emerging threats


## License
[MIT](https://choosealicense.com/licenses/mit/)

