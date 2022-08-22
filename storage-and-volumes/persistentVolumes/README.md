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

# Persistent Volume Claim
Represents a user's <b>request</b> for storage resources. When created, it searches for a PersistentVolume PV that match the PVC request requirements, if it finds, it (the PVC) will bind to that (the PV)
