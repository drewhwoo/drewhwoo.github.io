---
layout: post
title: Kubernetes container networking
---


<https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/>

## Docker networking

Host-private networking : containers can talk to other containers only if they are on the same machine.

Port fowarding for mapping of container port and host port.

Docker (host) creates a virtual bridge, called "docker0".

Each container has its own virtual ethernet device "veth" which is attached to the bridge.

Through the bridge, containers on the same host can communicate.


## Kunbernetes networking

Containers within a Pod can all reach each other’s ports on localhost, and all pods in a cluster can see each other without NAT.


## How k8s networking works

<https://kubernetes.io/docs/concepts/cluster-administration/networking/#how-to-achieve-this>

Every pod has its own IP, similar to VM and physical machine.
