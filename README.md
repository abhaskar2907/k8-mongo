# k8-mongo
MongoDB Deployment on Kubernetes Cluster via DeploymentSet

namespace = mongo-deployment
kubectl get namespaces

Make sure   /data/db  exists on worker

kubectl apply -f pvc.yml -n mongo-deployment
kubectl get pvc -n mongo-deployment

kubectl apply -f deployment.yml -n mongo-deployment
kubectl get deployments -n mongo-deployment

kubectl apply -f service.yml -n mongo-deployment
kubectl get svc -n mongo-deployment


