Kubernetes is a portable, extensible, open source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available.

It's a container orchestration platform that consists of several components and it works tirelessly to keep your servers in the state that you desire.

![[Pasted image 20240223090733.png]]

## Kubernetes Components

When you deploy Kubernetes, you get a cluster.

A Kubernetes cluster consists of a set of worker machines, called [[Notes#Nodes|Nodes]], that run containerized applications. Every cluster has at least one worker node.
The worker node(s) host the [[Notes#Pods|Pods]] that are the components of the application workload.

![[Pasted image 20240223092557.png]]

## Control Plane Components

The control plane's components make global decisions about the cluster (for example, scheduling), as well as detecting and responding to cluster events (for example, starting up a new pod when a Deployment's [[Notes#Replica|replica's]] field is unsatisfied).

**kube-apiserver:** The API server is a component of the Kubernetes [control plane](https://kubernetes.io/docs/reference/glossary/?all=true#term-control-plane) that exposes the Kubernetes API. The API server is the front end for the Kubernetes control plane.

**etcd:** Consistent and highly-available key value store used as Kubernetes' backing store for all cluster data.

**kube-scheduler:** Control plane component that watches for newly created Pods with no assigned node, and selects a node for them to run on.

**kube-controller-manager:** Control plane component that runs controller processes.
Logically, each controller is a separate process, but to reduce complexity, they are all compiled into a single binary and run in a single process.

**cloud-controller-manager:** A Kubernetes control plane component that embeds cloud-specific control logic. The cloud controller manager lets you link your cluster into your cloud provider's API, and separates out the components that interact with that cloud platform from components that only interact with your cluster.
> Note: The cloud-controller-manager only runs controllers that are specific to your cloud provider. If you are running Kubernetes on your own premises, or in a learning environment inside your own PC, the cluster does not have a cloud controller manager.

Go to: [[Node Components]]