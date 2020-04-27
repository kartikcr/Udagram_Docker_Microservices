# Udagram_Docker_Microservices
In this project, I developed a cloud-based application for uploading and filtering images with micro-service architecture.
Created and deployed this instagram like service with 2 Microservices: Feed and User, and deploying them using Docker and Kubernetes

Udagram Image Filtering Microservice:
a. Using AWS Elastic BeanStalk, deploy a complete end to end application which is a Node-Express application that runs script to process images, using a Node-Express server as a RestAPI Backend and a basic ionic client web app which consumes this RestAPI.
b. Added user authentication using AWS IAM and security by applying JWT to to Restrict Endpoint Usage
c. Backend using PostgreSQL and AWS RDS.

Udagram Image Filtering Microservice
Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

The project is split into three parts:

The Simple Frontend A basic Ionic client web application which consumes the RestAPI Backend. [Covered in the course]
The RestAPI Backend, a Node-Express server which can be deployed to a cloud service. [Covered in the course]
The Image Filtering Microservice, the final project for the course. It is a Node-Express application which runs a simple script to process images. [Your assignment]
Tasks
Setup Node Environment
You'll need to create a new node server. Open a new terminal within the project directory and run:

Initialize a new project: npm i
run the development server with npm run dev
Create a new endpoint in the server.ts file
The starter code has a task for you to complete an endpoint in ./src/server.ts which uses query parameter to download an image from a public URL, filter the image, and return the result.

We've included a few helper functions to handle some of these concepts and we're importing it for you at the top of the ./src/server.ts file.

import {filterImageFromURL, deleteLocalFiles} from './util/util';
Deploying your system
Follow the process described in the course to eb init a new application and eb create a new environment to deploy your image-filter service! Don't forget you can use eb deploy to push changes.

Overview of the Project Tasks
You have to start with the "Udagram - photo sharing" Monolith application and divide the application into smaller (micro)services. Each microservice must run in a separate Docker container. These containers (and ReplicaSets) have to be managed by using the Kubernetes cluster. You have to demonstrate the ability to independently scale-up, release, and deploy the project using Kubernetes, and TravisCI.

Pre-requisites
Has experience using Git and GitHub
Basic Linux Skills
Basic programming skills in Javascript and Python
Some familiarity with:
RESTful APIs
Web development (HTML, CSS, DNS)
