# simplek8s

## Kubectl commands

```shell script

kubectl get services

kubectl get pods

kubectl apply -f client-pod.yaml

kubectl describe pod

kubectl describe pod client-pod

kubectl delete -f <config file>

kubectl delete -f client-pod.yaml

kubectl get pod -o wide

kubectl set image <object_type>/<object_name> <container_name>=<new image to use>
kubectl set image deployment/client-deployment client=stephengrider/multi-client:v5

kubectl logs <pod name>

kubectl exec -it <pod name> sh
```

## Minikube commands

```shell script

minikube ip

```

## Docker commands

```shell script

docker build -t rostam63/multi-client .

docker push rostam63/multi-client

docker logs <container id>

docker exec -it <container id> sh

docker system prune -a 

```

### Reconfiguring Docker CLI

Reconfigure docker CLI to connect to docker instance inside Kubernetes node.

```shell script
eval $(minikube docker-env)
```
