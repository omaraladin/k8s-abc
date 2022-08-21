# Ingress
an Ingress is a k8s-object that manages external access to services in the cluster with more functionality than **NodePort** services  
functionalities, such as:  
* SSL Termination
* Advanced LoadBalancing
* Name-based virtual hosting  
Ingress uses routingRules to to determine WHICH Requests, should the routing be applied to. and Note that Ingresses routes traffic to **Services**
