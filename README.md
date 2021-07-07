### Install Docker
    https://docs.docker.com/desktop/

### Install minikube
    https://minikube.sigs.k8s.io/docs/start/

### Start-up
    - Start Docker engine
    - Run `minikube start` from command line
    - Verify by running `minikube status` from command line         


### kubectl apply commands in order
    
    kubectl apply -f mongo-secret.yaml
    kubectl apply -f mongo.yaml
    kubectl apply -f mongo-configmap.yaml 
    kubectl apply -f mongo-express.yaml

### give a URL to external service in minikube

    minikube service mongo-express-service

### kubectl get commands

    kubectl get pod
    kubectl get pod --watch
    kubectl get pod -o wide
    kubectl get service
    kubectl get secret
    kubectl get all | grep mongodb

### kubectl debugging commands

    kubectl describe pod mongodb-deployment-xxxxxx
    kubectl describe service mongodb-service
    kubectl logs mongo-express-xxxxxx
