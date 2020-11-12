SideCar Pattern
Sidecar containers are the containers that should run along with the main container in the pod. This sidecar pattern extends and enhances the functionality of current containers without changing it. Nowadays, We know that we use container technology to wrap all the dependencies for the application to run anywhere. A container does only one thing and does that thing very well.
Imagine that you have the pod with a single container working very well and you want to add some functionality to the current container without touching or changing, how can you add the additional functionality or extending the current functionality? This sidecar container pattern really helps exactly in that situation.

Process to start the Minikube :
minikube start

Create the pod
kubectl create -f pod.yml

Exec into pod
kubectl exec -it sidecar-container-demo -c main-container -- /bin/sh

Install curl
apt-get update && apt-get install -y curl

Launch localhost
curl localhost
