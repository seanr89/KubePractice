# KubePractice
Repo support to test out kubernetes etc..


## Commands

docker build
```
docker build . -t bun-app:latest
```

# Kubernetes

tools
1. kubectl (cli)
2. minikube

## Commands

allow minikube to access local docker-env
```
eval $(minikube docker-env)
```

start minikube access to registry
```
minikube start --insecure-registry true
```

Open and load the dashboard
```
minikube dashboard
```

Stop minikub
```
minikube stop
```

deploy the pod etc
```
kubectl apply -f pod.yml
```

ideas
```
kubectl get svc
```

Get pods
```
kubectl get pods
```

Access into kube
```
kubectl -exec -it bun-app -- /bin/bash
```

Port forwarding for remote out of app
```
kubectl port-forward bun-app 5000:5000
```

Go grab stuff
```
minikube service kubernetes --url
```


## Links
1. [minikube-url](https://minikube.sigs.k8s.io/docs/handbook/accessing/)
2. [docker-local](https://stackoverflow.com/questions/40144138/pull-a-local-image-to-run-a-pod-in-kubernetes)
3. [guide](https://zeet.co/blog/kubernetes-deployment-history)
4. [youtube-guide](https://www.youtube.com/watch?v=r8Z8yO5x-Zw&t=59s)
5. [another-guide](https://www.youtube.com/watch?v=i7PFg6aVcdI)