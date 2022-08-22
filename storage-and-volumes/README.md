# Why Volumes
a Container filesystem is **ephemeral** which should be!  
but for some scenarios you might want to avail some storage or file-system to be accessed by all pod containers, and you need it to survive a pod lifecycle  
that is what Volumes do  
# Volumes
volumes allow to store data **outside** the container filesystem, while still allowing the container to access data at run-time  

# Volumes Types
  * hostPath  
  stores data in a specific **directory on the Node**
  * emptyDir  
  stores data in a dynamically created location on the node, so it doesn't survive pod lifecycle. if the pod gets deleted, it is removed as well  
  you may use it to share data between containers within a single pod.  

# Persistent Volumes
Allows you to treat storage as an abstract resource and consume it with your Pods  
Uses a set of attroibutes to describe the underlying storage resource, whether a disk or a cloudStorageObject  

It goes like this:  
|- PersistentVolume -> PersistentVolumeClaim "assigned to the pod" -> Pod  
