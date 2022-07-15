---
title: "Architecture"
linkTitle: "Architecture"
weight: 4
---

## Goals

Odigos acts as a control plane for all the observability needs in a cluster. It is responsible for:

- Automatic instrumentation of applications
- Automatic configuration and deployment of collectors
- Infrastructure observability (Kubernetes nodes observability data)

## High Level Architecture

These tasks are performed by 4 microservices:

- Instrumentor
- Autoscaler
- Scheduler
- UI

The following diagram shows the architecture of the Odigos observability system.

![](Odigos_Arch.jpg)
