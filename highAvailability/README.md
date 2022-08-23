# High Availability
the classic multiple cp nodes, cp01, cp02.  and the kublet in each worker-node will interact with a loadbalancer that its backend is these multiple kube-apiserver on each cp node  

# etcd database in HA scenarios
  <b>1. Stacked etcd</b>  
  
  [Stacked etcd topology](https://d33wubrfki0l68.cloudfront.net/d1411cded83856552f37911eb4522d9887ca4e83/b94b2/images/kubeadm/kubeadm-ha-topology-stacked-etcd.svg)
  <b>2. External etcd</b>  
  [External etcd topology](https://d33wubrfki0l68.cloudfront.net/ad49fffce42d5a35ae0d0cc1186b97209d86b99c/5a6ae/images/kubeadm/kubeadm-ha-topology-external-etcd.svg)
