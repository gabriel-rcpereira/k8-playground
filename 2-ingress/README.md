# Follow the steps below to create to second deployment using Ingress to access MongoExpress through URL

## Create Secret
`kubectl apply -f mongo-secret.yml`

## Create MongoDB Deployment and Internal Service
`kubectl apply -f mongo.yml`

## Create Configmap
`kubectl apply -f mongo-configmap.yml`

## Create MongoExpress Deployment and Internal Service(Load Balancer)
`kubectl apply -f mongo-express.yml`

**Make sure the service was created as ClusterIP:**
`kubectl get svc mongo-express-service`

## Create Ingress
`kubectl apply -f mongo-express-ingress.yml`

**Make sure Ingress was created and get the *ADDRESS* value. The value should be added into *hosts* file related to "mymongodbexpress.com" domain.**
`kubectl get ingress mongo-express-ingress`