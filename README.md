# Reddit Clone App on Kubernetes with Ingress
This project demonstrates how to deploy a Reddit clone app on Kubernetes with Ingress and expose it to the world using Minikube as the cluster.
Below is an overview of the architecture of this Reddit Clone App running on Kubernetes with Ingress.
![Architecture Diagram] ![ultmate-kubernetes project](https://github.com/user-attachments/assets/be0212e9-5842-474f-b7ad-a3fa0f555ee2)


## Prerequisites
Before you begin, you should have the following tools installed on your local machine: 

- Docker
- Powershell if you want to try..
- kubectl
- Git

## Installation
Follow these steps to install and run the Reddit clone app on your local machine:

1) Clone this repository to your local machine: `git clone https://github.com/I-Am-Jigyanshu/reddit-clone-k8s-project`
2) Navigate to the project directory: `cd reddit-clone-k8s-project`
3) Build the Docker image for the Reddit clone app: `docker build -t reddit-clone-app .`
4) Deploy the app to Kubernetes: `kubectl apply -f deployment.yaml`
5) Deploy the Service for deployment to Kubernetes: `kubectl apply -f service.yaml`
6) Expose the app as a Kubernetes service: `kubectl expose deployment reddit-deployment --type=NodePort --port=3000`
7) Create an Ingress resource: `kubectl apply -f ingress.yaml`


## Project Points for Resume 📝

- **Project**:  Automating the Delivery of Highly Scalable Reddit Clone Application using CI/CD Pipeline with Docker, Docker Hub, and Kubernetes Minikube

- **Description**: As part of a software development project, I designed and implemented a robust continuous integration (CI) and continuous deployment (CD) pipeline for a Reddit clone application. The pipeline incorporated Docker, Docker Hub, and Kubernetes Minikube technologies to achieve a seamless, automated flow from code changes to deployment.

- For the CI component, I set up an automated pipeline that integrated code changes from the development team and tested them before pushing the updated container images to Docker Hub. This ensured that any changes made were thoroughly tested before deployment, thus improving the overall quality of the application.

- To ensure optimal performance, I also implemented monitoring and logging functionalities to identify and troubleshoot any issues that may arise. The pipeline was designed with automation in mind, minimizing manual interventions and reducing the likelihood of human errors.

- Key technologies used: Docker, Docker Hub, Kubernetes, Minikube, CI/CD, Containerization, Automation, Monitoring, Logging, Reddit Clone Application.

  Final Result : when we browse to the localhost with port 3000..
  reddit app..
  ![jigyanshu reddit ss](https://github.com/user-attachments/assets/33057af5-236f-434d-b85d-806882605114)


