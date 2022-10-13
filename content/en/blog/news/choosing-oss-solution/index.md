---
title: Odigos - allowing a choice between the 5 leading open-source observability backends
linkTitle: Odigos - allowing a choice between the 5 leading open-source observability backends
date: 2022-10-13
weight: 6
---

As observability grows in popularity, new open-source solutions continue to emerge, allowing companies to implement end-to-end observability solutions without spending a dime.

This growing trend of observability open-source software is in line with developments across other technology sectors. Already, web, mobile, and cloud solutions are increasingly built on open-source infrastructure. Future architectures are highly likely to be based on open source, as they are today in mobile solutions (Android platform), web solutions, where most websites are based on open-source technology; and cloud solutions, where almost all are based on open-source solutions as well.

Observability vendors offer solutions that process signals (distributed traces, metrics & logs) that are displayed on dashboards with performance KPI’s and insights reflecting the health and security of any applications. The challenge has been implementing these technologies to deliver their full potential of observability capabilities. Looking at the “getting started” page of most observability vendors, it is clear why implementing these solutions is a challenging process that includes: changing code, using SDK’s to auto-instrument applications, configuring & deploying collectors and finally, continuously managing them to scale (for new applications, new collectors, etc.).

Enter Odigos – an open-source, agnostic observability control plane that automates the whole process. With a quick & easy installation replacing days, if not weeks, of integration, companies can have all their application produce distributed tracing, metrics and logs within minutes. As an agnostic observability enabler, Odigos allows you to connect to any observability tool vendor out there, open-source or not.

Being big believers, supporters, and maintainers in the open-source community, Odigos is happy to announce that we are **now integrated with five open-source observability tools vendors.**

**Prometheus, Jaeger, Loki, Tempo & Signoiz** are all now supported by Odigos and can be installed within minutes.

## What does this mean

It means companies have **a choice** of vendors when implementing an end-to-end open-source observability solution. As shown in the table below, between the five vendors there are currently three different open-source solutions for processing and analyzing Distributed Tracing, Metrics & Logs.

|            | Traces | Metrics | Logs |
| ---------- | ------ | ------- | ---- |
| Prometheus |        | ✅      |      |
| Tempo      | ✅     |         |      |
| Loki       |        |         | ✅   |
| Jaeger     | ✅     |         |      |
| SigNoz     | ✅     | ✅      | ✅   |

Additionally, it’s now easy for companies can work with more than one Observability vendor. Do you like Prometheus for you Metrics but want to use Tempo for your distributed tracing? Not a problem. As the industry continues to grow and observability becomes ubiquitous, additional tools with new functionality are flourishing (Security, etc.) and we expect companies in the future to use more the one observability vendors.

This is just a first step. Odigos will continue to integrate open-source solutions, allowing our customers a gateway to choose the solution that best fits their needs. As additional functionality is developed, Odigos will continue supporting multiple vendors enabling companies to prepare and take advantage of the new observability-based solutions being developed

## The open-source vendors supported by Odigos

**Prometheus** – Prometheus is an open-source software application used for event monitoring and alerting. It records real-time metrics in a time series database built using a HTTP pull model, with flexible queries and real-time alerting.

**Jaeger** – Jaeger is open-source software for tracing transactions between distributed services. It's used for monitoring and troubleshooting complex microservices environments

**Loki** - Loki is a log aggregation system designed to store and query logs from all your applications and infrastructure.

**Tempo** - Tempo is an open source, easy-to-use, and high-scale distributed tracing backend.

**SigNoz** - Supports all three telemetry signals under a single dashboard. You can correlate your application metrics and traces, and use it for things like infrastructure monitoring
