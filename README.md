# Setup
https://kubernetes.io/docs/setup/learning-environment/minikube/

# Tutorials
https://kubernetes.io/docs/tutorials/hello-minikube/

## For docker + kubernetes

https://www.linode.com/docs/applications/containers/kubernetes/deploy-container-image-to-kubernetes/#build-the-docker-image

# To run:

NOTE: Replace bradebarrows with ur username. You must be running docker locally and be logged in:
'''docker login'''

## Getting it running:
```
docker build -t bradebarrows/nodeapp:v1 .
docker push bradebarrows/nodeapp:v1
#to not push https://stackoverflow.com/questions/42564058/how-to-use-local-docker-images-with-minikube
#Set the imagePullPolicy to Never
kubectl apply -f nodeapp.yaml   
kubectl apply -f deployment.yaml   
```