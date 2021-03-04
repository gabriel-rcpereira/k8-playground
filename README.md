# K8 Playground

### Prerequisites
1. [Install minikube](https://minikube.sigs.k8s.io/docs/start/)

### Creating first Deployment

The "1-deployment" folder has MongoDB Deployment with mongo-express. The deployment is composed by:

1. mongodb
1.1. Internal service
2. mongo-express
2.1. External service
3. K8 Secret
4. Config Map

### Increasing Ingress

The "2-ingress" folder has MongoDB Deployment with mongo-express the ingress was increasead to treat requests from domain. The deployment is composed by:

1. mongodb
1.1. Internal service
2. mongo-express
2.1. External service
3. mongo-express-ingress
4. K8 Secret
5. Config Map

### Volumes (WIP)

### Services (WIP)

### References
I read a lot of references mainly the K8 documentation but a didn't save them through the way(Lol). I hugely recommend the [TechWorld with Nana](https://www.youtube.com/watch?v=X48VuDVv0do).