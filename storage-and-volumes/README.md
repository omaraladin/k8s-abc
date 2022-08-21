# Why Volumes
a Container filesystem is **ephemeral** which should be!  
but for some scenarios you might want to avail some storage or file-system to be accessed by the pod, and you need it to survive a pod lifecycle  
that is what Volumes do  
# Volumes
volumes allow to store data **outside** the container filesystem, while still allowing the container to access data at run-time  

# Persistent Volumes
Allows you to treat storage as an abstract resource and consume it with your Pods  
  
It goes like this:  
|- PersistentVolume -> PersistentVolumeClaim "assigned to the pod" -> Pod  
asd
