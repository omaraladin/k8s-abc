# Static Pods
a pod that is managed directly by the kbuelet agent on a node, they are independent of k8s-apiserver or its client kubectl
automatically created by Manifest YAML files that are located in the manifest path on a node
  # Mirror Pods
  kubelet will create a mirror-pod for each staticPod allowing you only to see their status, but not managing them
