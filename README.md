# US Visa Approval Prediction
This project focuses on predicting the approval status of US visa applications using machine learning. It is designed as a classification problem, leveraging various features related to applicants and visa types to determine whether a visa will be approved or denied.

### Problem Statement
The aim is to create a machine learning model that can classify US visa applications into two categories: approved or denied, using historical visa data.

### Machine Learning Model
The classification model used in this project is K-Nearest Neighbors (KNN). KNN is a simple yet effective algorithm for classification tasks. It predicts the class of a sample based on the majority class of its k-nearest neighbors.

### Why KNN?
It works well with smaller datasets.
KNN makes no assumptions about the data distribution.

## Workflow:

1. constants
2. entity
3. components
4. pipeline
5. Main file



### Export the  environment variable
```bash


export MONGODB_URL="mongodb+srv://<username>:<password>...."

export AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID>

export AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY>


```


# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

	
## 3. Create ECR repo to store/save docker image
    - Save the URI: 324037277821.dkr.ecr.eu-north-1.amazonaws.com/visa

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optinal

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

   - AWS_ACCESS_KEY_ID
   - AWS_SECRET_ACCESS_KEY
   - AWS_DEFAULT_REGION
   - ECR_REPO


## Screenshot
### Prediction Page
![App Screenshot](https://github.com/VigneshvickyData/Data_Branching/blob/main/us1.png?raw=true)

![App Screenshot](https://github.com/VigneshvickyData/Data_Branching/blob/main/us2.png?raw=true)

## Screenshot
### Result Page
![App Screenshot](https://github.com/VigneshvickyData/Data_Branching/blob/main/u3.png?raw=true)