# Kubernetes Demo

## Install Docker
 
 - https://docs.docker.com/desktop/install/windows-install/

Build docker image
```ps
docker build . -t weatherapi-image
```
Run docker image
```ps
docker run -p 8080:8080 weatherapi-image
```
Build docker image for `quangnt1702` repo Docker Hub
```ps
docker build . -t quangnt1702/weatherapi-image:v1
```
Push docker image to `quangnt1702` repo Docker Hub
```ps
docker push quangnt1702/weatherapi-image:v1
```
## Install Kubernetes on Docker Desktop

- https://docs.docker.com/desktop/kubernetes/

```ps
kubectl apply -f deployment.yaml
```
```ps
kubectl get all
```
```ps
kubectl delete -f deployment.yaml
```
