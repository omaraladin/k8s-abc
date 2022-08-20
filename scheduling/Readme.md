# Scheduling
K8s-scheduler takes several things into account to assign pods to worker-nodes
* Available Node Resources
* Resources Requests
* Scheduling Configurations with labels options:
  * nodeSelctor
  for example nodes that are labled as compliant:yes
  * nodeName
  obvious!
