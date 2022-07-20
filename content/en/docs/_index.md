---
title: "Odigos Documentation"
linkTitle: "Documentation"
weight: 20
menu:
  main:
    weight: 20
---

Welcome to the Odigos user guide! We will show you how to get started sending telemetry data such as traces, metrics and logs within minutes, using Odigos.

Odigos is an Open-Source Observability Control Plane that allows developers to easily create and build their observability pipelines, by abstracting away the complexities of technologies such as eBPF and OpenTelemetry.

Every new line of code automatically gets metrics and distributed traces without intervention from the developer and with no code changes necessary. With Odigos, production issues can be resolved using the best observability tools available, without the overhead of instrumenting code or taking care of collector agents.

The name Odigos originates from Greek, meaning guide

## Odigos in Short

|                                      |                                                                                                                                               |
| ------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **🧑‍💻 Automatic instrumentation**     | Odigos detects the programming language of your applications and apply automatic instrumentation accordingly..                                |
| **📖 Open Technologies**             | Observability pipelines created by Odigos are based on popular, battle tested, open source technologies. Specificlly, OpenTelemetry and eBPF. |
| **⚖️ Scales with your data**         | Odigos scales the number of collectors based on the traffic of your applications. No need to manage complex collectors topology               |
| **📈 No learning curve**             | Use advanced features like tail-based sampling without complex YAML configurations                                                            |
| **✅ Best practices out of the box** | API key are saved as Kubernetes secrets, minimal collector images contains only relevant exporters and many more                              |
| **☸️ Cloud Native**                  | Odigos is specially designed to instrument containers deployed in Kubernetes. Providing a natural experience to Kubernetes users.             |

## Who is Odigos for?

**Application developers** - focus on writing code. Odigos takes care of producing metrics ands traces for any open source library in use, without any code changes.

**DevOps engineers** - Odigos automatically deploys and scales collectors for you, according to the current traffic of your applications. No need to spend time deploying and configuring collectors.

## Where do I start?

{{% alert title="Get started with Odigos!" %}}
Following this [guide](getting-started/) will just take a couple of minutes to complete:
You will get automatic full observability for microservices application written in Go, Java, Python, and Node.js.
{{% /alert %}}
