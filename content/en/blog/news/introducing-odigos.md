---
title: Introducing Odigos!
linkTitle: Introducing
weight: 2
---

Introducing [Odigos](https://github.com/keyval-dev/odigos)! an Open-Source Observability Control Plane that allows organizations to create & maintain their observability pipeline.
Odigos allows applications to provide traces, metrics, and logs within minutes - without making any code changes.

### The Problem

Real-time Observability is essential to deliver a seamless digital experience. It’s tough to get a holistic view of your entire application when it’s running on hundreds of pods deployed to dozens of nodes distributed across the world. Observability has become mission critical for teams who need to track, manage, and optimize the performance and availability of these environments.

When integrated correctly, Observability tools can monitor and troubleshoot issues by centralizing your data and providing smarter insights into key metrics on performance, usage, and user behavior. Observability tools should support the languages and frameworks you use, integrate easily with your container platform and the other tools you use, including any communication or alert.

The problem is that implementing, maintaining and scaling are contninuous tasks. Without proper execution and continuous configuration, observability tools are limited at best and many times ineffectual.

For R&D teams, applying Observability capabilities in the cloud requires specific skill sets, particularly considering the shift to [OpenTelemetry](https://opentelemetry.io/) & [eBPF](https://ebpf.io/). Organizations must ensure they have access to specific skills sets within a limited and fiercely competitive talent pool. Learning SDK’s, adding auto-instrumentation (for each language), writing code, deploying, and maintaining collectors – this all requires considerable time and knowledge that most organizations do not possess

In order to work around these integration issues, some large observability tool vendors offer their own agents, providing their own tailor-made solution. The problem with this is that it creates a vendor lock-in, by using proprietary agents that ingest and store data in a proprietary format. As enterprises increasingly seek compatibility with open source standards, as well as the ability to share and access data across departments, having data locked in proprietary silos hinders those efforts and raises costs.

[Odigos](https://github.com/keyval-dev/odigos) Observability Control Plane provides a comprehensive and fully automated solutions that allows orginaizations to build their Observability pipline within minutes. Odigos is focused on 3rd-party integrations, open source, open standards, and overall a more consolidated approach, reducing the complexity involved in combining multiple observability software vendors and open-source software solutions.

### The technology behind Odigos

Odigos automatically detects the programming language of every application in your cluster and performs automatic instrumentation accordingly. For compiled languages (like Go), eBPF is used in order to instrument the application. For virtual machine languages (like Java) OpenTelemetry is used. In addition, pipelines created by Odigos follow best practices such as: persisting API keys as Kubernetes secrets, use of minimal collector images, and much more.

The ability to install, configure and maintain an open-source, agnostic Observabiity Control Plane will impower organizations of all sizes the ability to adopt the right tools for them at any given time, and add more tools as needed.

**Odigos makes Observability simple and accessible to all.**
