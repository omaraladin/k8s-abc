# Checking Cluster and Node logs
* Services-related logs <code>sudo journalctl -u kubelet|docker</code>
* components-related logs  
  In kubeadm-initialized clusters <code>kubectl -n kube-system logs (kube-apiserver|kube-scheduler|kube-controller-manager)PodID</code>  
  In other installations <code>/var/log/(kube-apiserver|kube-schedulerkube-controller-manager).log</code>  
