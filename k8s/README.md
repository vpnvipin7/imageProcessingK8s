# Local execution plan ( WINDOWS vs MINIKUBE )

1) Install minikube from minikube.sigs.k8s.io/docs/start/
2) This will start the minikube locally. minimum memory should be 2GB.
    minikube start --memory=4000 
3) Run the enviorment command
    minikube docker-env
4) For windows OS run eval cmd as below 
    @FOR /f "tokens=*" %i IN ('minikube -p minikube docker-env') DO @%i


Now build the images inside the minikube docker image by running docker-compose build
