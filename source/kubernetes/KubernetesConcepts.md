# Kubernetes Essential Concepts

**Kubernetes (K8)**  is a portable, extensible open-source platform for managing containerized workloads and services

The K8 **Platform** is designed to be extensible. 

* A **Label**  can be attached to a resource to allow easy organization.
* An  **Annotation** can be attached to a resource to simplify workflows and allow easy/improved management.
* The K8 **Control Plane**  uses published APIs. Anyone can build a component and plug it in. 

For build instructions, images and containers, the Docker concepts can be used, though K8 supports more container types that just Docker.

* K8 **Build instructions** depend on the type of image / container being targets. They include "Dockerfile'  for Docker and so on. 
* A K8 **Image**  results from applying the build instructions. They include a Docker image for Docker and so on.
* A K8 **Container** results from loading / running an image in K8. 
* K8 supports multiple **Container Runtimes** including for Docker containers.

* A K8 **Pod** is a group of one or more Containers.

* A K8 **Deployment** manages a pod.

* A K8 **Service** exposes a pod to the outside world.

* A K8 **Node** runs one or more Pods.
