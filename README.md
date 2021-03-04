# K8 Playground
This pretty simple repo was created in order to train and apply basics K8 concepts.

## Prerequisites
1. [Install minikube and its dependencies](https://minikube.sigs.k8s.io/docs/start/)

## Creating first Deployment

The "1-deployment" folder has MongoDB Deployment with mongo-express. The deployment is composed by:

1. mongodb
1.1. Internal service
2. K8 Secret
3. Config Map
4. mongo-express
4.1. External service

## Increasing Ingress

The "2-ingress" folder has MongoDB Deployment with mongo-express the ingress was increasead to treat requests from domain. The deployment is composed by:

1. mongodb
1.1. Internal service
2. K8 Secret
3. Config Map
4. mongo-express
4.1. External service
5. mongo-express-ingress

## Volumes (WIP)

## References
I read a lot of references mainly the K8 documentation but a didn't save them through the way(Lol). I strongly recommend the [TechWorld with Nana](https://www.youtube.com/watch?v=X48VuDVv0do).