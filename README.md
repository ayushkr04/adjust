# adjust
STEP:1 - BUILD DOCKER IMAGE

Inorder to build the docker image, run the command:
docker build -t ayush0404/ruby:v1

I have saved the image in my Dockerhub.
A good practice is to store in the image in the private container registry. For example: We can store the images in the
Google container registry in GCP.

STEP:2:

Create a deployment manifest file with the created docker image.
Create the deployment using "kubectl create -f deployment.yaml"
Create 2 different service to expose the deployment.
Create the service using "kubectl create -f service.yaml"
Create hpa for the deployment.
Create the hpa using "kubectl create -f hpa.yaml"
Create an ingress with "kubectl create -f ingress.yaml"
