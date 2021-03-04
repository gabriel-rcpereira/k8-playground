# Follow the steps below to create to second deployment using Ingress to access MongoExpress through URL

## Create Secret
`kubectl apply -f mongo-secret.yml`

## Create MongoDB Deployment and Internal Service
`kubectl apply -f mongo.yml`

## Create Configmap
`kubectl apply -f mongo-configmap.yml`

## Create MongoExpress Deployment and Internal Service(Load Balancer)
`kubectl apply -f mongo-express.yml`

**Make sure the service was created:**
`kubectl get svc mongo-express-service`

## Enable a tunnel to access MongoExpress
`minikube tunnel`

**The *route* will show a public IP to access the MongoExpress through the 3000 port.**