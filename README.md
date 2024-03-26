## GATEWAY API ON KUBERNETES
Kubernetes jubeadmn version 1.27.4

# get the gateway api from Kong as it is marked as GA so it is going to be lasting, rename it if you want, in this repo it is called kong-gateway-api-install-in-first.yaml
```bash
wget https://github.com/kubernetes-sigs/gateway-api/releases/download/v1.0.0/standard-install.yaml
```


Outputs:
```bash
kubectl apply -f kong-gateway-api-install-in-first.yaml 
customresourcedefinition.apiextensions.k8s.io/gatewayclasses.gateway.networking.k8s.io created
customresourcedefinition.apiextensions.k8s.io/gateways.gateway.networking.k8s.io created
customresourcedefinition.apiextensions.k8s.io/httproutes.gateway.networking.k8s.io created
customresourcedefinition.apiextensions.k8s.io/referencegrants.gateway.networking.k8s.io created
```

# after do the same for the next ones called ....install-in-second.yaml ...etc..
