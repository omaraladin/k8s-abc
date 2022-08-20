# Multi-containers-pod
containers inside will share the Storagem Filesystenm, and Network of a single pod
  * Often describe as sidecars and logging legacy app may be a fit use-case

# InitContainers
initContainers are containers that will run once and in-sequence before the startup of appContainers, and they have several use-cases:
  * Cause a pod to Wait for another k8s-resource to be created
  * Perform sensitive data startup security tests outside of appContainers
  * Populate some data into a shared volume in the Pod
  * Communicate with a k8s-service before app startup
