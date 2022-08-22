# Persistent Volumes
allows you to treat storage as an abstract resource, ready to be consumed by Pods  

# StorageClassName
created to specify a storageClass charactristics, you can use them to metadata your storageClasses  

# Persistent Volume Reclaim Policy
defines what should happen to the persistentVolume storage <b>after</b> it has been used by a Pod  
  * Retain
  Keeps all data in storage
  * Recycle 
  Deletes all data in storage
  * Delete
  Delete the underlying storage resource, only works with Cloud Storage Resources
