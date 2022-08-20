# Probes:
  a way to determine the health of containers "I might say pods"
 
# Types:
  # 1. Liveness probes:
     Used to determine wheher or not a containerApplication is in a healthy state, and it is checked "constantly"
  # 2. Startup probes:
     Used to determine wheher or not a containerApplication has started up in a healthy state, and it is not checked "constantly"
  # 3. Readiness probes:
     Used to determine wheher or not a containerApplication is ready to accept traffic, and it is concerned with services
