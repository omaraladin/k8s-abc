# Services
a way to EXPOSE an application running as a set of Pods. It abstracts pods to an accessible service, so the client doesn't need to be aware of the pods or their number beneath
# Services Types
  # 1. NodePort
  Exposing an app OUTSIDE the k8s-cluster with a Port.  
  Use-case: When the CLIENT to the service is identified as OUTSIDE the k8s-cluster  
  # 2. ClusterIp
  Exposing an app INSIDE the k8s-cluster with an IP, other nodes in the cluster can communicate.  
  Use-case: When the CLIENT to the service is identified as "other pods or apps INSIDE the k8s-cluster"
  # 3. LoadBAlancer
  Use-case: When the CLIENT to the service is identified as OUTSIDE the k8s-cluster, it uses an **externalLoadBalancer** to accept traffic, so  
  it demands the k8s-cluster to be available to a cloudEnvironment, e.g. AWS, GCP, Azure
  # 4. ExternalName (outside CKA scope)

# Endpoints
the actual entity that k8s-service routes traffic to. They are objects that are linked to Services, they simply describe IP+Port of Pods, BAM!
