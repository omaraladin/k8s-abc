You have two services in two different namespaces as in the following  
|- namespace: web  
  |- pod: web-pod  
  |- service: web-svc  

|- namespace: backend  
  |- pod: backend-pod  
  |- pod: test-pod  
  |- service: backend-svc    

# Summary
Objects inside the same namespace can communicate with services using the shortNames only  
While objects in different namespaces than the service actually exists can communicate using FQDN, e.g. backend-svc.backend.svc.cluster.local  
you can check by executing nslookup command from same namespaces and different namespaces  
```kubectl -n backend exec test-pod -- nslookup backend-svc #Same namespace```  
```kubectl -n backend exec test-pod -- nslookup web-svc.web.svc.cluster.local #Different namespace```
