# multi-k8s

/> minikube start

/> minikube start --vm-driver=virtualbox

/> minikube status

/> kubectl cluster-info

cd simplek8s
/> kubectl apply -f client-pod.yaml
/> kubectl apply -f client-node-port.yaml

/> kubectl get pods
/> kubectl get services
	
/> minikube ip

/> minikube delete

/> kubectl describe pod <pod-name>

/> kubectl delete -f client-pod.yaml


/> kubectl apply -f client-deployment.yaml
/> kubectl get deployments

/> kubectl describe deployment client-deployment

/> kubectl set image deployment/client-deployment client=susgupta/multi-client:v5

/> minikube docker-env
/> eval $(minikube docker-env)

/> kubectl logs name-of-pod
/> kubectl exec -it name-of-pod sh

/> kubectl get deployments
/> kubectl delete deployment <deployment-name>

/> kubectl get services
/> kubectl delete service <service-name>

/> kubectl get storageclass
/> kubectl describe storageclass


Persistent Volume and PersistentVolumeClaim
/> kubectl get pv
/> kubectl get pvc

Creating secrets
/> kubectl create secret generic pgpassword --from-literal PGPASSWORD=12345asdf
/> kubectl get secrets


ingress-nginx
Mandatory command: 
/> kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-0.31.1/deploy/static/provider/cloud/deploy.yaml

/> minikube addons enable ingress
/> make dev-env
/> kubectl get pods -n ingress-nginx


/> minikube dashboard
