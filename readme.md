# Basic App

- created a basic express API that returns `Hello World`, running on port 3000
- added a Docker file, that relies on Node base image and exposes port 3000

# Image buid/test locally

- cd SomeTestAPI
- docker build -t sometestapi .
- docker run -d -p 3000:3000 sometestapi

# Deploying to Docker Hub

- docker login
- docker tag sometestapi aimalkhan26/sometesapi:latest
- docker push aimalkhan26/sometesapi:latest
- docker pull aimalkhan26/sometesapi:latest
- docker run -d -p 3000:3000 aimalkhan26/sometesapi:latest

# Deploying to Kubernetes