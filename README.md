# Overview
This project involved the orchestration of a containerized application using Google Kubernetes Engine (GKE).


# Requirements
Have a Google Cloud Account.
Kubernetes CLI (kubectl) is installed on your Local Machine
Install Google cloud CLI to interact with the cloud directly from local development.
- [gcloud CLI](https://cloud.google.com/sdk/docs/install#deb) 
Have the application containerized and pushed to docker hub as shown below:

![Alt text](image.jpeg)

# The steps on the deployment are:
## create manifest file for deployment to GKE

    1. Deploy the backend and frontend:
     
       kubectl apply -f backend-deployment.yaml
       kubectl apply -f frontend-deployment.yaml

    2.  Check the status of the pods:
       
       kubectl get pods

    3. Get the external IP of the frontend service:
       
       kubectl get svc frontend-service

# Test Your Application
    • Visit the external IP of the frontend service in your browser.
    
     [Live URL] (http://34.38.147.47:80)
