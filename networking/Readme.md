# Container Network Interface (CNI)
a CNI plugin is a network plugin that allows network-connectivity between pods in a k8s-cluster, examples of CNI plugins are:
* Calico
* Weave
* Romana
check the list <a href="https://github.com/containernetworking/cni#3rd-party-plugins">here</a> in k8s-cni Github page
# DNS
k8s uses DNS to allow pods to locate other pods and services using Domain Names instead of IP addresses. The default is CoreDNS which runs as a service in the kube-system namespace
* a pod with 192.168.1.10 in the default namespace will have the domain name 192-168-1-10.default.pod.cluster.local
* a pod with 192.168.1.20 in the production namespace will have the domain name 192-168-1-20.production.pod.cluster.local
# Network Policy
a networkPolicy is a k8s-object that allows to control and manage the traffic to and from (Ingress and Egress) to pods, using podSelectors, namespaceSelectors, or IpBlock to define WHERE the networkPolicy is applied. and the same inside [spec:] rules to define who is controled by the networkPolicy Rule think of it as SecurityGroups in networking, see the networkPolicyExample.yaml on this same path
