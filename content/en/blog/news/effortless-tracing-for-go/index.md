---
title: Effortless distributed tracing for Go applications
linkTitle: Effortless distributed tracing for Go applications
date: 2022-09-26
weight: 5
---

Today we are excited to announce version **v0.6** of Go automatic instrumentation and version **v0.1.3** of Odigos.
These versions focus on improving observability for Go developers.

Odigos is now able to automatically perform **context propagation** on any Go application.
An excellent example can be seen below in the trace created by Odigos:

![Automatically created distributed trace](vote_trace.png)

As you can see, context is propagated automatically between different libraries (an HTTP request that caused an invocation of a gRPC request) and across processes (marked in different colors).

## Bringing distributed traces to everyone

We believe the automatic creation of distributed traces is a key part of making observability simpler. The idea of distributed tracing first started with a paper called [Dapper](https://research.google/pubs/pub36356/) that Google published in **2010**. 12 years later, and still, the majority of companies have yet to implement distributed tracing.

One of the reasons implementation has been prolonged, is that distributed tracing is especially hard to implement when developing Go applications. Due to the static binaries produced by the language, until recently automatic instrumentation was just not possible. Fortunately, using eBPF we can now solve this.. Using an eBPF feature called uprobes allows us to extend binaries with minimal effect on performance (for example, the above trace took 3.1ms to complete).

## New features

In addition to context propagation this version introduces the following improvements:

- Removed dependency on goroutine id: The previous versions used goroutine id to correlate spans. Following feedback from the community that this is not an id we should count on, this version does not use goroutine id anymore. Instead, we are not using the `context.Context` object for span correlations. This is similar to how it happens when you write manual instrumentation and is much more stable.
- More accurate timestamps: We improved the way we calculate the start and end timestamps of every span.
- Bug fixes and performance improvements.

## We believe in community

Both Odigos and Go automatic instrumentation are developed in open source with the community.
Recently, the Go automatic instrumentation was donated to OpenTelemetry and is now developed together with the OpenTelemetry community in the form of a new SIG called Go Automatic Instrumentation.

We can’t wait to hear what you think. We invite you to follow us or reach out to us in the following ways:

- [GitHub Issues](https://github.com/keyval-dev/odigos)
- [Odigos Slack](https://join.slack.com/t/odigos/shared_invite/zt-1d7egaz29-Rwv2T8kyzc3mWP8qKobz~A)
- Go automatic instrumentation: #otel-go-instrumentation at the CNCF slack
