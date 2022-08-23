# Checking Pod status

* Broad status with <code>kubectl get pods</code>  
* detailed status with <code>kubectl (describe|logs) pod nginx-pod</code>  
* or maybe run commands to check from inside the container <code>kubectl exec nginx-pod -c nginx-pod-cont1 -- command</code>  
* or maybe login to the container <code>kubectl exec nginx-pod --stdin --tty -- /bin/bash</code>  

# Checking Container logs

* <code>kubectl logs nginx-pod [-c container1 OPTIONALLY] </code>
