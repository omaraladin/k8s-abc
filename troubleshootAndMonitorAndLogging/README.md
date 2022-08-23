# Troubleshooting

# Broad Overview
# 1. kube-apiserver
make sure <b>docker</b> and <b>kubelet</b> services are running

# 2. Nodes
To see the overall status <code>kubectl get nodes</code>  

to describe node events <code>kubectl describe nodes worker-2</code>  
after that maybe the node requires you to login into it, and check the status of <b>kubelet+docker</b> services  

# 3. Checking k8s-system pods
get pods status via <code>kubectl -n kube-system get pods -o wide</code>
or check pods events via <code>kubectl -n kube-system describe pod kube-apiserver</code>
