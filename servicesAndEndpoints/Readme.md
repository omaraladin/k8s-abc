# Services
a way to EXPOSE an application running as a set of Pods. It abstracts pods to an accessible service, so the client doesn't need to be aware of the pods or their number beneath
# Services Types
  # 1. NodePort
  # 2. ClusterIp
  Exposing an app INSIDE the k8s-cluster with an IP, other nodes in the cluster can communicate.  
  use it when the CLIENT is identified as other pods or apps INSIDE the k8s-cluster
  # 3. LoadBAlancer
  # 4. ExternalName (outside CKA scope)

# Endpoints
the actual entity that k8s-service routes traffic to. They are objects that are linked to Pods, they simply describe IP+Port of a Pod, BAM!
