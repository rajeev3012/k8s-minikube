
Cluster setup and Application deployment:-

1. Kubernetes Cluster Setup with Minikube:
	• Set up a local Kubernetes cluster using Minikube.
	• Minikube creates a lightweight cluster with a single node for development and testing purposes.


2. Containerization of a Node App:
	• Containerize Node.js application using Docker.
	• Write a Dockerfile that specifies the app’s dependencies, base image, and build instructions.
	• Build the Docker image using docker build -t my-node-app .

		# npm init -y
		# npm install express
		
		# docker build -t rajeev301212/node-app:1.0 .
   

3. Pushing the Docker Image to Docker Hub:
	• Create an account on Docker Hub (hub.docker.com).
	• Tag local image with Docker Hub username and repository name (e.g., docker tag my-node-app username/my-node-app).
	• Push the image to Docker Hub using docker push username/my-node-app.

		# docker push rajeev301212/node-app:1.0
				
		# docker login -u rajeev301212


4. Kubernetes Manifests:
	• Write Kubernetes manifests (e.g., deployment.yaml and service.yaml) for Node app.
	• Define the deployment, service, and other necessary resources in these YAML files.

		# kubectl apply -f deployment.yaml
		# kubectl apply -f service.yaml
		    	
		# kubectl get deployments
		# kubectl get pods
		# kubectl get services


5. Accessing the Deployed App:
	• Deploy your app to the Kubernetes cluster using kubectl apply -f deployment.yaml.
	• Expose the app using a service with kubectl apply -f service.yaml.
	• Access the deployed app in your browser by navigating to the service’s external IP or domain.

       	# minikube services node-app-service


