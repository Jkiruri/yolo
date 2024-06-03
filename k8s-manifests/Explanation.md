# Project description

This project utilizes Node.js for the backend, React for the frontend, and MongoDB as the database. Both the frontend and backend are packaged into Docker images, which are then containerized using Docker and orchestrated with Kubernetes.

# Set up process

# Tech stack

- `Docker`: Used for containerizing the frontend, backend, and database.
- `Kubernetes`: Used for orchestration.
- `kubectl`: CLI tool to interact with Kubernetes.

With the environment set and requirements met, below commands helps achieve the desired objectives.

- `kubectl apply -f mongopv.yaml`
- `kubectl apply -f mongopvc.yaml`
- `kubectl apply -f mongo.yaml`
- `kubectl apply -f mongo-service.yaml`
- `kubectl apply -f backend-deployment.yaml`
- `kubectl apply -f backend-service.yaml`
- `kubectl apply -f client-deployment.yaml`
- `kubectl apply -f client-service.yaml`

