## Example Voting App Kubernetes

This is based on the original [example-voting-app](https://github.com/dockersamples/example-voting-app) repository from the [docker-examples](https://github.com/dockersamples) GitHub page

and modified it to work on the Kubernetes cluster.


brew install minikube
kubectl get po -A
minikube dsahboard
# first perform deployment so pods are active running and then create service (cluster IP) [redis and DB] then create service (NodePort) [voting-app and result-app]. 
kubectl create -f <all files> 
# first all 5 deployment
# second all 4 service
minikube service --all
minikube dashboard
