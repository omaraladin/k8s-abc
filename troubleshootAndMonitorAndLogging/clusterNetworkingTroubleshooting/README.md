# kube-proxy and DNS
when troubleshooting network, it is important to check kube-proxy and kube-dns  
<code>kubectl -n kube-system logs (kube-proxy|coredns)PodID</code>

# netshoot (nicolaka/netshoot)
a great tip is to use this container-image which comes with many built in network tools, and then kubectl exec to test the cluster network functionality  

