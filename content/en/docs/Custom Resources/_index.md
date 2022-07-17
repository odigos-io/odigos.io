---
title: "Custom Resources"
linkTitle: "Custom Resources"
weight: 4
---

The different components of the Odigos observability control plane work together to achieve observability for the cluster. The interaction between the components is performed via the Kubernetes API server.

The autoscaler, instrumentor and scheduler are [Kuberentes Operator](https://kubernetes.io/docs/concepts/extend-kubernetes/operator/)s. They coordinate by writing and watching the odigos custom resources in the Kubernetes API server.

Odigos adds the following custom resources to the Kubernetes API server:

## Destination

This custom resource is used to define the backend destinations for the observability data.
Destinations can be either vendors (Datadog, Honeycomb, etc) or on premise.

The destination object holds any data that is needed to connect to the backend system.
Notice that sensitive fields such as API keys are stored in a Kubernetes secret and referenced by the destination object.

## InstrumentedApplication

This object is used to define the applications that should be instrumented. There is a single InstrumentedApplication object per selected Deployment / StatefulSet. The InstrumentedApplication object holds information about the application that should be instrumented, such as the detected programming language. InstrumentedApplication objects are created and managed by the instrumentor.

## Collector

This custom resource is used to define the collectors that will collect the observability data. The collector object is created and managed by the autoscaler service.