# Setup
https://kubernetes.io/docs/setup/learning-environment/minikube/

# Tutorial
https://kubernetes.io/docs/tutorials/hello-minikube/


# To run:

docker build -t bradebarrows/nodeapp:v1 .

docker push bradebarrows/nodeapp:v1

# to not push https://stackoverflow.com/questions/42564058/how-to-use-local-docker-images-with-minikube
# Set the imagePullPolicy to Never

kubectl apply -f nodeapp.yaml   
kubectl apply -f deployment.yaml   