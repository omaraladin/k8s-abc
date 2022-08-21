# Deployment
a Controller to maintain an application as a STATE, as simple as that
the hierarchy is like this
|-* Deployment
  -* Pod
    -* Containers "which are not reresented in K8s-ControlPlane"
    
# Scaling
with commands such as:
# kubectl scale deployments/my-app --replicas=10
or:
# kubectl edit deployment my-app #and then editing the replicas number in the YAML file
