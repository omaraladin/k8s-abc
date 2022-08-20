# Probes:
  a way to determine the health of containers, inside a pod each container could have a different probe type "which makes sense"
 
# Types:
  # 1. Liveness probes:
Used to determine wheher or not a containerApplication is in a healthy state, and it is checked "constantly"
  # 2. Startup probes:
Used to determine wheher or not a containerApplication has started up in a healthy state, and it is not checked "constantly"
  # 3. Readiness probes:
Used to determine wheher or not a containerApplication is ready to accept traffic, and it is concerned with services

# Self Healing
# Restart Policies
In a good example, this will be engineered with some probes to self-heal an unhealthy application detected by configured probes
Restart policies automatically restarts an application when it fails, and it is customizable to the following types

# Types:
  # 1. Always:
the default restartPolicy, it will always keep restarting the container, if it stopped or became unhealthy
  # 2. OnFailuer:
will run only if the container exited with an error code, or detected unhealthy by a LivenessProbe  
"Used for applications that are expected to run once, and then stops. because if Always policy is applied, it will keep restarting them"
  # 3. Never:
a container will never be restarted, whether stopped or detected as unhealthy via a LivenessProbe
