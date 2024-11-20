# MongoDB-Python-Flask-Web-Framework-REST-API-GKE

Overview This project demonstrates deploying a MongoDB database using Persistent Volumes on Google Kubernetes Engine (GKE), developing a Node.js application to interact with the database, and creating a Python Flask REST API for a bookshelf application. Both applications are containerized and deployed to GKE, with their configurations managed through ConfigMaps and exposed externally via Ingress.

Prerequisites

Google Cloud SDK

kubectl

Docker

Node.js and npm

Python and pip

Step 1: Set Up the GKE Cluster

1. Create a GKE Cluster
2. Create a Persistent Volume for MongoDB
3. Deploy MongoDB
4. Expose MongoDB

Step 2: Deploy the Student Server Application

Develop the Student Server Application: Follow the instructions to create studentServer.js.
Containerize the Application: Create a Dockerfile, build the Docker image, and push it to DockerHub.
Deploy to GKE: Apply the deployment and service YAML files for the student server application.

Step 3: Deploy the Bookshelf Flask API

Develop the Bookshelf Flask API: Follow the guide to create bookshelf.py.
Containerize the Flask API: Similar to the student server, create a Dockerfile, build the image, and push it to DockerHub.
Deploy to GKE: Apply the deployment and service YAML files for the bookshelf application.

Step 4: Configuration Management

Create ConfigMaps: Prepare and apply ConfigMaps for both applications to externalize the MongoDB connection details.

Step 5: Expose Applications Using Ingress

Setup Ingress: Enable the Ingress controller in Minikube and apply the Ingress service YAML file.
Verify Access: Ensure that the applications are accessible through the configured paths on the Ingress.
Accessing the Applications Student Server: Access the student server application using curl or a web browser through the defined Ingress path. Bookshelf API: Similarly, access the bookshelf API to perform CRUD operations on book records.
