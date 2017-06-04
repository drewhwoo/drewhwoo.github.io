---
layout: post
title: Kubernetes container networking
---


<https://kubernetes.io/docs/concepts/services-networking/connect-applications-service/>

## Docker networking

host-private networking : containers can talk to other containers only if they are on the same machine.

Port fowarding for mapping of container port and host port. 

## Kunbernetes networking

Containers within a Pod can all reach each other’s ports on localhost, and all pods in a cluster can see each other without NAT. 
