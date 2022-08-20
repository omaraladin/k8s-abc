# DaemonSets
a DaemonSet ensures that all (or some) Nodes run a copy of a the Pod specidied on the daemonset on them "Nodes".
# Relationship to Scheduling
DaemonSets respect normal scheduling rules, so if a pod is configured to not-run on a specific node, the daemonset will not assign a copy of the pod to that particular node
