## k8s-multinode-cluster-kind
Create k8s multinode cluster using kind

### Prerequisite:

go (https://golang.org/)

docker — Service needs to be running(https://www.docker.com/)

### Install Kind 

```shell
$ GO111MODULE=”on” go get sigs.k8s.io/kind@v0.8.1
```

#### Mac

```
$ brew install kind
```
https://kind.sigs.k8s.io/docs/user/quick-start/ 


```
$ kind create cluster --name=multinode --config=kind.yaml
$ kubectl get nodes
$ kubectl apply -f daemonsets.yaml
$ kubectl get pods -o wide 
```

### License
[Apache License](http://www.apache.org/licenses/LICENSE-2.0), Version 2.0
