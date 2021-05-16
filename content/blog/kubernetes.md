---
title: "Kubernetes"
date: 2021-02-03T20:23:51+05:30
slug: ""
description: ""
keywords: []
draft: false
tags: []
math: false
toc: false
---

### Q. What is Kubernetes?
    Kubernetes is a portable, extensible, open-source platform for managing containerized workloads and services, that facilitates both declarative configuration and automation. It has a large, rapidly growing ecosystem. Kubernetes services, support, and tools are widely available. Kubernetes automates the deployment, scaling, maintenance, scheduling, and operation of multiple application containers across clusters of nodes. Kubernetes contains tools for orchestration, service discovery, and load balancing that can be used with Docker and Rocket containers. As needs change, a developer can move container workloads in Kubernetes to another cloud provider without changing the code.

## Kubernetes Terminology and Architecture
Kubernetes introduces a lot of vocabulary to describe how your application is organized. We’ll start from the smallest layer and work our way up
# i. Containers
Containers are software images that represent complete runnable applications .
It differs from a VM as in a VM is an abstraction at the hardware level whereas a container is an abstraction at the app level.A docker container (commonly used ) is a lightweight , standalone executable package of software which includes everything.
1. Code
2. Runtime
3. System tools
4. System libraries
5. Settings
6. Kubernetes comes into play to orchestrate multiple containers similar to management of a distributed system
## ii. Pods
A Kubernetes pod is a group of containers, and is the smallest unit that Kubernetes administers. Pods have a single IP address that is applied to every container within the pod. Containers in a pod share the same resources such as memory and storage. This allows the individual Linux containers inside a pod to be treated collectively as a single application, as if all the containerized processes were running together on the same host in more traditional workloads
## iii. Deployments
Kubernetes deployments define the scale at which you want to run your application by letting you set the details of how you would like pods replicated on your Kubernetes nodes.
## iv. Services
A service is an abstraction over the pods, and essentially, the only interface the various application consumers interact with. As pods are replaced, their internal names and IPs might change. A service exposes a single machine name or IP address mapped to pods whose underlying names and numbers are unreliable. A service ensures that, to the outside network, everything appears to be unchanged
## v.Nodes
A Kubernetes node manages and runs pods; it’s the machine (whether virtualized or physical) that performs the given work.
The Kubernetes control plane
The Kubernetes control plane is the main entry point for admins and users to manage the various nodes.
The control plane includes
API server
Scheduler
Controller manager
Worker Node components
Kubelet- A Kubelet tracks the state of a pod to ensure that all the containers are running. It provides a heartbeat message every few seconds to the control plane.
Kube proxy - The Kube proxy routes traffic coming into a node from the service. It forwards requests for work to the correct containers.
Etcd - It is a distributed key-value store that Kubernetes uses to share information about the overall state of a cluster.
Kubernetes architecture
A bit more detailed architecture using the above mentioned terminologies
