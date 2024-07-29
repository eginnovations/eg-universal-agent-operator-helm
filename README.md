

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/eginnovations)](https://artifacthub.io/packages/search?repo=eginnovations)  
# eG Innovations

**eG Universal Agent Operator** automatically configures a host agent on every Kubernetes worker node. The host agent auto-discovers the worker nodes and application containers running as Pods on each node and tracks their performance and utilization levels. In-depth monitoring of applications running on containers is also provided using the same host agent. No additional agents are required for the containers.
This helm chart is optimized to run in Kubernetes cluster.

The eG Universal Agent Operator helm chart adds eG Universal Agent Operator to cluster.

  

## Steps To Deploy eG Universal Agent Operator Using Helm For Kubernetes/OpenShift

## Prerequisites

-   Helm3
-   Kubernetes 1.20 Or Higher

## Installing from Artifact Hub

The Helm chart for eG-Agent can be found in Artifact Hub under below URL.

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/eginnovations)](https://artifacthub.io/packages/search?repo=eginnovations)  
  
**Step 1 -** Adding the Repository. Run command.  
```
    helm repo add eginnovations https://eginnovations.github.io/eg-universal-agent-operator-helm
```
  
**Step 2 -** Installing the chart. Update required fields in values.yaml or use **--set** command.  
    Using values.xml:
```
    helm install eg-universal-agent-operator eginnovations/eg-universal-agent-operator 
```

## Installing eG-Agent Helm Chart locally

Clone the repository and cd inside repository directory and run the following command
```
     helm install eg-universal-agent-operator ./eg-universal-agent-operator
```
## List currently running charts in the cluster

The list of running charts can be obtained by running the follow command 
```
    helm ls
```
## Delete Running Chart To Uninstall a running Chart, Run command  
```	
	helm uninstall eg-universal-agent-operator
```