# Services
a way to EXPOSE an application running as a set of Pods. It abstracts pods to an accessible service, so the client doesn't need to be aware of the pods or their number beneath
# Endpoints
the actual entity that k8s-service routes traffic to. They are objects that are linked to Pods, they simply describe IP+Port of a Pod, BAM!
